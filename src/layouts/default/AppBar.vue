<template>
  <v-app-bar class="text-white" :elevation="8">
    <v-row align="center" justify="space-between" class="px-md-16 px-3">
      <v-col cols="5" class="text-center">
        <v-app-bar-title class="d-flex flex-row justify-start align-center">
          <v-row justify="center" align="center" class="text-h4">
            <v-col class="pe-1">I</v-col>
            <v-col class="px-0">
              <v-img class="d-flex pa-0" src="/src/assets/icanlogo.png" :width="50" aspect-ratio="16/9" cover />
            </v-col>
            <v-col class="ps-1">A N</v-col>
          </v-row>
        </v-app-bar-title>
      </v-col>
      <v-col cols="auto" class="d-md-flex d-none text-center ">
        <div>
          <v-btn>
            <a class="text-white text-h5" href="#Home">Home</a>
          </v-btn>
          <v-btn>
            <a class="text-white text-h5" href="#service">Services</a>
          </v-btn>
          <v-btn>
            <a class="text-white text-h5" href="#ourWork">Our Works</a>
          </v-btn>
          <v-btn>
            <a class="text-white text-h5" href="#ourTeam">Our Team</a>
          </v-btn>
          <v-btn>
            <a class="text-white text-h5" href="#contact">Contact</a>
          </v-btn>
        </div>
      </v-col>
      <v-col class="text-center  d-md-none d-xm-flex" cols="auto">
        <v-menu width="100%">
          <template v-slot:activator="{ props }">
            <v-app-bar-nav-icon v-bind="props">
            </v-app-bar-nav-icon>
          </template>
          <v-list class="mt-2 text-center text-white">
            <v-row class="w-75 mx-auto" align="center">
              <v-col cols="12">
                <a class="text-white text-h5" href="#Home">Home</a>
              </v-col>
              <v-col cols="12">
                <a class="text-white text-h5" href="#service">Services</a>
              </v-col>
              <v-col cols="12">
                <a class="text-white text-h5" href="#ourWork">Our Works</a>
              </v-col>
              <v-col cols="12">
                <a class="text-white text-h5" href="#ourTeam">Our Team</a>
              </v-col>
              <v-col cols="12">
                <a class="text-white text-h5" href="#contact">Contact</a>
              </v-col>
            </v-row>
          </v-list>
        </v-menu>
      </v-col>
    </v-row>
  </v-app-bar>
</template>

<script setup>
//
</script>
<style>
.v-app-bar,
.v-list {
  max-width: 100vw !important;
  background: linear-gradient(to top left, #807d42bd, #fdcf028c) !important;
  backdrop-filter: blur(20px) !important;
}

a {
  text-decoration: none;
}

.v-list {
  overflow: hidden !important;
}

.navItem:hover {
  background-color: rgba(255, 245, 255, 0.2);
  border-bottom-color: #abcdef;
}

a::after {
  background-image: linear-gradient(90deg, #c7cf74c4 0%, #ffd00093 49%, #d7c3629d 80%, #bcce5573 100%);
  content: "";
  width: 0;
  height: 3px;
  left: 0;
  bottom: 0;
  transition: width 0.35s ease 0s;
  position: absolute;
}

a:hover::after {
  width: 100%;
}
</style>
