<template>
<div>
    <div class="ncme-top-bar-left" flex="cross:center">
        <div class="ncme-top-bar-logo" style="">
            <img src="~@/assets/logo.png" alt="" v-if="platform != 'darwin'">
            <img src="~@/assets/logo-win32.png" alt="" v-else>
        </div>
        <div class="direction-buttons" flex>
            <button class="backward-button">
                <img src="~@/assets/icons/backward.png" alt="backward">
            </button>
            <button class="forward-button">
                <img src="~@/assets/icons/forward.png" alt="forward">
            </button>
        </div>
        <search-box></search-box>
    </div>
</div>
</template>

<script>
import SearchBox from "./SearchBox.vue";
export default {
  components: {
    SearchBox
  },
  data() {
    return {
      platform: require("os").platform()
    };
  },
  methods: {}
};
</script>

