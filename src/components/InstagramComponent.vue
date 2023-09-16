<template>
    <v-item-group mandatory>
        <v-lazy :min-height="200" :options="{ 'threshold': 0.5 }" transition="fade-transition">
            <v-row dense="true">
                <v-col v-for="(_,n) in 500" cols="4" offset-lg="1px" offset="1px">
                    <v-img :src="`https://picsum.photos/500/300?image=${n * 5 + 10}`"
                    :lazy-src="`https://picsum.photos/10/6?image=${n * 5 + 10}`"
                     aspect-ratio="1" cover>
                    </v-img>
                </v-col>
            </v-row>
        </v-lazy>
    </v-item-group>
</template>
<script setup></script>