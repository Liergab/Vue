<script setup>
import { ref } from 'vue';

const isShow = ref(true)

const handleClick = () => {
    isShow.value = !isShow.value
}
</script>

<template>
    <!-- using v-if v-else if else v-show -->
<h1>{{ isShow ? "true" :"false" }}</h1>
<button @click="handleClick">toggle</button>
</template>