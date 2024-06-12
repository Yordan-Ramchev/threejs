<script setup>
import { TresCanvas } from '@tresjs/core'
</script>

<template>
  <TresCanvas window-size clear-color="#82DBC5">
    <TresPerspectiveCamera
      :position="[3, 3, 3]"
      :look-at="[0, 0, 0]"
    />
    <TresMesh>
      <TresTorusGeometry :args="[1, 0.5, 16, 32]" />
      <TresMeshBasicMaterial color="orange" />
    </TresMesh>
  </TresCanvas>
</template>

