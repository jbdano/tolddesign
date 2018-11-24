<template>
    <section class="team-overview">
        <div class="to-background-img"></div>
        <div class="to-content">
            <h3 class="to-title">Allow us to introduce ourselves.</h3>
            <p class="to-description">We are engineering graduates turned self-taught web developers, 
                UX designers, and copywriters. Self-taught means we don’t stick to the 
                conventions of the industry. We simply do whatever it takes to do great 
                work and provide the most value to you.</p>
        </div>
    </section>
</template>

<script>
export default {
    name: 'TeamOverview',
}
</script>

<style lang="scss" scoped>

.team-overview {
    height: calc(400px + (400 - 400) * ((100vw - 300px) / (1600 - 300)));
    width: 100%;
    position: relative;
}

.to-background-img {
    height: 100%;
    background: url("../assets/traveling-map.jpeg");
    background-repeat: no-repeat;
    background-size: cover;
    width: 100%;
    filter: grayscale(100%) brightness(20%);
    width: calc(100vw - 30px);
    margin-left: -25px;
    background-position: center;
}

.to-content {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
    width: 100%;
    max-width: 800px;
}

.to-title {
    color: #FCFAF9;
    font-size: calc(24px + (36 - 24) * ((100vw - 300px) / (1600 - 300)));
}

.to-description {
    color: #FCFAF9;
}

</style>
