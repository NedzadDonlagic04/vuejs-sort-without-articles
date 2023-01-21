<script setup>
import { ref } from 'vue';

const bands = ref(['The Plot in You', 'The Devil Wears Prada', 'Pierce the Veil', 'Norma Jean', 'The Bled', 'Say Anything', 'The Midway State', 'We Came as Romans', 'Counterparts', 'Oh, Sleeper', 'A Skylit Drive', 'Anywhere But Here', 'An Old Dog']);

</script>

<template>
    <ul class="container">
        <li v-for="band in bands">{{band}}</li>
    </ul>
</template>

<style scoped>
    .container {
        background-color: white;
        width: 500px;
        list-style: inside square;
        border-radius: 5px;
        box-shadow: -3px -3px 10px black;
    }

    .container > li {
        width: 100%;
        border-bottom: 1px solid gray;
        padding: 1rem;
    }

    .container > li:last-child {
        border-bottom: none;
    }
</style>