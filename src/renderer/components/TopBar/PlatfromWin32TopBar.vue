<template>
  <div class="platfrom-win32-top-bar">
    <div class="ncme-top-bar-content" flex="main:justify cross:center">
     <TopBarLeft></TopBarLeft>
      <div flex="cross:center">
        <div flex="cross:center">
          <img src="~@/assets/icons/envelope18.png" style="margin:0 10px;border-radius:5px" alt="forward">
          <img src="~@/assets/icons/setting18.png" style="margin:0 22px;" alt="forward">
        </div>
        <div class="platfrom-win32-user-logo-box" flex="main:center cross:center">
          <div flex="cross:center">
              <div style="background:rgb(216,216,216);border-radius:50%;width: 23px; height:23px;margin-left: 5px;" flex="main:center cross:center">
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
</template>

<script>
import TopBarLeft from "./TopBarLeft.vue";
export default {
  components: {
    TopBarLeft
  },
  data() {
    return {};
  },
  methods: {}
};
</script>


