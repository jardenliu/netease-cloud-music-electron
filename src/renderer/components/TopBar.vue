<template>
<div class="ncme-top-bar">
  <PlatfromWin32TopBar  v-if="platform == 'darwin'"></PlatfromWin32TopBar>
  <!-- <PlatfromDarwinTopBar  v-if="platform == 'darwin'"></PlatfromDarwinTopBar> -->
</div>
</template>

<script>
import PlatfromDarwinTopBar from "./TopBar/PlatfromDarwinTopBar.vue";
import PlatfromWin32TopBar from "./TopBar/PlatfromWin32TopBar.vue";
export default {
  components: {
    PlatfromDarwinTopBar,
    PlatfromWin32TopBar
  },
  data() {
    return {
      platform: require("os").platform()
    };
  },
  methods: {}
};
</script>



