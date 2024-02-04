<script>
export default {
    name: 'AppHeader'
};
</script>



<template>
    <header>
        <nav class="container">
            <div class="logo">
                <img src="/IMG/dc-logo.png" alt="">
            </div>
            <ul>
                <li><a href="">CHARACTERS</a></li>
                <li><a href="">COMICS</a></li>
                <li><a href=""></a>MOVIES</li>
                <li><a href="">TV</a></li>
                <li><a href="">GAMES</a></li>
                <li><a href="">COLLECTIBLES</a></li>
                <li><a href="">VIDEOS</a></li>
                <li><a href="">FANS</a></li>
                <li><a href="">NEWS</a></li>
                <li><a href="">SHOP</a></li>
            </ul>
        </nav>
    </header>
</template>



<style scoped>
header {
    height: 100px;
    background-color: var(--dc-light);
    border: 1px solid black;
}

img {
    width: 80%;
}

ul {
    display: flex;
    font-weight: 600;
    font-size: 0.75rem;
    gap: 1rem;
}

li {
    padding: 2rem 0;
}

li:hover {
    border-bottom: 4px solid var(--dc-primary);
    color: var(--dc-primary);
}
</style>
