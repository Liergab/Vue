<script setup>
import { ref } from 'vue';
import FromChild from './components/FromChild.vue';

const handleInfo = (email, username, password) => {
  console.log(email)
  console.log(username)
  console.log(password)
}
</script>


<template>
  <div class="container">
   <FromChild @userInfo="handleInfo"/>
  </div>
</template>


<style>
.container{
  background: #F8DFD4;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}

</style>
