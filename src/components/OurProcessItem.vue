<template>
    <article class="op-grid-item">
        <i :class="[ 'op-grid-img', iconClass ]" v-bind:style="{ color: iconColor }"></i>
        <h4 class="op-grid-title" v-text="title"></h4>
        <p class="op-grid-desc"></p>
    </article>
</template>

<script>
export default {
    name: 'OurProcessItem',
    props: {
        iconClass: String,
        iconColor: String,
        title: String
    }
}
</script>

<style lang="scss" scoped>

.op-grid-img {
    font-size: 100px;
}

</style>
