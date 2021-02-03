<template>
  <v-container>
    <!-- Section First -->
    <section id="hero-section">
      <v-container>
        <v-row>
          <v-col
            class="d-flex justify-center flex-column align-center"
            style="margin-top: 253px"
          >
            <v-sheet color="transparent">
              <v-sheet color="transparent" class="sub-super-text d-flex align-center mb-8">
                <span class="line"></span>
                <p
                  class="py-0 my-0 text-uppercase"
                  style="font-size: 1.125rem; color: #FBD784; line-height: 22.05px; font-weight: 600; display: inline-block; letter-spacing: 6px;"
                >
                  A Hiking guide
                </p>
              </v-sheet>

              <h1
                class="text-capitalize text-h1"
                style="color: white; max-width: 59.6875rem; font-weight: 600; "
                ref="heading"
              >
                <v-sheet
                  color="transparent"
                  style="overflow: hidden; color: white;"
                  class="px-0 py-0"
                >
                  <!-- <span ref="heading" class="d-block main-heading-animation"> -->
                  Be prepared for the
                  <!-- </span> -->
                </v-sheet>
                <v-sheet
                  color="transparent"
                  style="overflow: hidden; color: white;"
                  class="px-0 py-0"
                >
                  Mountains and beyond!
                </v-sheet>
              </h1>
              <v-sheet
                color="transparent"
                class="mt-5 scroll-down-text"
                style="backface-visibility: hidden; font-size: 18px; color: white; font-weight: 800"
              >
                <span 
                  class="g-link"
                  @click="$vuetify.goTo('#get-started-section', { duration: 1000 })"
                >
                  scroll down
                </span>
                <v-icon color="white" size="24" class="ml-1 icon-animation">
                  $downarr
                </v-icon>
              </v-sheet>
            </v-sheet>
          </v-col>
        </v-row>
      </v-container>
    </section>

    <!-- Section Second -->
    <section id="get-started-section" style="margin-top: 28.9375rem;">
      <v-container style="max-width: 91.375rem">
        <v-row>
          <v-col
            cols="6"
            class="d-flex align-center justify-end"
            style="position: relative"
          >
            <p
              style="font-size: 15rem; font-weight: 700; color: rgba(225, 225, 225, .1); position: absolute; top: -8px; left: -64px; font-weight: 700"
            >
              01
            </p>
            <v-sheet color="transparent" class="px-0 py-0" max-height="439px">
              <v-sheet
                color="transparent"
                class="d-flex align-center mb-0 py-0"
              >
                <span class="line" style="margin-right: 24px"></span>
                <p
                  class="py-0 my-0 text-uppercase mb-2"
                  style="font-size: 1.125rem; color: #FBD784; line-height: 22.05px; font-weight: 600; display: inline-block; letter-spacing: 5px;"
                >
                  Get Started
                </p>
              </v-sheet>

              <h2
                v-observe-visibility="
                  (isVisible, entry) =>
                    visibilityChanged(isVisible, entry, 'section-2-heading')
                "
                ref="sectionSecondHeading"
                class="py-0 my-0"
                style="color: white; font-size: 4rem; max-width: 555px; font-weight: 600; line-height: 76.8px"
              >
                <v-sheet
                  color="transparent"
                  style="overflow: hidden; color: white;"
                  class="px-0 py-0"
                >
                  What level of hiker
                </v-sheet>
                <v-sheet
                  color="transparent"
                  style="overflow: hidden; color: white;"
                  class="px-0 py-0"
                >
                  are you?
                </v-sheet>
              </h2>
              <p
                class="mt-3 py-0"
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
                class="mt-2 g-link"
                style=" max-width: 131px; font-size: 18px; color: #FBD784;  font-weight: 800; cursor: pointer"
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
              v-tilt
              :src="require('@/assets/images/01.png')"
              max-height="45rem"
              max-width="35.375rem"
              contain
            />
          </v-col>
        </v-row>
      </v-container>
    </section>

    <!-- Section Third -->
    <section id="hiking-esentials-section" style="margin-top: 12.5rem">
      <v-container style="max-width: 91.375rem">
        <v-row>
          <v-col cols="6" class="d-flex">
            <v-img
              v-tilt
              :src="require('@/assets/images/02.png')"
              max-height="45rem"
              max-width="35.375rem"
              contain
            />
          </v-col>
          <v-col
            cols="6"
            class="d-flex align-center justify-end"
            style="position: relative"
          >
            <p
              style="font-size: 15rem; font-weight: 700; color: rgba(225, 225, 225, .1); position: absolute; top: -8px; left: -64px; font-weight: 700"
            >
              02
            </p>
            <v-sheet color="transparent" class="px-0 py-0" max-height="632px">
              <v-sheet
                color="transparent"
                class="d-flex align-center mb-0 py-0"
              >
                <span class="line" style="margin-right: 24px"></span>
                <p
                  class="py-0 my-0 text-uppercase mb-2"
                  style="font-size: 1.125rem; color: #FBD784; line-height: 22.05px; font-weight: 600; display: inline-block; letter-spacing: 5px;"
                >
                  Hiking Essentials
                </p>
              </v-sheet>

              <!-- v-observe-visibility="visibilityChanged" -->
              <h2
                v-observe-visibility="
                  (isVisible, entry) =>
                    visibilityChanged(isVisible, entry, 'section-3-heading')
                "
                class="py-0 my-0"
                ref="sectionThirdHeading"
                style="color: white; font-size: 4rem; max-width: 555px; font-weight: 600; line-height: 76.8px"
              >
                <v-sheet
                  color="transparent"
                  style="overflow: hidden; color: white;"
                  class="px-0 py-0"
                  >Picking the right
                </v-sheet>
                <v-sheet
                  color="transparent"
                  style="overflow: hidden; color: white;"
                  class="px-0 py-0"
                >
                  Hiking Gear!
                </v-sheet>
              </h2>
              <p
                class="mt-3 py-0"
                style="font-size: 18px; color: white; max-width: 632px;  font-weight: 800"
              >
                The nice thing about beginning hiking is that you don’t really
                need any special gear, you can probably get away with things you
                already have. Let’s start with clothing. A typical mistake
                hiking beginners make is wearing jeans and regular clothes,
                which will get heavy and chafe wif they get sweaty or wet.
              </p>
              <p
                class="mt-2 g-link"
                style=" max-width: 131px; font-size: 18px; color: #FBD784;  font-weight: 800; cursor: pointer"
              >
                read more
                <v-icon
                  color="white"
                  size="24"
                  class="ml-4"
                  style="transform: rotate(270deg);"
                >
                  $downarr
                </v-icon>
              </p>
            </v-sheet>
          </v-col>
        </v-row>
      </v-container>
    </section>

    <!-- Section Fourth -->
    <section
      id="where-you-go-section"
      style="margin-top: 12.5rem; margin-bottom: 150px"
    >
      <v-container style="max-width: 91.375rem">
        <v-row>
          <v-col
            cols="6"
            class="d-flex align-center justify-end"
            style="position: relative"
          >
            <p
              style="font-size: 15rem; font-weight: 700; color: rgba(225, 225, 225, .1); position: absolute; top: -8px; left: -64px; font-weight: 700"
            >
              03
            </p>
            <v-sheet color="transparent" class="px-0 py-0" max-height="439px">
              <v-sheet
                color="transparent"
                class="d-flex align-center mb-0 py-0"
              >
                <span class="line" style="margin-right: 24px"></span>
                <p
                  class="py-0 my-0 text-uppercase mb-2"
                  style="font-size: 1.125rem; color: #FBD784; line-height: 22.05px; font-weight: 600; display: inline-block; letter-spacing: 5px;"
                >
                  where you go is the key
                </p>
              </v-sheet>

              <!-- v-observe-visibility="visibilityChanged" -->
              <h2
                v-observe-visibility="
                  (isVisible, entry) =>
                    visibilityChanged(isVisible, entry, 'section-4-heading')
                "
                ref="sectionFourthHeading"
                class="py-0 my-0"
                style="color: white; font-size: 4rem; max-width: 540px; font-weight: 600; line-height: 76.8px"
              >
                <v-sheet
                  color="transparent"
                  style="overflow: hidden; color: white;"
                  class="px-0 py-0"
                >
                  Understand Your
                </v-sheet>
                <v-sheet
                  color="transparent"
                  style="overflow: hidden; color: white;"
                  class="px-0 py-0"
                >
                  Map & Timing
                </v-sheet>
              </h2>
              <p
                class="mt-3 py-0"
                style="font-size: 18px; color: white; max-width: 632px;  font-weight: 800"
              >
                To start, print out the hiking guide and map. If it’s raining,
                throw them in a Zip-Lock bag. Read over the guide, study the
                map, and have a good idea of what to expect. I like to know what
                my next landmark is as I hike. For example, I’ll read the guide
                and know that say, in a mile, I make a right turn at the
                junction..
              </p>
              <p
                class="mt-2 g-link"
                style="max-width: 131px; font-size: 18px; color: #FBD784;  font-weight: 800; cursor: pointer"
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
              v-tilt
              :src="require('@/assets/images/03.png')"
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
import { Component, Vue, Ref, Watch } from "nuxt-property-decorator";
import { gsap } from "gsap";

