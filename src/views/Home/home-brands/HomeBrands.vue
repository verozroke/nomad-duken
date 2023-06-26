<template>
    
    <div class="home-brands" id="home-brands">
        <div class="home-brands__title">БРЕНДЫ</div>
        <div class="home-brands__list">
            <HomeBrandCard brand-name="Qazaq Republic" image-url="https://scontent.fnqz4-1.fna.fbcdn.net/v/t39.30808-6/312245491_461216669323977_3585987865193258719_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=730e14&_nc_ohc=iq_9pNuP8KsAX-ewGs_&_nc_ht=scontent.fnqz4-1.fna&oh=00_AfCEj3X7rf4RtgqUblLCXs0jrffJ0Q5uDRGeGHV5itk33g&oe=649EABC6"/>
            <HomeBrandCard image-url="/img/1.jpg" brand-name="Zardozi" />
            <HomeBrandCard image-url="/img/2.jpg" brand-name="Etéreo"/>
            <HomeBrandCard image-url="https://a.lmcdn.ru/img600x866/M/P/MP002XW04JDO_12982612_4_v1.jpeg" brand-name="Urban Whisper"/>
        </div>
    </div>
</template>

<script setup>
import HomeBrandCard from './HomeBrandCard.vue';


</script>

<style lang="scss" scoped>

.home-brands {
    display: flex;
    flex-direction: column;
    &__title {
        padding: 32px 0;
        text-align: center;
        background-color: #000;
        font-size: 32px;
        font-family: 'Oswald', sans-serif;
        letter-spacing: 1em;
        color: #fff;
    }
    &__list {
        width: 100%;
        display: flex;
        flex-wrap: wrap;
    }
}

</style>