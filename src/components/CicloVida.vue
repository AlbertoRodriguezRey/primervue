<template>
  <div>
    <h1>Ciclo vida y métodos VUE</h1>
    <h2 style="color: red">{{ mensaje }}</h2>
    <button v-on:click="cambiarMensaje()">Cambiar Mensaje v-on:</button><br />
    <button @click="cambiarMensaje()">Camibar mensaje @Click</button>
  </div>
</template>

<script>
export default {
  name: "CicloVida",
  data() {
    return {
      mensaje: "Hoy es viernes!!!",
    };
  },

  methods: {
    //AQUI INCLUIMOS NUESTROS METODOS PERSONALIZADOS
    cambiarMensaje() {
      //PARA ACCEDER A LAS VARIABLES DE data() DEL COMPONENT
      //DEBEMOS USAR LA PALABRA this
      this.mensaje = "Hoy se sale!!!";
    },
  },

  mounted() {
    console.log("El componente se ha montado ");
  },
  created() {
    console.log("El componente se ha creado ");
  },
  updated() {
    console.log("El componente se ha actualizado ");
  },
  unmounted() {
    console.log("El componente se ha destruido ");
  },
};
</script>
