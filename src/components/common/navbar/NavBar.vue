<template>
  <div class="nav-bar">
    <div class="left"><slot name="left"></slot></div>
    <div class="center"><slot name="center"></slot></div>
    <div class="right"><slot name="right"></slot></div>
  </div>
</template>
<script >
export default {
  name: "NavBar",
};
</script>
<style scoped>
.nav-bar {
  display: flex;
  height: 44px;
  line-height: 44px;
  text-align: center;
  box-shadow: 0 0px 5px rgba(100, 100, 100, 0.6);
  color: white;
  background-color: var(--color-tint);
  font-size: 18px;
}
.left,
.right {
  width: 60px;
}
.center {
  flex: 1;
}
</style>