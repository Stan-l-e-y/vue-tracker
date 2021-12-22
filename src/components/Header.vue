<template>
  <header>
    <h1>{{ title }}</h1>
    <Button @click="onClick()" text="Add Task" color="green"></Button>
  </header>
</template>

<script>
import Button from './Button.vue';

export default {
  name: 'Header',
  props: {
    title: {
      default: 'weed',
    },
  },
  components: {
    Button,
  },
  methods: {
    onClick() {
      console.log('weed');
    },
  },
};
</script>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}
</style>
