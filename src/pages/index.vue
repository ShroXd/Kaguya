<script setup lang="ts">
import Card from '~/components/Card.vue'
</script>

<template>
  <card class="cursor-pointer">
    <div class="text-12xl">
      あ
    </div>
    <hr class="my-6">
    <div class="flex justify-around">
      <div class="text-6xl">
        ア
      </div>
      <div class="text-6xl">
        a
      </div>
    </div>
  </card>
</template>

<route lang="yaml">
meta:
  layout: home
</route>
