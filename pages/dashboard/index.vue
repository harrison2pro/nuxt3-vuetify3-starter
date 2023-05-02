<template>
<div class="main-dash">
  <v-row>
    <v-col md="5">
        <div class="welcome">
          <p>Thuesday, August  3rd</p>
          <h3>Welcome , Angelica G.</h3>
        </div>
      <v-row no-gutters >
        <v-col md="6" sm="6" lg="6" class="padding-for-col"><HoverIcon/></v-col>
        <v-col md="6" sm="6" lg="6"  class="padding-for-col"> <HoverIcon/></v-col>
        <v-col md="6" sm="6" lg="6"  class="padding-for-col"> <HoverIcon/></v-col>
        <v-col md="6"  sm="6" lg="6"  class="padding-for-col"> <HoverIcon/></v-col>
      </v-row>
      <v-row no-gutters>
        <v-col md="6">
          <ReviewBox/>
        </v-col>
        <v-col md="6">
          <Statistics/>
        </v-col>
      </v-row>
    </v-col>
    <v-col md="7">

    </v-col>
  </v-row>
</div>
</template>

<script setup>
definePageMeta({
  layout: "dashboard",
});
</script>

<style scoped>
.padding-for-col{
  padding:3px;
}
.main-dash{
  padding:25px;
}
.welcome h3{
  font-style: normal;
  font-weight: 700;
  font-size: 22px;
  color: #FFFFFF;
  margin-top: 8px;
}
.welcome p{
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
  color: #7F879E;
}
</style>