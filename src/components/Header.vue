<template>
    <header>
        <h2>{{title}}</h2>
        <Button  @btn-click="$emit('toggle-add-task')"  :text="showAddTask?'Close':' Add Task'" :color="showAddTask?'red':'green'" />
    </header>
</template>

<script>
import Button from './Button'

export default {
  components: { Button },
    name:'HeaderVue',
    props:{
      title: String,
      showAddTask:Boolean

    },

  

   
}
</script>
<style scoped>
header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
}


</style>