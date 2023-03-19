<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <!-- <header>
    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header> -->
  <header>
    <h1 class="title">Gabriel Santos</h1>
    <nav class="main-menu">
      <RouterLink to="/" class="menu-item">
        <v-btn color="secondary">
          <v-icon icon="mdi-home" size="large"></v-icon>
          Início
        </v-btn>
      </RouterLink>
      <RouterLink to="/" class="menu-item">
        <v-btn color="secondary">
          <v-icon icon="mdi-package-variant" size="large"></v-icon>
          Soluções
        </v-btn>
      </RouterLink>
      <RouterLink to="/about" class="menu-item">
        <v-btn color="secondary">
          <v-icon icon="mdi-information" size="large"></v-icon>
          Sobre
        </v-btn>
      </RouterLink>
      <RouterLink to="/contact" class="menu-item">
        <v-btn color="secondary">
          <v-icon icon="mdi-at" size="large"></v-icon>
          Contato
        </v-btn>
      </RouterLink>
    </nav>
  </header>

  <RouterView />
</template>

<style scoped>
header {
  display: flex;
  flex-flow: column nowrap;
  align-items: center;
}
.title {
  font-family: 'Times New Roman', Times, serif;
  font-size: 43pt;
  border-bottom: 2px solid #2c3e50;
  padding: 0 50px;
}
.main-menu {
  display: flex;
  flex-flow: row nowrap;
  margin: 20px 0;
}
.menu-item + .menu-item {
  margin-left: 10px;
}
</style>
