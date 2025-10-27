<template>
    <div id="parimpar">
        <h1>Par e Impar</h1>
        <button @click="numeroRandom">Generar número aleatorio</button>
        <h2>El número generado es: {{ numero }}</h2>
        <h3 v-if="numero === 0" style="color:green">El número es CERO</h3>
        <h3 v-else-if="numero % 2 === 0" style="color:blue">El número es PAR</h3>
        <h3 v-else style="color:red">El número es IMPAR</h3>
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
                this.numero = parseInt(Math.random() * 51);
            }
        }

}
</script>

<style>
#parimpar {
    text-align: center;
    background-color: aqua;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 2px 2px 10px gray;
    margin: 20px;
}

#parimpar button {
    padding: 10px 20px;
    font-size: 16px;
    border: none;
    border-radius: 5px;
    background-color: lightgray;
    cursor: pointer;
    box-shadow: 2px 2px 5px gray;
    transition: background-color 0.3s, color 0.3s;

}
#parimpar button:hover {
    background-color: gray;
    color: white;

}
</style>
