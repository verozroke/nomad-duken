<template>
    <div class="home-topical" id="home-topical ">
        <div class="home-topical__title">АКТУАЛЬНО</div>
        <HomeTopicalGrid/>
    </div>
</template>

<script setup>
import HomeTopicalGrid from './grid/HomeTopicalGrid.vue';

</script>

<style lang="scss" scoped>


.home-topical {
    display: flex;
    flex-direction: column;
    background-color: #000;

    align-items: center;
    &__title {
        padding: 32px 0;
        text-align: center;
        background-color: #000;
        font-size: 32px;
        font-family: 'Oswald', sans-serif;
        letter-spacing: 1em;
        color: #fff;
    }
}

</style>