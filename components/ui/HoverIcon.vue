<template>
<div class="hover-icon">
  <v-row no-gutters>
    <v-col md="3" class="image-padding">
      <div class="img-holder">
        <img src="/images/dash/main-icons/endorsment.svg" alt="">
      </div>
    </v-col>
    <v-col md="8">
    <div class="info-holder">
      <h3> 12 People</h3>
      <p>Endorsment</p>
    </div>
    </v-col>
  </v-row>
</div>
</template>

<script>
export default {
  name: "HoverIcon"
};
</script>

<style scoped>
.info-holder {padding-left: 12px;}
.hover-icon {
  background: #2D303F;
  border-radius: 12px;
  padding:12px;
  width: 89%;
  margin-bottom: 10px;
}
.image-padding{
}
.img-holder{
  background: #353949;
  border-radius: 8px;
  display: flex;
  width:100%;
  height:100%;
  justify-content: center;
  align-items: center;
}
.hover-icon h3{
  font-style: normal;
  font-weight: 700;
  font-size: 16px;
  color: #FFFFFF;
}
.hover-icon p{
  font-style: normal;
  font-weight: 500;
  font-size: 12px;
  color: #7F879E;
}
</style>