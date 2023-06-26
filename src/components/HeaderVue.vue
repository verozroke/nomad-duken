<template>
    <header class="header">
        <div class="header__main">
            <div class="header__title">NOMAD DÜKEN</div>
            <!-- <div class="header__login">
                <v-btn class="ma-2 text-black" color="orange-darken-2" >
                    <v-icon start icon="mdi-arrow-left"></v-icon>
                    Back
                </v-btn>
            </div> -->
        </div>
        <div class="header__nav">
            <ul>
                <!-- TODO: v-for) -->
                <li><v-btn height="25"  rounded="0" variant="text" class="text-capitalize">Одежда</v-btn></li>
                <li><v-btn height="25" rounded="0"  variant="text" class="text-capitalize">Обувь</v-btn></li>
                <li><v-btn height="25" rounded="0"  variant="text" class="text-capitalize">Аксессуары</v-btn></li>
                <li><v-btn height="25" rounded="0"  variant="text" class="text-capitalize">Спорт</v-btn></li>
                <li><v-btn height="25" rounded="0"  variant="text" class="text-capitalize">Красота</v-btn></li>
                <li><v-btn height="25" rounded="0"  variant="text" class="text-capitalize">Дом</v-btn></li>
            </ul>
        </div>
    </header>
</template>

<script setup>

</script>

<style lang="scss" scoped>

.header {
    position: sticky;
    top: 0;
    z-index: 3;
    &__main {
        display: flex;
        color: #fff;

        align-items: center;
        justify-content: center;
        background-color: #000;
        height: 50px;
    }

    &__title {
        z-index: 1;
        font-size: 24px;
        font-family: 'DM Serif Display', serif;
    }
    
    &__nav {
        display: flex;
        justify-content: center;
        align-items: center;
        & ul {
            display: flex;
            height: 25px;    
        }
        color: #fff;
        
        background-color: #000;
        height: 25px;
    }
}

</style>