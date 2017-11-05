<template>
  <div id="app">
    <Toolbar :current="current" @change="change"></Toolbar>
    <router-view/>
  </div>
</template>

<script>
  import Toolbar from '@/components/Toolbar'
  import './assets/iview/dist/styles/iview.css'

export default {
  name: 'app',
  data(){
      return {
          current:2
      }
  },
  methods : {
      change : function(evt){
          alert(evt)
      }
  },
  components:{
    Toolbar
  }
}
</script>

<style>
body{
  font-family: Arial, "microsoft yahei", Verdana, sans-serif;
  font-size:14px;
}
a{
  color:#797979;
}
</style>
