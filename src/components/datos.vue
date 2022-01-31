no he podido averiguar por qué se queda una zona vacia encima de esta sección
<template>
    <section id="datos">
      <h1>Asus TUF Gaming F15 FX506HM-HN014</h1>
      <h2>1229€ <span id="iva">sin IVA: 1015,70€</span></h2>
      <div id="contador">
          <button class="boton" @click="cambiar('-1')" type="button" name="boton">-</button>
          <input id="numero" type="text" name="numero" :value="contador">
          <button class="boton" @click="cambiar('1')" type="button" name="boton">+</button>
      </div>
      <br>
      <div id="carrito">
      <button id="botoncarrito"><span class="icono"><i class="fas fa-shopping-basket"></i></span> AÑADIR AL CARRITO</button>
      </div>    
    </section>  
</template>

<script>
export default {
    Name: 'Datos',
    data () {
        return {
            contador: 1
        }
    },
    methods: {
        cambiar(num) {
            this.contador += +num;
            if (!isNaN(this.contador) && (this.contador < 0)) {
              this.contador = 0
            }
        }
    }
}
</script>

<style scoped>
    #datos{
        display: flex;
        flex-direction: column;
        padding-left: 18rem;
    }

    h1{
        color: black;
        font-weight: bolder;
    }

    h2{
        color:cornflowerblue;
    }

    #iva{
        font-size: 50%;
        color:gray;
    }

    #contador{
        margin-bottom: 1.5rem;
    }
    #numero{
        width: 20px;
        height: 20px;
        font-size: 120%;
        text-align: center;
    }
   
    .boton {
        border: 1px solid grey;
        width: 25px;
        height: 25px;
        font-size: 120%;
        text-align: center;
    }
    
    #botoncarrito{
        height: 40px;
        width: 250px;
        background-color: cornflowerblue;
        color:white;
        font-weight: bold;
        font-size: 120%;
        padding: 0.4rem;
    }
</style>