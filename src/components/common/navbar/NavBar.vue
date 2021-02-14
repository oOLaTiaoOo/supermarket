<template>
  <div class="nav-bar">
      <div class="left"><slot name="left"></slot></div>
      <div class="center"><slot name="center">购物推荐</slot></div>
      <div class="right"><slot name="right"></slot></div>
  </div>
</template>

<script>
export default {
    name:'navbar'
}
</script>

<style>
.nav-bar{
  display: flex;
  height: 44px;
  font-size: 15px;
  line-height: 44px;
  text-align: center;
  box-shadow: 0 1px 1px rgba(100,100,100,1);

}

.left{
  width: 20%;
}

.center{
  width: 60%;
}
.right{
  width: 20%;
}

</style>