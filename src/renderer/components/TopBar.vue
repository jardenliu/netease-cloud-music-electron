<template>
  <div class="ncme-top-bar">
      <div class="platfrom-osx-top-bar" v-if="platform == 'darwin'">
        <div class="ncme-top-bar-content" flex="main:justify cross:center">
        <div style="padding-left:9px;height:37px" flex="cross:center">
          <div style="margin-top:2px"><img src="~@/assets/netease_cloud_music.png"  alt=""></div>
          <div style="margin-left:63px;" flex>
            <button class="backward-button">
              <img  src="~@/assets/backward.png"  alt="backward">
              </button>
            <button class="forward-button"><img  src="~@/assets/forward.png"  alt="forward"></button>
          </div>
        </div>
        <div>
          right
        </div>
      </div>
      </div>
      
  </div>
</template>

<script>
export default {
  data() {
    return {
      platform: require("os").platform()
    };
  },
  methods: {}
};
</script>

