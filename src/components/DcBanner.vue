<script>
export default {
    name: 'DcBanner',
    props: {
        icon: String,
        text: String,
    },

};
</script>


<template>
    <img :src="icon" alt="">
    <span>{{ text }}</span>
</template>






<style scoped>
span {
    color: var(--dc-light);
    text-transform: uppercase;
    font-size: 10px;
    padding-left: 1rem;
}

img {
    width: 30%;
}
</style>