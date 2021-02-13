<template>
    <Tabbar>
      <Tabbaritem path="/home" activecolor="rgb(218, 97, 117)">
        <img slot="itemicon" src="~assets/img/tabbar/home.svg" alt="">
        <img slot="itemiconactive" src="~assets/img/tabbar/home_active.svg" alt="">
        <div slot="itemtext">首页</div>
      </Tabbaritem>
      <Tabbaritem path="/category"  activecolor="rgb(218, 97, 117)">
        <img slot="itemicon" src="~assets/img/tabbar/category.svg" alt="">
        <img slot="itemiconactive" src="~assets/img/tabbar/category_active.svg" alt="">
        <div slot="itemtext">分类</div>
      </Tabbaritem>
      <Tabbaritem path="/cart"  activecolor="rgb(218, 97, 117)">
        <img slot="itemicon" src="~assets/img/tabbar/shopcart.svg" alt="">
        <img slot="itemiconactive" src="~assets/img/tabbar/shopcart_active.svg" alt="">
        <div slot="itemtext">购物车</div>
      </Tabbaritem>
      <Tabbaritem path="/profile"  activecolor="rgb(218, 97, 117)">
        <img slot="itemicon" src="~assets/img/tabbar/profile.svg" alt="">
        <img slot="itemiconactive" src="~assets/img/tabbar/profile_active.svg" alt="">
        <div slot="itemtext">我的</div>
      </Tabbaritem>
    </Tabbar>
</template>

<script>

import Tabbar from 'components/common/Tabbar/Tabbar'
import Tabbaritem from 'components/common/Tabbar/Tabbaritem'

export default {
  name: 'maintabbar',
  components:{
    Tabbar,
    Tabbaritem
  }
}
</script>

<style>

</style>
