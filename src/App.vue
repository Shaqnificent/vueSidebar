<template>
  <div class="app">
    <Sidebar />
    <router-view />
  </div>

</template>

<script setup>
import Sidebar from './components/Sidebar.vue'
</script>

<style lang="scss">
:root {
  --primary: blue;
  --primary-alt: lightBlue;
  --grey: grey;
  --dark: black;
  --dark-alt: darkGrey;
  --light: lightGrey;
  --sidebar-width: 300px;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Fira sans', sans-serif;
}

body {
  background: var(--light);
}

button {
  cursor: pointer;
  appearance: none;
  border: none;
  outline: none;
  background: none;
}
.app {
  display: flex;

  main {
    flex: 1 1 0;
    padding: 2rem;

    @media (max-width: 768px){
      padding-left: 6rem;
    }
  }
}

</style>
