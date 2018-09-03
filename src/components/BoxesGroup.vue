<template>
 <div class="boxes-group">
   <Box v-bind:isSmall="true" />
   <Box v-bind:isSmall="false" />
   <Box v-bind:isSmall="true" />
 </div>
</template>

<script>
import Box from './Box';

export default {
  name: 'BoxesGroup',
  components: {
    Box,
  },
  data: () => {
    return {
      isSmall: '',
    };
  },
};
</script>

<style scoped>
.boxes-group {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}
</style>