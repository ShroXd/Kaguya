<template>
  <div class="container">
    <div
      class="animate py-8 px-6 border-1 border-light-800 shadow hover:(shadow-xl) ease-in duration-150 w-auto inline-block"
    >
      <slot />
    </div>
  </div>
</template>

<style lang="scss">
.container {
  perspective: 1000px;
}

.animate {
  transform-style: preserve-3d;

  &:hover {
    transform: rotateX(20deg);
  }
}
</style>
