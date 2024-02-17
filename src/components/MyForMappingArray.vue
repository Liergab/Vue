<script setup>
import { ref } from 'vue';

const arrays = ref([
    {name:'Bryan',id:1}, 
    {name:'Gab',id:2}, 
     {name:'Ian',id:3},
    ])
</script>

<template>
    <ul>
        <li v-for="(array) in arrays" :key="array.id">{{ array.name }} {{ array.id }}</li>
    </ul>
 
</template>