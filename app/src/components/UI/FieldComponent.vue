<template>
  <div class="field">
    <label for="field">
      {{ label }}
    </label>
    <div>
      <input id="field" :type="type" name="field" :placeholder="placeholder">
    </div>
  </div>
</template>

<script>
export default {
  name: "FieldComponent",
  props: {
    type: String,
    label: String,
    placeholder: String
  }
}
</script>

<style lang="less" scoped>
.field {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  gap: 8px;
  padding-bottom: 10px;
  border-bottom: solid 0.3px var(--gray-500);
  label {
    color: var(--gray-500, #667085);
    font-feature-settings: 'clig' off, 'liga' off;
    font-size: 13px;
    font-style: normal;
    font-weight: 500;
    line-height: 16px;
    letter-spacing: -0.078px;
  }
  input {
    display: flex;
    align-items: flex-start;
    gap: 8px;
    border: none;
  }
}
</style>