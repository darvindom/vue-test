<script lang="ts">
import { defineComponent } from "vue";
import Input from "./Form/Input.vue";

export default defineComponent({
  components: {
    Input,
  },
  setup() {
    return {};
  },
});
</script>

<template>
  <Input class="search" label="Search">
    <template #prepend>
      <font-awesome-icon icon="search" />
    </template>
  </Input>
</template>

<style lang="scss" scoped>
.search {
  margin-top: 4rem;
}
</style>
