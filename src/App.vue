<template>
  <div id="app">
    <input type="text" v-model="todo" v-on="keyup: submitForm | key 'enter'"/><button type="button" @click="addTodo">Add</button>
    <div>
      <h2>Todos</h2>
      <ul>
        <li v-for="todo in todoList">
          {{todo}}
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      todo: '',
      todoList: []
    }
  },
  methods: {
    addTodo: function(){
      this.todoList.push(this.todo)
    },
    removeTodo: function(){
      if(this.todoList.indexOf(this.todo) > -1)
      {
        var i
        this.todoList[]
      }
    }
  },
  computed: function() {
    
  }
}
</script>

<style lang="scss">

</style>
