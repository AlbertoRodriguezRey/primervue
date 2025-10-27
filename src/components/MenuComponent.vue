<template>
    <div>
        <ul id="menu">
            <li>
                <router-link to="/">Home</router-link>
            </li>
            <li>
                <router-link to="/ciclovida">Ciclo Vida</router-link>
            </li>
            <li>
                <router-link to="/parimpar">Par e Impar</router-link>
            </li>
            <li>
                <router-link to="/directivos">Directivas</router-link>
            </li>
            <li>
                <router-link to="/cine">Cine</router-link>
            </li>
            <li>
                <router-link to="/musica">Musica</router-link>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: "MenuComponent"
}
</script>

<style>
    ul#menu li {
        display: inline;
        margin-right: 2px;
        background-color: lightgrey;
        padding: 10px;
        border-radius: 5px;
        box-shadow: 2px 2px 5px gray;
        transition: background-color 0.6s, color 0.6s;
        transition: font-size 0.4s;
    }
    
    ul#menu li a {
        text-decoration: none;
        color: black;
        font-family:'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
        font-weight:bold;
    }

    ul#menu li:hover {
        background-color: gray;
        font-size: 20px;
    }
</style>