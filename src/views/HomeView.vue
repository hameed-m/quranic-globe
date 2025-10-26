<template>
  <TresCanvas window-size >
    <FirstExperience />
  </TresCanvas>
</template>

<script setup lang="ts">
import FirstExperience from '@/components/FirstExperience.vue';
import { TresCanvas } from '@tresjs/core';
// import * as THREE from 'three';

// const scene = new THREE.Scene();
// const camera = new THREE.PerspectiveCamera(75, window.innerWidth / window.innerHeight, 0.1, 1000);

// const renderer = new THREE.WebGLRenderer();
// renderer.setSize(innerWidth, innerHeight);

// const geometry = new THREE.BoxGeometry();
// const material = new THREE.MeshBasicMaterial({ color: 0x00ff00 });
// const cube = new THREE.Mesh(geometry, material);
// scene.add(cube);

// camera.position.z = 5;

// document.body.appendChild(renderer.domElement);


</script>
