<template>
    <div>
        <h1>Par e Impar</h1>
        <button @click="numeroRandom">Generar número aleatorio</button>
        <h2>El número generado es: {{ numero }}</h2>
        <h3 v-if="numero % 2 === 0" style="color:green">El número es PAR</h3>
        <h3 v-else style="color:blue">El número es IMPAR</h3>
    </div>
</template>

<script>
export default {
    name: "ParImpar",
    data() {
        return {
            numero: 0
        }
    },
    methods: {
            numeroRandom() {
                this.numero = Math.floor(Math.random() * 100) + 1;
            }
        }

}
</script>