import "splitting/dist/splitting.css";
import "splitting/dist/splitting-cells.css";
import splitting from "splitting";

@Component
export default class Index extends Vue {
  @Ref("heading") heading;
  @Ref("sectionSecondHeading") sectionSecondHeading;
  @Ref("sectionThirdHeading") sectionThirdHeading;
  @Ref("sectionFourthHeading") sectionFourthHeading;

  isSection2Visible = false;
  tl2 = null;
  tl3 = null;
  tl4 = null;

  visibilityChanged(isVisible, _entry, whichSection) {
    this.isSection2Visible = isVisible;

    // Checking we are on which section currently
    // and then executing the code according to the section
    if (whichSection === "section-2-heading") {
      if (isVisible && this.tl2) {
        this.tl2.play();
      } else {
        this.tl2.reverse();
      }
    }

    if (whichSection === "section-3-heading") {
      if (isVisible && this.tl3) {
        this.tl3.play();
      } else {
        this.tl3.reverse();
      }
    }

    if (whichSection === "section-4-heading") {
      if (isVisible && this.tl4) {
        this.tl4.play();
      } else {
        this.tl4.reverse();
      }
    }
  }

  mounted() {
    //Splitting the heading into spans
    splitting({ target: this.heading, by: "words" });
    splitting({ target: this.sectionSecondHeading, by: "words" });
    splitting({ target: this.sectionThirdHeading, by: "words" });
    splitting({ target: this.sectionFourthHeading, by: "words" });
    // gsap initializations
    const tl = gsap.timeline({ paused: true });
    this.tl2 = gsap.timeline({ paused: true });
    this.tl3 = gsap.timeline({ paused: true });
    this.tl4 = gsap.timeline({ paused: true });

    // common animation
    const textAnimation = {
      opacity: 0,
      y: 100,
      duration: 0.4,
      stagger: 0.11
    };

    // hero banner
    tl.from("#hero-section .word", textAnimation)
    .from('#navbar', { opacity: 0, duration: .2 })
    .from('#hero-section .sub-super-text', { opacity: 0, duration: .2 }, '-=.2')
    .from('#hero-section .scroll-down-text', { opacity: 0}, '-=.2')

    // Section 2;
    this.tl2.from("#get-started-section .word", textAnimation);

    // Section 3;
    this.tl3.from("#hiking-esentials-section .word", textAnimation);

    // Section 4;
    this.tl4.from("#where-you-go-section .word", textAnimation);

    // On window load play the banner textAnimation
    window.addEventListener("load", () => {
      setTimeout(() => {
        tl.play();
      }, 500);
    });
  }
}
</script>
<style lang="scss">
#bg {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  background-image: linear-gradient(
      180deg,
      rgba(2, 0, 36, 0) -50%,
      rgba(11, 29, 38, 1) 86%,
      rgba(11, 29, 38, 1) 100%
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

.icon-animation {
  animation: downAnimation 1.5s ease-in-out infinite;
}

.main-heading-animation {
  color: white;
}

@keyframes downAnimation {
  0% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(10px);
  }
  100%{
    transform: translateY(0)
  }
}
</style>
