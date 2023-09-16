<template>
    <v-item-group mandatory>
        <v-lazy :min-height="200" :options="{ 'threshold': 0.5 }" transition="fade-transition">
            <v-row dense="true">
                <v-col v-for="_ in 500" cols="4" offset-lg="1px" offset="1px">
                    <v-img src="../assets/m" aspect-ratio="1/1" cover>
                    </v-img>
                </v-col>
            </v-row>
        </v-lazy>
    </v-item-group>
</template>
<script setup></script>