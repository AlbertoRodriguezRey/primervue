<template>
    <div>
        <h1>Ejemplo directivas</h1>
        <h3>{{ $data }}</h3>
        <ul v-if="series.length > 0">
            <li v-for="serie in series" :key="serie">
                {{ serie }}
            </li>

        </ul>
        <label>Añadir serie:</label><br/>
        <input type="text" v-model="serieNueva"/><br/>
        <button @click="añadirSerie">Añadir serie</button><br/>
        <label>Introduce un nombre:</label><br/>
        <input type="text" v-model="nombre"/><br/>
        <label>Introduce un número:</label><br/>
        <input type="number" v-model="numero"/><br/>
        <h3 v-if="numero > 0" style="color:green">POSITIVO</h3>
        <h3 v-else-if="numero < 0" style="color:red">NEGATIVO</h3>
        <h3 v-else style="color:darkblue">CERO</h3>


    </div>
</template>

<script>
    export default {
        name: "DirectivasComponent",
        data() {
            return {
                numero: 0,
                series: ['Breaking Bad', 'La casa de papel', 'Juego de tronos', 'Los Soprano'],
                nombre: 'Alberto',
                serieNueva: ""
            }
        },
        methods: {
            añadirSerie() {
                this.series.push(this.serieNueva);

            }
        }
    }
</script>

<style>
 h1 {
     color: blue;
 }
</style>