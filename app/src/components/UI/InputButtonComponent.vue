<template>
  <input type="button" :value="value">
</template>

<script>
export default {
  name: "InputButtonComponent",
  props: {
    value: String
  }
}
</script>

<style lang="less" scoped>
input[type=button] {
  display: flex;
  padding: 11px 24px;
  align-items: flex-start;
  gap: 8px;
  border-radius: 8px;
  background: var(--accent, #2D66EE);
  color: white;
  border: none;
}
</style>