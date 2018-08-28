<template>
 <div class="box" v-bind:class="{ big: big, small: small }"></div>
</template>

<script>
export default {
  name: 'Box',
  props: {
    big: Boolean,
    small: Boolean,
  },
};
</script>

<style scoped>
.box {
  background: #313131;
  box-shadow: 0px 4px 30px rgba(0, 0, 0, 0.35);
  filter: blur(2px);
  border-radius: 8px;
  margin: 0 3rem;
}

.big {
  height: 28rem;
  width: 14rem;
}

.small {
  height: 20rem;
  width: 14rem;
}
</style>