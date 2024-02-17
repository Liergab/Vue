<script setup>
import {computed, reactive, ref} from 'vue';

const count = ref(0)

const IncrementHandle = () => {
    count.value++
}

const sample = computed(() => {
    return count.value
})





</script>

<template>
    <h2>{{ sample }}</h2>
    <h1>Count: {{ count }}</h1>
    <button @:click="IncrementHandle">Increment</button>
</template>