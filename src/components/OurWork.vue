<template>
  <v-container class="mt-16 pt-16 color" id="ourWork">
    <h1 class="text-center text-h2 font-weight-bold mt-16">Our latest work</h1>
    <v-row align="center" justify="center" class="mt-16 ">
      <v-col cols="12" md="8" class="text-h5">
        <v-card height="250" hover data-aos="fade-up" data-aos-duration="3000"
          class="cardWork d-flex align-center justify-space-between pa-0">
          <div class="text-left">
            <v-card-item>
              <v-card-title>
                Website Design
              </v-card-title>
              <v-card-subtitle>
                Ecommerce
              </v-card-subtitle>
              <hr class="divider mb-4">
              <v-card-text class="pa-0 ">
                Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ab esse totam, neque sequi delectus adipisci
                nesciunt dolorem eligendi corrupti optio. Placeat exercitationem debitis in quia reiciendis nostrum
                repudiandae laborum suscipit!
              </v-card-text>
            </v-card-item>
            <v-card-actions>
              <v-btn class="btn">Read More</v-btn>
            </v-card-actions>
          </div>
          <div>
            <v-img class="img-Work" src="/design.png" width="300"></v-img>
          </div>
        </v-card>
      </v-col>
      <v-col cols="12" md="8" class="text-h5">
        <v-card height="250" hover class="d-flex align-center justify-space-between  pa-0 cardWork">
          <div>
            <v-img class="img-Work cardMiddle" src="/design.png" width="300" cover></v-img>
          </div>
          <div class="text-left">
            <v-card-item>
              <v-card-title>
                Practical training
              </v-card-title>
              <v-card-subtitle>
                for graduates
              </v-card-subtitle>
              <hr class="divider mb-4">

              <v-card-text class="pa-0">
                Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ab esse totam, neque sequi delectus adipisci
                nesciunt dolorem eligendi corrupti optio. Placeat exercitationem debitis in quia reiciendis nostrum
                repudiandae laborum suscipit!
              </v-card-text>
            </v-card-item>
            <v-card-actions>
              <v-btn class="btn">Read More</v-btn>
            </v-card-actions>
          </div>
        </v-card>
      </v-col>
      <v-col cols="12" md="8" class="text-h5">
        <v-card height="250" hover data-aos="fade-down" data-aos-duration="3000"
          class="cardWork d-flex align-center justify-space-between pa-0">
          <div class="text-left">
            <v-card-item>
              <v-card-title>
                VideoEdit Workshop
              </v-card-title>
              <v-card-subtitle>
                Subtitle
              </v-card-subtitle>
              <hr class="divider mb-4">

              <v-card-text class="pa-0">
                Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ab esse totam, neque sequi delectus adipisci
                nesciunt dolorem eligendi corrupti optio. Placeat exercitationem debitis in quia reiciendis nostrum
                repudiandae laborum suscipit!
              </v-card-text>
            </v-card-item>
            <v-card-actions>
              <v-btn class="btn">Read More</v-btn>
            </v-card-actions>
          </div>
          <div>
            <v-img class="img-Work" src="/photo_2024-05-22_10-29-30.jpg" width="300"></v-img>
          </div>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>
<style>
.v-card {
  box-shadow: 0 15px 25px rgba(244, 241, 182, 0.2);
  backdrop-filter: blur(20px);
  padding: 10px;
  text-align: center;
  background: linear-gradient(to top left, #d0e694b5, #e5cd61bd);
  transition: background-color 2s;
}

.divider {
  width: 20px;
  height: 5px;
  border: none;
  background-image: linear-gradient(90deg, #c7cf74c4 0%, #ffd00093 49%, #d7c3629d 80%, #bcce5573 100%);
  transition: all 2s;
}

.btn:hover {
  background-image: linear-gradient(90deg, #d6c85bb2 0%, #e1c443b3 49%, #d7c362ae 80%, #d6c85b92 100%);
  animation: slidebg 5s linear infinite;
}

@keyframes slidebg {
  to {
    background-position: 20vw;
  }
}

.img-Work {
  transition: all 1s;
  clip-path: polygon(32% 0, 100% 0, 100% 100%, 0% 100%);
  background-color: rgba(247, 248, 162, 0.601);
}

.cardMiddle {
  clip-path: polygon(0 0, 75% 0, 100% 100%, 0% 100%);
  background-color: rgba(247, 248, 162, 0.601);
  transition: all 1s;
}

.v-card:hover .img-Work {
  transform: scale(1.1) !important;
}

.v-card:hover .divider {
  width: 140px;
}

@media screen and (max-width: 600px) {

  .cardWork {
    flex-wrap: wrap;
    height: 600px !important;
    justify-content: center !important;
    align-items: center;
  }

  .img-Work {
    clip-path: polygon(0 0, 100% 0%, 100% 100%, 0 100%);

  }

}
</style>