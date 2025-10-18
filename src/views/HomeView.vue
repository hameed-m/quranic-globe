<template>
    <TresCanvas shadows window-size>
      <TresPerspectiveCamera :position="[5, 5, 5]" />
    </TresCanvas>
</template>

<script setup lang="ts">
import { TresCanvas } from '@tresjs/core'
</script>
