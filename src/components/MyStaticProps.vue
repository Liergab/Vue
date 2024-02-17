<script setup>

const props = defineProps(['name','sample','Data'])
</script>

<template>
    <div class="MyContainer">
        <h1>{{ props.name }}</h1>
        <ul v-for="(s) in props.sample" key="s">
            <li>{{ s }}</li>
        </ul>
        <ul v-for="(d) in props.Data" :key="d.id">
            <li>{{ d.name }}</li>
            <li>{{ d.post }}</li>
        </ul>
    </div>
</template>

<style>
.MyContainer{
    display: flex;
    flex-direction: column;
}
</style>