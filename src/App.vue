<template>
  <AdminList/>
</template>

<script>
import AdminList from './components/AdminList.vue'

export default {
  name: 'App',
  components: {
    AdminList
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  margin-top: 60px;
}
</style>
