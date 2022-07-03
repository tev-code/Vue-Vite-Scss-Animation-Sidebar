<template>
  <div class="app">
  <Sidebar />
  <router-view/>
  </div>

</template>
<script setup>
import Sidebar from './components/Sidebar.vue'

</script>

<style lang="scss">
:root {
  --primary: #fcd34d;
  --grey:#f59e0b;
  --dark:#d97706 ;
  --dark-alt: #b45309;
  --light: #fafafa;
  --sidebar-width: 300px;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Gantari', sans-serif;
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

    @media (max-width) {
      padding-left: 6rem;
    }
  }
}

</style>
