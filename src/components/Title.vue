<template>
<div class="title-wrapper">
  <p class="title-copy">Some Title</p>
</div>
</template>

<script>
export default {
  name: 'Title',
};
</script>

<style scoped>
.title-wrapper {
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  align-items: center;
  height: 100%;
  letter-spacing: 0.08em;
  color: #4e4a45;
  font-weight: 400;
  font-size: 46px;
}

.title-copy {
  margin: 0;
}
</style>