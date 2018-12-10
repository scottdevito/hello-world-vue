<template>
   <div class="box" v-bind:style="[isSmall ? smallStyles : bigStyles]">
     <h2 class="text-copy">Some Text</h2>
     <img :src="imgSrc" />
     <button class="box-button">Details</button>
   </div>
</template>

<script>
export default {
  name: 'Box',
  props: ['isSmall', 'imgSrc'],
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
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;
  background: #313131;
  box-shadow: 0px 4px 30px rgba(0, 0, 0, 0.35);
  filter: blur(0.2px);
  border-radius: 8px;
  margin: 0 3rem;
}

.box-button {
  background: linear-gradient(90deg, #fdc165 -29.31%, #fcf7f0 166.81%);
  box-shadow: 0px 4px 10px rgba(253, 193, 101, 0.25);
  border-radius: 4px;
  height: 2rem;
  width: 8rem;
  padding: 0.5rem 1rem;
  border: none;
  color: #000;
  font-weight: 500;
  cursor: pointer;
  transition: ease 1s all;
}

.box-button:focus {
  outline: none;
}

.text-copy {
  font-weight: 300;
  line-height: normal;
  font-size: 36px;
  color: #fdfdfd;
  margin: 0;
}
</style>