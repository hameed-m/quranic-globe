<template>
  <TresPerspectiveCamera :position="[15, 15, 15]" />
  <Stars :rotation="[0, 0, 0]" />
  <OrbitControls :min-distance="12" :max-distance="30" />
  <TresAmbientLight :intensity="0.5" />
  <TresDirectionalLight :args="['#ffffff', 0.8]" />
  <TresMesh>
    <TresSphereGeometry :args="[10, 32, 16]"/>
    <TresMeshStandardMaterial
      :color="oceanColor"
      :metalness="0.8"
      :roughness="0.2"
      :emissive="emissiveColor"
    />
    <TresMeshBasicMaterial :args="[{ color: 0xffff00}]" />
  </TresMesh>

  <TresAxesHelper />
  <TresGridHelper :args="[10]" />
</template>
<script setup lang="ts">
// import { ref } from 'vue';
import { OrbitControls, Stars } from '@tresjs/cientos';
// import { useLoop } from '@tresjs/core';

// const sphereRef = ref();

// Ocean-like colors
const oceanColor = '#1a5f7a'; // Deep ocean blue
const emissiveColor = '#0d3b52'; // Darker blue glow

// const { onBeforeRender } = useLoop();

// Slow rotation to simulate water movement
// onBeforeRender(({ elapsed }) => {
//   if (sphereRef.value) {
//     sphereRef.value.rotation.y = elapsed * 0.1; // Slow rotation
//   }
// });
</script>
