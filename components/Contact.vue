<template>
  <div class="w-full box relative flex items-center justify-center gap-2" id="Contact">
    <div class="absolute top-0 left-0 w-full h-full overflow-hidden">
      <Stars></Stars>
    </div>
    <div class="w-full lg:h-full flex flex-col-reverse lg:flex-row justify-center items-center lg:mx-32 mb-20 lg:mb-0 gap-5 z-10">
      <div class="w-full lg:w-[35%] lg:max-w-[35%] lg:h-[80%] rounded-xl form overflow-hidden border border-gray-600">
        <GetInTouch></GetInTouch>
      </div>
      <div class="min-h-[60vh] h-1 w-full lg:flex-1 lg:static absolute top-0 left-0 z-[-1]">
        <Earth></Earth>
      </div>
    </div>
  </div>
</template>

<script setup>
import Earth from './Earth.vue';
import GetInTouch from './GetInTouch.vue';
</script>

<style lang="scss" scoped>
.form {
  @media (max-width: 1024px) {
    min-height: calc(85vh - 80px);
    height: 1px;
  }
}
.box {
  @media (min-width: 1024px) {
    min-height: calc(100vh - 80px);
    height: 1px;
  }
}
</style>
