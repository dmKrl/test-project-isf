<template>
  <div class="app">
    <navbar></navbar>
    <router-view></router-view>
  </div>
</template>

<script>
import Navbar from '@/components/Navbar/Navbar.vue';
export default {
  components: {
    Navbar,
  },
};
</script>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

html {
  background: #f4f4f4;
  overflow-x: hidden;
}
textarea:focus {
  outline: none;
}
button {
  cursor: pointer;
}
.app {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 20px;
  gap: 20px;
}
.task-done {
  color: rgb(47, 134, 47);
}
.task-nodone {
  color: rgb(239, 53, 53);
}
.task-buttons {
  display: flex;
  flex-wrap: wrap;
  justify-content: flex-end;
  gap: 10px;
}
</style>
