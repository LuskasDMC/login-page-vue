<template>
  <div id="app" >
    <div class="row justify-content-center align-items-center mr-0 h-100">
      <div class="col-10">
        <WhitheModal/>
      </div>
    </div>
  </div>
</template>

<script>
  import WhitheModal  from './components/Modal/WitheModal'
  import "@fortawesome/fontawesome-free"
  export default {
    name: 'App',
    components:{
      WhitheModal: WhitheModal,
    },
    beforeCreate(){
      console.log("vai montar")
    },
  }
</script>

<style>
  @import "assets/css/index.css";
</style>
