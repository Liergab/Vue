<script setup>
import { ref} from 'vue';
   
const username =ref("")
const email =ref("")
const password =ref("")
  

</script>

<template>

    <form @submit.prevent="$emit('userInfo', username, email, password)">
        <input type="text" placeholder="username" v-model="username">
        <input type="text" placeholder="email" v-model="email">
        <input type="password" placeholder="password" v-model="password">
        <button type="submit">submit</button>
    </form>
 
</template>