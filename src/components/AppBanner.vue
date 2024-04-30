<script>
export default {
    data() {
        return {
            title: "Foto di una montagna",
            image: "mountain.jpg",
        };
    },
    methods: {
        getImagePath(imageName) {
            return new URL(`../assets/img/${imageName}`, import.meta.url).href
        },
    },
};
</script>

<template>
    <div class="banner">
        <img :src="getImagePath(image)" :alt="`${title}`">
        <h3>{{ title }}</h3>
    </div>
</template>

<style>
.banner {
    border: 5px dashed green;
    margin-top: 10px;
    max-width: 500px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 1em;
    padding: 1em;
    margin: 0 auto;
    font-family: Verdana, Geneva, Tahoma, sans-serif;
}

.banner img {
    max-width: 100%;
    
}
</style>