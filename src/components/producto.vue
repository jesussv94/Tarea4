<template>
    <section id="imagenes">
      <div id="imagenPrincipal"> 
          <img v-bind:src="fotos[0]" alt="Asus tuf gaming">
      </div>
        <div id="miniaturas">
          <a @click="cambiarFoto(1)"><img  v-bind:src="fotos[1]" alt="Asus tuf gaming"></a>
          <a @click="cambiarFoto(2)"><img  v-bind:src="fotos[2]" alt="Asus tuf gaming"></a>
        </div>
    </section>
</template>

<script>
export default {
    Name: 'Imagenes',
    data () {
        return {
            fotos: [
                require ('../assets/pc1.jpg'),
                require ('../assets/pc2.jpg'),
                require ('../assets/pc3.jpg')]
        }
    },
    methods: {
        cambiarImagen(id) {
            this.fotos[0] = this.fotos[id]
        }
    }
}
</script>


<style scoped>

#imagenPrincipal{
    justify-content: left;
    display: flex;
}

#imagenPrincipal img{
    height: 350px;
    margin-right: 2rem;
}

    #imagenes {
    height: 100px;
    border-radius: 25px;
    padding: 1rem;
    margin: 1rem;
    flex: 0 1 50%;
}

#miniaturas{
    display: flex;
    flex-direction: row;
    justify-content: left;
    padding-top: 0.5rem;
}

#miniaturas img{
    height: 100px;
    margin-right: 0.5rem;
    border:grey solid 1px;
}
</style>