<script setup>
import Header from './components/HeaderComponent.vue'
import Tabs from './components/TabsComponent.vue'

</script>

<template>
  <v-app>
    <v-container>
      <Header></Header>
      <v-main>
        <Tabs></Tabs>
      </v-main>
    </v-container>
  </v-app>
</template>

<style scoped>
@media (min-width: 1280px) {
  .v-container{
    width: 900px !important;
  }
}
#app{
  background-color: aqua !important;
}
</style>
