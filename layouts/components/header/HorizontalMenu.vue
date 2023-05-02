<template>
<ul>
  <li v-for="i in items">
    <nuxt-link :to="i.path"><img :src="i.icon" :alt="i.title">{{i.title}}</nuxt-link>
  </li>
</ul>
</template>

<script>
export default {
  name: "HorizontalMenu",
  data(){
    return{
      items:[
        {title:'Dashboard',icon:'/images/dash/icons/dash.svg',path:'/dashboard/'},
        {title:'Market',icon:'/images/dash/icons/market.svg',path:'/dashboard/'},
        {title:'Chat',icon:'/images/dash/icons/message.svg',path:'/dashboard/'},
        {title:'Subscription',icon:'/images/dash/icons/dollor.svg',path:'/dashboard/'},
        {title:'Help Center',icon:'/images/dash/icons/faq.svg',path:'/dashboard/'}
      ]
    }
  }
};
</script>

<style scoped>
ul{
  display: flex;
  gap: 30px;
}
ul li {
  list-style: none;
}
ul li a{
  display: flex;
  align-items: center;
  gap: 14px;
}
</style>