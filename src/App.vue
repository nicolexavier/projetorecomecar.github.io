<template>
  <v-app>
    <div class="d-flex flex-column h-100">
      <!-- Navigation bar -->
      <div class="d-flex align-center justify-space-around" id="navbar">
        <div class="flex-same-width white--text font-weight-black">
          (logo) Projeto Recomeçar
        </div>
        <div class="flex-same-width">
          <router-link to="/">Home</router-link> |
          <router-link to="/about">About</router-link>
        </div>
        <div class="flex-same-width white--text">
          Links
        </div>
      </div>

      <!-- Route visualization -->
      <div id="background">
        <div id="main-container" class="d-flex align-center justify-center">
          <router-view />
        </div>
      </div>
    </div>
  </v-app>
</template>

<style lang="scss">
// SASS variables
$primary-color: #1cce1cd7;

// Global configurations
p {
  text-indent: 15px;
}

// General Classes
.h-100 {
  height: 100% !important;
}

.flex-same-width {
  display: flex;
  justify-content: center;
  flex: 1 1 0px;
}

.primary-color {
  color: $primary-color;
}

// Specific ID's
#navbar {
  height: 5%;
  background-color: #000000;
}

#background {
  height: 95%;
  width: 100%;
  // background-color: #1c1c1c;
  background-image: url("./assets/background.jpeg") !important;
  background-size: cover;
}

#main-container {
  padding-left: 10vw;
  padding-right: 10vw;

  background-color: rgba(0, 0, 0, 0.7);

  height: 100%;
  width: 100%;
}
</style>
