<template>
    <HeaderApp title="Vue.js" :titleD="title" :extD="ext" :menus="menus"/>
</template>

<script>
import HeaderApp from './components/Header.vue'

export default {
  name: 'App',
  data : () =>( {
    title : 'Vue',
    ext : true ,
    menus : ['Home' , 'About' , 'Contact']
  }),
  components: {
     HeaderApp
  }
}
</script>

<style>

</style>
