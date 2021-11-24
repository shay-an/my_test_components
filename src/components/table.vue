<template>
  <div class="bg">
    <div class="table">
      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isShow: true,
    };
  },
  methods: {
    show() {
      this.isShow = false;
    },
  },
};
</script>

<style>
.bg {
  position: fixed;
  left: 0;
  top: 0;
  right: 0;
  bottom: 0;
  background: rgba(0, 0, 0, 0.5);
}
.table {
  position: fixed;
  left: 0;
  top: auto;
  right: 0;
  bottom: 0;
  background: red;
}
</style>