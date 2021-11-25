<template>
  <div id="app">
    <NavigationBar></NavigationBar>
    <div class="container">
      <div class="row justify-content-center">
        <div class="col-6">
          <Message></Message>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import NavigationBar from './components/NavigationBar.vue'
import Message from './components/Message.vue'

export default {
  name: 'App',
  components: {
    NavigationBar,
    Message
  }
}
</script>

<style>
    NavigationBar
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
