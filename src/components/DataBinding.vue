<template>
    <div class="componente">
        <h1>Componente com Data Binding</h1>
        <p>{{ valor }}</p>
        <!-- <input type="text" v-bind:value="valor"/> -->
        <input type="text" v-bind:value="valor"
        v-on:input="(e)=>valor = e.target.value"/>
    </div>
</template>

<script setup>
import {ref} from "vue"
const valor = ref("Vue é bagual!")
</script>