<template>
  <div id="app">
    <Header/>
    <div class="main">
      <!-- name 指的是路由main:PostList -->
      <router-view name="slidebar"></router-view>
      <router-view name="main"></router-view>
    </div>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import PostList from './components/PostList.vue'
export default {
  name: 'App',
  components: {
    Header,
    PostList
  }
}
</script>

<style>
.main {
  width: 80%;
  margin: 0 auto;
}
</style>
