<template>
  <v-footer padless app height="280px" absolute color="transparent">
    <v-container style="max-width: 91.375rem">
      <v-row>
        <v-col cols="6" class="d-flex flex-column ">
          <h1
            style="font-size: 2rem; line-height: 38px; letter-spacing: 0.01em; color:white"
          >
            MNTN
          </h1>
          <p
            class=" mb-7"
            style="font-weight: 400; font-size: 1.125rem; color: white; line-height: 32px; font-weight: 700;  max-width: 18.9375rem;"
          >
            Get out there & discover your next slope, mountain & destination!
          </p>

          <p
            class=" mt-auto"
            style="font-weight: 400; color: rgba(225, 225, 225, .5); font-size: 1.125rem"
          >
            Copyright 2019 MNTN, Inc. Terms & Privacy
          </p>
        </v-col>

        <v-col
          cols="3"
          v-for="footerLink in footerLinks"
          :key="footerLink.heading"
          class="d-flex justify-end"
        >
          <v-list dense color="transparent" class="px-0 py-0 mx-0 my-0">
            <v-subheader
              class="px-0 py-0 mx-0 my-0"
              style="color: #FBD784; font-size: 1.5rem; font-weight: 700; line-height: 32px"
              >{{ footerLink.heading }}
            </v-subheader>

            <v-list-item-title
              v-for="(link, i) in footerLink.links"
              :key="i"
              style="color: #fff; font-weight: 600; margin: 0; padding: 0; cursor: pointer; font-size: 18px; margin-bottom: 1px"
              class=""
            >
              {{ link }}
            </v-list-item-title>
          </v-list>
        </v-col>
      </v-row>
    </v-container>
  </v-footer>
</template>

<script>
export default {
  data() {
    return {
      footerLinks: [
        {
          heading: "More on The Blog",
          links: [
            "About MNTN",
            "Contributors & Writers",
            "Write For Us",
            "Contact Us",
            "Privacy Policy"
          ]
        },
        {
          heading: "More on MNTN",
          links: ["The Team ?", "Jobs", "Press"]
        }
      ]
    };
  }
};
</script>

<style></style>
