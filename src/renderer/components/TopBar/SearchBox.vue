<template>
<div class="search-box" flex="cross:center">
    <div class="search-box-content" flex="cross:center">
        <div flex="cross:center" style="z-index: 2;">
            <img src="~@/assets/icons/search.png"  alt="search_icon">
        </div>
        <div flex="cross:center" class="input-box" style="z-index: 2;">
            <input type="text" placeholder="搜索音乐，歌手，歌词，用户">
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


<style>
.search-box {
  position: relative;
}

.search-box-content {
  height: 24px;
  background: white;
  z-index: 1;
  border-radius: 15px;
  padding: 0 3px;
  margin-left: 8px;
}

.platfrom-win32-top-bar .search-box-content {
  background: rgba(0, 0, 0, 0.2);
  height: 22px;
}

.search-box-content input {
  border: none;
  height: 22px;
  width: 202px;
  font-size: 14px;
  background: inherit;
  margin-left: 1px;
}
.search-box-content input:focus {
  outline: none;
}
.search-box-content input::-webkit-input-placeholder {
  font-size: 11.5px !important;
  color: #a2a2a2;
}
</style>
