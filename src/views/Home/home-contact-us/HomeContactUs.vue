<template>
    <div class="home-contact-us">
        <div class="home-contact-us__title">СВЯЖИТЕСЬ С НАМИ</div>
        <div class="list">
            <v-btn size="large" rounded="lg"  prepend-icon="$vuetify" color="#E1306C" class="text-white text-capitalize" stacked>
            Наш Instagram
            </v-btn>            
            <v-btn size="large" rounded="lg" prepend-icon="$vuetify" color="#0088cc" class="text-white text-capitalize" stacked>
                Наш Telegram
            </v-btn>            
            <v-btn size="large" rounded="lg"  prepend-icon="$vuetify" color="#25D366" class="text-white text-capitalize"  stacked>
                Наш Whatsapp
            </v-btn>
        </div>
    </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>

.home-contact-us {
    background-color: #000;
    display: flex;
    flex-direction: column;
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


.list {
    display: flex;
    gap: 5em;
}

</style>