<script setup lang="ts">
const { $sayHello } = useNuxtApp();

$sayHello("Guillaume");

const { $hello } = useNuxtApp();

useHead({
    script: [
        { src: "https://identity.netlify.com/v1/netlify-identity-widget.js" },
    ],
});
</script>

<template>
    <div>
        <h2>About me, iiiindex vue</h2>
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