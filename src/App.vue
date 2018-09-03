<template>
 <div id="app">
   <Title class="title" />
   <BoxesGroup class="boxes-group" />
 </div>
</template>

<script>
import BoxesGroup from './components/BoxesGroup';
import Title from './components/Title';

export default {
  name: 'app',
  components: {
    BoxesGroup,
    Title,
  },
};
</script>

<style>
#app {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-image: url('https://images.unsplash.com/photo-1497454307763-23418967f087?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=7d558fe0b57075b44c31b1e57327ace6&auto=format&fit=crop&w=1950&q=80');
  background-size: cover;
  background-repeat: no-repeat;
  background-position: bottom;
  height: 100vh;
  width: 100vw;
  font-family: 'Ubuntu', sans-serif;
}

body {
  margin: 0;
  padding: 0;
}

.boxes-group {
  flex: 2;
}

.title {
  flex: 0.5;
}
</style>