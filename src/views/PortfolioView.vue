<template>
  <div v-for="item in items" v-bind:key="item.company as string">
    <ProjectListing :item="item" />
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import ProjectListing from '/src/components/ProjectListing.vue'
const items = ref([
  {
    company: `snowglobe.js`,
    title: `Founder | Tech Lead`,
    description: `PRODUCT: Snowglobe is a serverless p2p platform for TRPGs
        TECH: Three.js, Less.js, Tone.js, Node.js, FileSystem, Socket.io, WebRTC, Simple-peer.js, AWS,
        FEATS:
        Organized/Mentored/Lead Volunteer Engineers & Designers
        Engineering Architecture
        Business/Technology Advocate
      `,
    images: [
      `/src/assets/snowglobe00.gif`,
      `/src/assets/snowglobe01.gif`,
      `/src/assets/snowglobe02.gif`,
      `/src/assets/snowglobe03.gif`
    ]
  },
  {
    company: `MasterCard`,
    title: `Senior Software Engineer | Front End | Team Supernova | InRhythm Contractor`,
    description: `PROJECT: MasterCard Click to pay is a fast secure online payment gateway
        TECH: Vue.js, VueX, Sass, Jest, GitLab Pipeline
        FEATS:
        Flawless Support
        Exceeded KPI
        Mentored/Lead Junior Engineers
        Design & Business Advocate
      `,
    images: [`/src/assets/mastercard00.jpg`, `/src/assets/mastercard01.jpg`]
  },
  {
    company: `Goldman Sachs`,
    title: `Senior Software Engineer | Front End | Team Marquee Engineering | InRhythm Contractor`,
    description: `PROJECT: Marquee is an data-informed asset & currency trading platform client
        TECH: React.js, RxJS, Typescript, Electron.js, Sass, Cypress, GitLab Pipeline
        FEATS:
        Exceeded KPI
        Reduced onboard time with Architecture Flowchart
        Increased accuracy with predictive client data for sporadic API
        Collaborated with Design
      `,
    images: [
      `/src/assets/goldmansachs00.png`,
      `/src/assets/goldmansachs01.png`,
      `/src/assets/goldmansachs02.png`,
      `/src/assets/goldmansachs03.gif`
    ]
  },
  {
    company: `Viacom`,
    title: `Senior Software Engineer | Front End | AdTech | Team Bento`,
    description: `PROJECT: Video Player & Ads for the launch of Comedy Central's Trevor Noah Show
        TECH: React.js, RxJS, Typescript, Electron.js, Sass, Mocha, GitLab Pipeline
        FEATS:
        Exceeded KPI, Equaled a team of five in story points for multiple sprints
        Mentored/Lead Junior Engineers
        Ate the most pizza
      `,
    images: [`/src/assets/viacom00.png`]
  },
  {
    company: `Time`,
    title: `Software Engineer | Front End | Big Human Contract`,
    description: `PROJECT: Implement Design and Infiniscroll
        TECH: Drupal, Less.js, PHP
        FEATS:
        Implemented Infiniscroll
        Collaborated with Design
      `,
    images: [`/src/assets/time00.png`]
  }
])
</script>

<style>
</style>
