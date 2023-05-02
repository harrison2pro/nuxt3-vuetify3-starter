<template>
<div class="top-navigation">
  <v-row no-gutters>
    <v-col md="2" lg="2">
     <Logo/>
    </v-col>
    <v-col md="8" class="top-navigation-menu-holder">
      <HorizontalMenu/>
    </v-col>
    <v-col md="2">
      <ProfileInMenu/>
    </v-col>
  </v-row>
</div>
</template>

<script>
export default {
  name: "TopNavigation"
};
</script>

<style scoped>
.top-navigation{
  background-color:#2D303F;
  min-height: 56px;
  padding:20px;
  border-bottom:1px solid #353949;
}
.top-navigation-menu-holder{
  justify-content: center;
  display: flex;
  align-items: center;
}
</style>