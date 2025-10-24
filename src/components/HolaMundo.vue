<template>
  <div>
    <h1>Mi primer vue de viernes, que ilusion!!!</h1>
    <img src="../assets/images/logoChampions.png"/>
    <h2>Mi nombre es: {{nombre}}</h2>
    </div>
</template>

<script>
//VUE UTILIZA CODIGO JS (ESPECIAL)
//CADA COMPONENT QUE GENEREMOS DEBE TENER UN NOMBRE OBLIGATORIO
//Y DEBEMOS EXPORTARLO CON DICHO NOMBRE. EL name ES LA ETIQUETA QUE
//UTILIZARAN OTROS COMPONENTES PARA DIBUJARLO
export default {
  name: "HolaMundo",
  data() {
    //LAS VARIABLES SON DECLARADAS EN FORMATO JSON
    //DENTRO DE UN RETURN
    return {
        nombre: "Alberto Rodriguez-Rey",
        edad: 25,
        aficiones: ["Programar", "dormir", "Jugar"],
        direccion: { calle: "Calle Falsa", numero: 123, ciudad: "Springfield"}
    }
  }
};
</script>

<style>
h1 {
  color: blue;
}
@import '../assets/css/estilos.css';
</style>
