<script setup lang="ts">
const { $sayHello } = useNuxtApp();

$sayHello("Guillaume");

const { $hello } = useNuxtApp()
</script>

<template>
    <div>
        <h2>hezzzz guys About, iiiindex vue</h2>
        <img src="@/assets/img1.png" />
        <Alert />
    </div>
</template>

<style scoped>
h2 {
    margin-bottom: 20px;
    font-size: 36px;
}
</style>