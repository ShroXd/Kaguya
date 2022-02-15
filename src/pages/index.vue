<script setup lang="ts">
import Card from '~/components/Card.vue'

interface Kana {
  hiragana: string
  katakana: string
  romaji: string
}

// const data: Kana[] = [{
//   hiragana: 'あ',
//   katakana: 'ア',
//   romaji: 'a',
// }, {
//   hiragana: 'い',
//   katakana: 'イ',
//   romaji: 'i',
// }, {
//   hiragana: 'う',
//   katakana: 'ウ',
//   romaji: 'u',
// }, {
//   hiragana: 'え',
//   katakana: 'エ',
//   romaji: 'e',
// }, {
//   hiragana: 'お',
//   katakana: 'オ',
//   romaji: 'o',
// }]

const data: Kana[] = [{
  hiragana: 'あ',
  katakana: 'ア',
  romaji: 'a',
}]

// eslint-disable-next-line @typescript-eslint/no-unnecessary-type-constraint
// const pick = <T extends unknown>(array: T[]) => array[Math.floor(Math.random() * array.length)]
</script>

<template>
  <card v-for="k, idx in data" :key="idx" class="cursor-pointer m-8">
    <div class="text-12xl">
      {{ k.hiragana }}
    </div>
    <hr class="my-6">
    <div class="flex justify-around">
      <div class="text-6xl">
        {{ k.katakana }}
      </div>
      <div class="text-6xl">
        {{ k.romaji }}
      </div>
    </div>
  </card>
</template>

<route lang="yaml">
meta:
  layout: home
</route>
