<template>
  <div class="flex flex-wrap justify-center">
    <div class="card-zoom w-full h-[15em]">
      <div class="bg-black/30 rounded-xl w-full h-full absolute z-10" />
      <div
        class="card-zoom-image" id="bg"
      ></div>
      <div
        class="
          absolute
          card-zoom-content
          scale-90
          z-10
          bg-black/30
          rounded-full
        "
      >
        <v-icon
          name="PlayIcon"
          class="text-gray-100 text-[3em] cursor-pointer w-16 h-16"
        />
      </div>
    </div>
  </div>
</template>
<style lang="css">
  #bg {
    background-image: url('../../../../assets/images/video1.jpg');
  }
</style>