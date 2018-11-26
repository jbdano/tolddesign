<template>
    <section class="contact">
        <div class="contact-back-filter"></div>
        <div class="contact-grid">
            <h3>Get in touch.</h3>
            <p>Questions? Want a quote? Just want to say, "What's Up?" Use the contact form and we will get back to you the same day.</p>
            <p>Or email us directly at <a href="#">hello@told.design</a>.</p>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Contact',
}
</script>

<style lang="scss" scoped>

.contact {
    background: url("../assets/open-sign.png");
    background-repeat: no-repeat;
    background-size: cover;
    padding: 50px;
    position: relative;
}

.contact-back-filter {
    position: absolute;
    top: 0;
    left: 0;
    height: 100%;
    width: 100%;
    background-color: rgba(0,0,0,.5);
}

.contact-grid {
    position: relative;
    display: grid;
    grid-template-columns: 1fr;

    h1, h2, h3, h4, h5, p, a {
        color: white;
        margin-bottom: 15px;
    }
}

</style>
