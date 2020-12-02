<template>
<todo-list list-name="My to-dos"/>

</template>

<script>
import TodoList from './Components/TodoList';
export default {
  components:{
   TodoList
  }
}
</script>
<!--global style-->
<style>
body{
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
