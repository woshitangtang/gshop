<template>
    <div>

    </div>
</template>
<script>
  import Vue from 'vue'
  import VueRouter from 'vue-router'

  import Msite from '../pages/Msite/Msite'
  import Order from '../pages/Order/Order'
  import Search from '../pages/Search/Search'
  import Profile from '../pages/Profile/Profile'

  Vue.use(VueRouter)

  export default new VueRouter({
    mode:'history',
    routes:[
      {
        path:'/',
        redirect:Msite
      },
      {
        path:'/msite',
        component:Msite
      },
      {
        path:'/order',
        component:Order
      },
      {
        path:'/search',
        component:Search
      },
      {
        path:'/profile',
        component:Profile
      }
    ]
  })
</script>
<style>

</style>
