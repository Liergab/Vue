<script setup>
import { ref } from 'vue';

    const formData = ref({username:"", email:"", password:""})
</script>

<template>
    <div class="thisContainer">
    <form class="formLayout">
        <input 
            type="text" 
            placeholder="Enter username" 
            class="input" 
            v-model="formData.username"
        >
        <input 
            type="email" 
            placeholder="Enter email" 
            class="input" 
            v-model="formData.email"
        >
        <input 
            type="password" 
            placeholder="Enter password" 
            class="input" 
            v-model="formData.password"
        >
    </form>
    <div class="Output-container">
        <h1 class="text-white">Output</h1>
        <p class="text-white">{{ formData.username }}</p>
        <p class="text-white">{{ formData.email }}</p>
        <p class="text-white">{{ formData.password }}</p>
    </div>
</div>
</template>

<style>
.thisContainer{
    display: flex;
    flex-direction: column;
}
.formLayout{
    display: flex;
    flex-direction: column;
    gap:12px;
    border: 1px solid gray;
    background: gray;
    padding: 16px;
    border-radius: 12px;
}

.input{
    padding: 8px 4px;
    border-radius: 4px;
    border: 1px solid gray;
}

.text-white{
    color: gainsboro;
}

.Output-container{
    display: flex;
    flex-direction: column;
    gap: 10px;
}
</style>