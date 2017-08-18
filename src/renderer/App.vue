<template>
  <div id="app">
    <sidebar></sidebar>
    <router-view></router-view>
  </div>
</template>

<script>
  import sidebar from './components/Sidebar'

  export default {
    name: 'ifdesk',
    components: {
      sidebar
    }
  }
</script>

<style>
  /* CSS */
  #app {
    height: 100%;
    widows: 100%;
  }
</style>
