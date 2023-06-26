<template>
    <div class="home-sales" id="home-sales">
        <div class="home-sales__title">РАСПРОДАЖИ</div>
        <HomeSalesCarousel/>
    </div>
</template>

<script setup>

import HomeSalesCarousel from './carousel/HomeSalesCarousel.vue'

</script>

<style lang="scss" scoped>

.home-sales {
    display: flex;
    flex-direction: column;
    align-items: center;
    background-color: #000;

    &__title {
        padding: 32px 0;
        text-align: center;
        font-size: 32px;
        font-family: 'Oswald', sans-serif;
        letter-spacing: 1em;
        color: #fff;
    }
}





</style>