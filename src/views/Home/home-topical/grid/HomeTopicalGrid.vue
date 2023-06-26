<!-- eslint-disable vue/no-v-text-v-html-on-component -->
<template>
    <v-row dense class="grid">
        <v-col v-for="card in cards" :key="card.title" :cols="card.flex">
            <v-card   theme="dark">
                <v-img
                :src="card.src"
                style="text-align: center;"
                class="align-center"
                gradient="to bottom, rgba(0,0,0,.4), rgba(0,0,0,.7)"
                height="400px"
                cover
                >
                    <v-card-title
                        class="text-white card-title"
                        v-text="card.title"
                    ></v-card-title>
                </v-img>

                <v-card-actions style="font-size: 20px; padding: 0 20px;">
                    {{ card.text }} 
                <v-spacer></v-spacer>
                    <v-btn icon="mdi-arrow-right" class="text-capitalize"/>
                </v-card-actions>
            </v-card>
        </v-col>
    </v-row>
</template>

<script setup>
import { ref } from 'vue';


const cards = ref([
        {
            title: 'Сделано в Италии',
            text: 'Легендарные бренды',
            src: 'https://images.unsplash.com/photo-1545007805-a44ee83438fa?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1170&q=80',
            flex: 6,
        },
        {
            title: 'Добавьте цвета',
            text: 'В летние образы',

            src: 'https://images.unsplash.com/photo-1619166719123-471cee9ce91e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1170&q=80',
            flex: 6,
        },
        {
            title: 'Наивные украшения',
            text: 'Ностальгия по детству',

            src: 'https://images.unsplash.com/photo-1545007805-a44ee83438fa?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1170&q=80',
            flex: 12,
        },        {
            title: 'Наивные украшения',
            text: 'Ностальгия по детству',

            src: 'https://images.unsplash.com/photo-1545007805-a44ee83438fa?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1170&q=80',
            flex: 4,
        },        {
            title: 'Наивные украшения',
            text: 'Ностальгия по детству',

            src: 'https://images.unsplash.com/photo-1545007805-a44ee83438fa?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1170&q=80',
            flex: 4,
        },        {
            title: 'Наивные украшения',
            text: 'Ностальгия по детству',

            src: 'https://sevimi.by/wp-content/uploads/2020/08/stilnye-zhenskie-ukrasheniya.jpg',
            flex: 4,
        },
])

</script>

<style lang="scss" scoped>

.grid {
    width: 90%;
    font-family: 'Roboto Slab', serif;
}


.card-title {
    letter-spacing: 5px;
    font-size: 32px;
}



</style>