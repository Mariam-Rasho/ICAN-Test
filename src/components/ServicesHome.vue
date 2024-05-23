<script setup>
import { Swiper, SwiperSlide } from "swiper/vue";
import { EffectCards, Pagination, Autoplay } from "swiper/modules";
import "swiper/css/effect-cube";
import "swiper/css/autoplay";
import 'swiper/css/pagination';
import "Swiper/css";
const services = [
    "/photo_2024-05-17_23-46-22.jpg", "/photo_2024-05-17_23-46-08.jpg", "/thisisengineering-bwZcAefzmD8-unsplash.jpg", "/photo_2024-05-17_23-45-52.jpg", "/images (1).jpg",
]
</script>
<template>
    <v-container class="mt-16 pt-16 mx-auto w-100" id="service">
        <h1 class="text-center font-weight-bold text-h2 mt-16">OUR SERVICES</h1>
        <v-row align="center" justify="center" class="mt-16">
            <v-col cols="12" md="6" class="text-h5">
                <div>
                    Technical Solutions for consulting, software and everything related to information and
                    communications
                    technology
                </div>
                <v-row class="mt-3" align="center" justify="center">
                    <v-col cols="12" md="6" data-aos="fade-right" data-aos-duration="3000">
                        <v-card class="pa-0 card" title="Software"
                            text=" software services (Windows, Android, IOS, websites)">
                        </v-card>
                    </v-col>
                    <v-col cols="12" md="6" data-aos="fade-left" data-aos-duration="3000">
                        <v-card class="pa-0 card" title="Graphic Design"
                            text=" software services (Windows, Android, IOS, websites)">

                        </v-card>
                    </v-col>
                    <v-col cols="12" md="6" data-aos="fade-left" data-aos-duration="3000">
                        <v-card class="pa-0 card" title="Video Editing"
                            text="software services (Windows, Android, IOS, websites)">
                        </v-card>
                    </v-col>
                    <v-col cols="12" md="6" data-aos="fade-right" data-aos-duration="3000">
                        <v-card class="card pa-0" title="Digital Marketing"
                            text=" software services (Windows, Android, IOS, websites)">
                        </v-card>
                    </v-col>
                    <v-col cols="12" md="6" data-aos="flip-left" data-aos-easing="ease-out-cubic"
                        data-aos-duration="2000">
                        <v-card class="pa-0 card" title="Exhibition of Graduation Projects"
                            text=" software services (Windows, Android, IOS, websites)">
                        </v-card>
                    </v-col>
                    <v-col cols="12" md="6" data-aos="flip-right" data-aos-easing="ease-out-cubic"
                        data-aos-duration="2000">
                        <v-card class="pa-0 card" title="Practical and Vocational Training"
                            text=" software services (Windows, Android, IOS, websites)">
                        </v-card>
                    </v-col>
                </v-row>
            </v-col>
            <v-col cols="12" md="4" class="mx-10">
                <Swiper class="w-100" :space-between="50" :modules="[EffectCards, Pagination, Autoplay]"
                    :effect="'cards'" :grabCursor="true" :pagination="{
                    clickable: true,
                }" :loop="true" :autoplay="{
                    delay: 2500,
                    disableOnInteraction: false,
                }">
                    <SwiperSlide v-for=" service  in  services " :key="service" class="align-center pa-0">
                        <v-card height="400" class="pa-0"><img class="align-center" :src=service cover width="100%"
                                height="100%"></v-card>
                    </SwiperSlide>

                </Swiper>
            </v-col>
        </v-row>

    </v-container>
</template>
<style scoped>
.swiper {
    height: 400px;
    width: 400px;
    overflow: visible;
}

.img {
    height: 100%;
    width: 100%;
}


.card:hover {
    box-shadow: 0px 10px 10px 4px rgba(243, 244, 161, 0.415);
}
</style>