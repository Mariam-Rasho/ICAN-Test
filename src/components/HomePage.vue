<template>
  <v-container class="bg-hero pa-0" id="Home">
    <v-responsive class="align-start text-center" height="600">
      <v-row align="center" justify="center">
        <v-col cols="12" md="6" class="pb-md-5 pt-10" data-aos="fade-up" data-aos-duration="4000">
          <h1 class="text-md-h1 text-h3 font-weight-medium" data-aos="zoom-in" data-aos-duration="2000"
            data-aos-offset="200" data-aos-easing="ease-in-out">ICAN</h1>
          <div class="my-7">
            <vue-typewriter-effect
              :strings="['Software Development', 'Graphic Design', 'Video Editing', 'Digital Marketing', 'Technical Support',]"
              class="text-md-h2 text-h5 text-center font-weight-bold  pb-16 text-home">
            </vue-typewriter-effect>
          </div>
          <div class="text-md-h6 px-5">
            Technical Solutions for consulting, software and technical solutions and everything related to information
            and communications technology, managed by Engineer Basil Tanbakjy.
          </div>
          <v-btn rounded="xl" size="large" class="bg text-blue-lighten-5 bg-indigo-lighten-1 text-h6 mt-5"
            elevation="16">Read
            More</v-btn>
        </v-col>


        <v-col md="5" cols="12" class="carousel">
          <v-carousel hide-delimiters :show-arrows="false" cycle data-aos="flip-left" data-aos-easing="ease-out-cubic"
            data-aos-duration="1000">
            <v-carousel-item v-for="item in items" :key="item" :src="item.src" cover width="800" height="600">
            </v-carousel-item>
          </v-carousel>
        </v-col>

        <!-- <v-col md="6" cols="12">
          <div>
            <TransitionGroup name="fade">
              <v-img :key="currentIndex" :src="currentIndex" contain data-aos="flip-left" data-aos-easing="ease-out"
                data-aos-duration="2000" width="300" />
            </TransitionGroup>
          </div>
        </v-col> -->
      </v-row>
    </v-responsive>
    <div class="svg pa-0 waveMove ">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320" class="svg pa-0">
        <path fill="#fff" fill-opacity="1"
          d="M0,256L80,266.7C160,277,320,299,480,288C640,277,800,235,960,208C1120,181,1280,171,1360,165.3L1440,160L1440,320L1360,320C1280,320,1120,320,960,320C800,320,640,320,480,320C320,320,160,320,80,320L0,320Z">
        </path>

      </svg>
    </div>
    <div class="d-flex align- justify-center">
      <v-btn icon="mdi mdi-linkedin" size="large" class="bg mx-3" href="https://www.linkedin.com/in/"
        elevation="24"></v-btn>
      <v-btn icon="mdi mdi-facebook" size="large" class="bg mx-3" href="https://www.facebook.com/"
        elevation="24"></v-btn>
      <v-btn icon="mdi mdi-github" size="large" class="bg mx-3" href="https://github.com/Mariam-Rasho/"
        elevation="24"></v-btn>
      <v-btn icon="mdi mdi-gmail" size="large" class="bg mx-3" href="mailto:www.@gmail.com" elevation="24"></v-btn>
    </div>
  </v-container>
</template>

<script setup>
import VueTypewriterEffect from "vue-typewriter-effect";
const items = [
  {
    src: '/dev1.png',
  },
  {
    src: '/design.png',

  },
  {
    src: '/video.png',
  }
  , {
    src: '/dev3.png',
  },

  {
    src: '/tec2.png',
  }
  ,
];
</script>
<style>
.bg-hero {
  max-width: 100vw !important;
  background: linear-gradient(to top left, #484725bd, #dec34abb) !important;
  backdrop-filter: blur(2px) !important;
}

.bg {
  max-width: 100vw !important;
  background: linear-gradient(to top left, #807d42, #fdcd02) !important;
  backdrop-filter: blur(2px) !important;
}

h1 {
  font-size: 72px;
  background: linear-gradient(to right, #050202 40%, #fcf401 60%);
  background-clip: text;
  -webkit-text-fill-color: transparent;
}

.svg {
  width: 100%;
  position: absolute;
  bottom: -5px;
  z-index: -1;
}

.v-btn:hover {
  transform: translateY(-9px) !important;
  transition: all 0.7s ease-in-out;
  color: aliceblue;
}

@media screen and (max-width: 600px) {
  .carousel .v-img {
    width: 100vw !important;
    height: 200px !important;
  }
}
</style>
