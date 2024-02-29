<template>
    <div>fffhello
        <li v-for="post of posts" :key="post.slug">
            <NuxtLink :to="post.slug">{{ post.title }}</NuxtLink>
        </li>

        <li v-for="post in posts" :key="post.slug">
            <NuxtLink :to="`/blog/${post.slug}`">{{ post.title }}</NuxtLink>
        </li>
    </div>
</template>
  
<script>
export default {
    async asyncData({ $content }) {
        const posts = await $content("blog").fetch();
        console.log(posts); // Vérifiez les données récupérées dans la console


        return {
            posts,
        };
    },
};
</script>