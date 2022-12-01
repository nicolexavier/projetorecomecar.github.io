<template>
  <v-app>
    <!-- Navigation bar -->
    <div class="d-flex align-center justify-center" id="navbar">
			<img src="./assets/logo.png" style="width: 25px; height:25px; margin-right: 20px;"/>
      <div class="white--text font-weight-black">
        Projeto Recomeçar
      </div>
    </div>

    <!-- Route visualization -->
    <router-view />
  </v-app>
</template>

<style lang="scss">
// SASS variables
$primary-color: #1cce1cd7;
$secondary-color: #93a889;

// Global configurations
html {
  min-height: 100%;
  overflow-y: scroll;
  overflow-x: none;
}

body {
  width: 100%;
  height: 100%;
  min-height: 100%;
  margin: 0px;
  padding: 0px;
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

.main-text {
  font-size: 1rem;
}

// Specific ID's
#navbar {
  height: 5vh;
  background-color: #3e563e;
}

@media (max-width: 960px) {
  .main-text {
    font-size: 1rem;
  }
}

@media (min-width: 961px) {
  .main-text {
    font-size: 1.2rem;
  }
}
</style>
