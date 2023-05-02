<template>
<div class="statistics">
<v-row>
  <v-col>
    <h3>
    35,216
  </h3>
    <p> Views past Month
    </p>
  </v-col>
  <v-col>
    <img src="/images/dash/buttons.svg" alt="">
  </v-col>
</v-row>
  <ul class="statistics-ul">
    <li class="active">Monthly</li>
    <li>Weekly</li>
    <li>Yearly</li>
  </ul>
</div>
</template>

<script>
export default {
  name: "Statistics"
};
</script>

<style scoped>
.statistics{
  background: #2D303F;
  border-radius: 12px;
  padding:12px;
  width: 89%;

}
.statistics h3{
  font-style: normal;
  font-weight: 700;
  font-size: 16px;
  color: #FFFFFF;
  margin-bottom: 3px;
  margin-top: 0;
}
.statistics p{
  font-style: normal;
  font-weight: 700;
  font-size: 8px;
  color: #747B84;
}
.statistics-ul{
  display: flex;
  gap:10px;
  padding: 0
}
.statistics-ul li{
  list-style: none;
  color: #FFFFFF;
  font-style: normal;
  font-weight: 700;
  font-size: 7px;
  padding:1px 5px;
  border-radius:12px

}
.active{
  background: #23262B;

}
</style>