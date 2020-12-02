<template>
  <form class="col-12 col-sm-10 col-md-8 col-lg-6" @submit.prevent="addTodo">
    <input type="text" class="form-control" placeholder="New Todo" v-model="newTodo">
    <div class="row">
      <div class="col-xs-12 col-sm-8 col-sm-offset-2 col-md-6 col-md-offset-3">
        <button
            class="btn btn-primary" @click="addTodo">Submit!
        </button>
      </div>
    </div>
  </form>
</template>
<script>
export default {
  data(){
    return{
      newTodo:''
    }
  },
  methods:{
    addTodo(){
      if(this.newTodo.length>0){
        this.$emit('on-new-todo',this.newTodo);
      }
      this.newTodo=''
    }
  }
}
</script>
<style scoped></style>