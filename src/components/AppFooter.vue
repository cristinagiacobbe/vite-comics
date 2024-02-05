<script>
import SocialIcons from './SocialIcons.vue'

export default {
    name: 'AppFooter',
    components: {
        SocialIcons,
    },
    data() {
        return {
            icons: ["/IMG/footer-facebook.png", "/IMG/footer-periscope.png", "/IMG/footer-pinterest.png", "/IMG/footer-twitter.png", "/IMG/footer-youtube.png"]
        }
    }
};

</script>

<template>
    <div class="top_footer">
        <div class="container">
            <div class="row">
                <div class="col-2">
                    <h4>DC COMICS</h4>
                    <ul>
                        <li>Character</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                    <h4>SHOP</h4>
                    <ul>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>
                    </ul>
                </div>
                <div class="col-2">
                    <h4>DC</h4>
                    <ul>
                        <li>Terms of use</li>
                        <li>Privacy policy</li>
                        <li>Ad choices</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent workshops</li>
                        <li>CPSC Certificates</li>
                        <li>Ratings</li>
                        <li>Shop Help</li>
                        <li>Contact us</li>
                    </ul>
                </div>
                <div class="col-2">
                    <h4>SITES</h4>
                    <ul>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Powwer Visa</li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
    <div class="bottom_footer">
        <div class="container">
            <div class="follow">
                <h4>FOLLOW UP</h4>
            </div>
            <div class="social_icons" v-for="icon in icons">
                <SocialIcons :icon="icon"></SocialIcons>
            </div>
        </div>
    </div>
</template>


<style scoped>
.top_footer {
    background-image: url('./IMG/dc-logo-bg.png'), url('./IMG/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: 500px, cover;
    background-position: 80%, top;
    height: 400px;
}

.row {
    display: flex;
    gap: 5rem
}

.col-2 {
    width: calc(100% / 12 * 2);
    color: var(--dc-light);
    font-size: small;
}

ul {
    list-style: none;
    padding-left: 0;
    margin-left: 0;
}

h4 {
    margin-top: 2rem;
    font-weight: 700;
    color: var(--dc-light);

}

.bottom_footer {
    background-color: var(--dc-dark);
}

.bottom_footer>.container {
    justify-content: end;
    gap: 1rem;

    height: 50px;
}

.follow h4 {
    color: var(--dc-primary);
    align-items: center;
}
</style>