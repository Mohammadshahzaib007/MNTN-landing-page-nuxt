<template>
  <v-container>
    <!-- Section First -->
    <section>
      <v-container>
        <v-row>
          <v-col
            class="d-flex justify-center flex-column align-center"
            style="margin-top: 253px"
          >
            <v-sheet color="transparent">
              <v-sheet color="transparent" class="d-flex align-center mb-8">
                <span class="line"></span>
                <p
                  class="py-0 my-0 text-uppercase"
                  style="font-size: 1.125rem; color: #FBD784; line-height: 22.05px; font-weight: 600; display: inline-block"
                >
                  A Hiking guide
                </p>
              </v-sheet>

              <h1
                class="text-capitalize "
                style="color: white; max-width: 59.6875rem; font-size: 5.5rem; font-weight: 600; "
              >
                Be prepared for the Mountains and beyond!
              </h1>
              <p
                class="mt-5"
                style="font-size: 18px; color: white;  font-weight: 800"
              >
                scroll down
                <v-icon color="white" size="24" class="ml-4">$downarr</v-icon>
              </p>
            </v-sheet>
          </v-col>
        </v-row>
      </v-container>
    </section>

    <!-- Section Second -->
    <section style="margin-top: 52.6875rem;">
      <v-container style="max-width: 91.375rem">
        <v-row>
          <v-col
            cols="6"
            class="d-flex align-center"
            style="position: relative"
          >
            <p
              style="font-size: 15rem; font-weight: 700; color: rgba(225, 225, 225, .1); position: absolute; top: 0; left: -136px font-weight: 700"
            >
              01
            </p>
            <v-sheet color="transparent" class="px-0 py-0" max-height="439px">
              <v-sheet
                color="transparent"
                class="d-flex align-center mb-0 py-0"
              >
                <span class="line"></span>
                <p
                  class="py-0 my-0 text-uppercase"
                  style="font-size: 1.125rem; color: #FBD784; line-height: 22.05px; font-weight: 600; display: inline-block"
                >
                  Get Started
                </p>
              </v-sheet>

              <h1
                class="text-capitalize py-0 my-0"
                style="color: white; font-size: 4rem; max-width: 555px; font-weight: 600; "
              >
                What level of hiker are you?
              </h1>
              <p
                class="mt-0 py-0"
                style="font-size: 18px; color: white; max-width: 632px;  font-weight: 800"
              >
                Determining what level of hiker you are can be an important tool
                when planning future hikes. This hiking level guide will help
                you plan hikes according to different hike ratings set by
                various websites like All Trails and Modern Hiker. What type of
                hiker are you – novice, moderate, advanced moderate, expert, or
                expert backpacker?
              </p>
              <p
                class="mt-5"
                style="font-size: 18px; color: #FBD784;  font-weight: 800"
              >
                read more
                <v-icon
                  color="white"
                  size="24"
                  class="ml-4"
                  style="transform: rotate(270deg);"
                  >$downarr</v-icon
                >
              </p>
            </v-sheet>
          </v-col>
          <v-col cols="6" class="d-flex justify-end">
            <v-img
              :src="require('@/assets/images/01.png')"
              max-height="45rem"
              max-width="35.375rem"
              contain
            />
          </v-col>
        </v-row>
      </v-container>
    </section>
  </v-container>
</template>

<script>
export default {};
</script>

<style lang="scss">
#bg {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  background-image: radial-gradient(
      circle,
      rgba(0, 0, 0, 0.2),
      rgba(0, 0, 0, 0.8)
    ),
    url("../assets/images/bg.jpg");
  height: 1900px;
  background-size: cover;
  background-position: center;
}
.line {
  width: 72px;
  height: 2px;
  display: inline-block;
  background: #fbd784;
  margin-right: 32px;
}
</style>
