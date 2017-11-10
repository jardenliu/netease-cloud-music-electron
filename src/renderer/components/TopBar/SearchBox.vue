<template>
<div class="search-box" flex="cross:center">
    <div class="search-box-content" flex="cross:center">
        <div flex="cross:center">
            <img src="~@/assets/icons/search.png"  style="position: relative;left: -5px;" alt="search_icon">
        </div>
        <div flex="cross:center">
            <input type="text" placeholder="搜索音乐，歌手，歌词，用户">
        </div>
    </div>
</div>
</template>


<script>
export default {};
</script>

<style>
.search-box {
  height: 24px;
  position: relative;
  left: -4px;
}
.search-box-content {
  background: white;
  z-index: 1;
}

.search-box-content input {
  border: none;
  height: 22px;
  margin-left: -5px;
  width: 194px;
  font-size: 14px;
}
.search-box-content input:focus {
  outline: none;
}
.search-box-content input::-webkit-input-placeholder {
  font-size: 12px !important;
  color: #a2a2a2;
}

.search-box:before {
  content: " ";
  display: block;
  background: white;
  width: 22px;
  height: 24px;
  position: relative;
  border-top-left-radius: 50%;
  border-bottom-left-radius: 50%;
  left: 12px;
}

.search-box::after {
  content: " ";
  display: block;
  background: white;
  width: 22px;
  height: 24px;
  position: relative;
  border-top-right-radius: 50%;
  border-bottom-right-radius: 50%;
  left: -8px;
}
</style>
