<template>
    <!-- :style="{'background-image': `url('${imageUrl}')`}" -->
    <v-parallax class="card" :src="imageUrl">
            <div class="container" >
                <div class="card__overlay"></div>
                <div class="card__title">{{ brandName }}</div>
                <v-btn class="card__button"  rounded="0" variant="outlined">Смотреть</v-btn>
            </div>
    </v-parallax>
</template>

<script setup>



defineProps({
    imageUrl: String,
    brandName: String,
})

</script>

<style lang="scss" scoped>


.container {
    color: #fff;
    display: flex;
    flex-direction: column;
    opacity: 0;
    transition: .2s;
    justify-content: center;
    gap: 3em;
    align-items: center;
    height: 100%;
}
.card {
    
    // background-repeat: no-repeat;
    // background-size: cover;
    &:hover {
        .container {
            opacity: 1;
            transition: .2s;
        }
        .card__button,
        .card__title {
            transition: .2s;
            opacity: 1;
            transform: translateY(0);
        }
    }
    position: relative;
    height: 65vh;
    // background-position: center;
    width: 50%;
    &__title {
        z-index: 1;
        opacity: 0;
        transform: translateY(200px);
        transition: .2s;
        font-size: 64px;
        font-family: 'DM Serif Display', serif;
        color: #fff;
    }
    &__button {
        transition: .2s;
        opacity: 0;
        transform: translateY(200px);
    }
    &__overlay {
        z-index: 0;
        position: absolute;
        top: 0;
        bottom: 0;
        left: 0;
        right: 0;
        background-color: rgba(0, 0, 0, 0.525);
    }
}


</style>
