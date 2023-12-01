<template>
  <header class="header">
    <h2>weather appliciation</h2>
    <p>{{ username }}님 반갑습니다!</p>
  </header>
</template>

<script>
export default {
  name: "HeaderDisplay",
  props: {
    userInfo: {
      type: Object,
      default() {
        return {
          id: "guest",
          name: "Guest",
        };
      },
    },
  },
};
</script>

<style>
.header {
  background: linear-gradient(to right, #12c2e9, #c471ed, #f64f59);
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1em 1em;
}
header h2 {
  color: #fff;
}
.header p {
  font-size: 12px;
  color: #fff;
}
</style>