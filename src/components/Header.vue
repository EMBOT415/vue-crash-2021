<template>
  <header>
    <h1>{{ title }}</h1>
    <Button text="Add Task" color="blue" />
  </header>
</template>

<script>
// import { defineComponent } from '@vue/composition-api'
import Button from './Button'
// import Button from './Button.vue'
export default {
  name: 'Header',
  props: {
    title: String,
  },
  components: {
    Button
  }

}
</script>

<style scoped> 
 header {
   display: flex;
   justify-content: space-between;
   align-items: center;
   margin-bottom: 20px;
 }
</style>