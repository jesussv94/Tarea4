<template>
  <cabecera/>
  <caminodemigas/>
  <producto/>
  <datos/>
  <descripcion/>
  <pie/>
</template>

<script>
import cabecera from './components/cabecera.vue'
import caminodemigas from './components/caminodemigas.vue'
import producto from './components/producto.vue'
import datos from './components/datos.vue'
import descripcion from './components/descripcion.vue'
import pie from './components/pie.vue'

export default {
  name: 'App',
  components: {
    cabecera, 
    caminodemigas,
    producto,
    datos,
    descripcion,
    pie
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
html{
  background-color: gainsboro;
  height: 100vh;
}
</style>
