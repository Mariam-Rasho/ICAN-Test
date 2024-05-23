<template>
    <v-container id="ourTeam">
        <h1 class="text-center my-16 pt-16">OUR Team</h1>
        <v-row align="center" justify="space-around">
            <v-col cols="12" md="3">
                <v-card class="pa-0 mx-auto" width="300" flat variant="text" data-aos="zoom-in" data-aos-duration="2000"
                    data-aos-offset="200" data-aos-easing="ease-in-out">
                    <v-img src="/pexels-simon-robben-55958-614810.jpg" height="250" cover></v-img>
                    <v-card-title class="title">
                        Ameer AL-Masry
                    </v-card-title>
                    <div class="content">
                        <v-card-subtitle>
                            web developer
                        </v-card-subtitle>
                        <v-card-text>Lorem, ipsum dolor sit amet consectetur adipisicing elit.</v-card-text>
                    </div>
                    <v-card-actions class="connectTeam d-flex justify-center pt-5">
                        <v-btn icon="mdi mdi-linkedin" size="small" class="mx-3" href="https://www.linkedin.com/in/"
                            elevation="24"></v-btn>
                        <v-btn icon="mdi mdi-facebook" size="small" class="mx-3" href="https://www.facebook.com/"
                            elevation="24"></v-btn>
                        <v-btn icon="mdi mdi-gmail" size="small" class="mx-3" href="mailto:www.@gmail.com"
                            elevation="24"></v-btn>
                    </v-card-actions>
                </v-card>
            </v-col>
            <v-col cols="12" md="3"> <v-card class="pa-0 mx-auto" width="300" data-aos="zoom-in"
                    data-aos-duration="2000" data-aos-offset="200" data-aos-easing="ease-in-out">
                    <v-img
                        src="https://images.pexels.com/photos/6592547/pexels-photo-6592547.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
                        height="250" cover></v-img>
                    <v-card-title class="title">
                        Anaa Foster
                    </v-card-title>
                    <div class="content">
                        <v-card-subtitle>
                            web developer
                        </v-card-subtitle>
                        <v-card-text>Lorem, ipsum dolor sit amet consectetur adipisicing elit.</v-card-text>
                    </div>
                    <v-card-actions class="connectTeam d-flex justify-center pt-5">
                        <v-btn icon="mdi mdi-linkedin" size="small" class="mx-3" href="https://www.linkedin.com/in/"
                            elevation="24"></v-btn>
                        <v-btn icon="mdi mdi-facebook" size="small" class="mx-3" href="https://www.facebook.com/"
                            elevation="24"></v-btn>
                        <v-btn icon="mdi mdi-gmail" size="small" class="mx-3" href="mailto:www.@gmail.com"
                            elevation="24"></v-btn>
                    </v-card-actions>
                </v-card></v-col>
            <v-col cols="12" md="3"> <v-card class="pa-0 mx-auto" width="300" data-aos="zoom-in"
                    data-aos-duration="2000" data-aos-offset="200" data-aos-easing="ease-in-out">
                    <v-img
                        src="https://www.fashionbeans.com/wp-content/uploads/2016/11/fringehaircollectiontop3-768x346.jpg"
                        height="250" cover></v-img>
                    <v-card-title class="title">
                        Diane Carter
                    </v-card-title>
                    <div class="content">
                        <v-card-subtitle>
                            web developer
                        </v-card-subtitle>
                        <v-card-text>Lorem, ipsum dolor sit amet consectetur adipisicing elit.</v-card-text>
                    </div>
                    <v-card-actions class="connectTeam d-flex justify-center pt-5">
                        <v-btn icon="mdi mdi-linkedin" size="small" class="mx-3" href="https://www.linkedin.com/in/"
                            elevation="24"></v-btn>
                        <v-btn icon="mdi mdi-facebook" size="small" class="mx-3" href="https://www.facebook.com/"
                            elevation="24"></v-btn>
                        <v-btn icon="mdi mdi-gmail" size="small" class="mx-3" href="mailto:www.@gmail.com"
                            elevation="24"></v-btn>
                    </v-card-actions>
                </v-card></v-col>
        </v-row>
    </v-container>
</template>
<style scoped>
.connectTeam {
    transform: translate(100%, -40px);
    transition: all 2s;
}

.content {
    transform: translate(100%, -50px);
    transition: all .8s;

}

.v-card:hover .content {
    transform: translateY(-60px);
    background-color: #ffe4c4;
    background-image: linear-gradient(90deg, #c8cf74ad 0%, #ffd0006d 49%, #d7c36265 80%, #bcce5573 100%);

}

.title {
    transition: all .9s;
}

.v-card:hover .title {
    overflow: hidden !important;
    transition: all .7s;
    background-color: #ffe4c4;
    text-align: right;
    clip-path: polygon(0 68%, 0 0, 100% 0, 100% 100%);
    background-image: linear-gradient(90deg, #c8cf74ad 0%, #ffd0006d 49%, #d7c36265 80%, #bcce5573 100%);
    transform: translateY(-485%);
    padding: 10px;
}

.v-card:hover .connectTeam {
    transform: translate(0%, -70px);
    background-color: #ffe4c4;
    background-image: linear-gradient(90deg, #c8cf74ad 0%, #ffd0006d 49%, #d7c36265 80%, #bcce5573 100%);
}

.v-card {
    background: transparent !important;
    box-shadow: none;
}
</style>