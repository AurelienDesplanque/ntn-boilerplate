
  
<script setup>
asyncData({ $content }) {
    console.log("je rr");
    const posts = await $content("blog").fetch();

    return {
        posts,
    };
};
</script>

<template>
    <div>
        <li v-for="post of posts" :key="post.slug">
            <NuxtLink :to="post.slug">{{ post.title }}</NuxtLink>
        </li>
    </div>
</template>