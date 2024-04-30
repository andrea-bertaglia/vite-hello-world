<script>
export default {
    data() {
        return {
            text: "La mia prima app con Vite!"
        }
    },
}
</script>

<template>
    <h2 class="title">{{ text }}</h2>
</template>

<style>
.title {
  background-color: lightseagreen;
  color: greenyellow;
  font-size: 2rem;
  padding: 1em;
  text-align: center;
}
</style>