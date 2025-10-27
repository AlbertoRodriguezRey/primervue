<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <div>
    <h3>Hola a quien este viendo</h3>
    <h1 style="color:red" id="estatico">Elemento estatico</h1>
    <MenuComponente/>
    <hr/>
    <router-view></router-view>
  </div>
  <!-- <HolaMundo/>
  <CineComponent/>
  <MusicaComponent/>
  <HomeComponent/> -->
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import HolaMundo from './components/HolaMundo.vue'
// import CineComponent from './components/CineComponent.vue'
// import MusicaComponent from './components/MusicaComponent.vue'
// import HomeComponent from './components/HomeComponent.vue'
import MenuComponente from './components/MenuComponent.vue'


export default {
  name: 'App',
  components: {
    // HelloWorld,
    // HolaMundo,
    // CineComponent,
    // MusicaComponent,
    // HomeComponent
    MenuComponente
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

#estatico {
  transition: font-size 0.4s;
}
#estatico:hover {
  font-size: 40px;
}
</style>
