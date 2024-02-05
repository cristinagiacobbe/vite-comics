<script>
export default {
    name: 'ComicCards',
    props: {
        image: String,
        title: String,
    }
}
</script>



<template>
    <img :src="image" alt="">
    <h4>{{ title }}</h4>
</template>

<style scoped>
img {
    width: 100%;
}

h4 {
    color: white;
    text-transform: uppercase;
}
</style>

