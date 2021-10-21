<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  setup() {},
});
</script>

<template>
  <div class="header">
    <div class="container">
      <div class="header-menu"><font-awesome-icon icon="bars" /></div>
      <div class="header-links">
        <a href="#"><span>Home</span></a>
        <a href="#" class="active"><span>Validoters</span></a>
        <a href="#"><span>Followers</span></a>
      </div>
      <div class="header-usericon"><font-awesome-icon icon="user" /></div>
    </div>
  </div>
</template>
