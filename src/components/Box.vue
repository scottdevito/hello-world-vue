<template>
   <div class="box" v-bind:style="[isSmall ? smallStyles : bigStyles]">{{ isSmall }}</div>
</template>

<script>
export default {
  name: 'Box',
  props: ['isSmall'],
  data: function() {
    return {
      bigStyles: {
        height: '20rem',
        width: '14rem',
      },
      smallStyles: {
        height: '16rem',
        width: '14rem',
      },
    };
  },
};
</script>

<style scoped>
.box {
  background: #313131;
  box-shadow: 0px 4px 30px rgba(0, 0, 0, 0.35);
  filter: blur(1px);
  border-radius: 8px;
  margin: 0 3rem;
}

.big {
  height: 22rem;
  width: 14rem;
}

.small {
  height: 20rem;
  width: 14rem;
}
</style>