<template>
    <div class="tab-bar-item">
        <div v-if="!isactive" @click="activecli">
          <slot name="itemicon"></slot>
        </div>
        
        <div v-else>
          <slot name="itemiconactive"></slot>
        </div>
                
        <div :style="activestyle">
          <slot name="itemtext"></slot>
        </div>
    </div>
</template>

<script>
export default {
  name: 'App',
  props:{
    path:String,
    activecolor:{
      type:String,
      default:'rgb(218, 97, 117)'
    }
  },
  // data(){
  //   // return{
  //   //   isactive: false
  //   // }
  // },
  methods:{
    activecli(){
      this.$router.push(this.path)
      //console.log(this.path)
    }
  },
  computed:{
    isactive(){
      return this.$route.path.indexOf(this.path) !== -1
    },
    activestyle(){
      return this.isactive ? {color:this.activecolor} : {}
    }
  }
}
</script>

<style>

  .tab-bar-item{
    flex: 1;
    text-align: center;
    height: 49px;
    font-size: 14px;
  }

  .tab-bar-item img {
      width: 24px;
      height: 24px;
      margin-top: 3px;
      vertical-align: middle;
  }
  


</style>
