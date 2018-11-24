<template>
    <section class="home-hero">
        <div class="hh-background-img"></div>
        <div class="hh-content theme-color-white">
            <h1 class="hh-title"><span class="theme-color-green">told</span>.design</h1>
            <p class="hh-subtitle">website and content development for mission-driven startups</p>
            <div class="hh-button-group">
                <a class="theme-inline-button theme-inline-button-primary" href="#">WORK WITH US</a>
                <a class="theme-inline-button theme-inline-button-secondary" href="#">VIEW PORTFOLIO</a>
            </div>
        </div>
    </section>
</template>

<script>
export default {
  name: 'HomeHero',
};
</script>

<style lang="scss" scoped>

.home-hero {
    height: 100vh;
    width: 100%;
    position: relative;

    @media screen and (min-width: 768px) {
        height: 90vh;
    }
}

.hh-background-img {
    height: 100%;
    background: url("../assets/iphone-desk-laptop-notebook.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    width: 100%;
    filter: grayscale(100%) brightness(50%);
}

.hh-content {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
    width: 100%;
    max-width: calc(100vw - 50px);
}

.hh-title {
    margin-bottom: 50px;
    color: #FCFAF9;
}

.hh-subtitle {
    font-size: calc(18px + (24 - 18) * ((100vw - 300px) / (1600 - 300)));
    margin-bottom: 50px;
    color: #FCFAF9;
}

.hh-button-group > a {

    @media screen and (max-width: 450px) {
        display: block;
        border-radius: 0px;
    }

    &:first-child {
        @media screen and (min-width: 450px) {
            margin-right: 25px;
        }
    }
}

</style>
