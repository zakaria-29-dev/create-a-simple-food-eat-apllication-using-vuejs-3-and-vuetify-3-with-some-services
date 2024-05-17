<template>
  <v-app>
    <app-navbar />
    <v-main>
      <v-container>
        <v-row>
          <v-col cols="12" md="6">
            <h1 class="mt-16 ml-16">Delicious Food Is<br />Waiting For You</h1>
            <p class="mt-6 ml-16">
              Our team of registered <br />
              nurses and skilled healthcare<br />professionals provide
              in-home<br />nursing
            </p>
            <v-btn class="mt-8 ml-16 rounded-pill" color="#9B7150">
              Food Menu
            </v-btn>
            <v-btn class="mt-8 ml-4 rounded-pill"> Book a Table </v-btn>
          </v-col>
          <v-col cols="12" md="6">
            <v-img src="/1.png" :width="500" aspect-ratio="16/9" cover></v-img>
          </v-col>
          <v-col cols="12" md="12">
            <h1 class="text-center">Top List</h1>
            <h4 class="text-center">Our mainstay menu</h4>
          </v-col>
          <v-col cols="12" sm="12">
            <v-row>
              <v-col cols="12" sm="4" class="d-flex justify-center">
                <v-card color="transparent" max-width="200" flat>
                  <v-img height="70" src="/1.png" class="imag"></v-img>
                  <v-card
                    class="mt-n10 rounded-xl"
                    max-width="300"
                    color="#CDAC8B"
                  >
                    <v-card-item class="text-center">
                      <v-card-title class="mt-10">Noodles three</v-card-title>

                      <v-card-subtitle>
                        <span class="me-1"
                          >White plate with <br />dried shrimps</span
                        >
                      </v-card-subtitle>
                      <v-card-title>12$</v-card-title>
                    </v-card-item>

                    <v-card-text>
                      <v-row align="center" class="mx-0">
                        <v-icon
                          color="yellow"
                          icon="mdi mdi-star"
                          size=""
                        ></v-icon>
                        <div class="ms-4">
                          <h6>8.1</h6>
                        </div>
                        <v-spacer></v-spacer>
                        <div class="text-grey ms-4">
                          <v-icon color="brown">mdi mdi-plus-circle</v-icon>
                        </div>
                      </v-row>
                    </v-card-text>
                  </v-card>
                </v-card>
              </v-col>
              <v-col cols="12" sm="4" class="d-flex justify-center">
                <v-card color="transparent" max-width="300" flat>
                  <v-img height="100" src="/3.png" class="imag"></v-img>
                  <v-card
                    class="mt-n10 rounded-xl"
                    max-width="300"
                    color="#CDAC8B"
                  >
                    <v-card-item class="text-center">
                      <v-card-title class="mt-10">Noodles one</v-card-title>

                      <v-card-subtitle>
                        <span class="me-1"
                          >Noodles spicy boil with <br />seafood and pork in hot
                          pot</span
                        >
                      </v-card-subtitle>
                      <v-card-title>20$</v-card-title>
                    </v-card-item>

                    <v-card-text>
                      <v-row align="center" class="mx-0">
                        <v-icon
                          color="yellow"
                          icon="mdi mdi-star"
                          size=""
                        ></v-icon>
                        <div class="ms-4">
                          <h6>9.2</h6>
                        </div>
                        <v-spacer></v-spacer>
                        <div class="text-grey ms-4">
                          <v-icon color="brown">mdi mdi-plus-circle</v-icon>
                        </div>
                      </v-row>
                    </v-card-text>
                  </v-card>
                </v-card>
              </v-col>
              <v-col cols="12" sm="4" class="d-flex justify-center">
                <v-card color="transparent" max-width="200" flat>
                  <v-img height="70" src="/4.png" class="imag"></v-img>
                  <v-card
                    class="mt-n10 rounded-xl"
                    max-width="300"
                    color="#CDAC8B"
                  >
                    <v-card-item class="text-center">
                      <v-card-title class="mt-10">Noodles two</v-card-title>

                      <v-card-subtitle>
                        <span class="me-1">Noodles prawn <br />spicy soup</span>
                      </v-card-subtitle>
                      <v-card-title>16$</v-card-title>
                    </v-card-item>

                    <v-card-text>
                      <v-row align="center" class="mx-0">
                        <v-icon
                          color="yellow"
                          icon="mdi mdi-star"
                          size=""
                        ></v-icon>
                        <div class="ms-4">
                          <h6>8.5</h6>
                        </div>
                        <v-spacer></v-spacer>
                        <div class="text-grey ms-4">
                          <v-icon color="brown">mdi mdi-plus-circle</v-icon>
                        </div>
                      </v-row>
                    </v-card-text>
                  </v-card>
                </v-card>
              </v-col>
            </v-row>
          </v-col>
          <v-col cols="12" md="6">
            <v-img src="/5.webp" :width="500" aspect-ratio="16/9" cover></v-img>
          </v-col>
          <v-col cols="12" md="6">
            <h1 class="" style="margin-top: 100px">
              Best Potatoes For<br />French Fries
            </h1>
            <p class="mt-6">
              Russet potatoes are ideal Since they're dense, they<br />
              don't contain as mush water inside, which allows<br />
              them to get extra crispy
            </p>
          </v-col>
          <v-col cols="12" md="12">
            <h1 class="text-center">Our services</h1>
          </v-col>
          <v-col cols="12" sm="12">
            <div class="d-flex justify-space-evenly mt-4" color="transparent">
              <v-chip
                class="ma-2"
                color="black"
                variant="outlined"
                v-for="(food, i) in foods"
                :key="i"
              >
                <v-icon :icon="food.icon" start></v-icon>
                {{ food.title }}
              </v-chip>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </v-main>
  </v-app>
</template>

<script setup>
const foods = [
  { title: "Online booking", icon: "mdi mdi-cellphone-sound" },
  { title: "Catering service", icon: "mdi mdi-food-outline" },
  { title: "Membership", icon: "mdi mdi-account-group" },
  { title: "Delivery service", icon: "mdi mdi-truck-delivery-outline" },
];
</script>
<style scoped>
.imag {
  z-index: 9999 !important;
}
</style>
