<template>
  <div id="app">
    <!-- The HomePage is rendered here, which includes MainNavbar -->
    <router-view/>
  </div>
</template>

<script>


export default {
  name: 'App',
  components: {},

  mounted() {

    if (localStorage.loggedIn === true) {
      localStorage.getItem('username')
      localStorage.getItem('userRightsId')

    }

  }
};


</script>

<style>
#app {
  font-family: Verdana, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #3a2d28;

  margin-left: 30px;
  margin-right: 30px;

}



</style>
