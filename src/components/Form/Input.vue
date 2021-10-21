<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  props: {
    modelValue: String,
    label: {
      type: String,
    },
  },
  emits: ["update:modelValue"],
  setup(props) {
    function onInput($event: any) {
      this.$emit("update:modelValue", $event.target.value);
    }
    return { onInput };
  },
});
</script>

<template>
  <div class="group">
    <input :value="modelValue" @input="onInput" />
    <!-- <span class="highlight"></span> -->
    <!-- <span class="bar"></span> -->
    <label>{{ label }}</label>
    <div class="prepend">
      <slot name="prepend"></slot>
    </div>
  </div>
</template>
