<template>
<div class="review-box">
  <h3>Reviews</h3>
  <div class="rate-holder">

<div class="rate-master">
  <v-rating
    v-model="rage"
    readonly
    size="x-small"

    half-increments
    color="#F09819FF"
  ></v-rating>
</div>
  <p>1.210 reviews</p>
</div>

  <div class="bar-holder">
      <p>Exellent</p>
        <RateBar :rate="70"/>
      <span>12</span>
  </div>

  <div class="bar-holder">

    <p>Very good</p>
    <RateBar :rate="10"/>
    <span>13</span>
  </div>
  <div class="bar-holder">

    <p>Average</p>
    <RateBar :rate="20"/>
    <span>23</span>
  </div>
  <div class="bar-holder">

    <p>Poor</p>
    <RateBar :rate="10"/>
    <span>3</span>
  </div>
  <div class="bar-holder">

    <p>Terrible</p>
    <RateBar :rate="23"/>
    <span>4</span>
  </div>
</div>
</template>

<script>
import RateBar from "~/components/ui/RateBar.vue";
import { FontAwesomeIcon } from "@fortawesome/vue-fontawesome";

export default {
  name: "ReviewBox",
  data(){
    return{
      rage:4.5
    }
  },
  components: { FontAwesomeIcon, RateBar }

};
</script>

<style scoped>

.review-box {
  background-color:#2D303F;
  padding:10px;
  border-radius: 12px;
  width:90%;
}
.review-box h3{
  font-style: normal;
  font-weight: 700;
  font-size: 20px;
  color: #FFFFFF;
  margin: 0 0 5px 0;
}
.bar-holder{
  display: flex;
  gap:5px;
  align-items: center;
}
.bar-holder p{
  font-style: normal;
  font-weight: 700;
  font-size: 10px;
  text-align: center;
  color: #FFFFFF;
  width: 26%;
}
.bar-holder span{
  font-style: normal;
  font-weight: 700;
  font-size: 8px;

  text-align: center;


  color: #FFFFFF;
}
.review-box{

}
.rate-holder{
  display: flex;
  gap: 3px;
  align-items: center;
}
.rate-holder p{
  font-style: normal;
  font-weight: 500;
  font-size: 10px;

  color: #FFFFFF;

}
.rate-master{
}
</style>