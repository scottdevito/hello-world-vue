<template>
 <div class="boxes-group">
   <Box big="false" small="true" />
   <Box big="true" small="false" />
   <Box big="false" small="true" />
 </div>
</template>

<script>
import Box from './Box';

export default {
  name: 'BoxesGroup',
  components: {
    Box,
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