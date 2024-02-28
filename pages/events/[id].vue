<script setup>
    
    const route= useRoute();
    console.log(route.params);
</script>

<template>
    <div>
        event id: {{ $route.params.id }}
    </div>
</template>