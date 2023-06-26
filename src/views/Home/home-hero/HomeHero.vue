<template>
    <v-parallax src="/img/homehero.jpg" id="HomeHero" class="hero">
        <div class="hero__overlay"></div>
        <div class="hero__container">
            <div class="hero__title">
                NOMAD DÜKEN
            </div>
            <ul class="hero__nav">
                <!-- TODO: v-for) -->
                <li><v-btn @click="scrollDown('home-brands')" rounded="0"  variant="outlined">Бренды</v-btn></li>
                <li><v-btn rounded="0"  variant="outlined">Новинки</v-btn></li>
                <li><v-btn @click="scrollDown('home-topical')" rounded="0"  variant="outlined">Актуально</v-btn></li>
                <li><v-btn @click="scrollDown('home-sales')"  rounded="0"  variant="outlined">Распродажи</v-btn></li>
                <li><v-btn rounded="0"  variant="outlined">Товары</v-btn></li>
            </ul>
        </div>
    </v-parallax>
</template>

<script setup>
function scrollDown(blockID) {
    const $block = document.getElementById(blockID);
    $block.scrollIntoView({
        behavior: 'smooth',
        block: 'start'
    })
}

</script>

<style lang="scss" scoped>

.hero {
    position: relative;
    height: calc(100vh - 75px);
    &__container {
        font-weight: 300;
        height: 100%;
        flex-direction: column;
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 5em;
        z-index: 1;
    }
    &__overlay {
        z-index: 0;
        position: absolute;
        top: 0;
        bottom: 0;
        left: 0;
        right: 0;
        background-color: rgba(0, 0, 0, 0.497);
    }
    &__title {
        z-index: 1;
        font-size: 150px;
        font-family: 'DM Serif Display', serif;
        color: #fff;
    }
    &__nav {
        color: #fff;
        width: 1000px;
        display: flex;
        justify-content: space-between;
    }
}

</style>