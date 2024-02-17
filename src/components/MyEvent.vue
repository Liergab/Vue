<script setup>
import { ref, reactive } from 'vue';


let count = ref(0);

const HandleIncrement = () => {
    count.value++
}

</script>

<template>
    <h1>Count:{{ count }}</h1>
    <button @:click="HandleIncrement">Increment</button>
</template>