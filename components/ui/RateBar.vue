<template>
  <div class="rate-bar">
    <div class="rate-bar-inner" :style="'width:'+rate+'%'"></div>
  </div>
</template>

<script>
export default {
  name: "RateBar",
  props:['rate']
};
</script>

<style scoped>
.rate-bar{
  width:100%;
  height:10px;
  border-radius:0 50px 50px 0;
  background-color: #23262B;
}
.rate-bar-inner{
  width:0;
  height: 100%;
  background: rgb(237,222,93);
  background: linear-gradient(90deg, rgba(237,222,93,1) 0%, rgba(240,152,25,1) 100%);
}
</style>