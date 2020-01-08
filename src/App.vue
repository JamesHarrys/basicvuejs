<template>
  <div id="app">
    <ToDos v-bind:todos="todos"/>
  </div>
</template>

<script>
import ToDos from "./components/ToDos";
export default {
  name: 'app',
  components: {
    ToDos
  },
  data() {
    return {
      todos: [
        {
          id: 1,
          title: 'ToDo One',
          completed: false
        },
        {
          id: 2,
          title: 'ToDo Two',
          completed: false
        },
        {
          id: 3,
          title: 'ToDo Three',
          completed: false
        },
      ]
    }
  }
}
</script>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: UniversTE20T, Helvetica, sans-serif;
  line-height: 1.4;
}
</style>
