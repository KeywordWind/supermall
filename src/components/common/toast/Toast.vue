<template>
  <div v-show="isShow" id="toast">
    <div>{{ message }}</div>
  </div>
</template>
<script>
export default {
  name: "Toast",
  data() {
    return {
      message: "",
      isShow: false,
    };
  },
  methods: {
    show(message, duration = 2000) {
      this.isShow = true;
      this.message = message;
      setTimeout(() => {
        this.isShow = false;
        this.message = "";
      }, duration);
    },
  },
};
</script>
<style scoped>
#toast {
  position: fixed;
  top: 50%;
  left: 50%;
  padding: 8px 10px;
  transform: translate(-50%, -50%);
  background-color: rgba(0, 0, 0, 0.4);
  color: #fff;
  z-index: 10;
}
</style>