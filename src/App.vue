<template>
  <div>
    <HeaderApp title="Vue.js" :titleD="title" :extD="ext" :menus="menus" />
    <PracticeApp  />
   
  </div>
</template>

<script>
import HeaderApp from './components/HeaderApp.vue'
import PracticeApp from './components/ParcticeTow.vue'
export default {
  name: 'App',
  data: () => ({
    title: 'Vue',
    ext: true,
    menus: ['Home', 'About', 'Contact'],
  }),
  components: {
    HeaderApp, PracticeApp
  }
}
</script>

<style>

</style>
