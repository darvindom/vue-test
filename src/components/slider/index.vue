<script lang="ts">
import { defineComponent } from "vue";
import Footer from "./Footer.vue";
export default defineComponent({
  components: { Footer },
  props: {
    title: String,
  },
  setup() {},
});
</script>

<template>
  <div class="slider">
    <div class="slider-header">
      {{ title }}
    </div>
    <slot></slot>
    <Footer></Footer>
  </div>
</template>

<style lang="scss" scoped>
.slider {
  &-header {
    font-weight: bold;
  }
}
</style>
