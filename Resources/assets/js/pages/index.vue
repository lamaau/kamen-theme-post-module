<template>
  <kamen-wrapper>
    <template #main>
      <div>
        <kamen-heading title="Todays Headlines" />

        <kamen-post-card size="lg" />
      </div>

      <kamen-heading title="Videos" right-text="See All" />

      <div class="grid gap-4 mt-4 md:grid-cols-2 grid-cols-1">
        <kamen-video-card
          v-for="(item, index) in Array.from({ length: 4 })"
          :key="index"
        />
      </div>
    </template>
  </kamen-wrapper>
</template>
<script>
import KamenTheme from "Kamen/layouts/kamen.vue";

export default {
  layout: KamenTheme,
};
</script>