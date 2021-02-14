<template>
    <div id="home">
      <navbar class="home-nav"></navbar>
    </div>
</template>

<script>
import navbar from "@/components/common/navbar/NavBar"

export default {
  name: 'home',
  components:{
      navbar
  }
}
</script>

<style>
  .home-nav{
      background-color: var(--color-tint);
      color: seashell;
  }
</style>
