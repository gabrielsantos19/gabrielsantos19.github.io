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
  <header class="header">
    <img class="logo" src="@/assets/logos/gabriel_santos.svg">
    <!-- <h1 class="title">Gabriel Santos</h1> -->
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

  <RouterView class="router-view" />
</template>

<style scoped>
.header {
  max-width: 100%;
  display: flex;
  flex-flow: column nowrap;
  align-items: center;
  overflow: hidden;
}
.logo {
  width: 550px;
  max-width: 98%;
  padding: 20px 30px;
}
.title {
  flex: 1 1 auto;
  font-family: 'Times New Roman', Times, serif;
  padding: 0 50px;
  text-align: center;
  font-size: 7vh;
  white-space: nowrap;
}
.main-menu {
  max-width: 100%;
  display: flex;
  flex-flow: row nowrap;
  padding: 10px 35px;
  overflow: auto;

  border: 0 solid #2c3e50;
  border-width: 1.5px 0;
}
.menu-item + .menu-item {
  margin-left: 10px;
}
.router-view {
  max-width: 100%;
  overflow: hidden;
}
</style>
