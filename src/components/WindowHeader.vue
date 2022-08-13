<template>
  <div class="messagers__window-header">
    <div class="messagers__window-header-img">
      <img :src="avatars[src]" alt="" class="messagers__window-avatar" />
    </div>
    <div class="messagers__window-info">
      <h2 class="messagers__window-name">{{ name }}</h2>
      <p class="messagers__window-status">{{ status }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "WindowHeader",
  props: {
    src: String,
    name: String,
    status: String,
  },
  data() {
    return {
      avatars: {
        alex: require("@/assets/img/alex.png"),
        jane: require("@/assets/img/jane.png"),
      },
    };
  },
};
</script>

<style>
</style>