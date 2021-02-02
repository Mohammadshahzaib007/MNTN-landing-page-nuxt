<template>
  <v-app-bar color="transparent" elevation="0" app absolute class="mt-10">
    <v-container style="max-width: 1760px">
      <v-row>
        <v-col cols="2"
          ><v-toolbar-title
            ><h1
              style="font-size: 2rem; line-height: 38px; letter-spacing: 0.01em; color:white"
            >
              MNTN
            </h1>
          </v-toolbar-title></v-col
        >
        <v-col cols="8" class="d-flex justify-center align-center">
          <nuxt-link
            text
            to="#"
            class="text-capitalize mr-10 g-link"
            v-for="navLink in navLinks"
            :key="navLink"
            style="font-size: 1.0625rem; font-weight: 600; line-height: 20.55px; color:white"
          >
            {{ navLink }}
          </nuxt-link>
        </v-col>
        <v-col cols="2" class="d-flex justify-end align-center">
          <v-icon size="24" color="white">$account</v-icon>
          <nuxt-link
          to="#"
            text
            class="text-capitalize px-0 py-0 mx-0 my-0 ml-2 g-link"
            style="font-size: 1.125rem; font-weight: 600; line-height: 21.76px; color:white"
            >Account</nuxt-link
          >
        </v-col>
      </v-row>
    </v-container>
  </v-app-bar>
</template>

<script>
export default {
  data() {
    return {
      navLinks: ["Equipment", "About us", "Blog"]
    };
  }
};
</script>

<style lang="scss" scoped></style>
