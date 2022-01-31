<template>
  <header id="cabecera">
        <section id="cabeceraArriba">
            <div id="logo">
                <img src="../assets/img1.png"/>
                t<span id="nombre">Informática</span>
            </div>
            <div>
                <form @submit.prevent="handleEnviar">
                    <input type="text" placeholder="Buscar productos ...">
                    <button class="boton">Buscar</button>
                </form>
            </div>
            <div>
                <a id="registro" href="#">REGISTRO</a>
                <a id="inicio" href="#">INICIAR SESIÓN</a>
            </div>
        </section>
        <section id="menu">
            <nav>
                <ul>
                    <li><a href="#">INICIO</a></li>
                    <li><a href="#">PORTÁTILES</a></li>
                    <li><a href="#">SOBREMESA</a></li>
                    <li><a href="#">GAMING</a></li>
                    <li><a href="#">PERIFÉRICOS</a></li> 
                </ul>
            </nav>
        </section>
    </header>
</template>

<script>
export default {

}
</script>

<style scoped>

img{
    height: 40px;    
}
#cabeceraArriba{
    display: flex;
    justify-content: space-around;
    margin-bottom: 1rem;
    align-items: center;
}

#logo{
    color: teal;
    font-size: 250%;
}
#nombre{
    color: steelblue;
}

.boton{
    background-color: slategrey;
    color: white;
    padding: 0.4rem;
    border-radius: 15px;
    font-size: 100%;
}
input{
    padding: 0.4rem;
    margin-right: 0.5rem;
    border-radius: 15px;
}

#registro{
    text-decoration: none;
    color: grey;
    background-color: lightblue;
    border-radius: 15px;
    border: black solid 1px;
    padding:0.5rem;
    margin-right: 0.5rem;
}

#inicio{
    text-decoration: none;
    background-color: palegreen;
    border-radius: 15px;
    border: black solid 1px;
    color: grey;
    padding:0.5rem;
}

#menu{
    display: flex;
    justify-content: space-around;
    list-style: none;
    background-color: snow;
}

#menu nav ul{
    display: flex;
    list-style: none;
}

#menu nav ul li{
    margin-right: 3.5rem;
}

#menu nav ul li a{
    text-decoration: none;
    color:cornflowerblue;
    font-size: 150%;
    font-weight: bold;
}
</style>