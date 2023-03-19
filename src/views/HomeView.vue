<script setup>
import TheWelcome from '../components/TheWelcome.vue'
import { RouterLink } from 'vue-router'
import Solutions from '@/assets/solutions.js'
</script>

<template>
  <main>
    <h1>Soluções</h1>
    <div class="portifolio">
      <v-card
        v-for="solution in Solutions"
        class="card"
        :title="solution.title"
        :subtitle="solution.subtitle"
        :text="solution.text"
      >
        <v-card-actions>
          <v-btn :href="solution.page">
            Ver mais
          </v-btn>
        </v-card-actions>
      </v-card>
    </div>
  </main>
</template>

<style scoped>
main {
  flex: 1;
  display: flex;
  flex-flow: column nowrap;
  align-items: center;
}
.portifolio {
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
}
.card {
  width: 300px;
  margin: 20px;
}
</style>