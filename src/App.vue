<script setup>

</script>

<template>
  <div class="App">
    <h1>Test App</h1>

    <ElDivider />

    <div class="App-buttonContainer">
      <ElButton>Test Action 1</ElButton>
      <ElButton type="primary">Test Action 2</ElButton>
      <ElButton type="success">Test Action 3</ElButton>
      <ElButton type="info">Test Action 4</ElButton>
      <ElButton type="warning">Test Action 5</ElButton>
      <ElButton type="danger">Test Action 6</ElButton>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.App {
  width: 100%;
  height: 100vh;
  max-width: 400px;
  margin: auto;
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;

  &-buttonContainer {
    width: 100%;
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    justify-content: space-between;
  }

  button {
    margin: 0;
  }
}
</style>
