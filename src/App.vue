<template>
    <HeaderApp title="Vue.js" :titleD="title" :extD="ext"/>
</template>

<script>
import HeaderApp from './components/Header.vue'

export default {
  name: 'App',
  data : () =>( {
    title : 'Vue',
    ext : true
  }),
  components: {
     HeaderApp
  }
}
</script>

<style>

</style>
