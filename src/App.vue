<template>
  <div id="app">
  <Todos v-bind:todos="todos"/>
  </div>
</template>

<script>
import Todos from './components/Todos'

export default {
  name: 'app',
  components: {
    Todos
  },
  data(){
    return{
      todos: [
        {
          id: 1,
          title: 'VueJS Crash course',
          completed: false
        },
        {
          id: 2,
          title: 'ML Course',
          completed: false
        },
        {
          id: 3,
          title: 'Neural Network Course',
          completed: true
        },
        {
          id: 4,
          title: 'Django Crash Course',
          completed: false
        },

      ]
    }
  }
}
</script>

<style>
 *{
   box-sizing: border-box;
   margin: 0;
   padding: 0;
 }

 body{
   font-family: Arial, Helvetica, sans-serif;
   line-height: 1.4;
 }
</style>
