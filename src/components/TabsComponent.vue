<template>
    <v-tabs v-model="tab" bg-color="transparent" color="black" grow >
        <v-tab v-for="item in items" :key="item" :value="item" color="black" >
            {{ item }}
        </v-tab>
    </v-tabs>

    <v-window v-model="tab">

        <v-window-item value="INSTAGRAM">
            <Instagram></Instagram>
        </v-window-item>

        <v-window-item value="TIKTOK">
            <Tiktok></Tiktok>
        </v-window-item>

    </v-window>
</template>
<script setup>
import Instagram from './InstagramComponent.vue'
import Tiktok from './TiktokComponent.vue'


import { ref } from 'vue'
const items = ref(['INSTAGRAM', 'TIKTOK'])
const text = ref('INSTAGRAMTIKTOK')
const tab = ref('INSTAGRAMTIKTOK')


</script>