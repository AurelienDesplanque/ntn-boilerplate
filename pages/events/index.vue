
  
<script>
export default {
    async asyncData() {
        console.log("je rr");
    },
};
</script>

<template>
    <div>
        <li v-for="post of posts" :key="post.slug">
            <NuxtLink :to="post.slug">{{ post.title }}</NuxtLink>
        </li>
    </div>
</template>