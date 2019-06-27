<template>
  <div id="app">
    <my-head></my-head>
    <router-view/>
    <my-footer></my-footer>
  </div>
</template>

<script>
  import MyHead from "@/components/head.vue"
  import MyFooter from "@/components/footer.vue"

  export default {
    components:{
      MyHead,
      MyFooter
    }
  }
</script>

<style lang="scss">
html,body{
  margin: 0;
  min-width: 1200px;
  background-color: #f9fafc;
}

  .clear:after{
    content: '';
    display: block;
    clear: both;
  }
</style>
