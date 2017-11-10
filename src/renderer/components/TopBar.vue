<template>
<div class="ncme-top-bar">
  <div class="platfrom-darwin-top-bar" v-if="platform == 'darwin'">
    <div class="ncme-top-bar-content" flex="main:justify cross:center">
      <div style="padding-left:9px;height:37px" flex="cross:center">
        <div style="margin-top:2px;margin-left:10px;cursor: pointer;">
          <img src="~@/assets/logo.png" alt="">
        </div>
        <div style="margin-left:71px;" flex>
          <button class="backward-button">
            <img src="~@/assets/icons/backward.png" alt="backward">
          </button>
          <button class="forward-button">
            <img src="~@/assets/icons/forward.png" alt="forward">
          </button>
        </div>
        <search-box></search-box>
      </div>
      <div flex="cross:center">
        <div flex="cross:center">
          <img src="~@/assets/icons/envelope18.png" style="margin:0 10px;border-radius:5px" alt="forward">
          <img src="~@/assets/icons/setting18.png" style="margin:0 22px;" alt="forward">
        </div>
        <div class="platfrom-darwin-user-logo-box" flex="main:center cross:center">
          <div flex="cross:center">
              <div style="background:rgb(216,216,216);border-radius:50%;width: 23px; height: 23px;    margin-left: 5px;" flex="main:center cross:center">
                <img src="~@/assets/icons/unsigninUser.png" style="border-radius:40%;" alt="unsigninUser">
              </div>
              <div style="margin-left:3px;">
                <img src="~@/assets/icons/down.png"  alt="forward">
              </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
</template>

<script>
import SearchBox from "./TopBar/SearchBox.vue";
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

<style>
.platfrom-darwin-user-logo-box {
  position: relative;
  width: 64px;
}

.platfrom-darwin-user-logo-box:before {
  position: absolute;
  content: " ";
  height: 60px;
  width: 1px;
  border-right: 1px solid rgba(0, 0, 0, 0.1);
  top: -27px;
  left: -2px;
}
</style>



