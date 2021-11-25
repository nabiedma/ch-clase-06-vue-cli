<template>
  <div id="app">
    <NavigationBar sitio="Recetas" />
    <div class="container">
      <div class="row justify-content-center">
        <div class="col-3" v-for="(mensaje, i) in mensajes" :key="i">
          <Message :mensaje="mensaje"></Message>
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
  },
  data() {
    return {
      mensajes: [
        {
          usuario: "Conrado",
          msg: "Bienvenido al curso!",
          tipo: "success"
        },
        {
          usuario: "Nicolás",
          msg: "Cómo vas llevando el curso?",
          tipo: "success"
        },
        {
          usuario: "Cerebro",
          msg: "Recordá descansar, es importante!",
          tipo: "danger"
        },
      ]
    }
  },
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
