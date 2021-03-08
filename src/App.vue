<template>
  <v-app>
    <div class="d-flex flex-column">
      <!-- Navigation bar -->
      <div class="d-flex align-center justify-space-around" id="navbar">
        <div class="white--text font-weight-black">
          [logo] Projeto Recomeçar
        </div>

        <div class="white--text font-weight-black">
          Links
        </div>
      </div>

      <!-- Route visualization -->
      <router-view />
    </div>
  </v-app>
</template>

<style lang="scss">
// SASS variables
$primary-color: #1cce1cd7;
$secondary-color: #93a889;

// Global configurations
html {
  overflow-x: none;
}

body {
  width: 100%;
  height: 100%;
  margin: 0;
}

p {
  text-indent: 15px;
}

// General Classes
.container-spacing {
  padding-left: 15vw;
  padding-right: 15vw;
}

.h-100 {
  height: 100vh !important;
}

.h-50 {
  height: 50vh !important;
}

.w-100 {
  width: 100vw !important;
}

.primary-color {
  color: $primary-color;
}

.secondary-color {
  color: $secondary-color;
}

// Specific ID's
#navbar {
  position: fixed;
  height: 5vh;
  width: 100vw;
  background-color: #3e563e;
}
</style>
