<template>
  <div v-for="task in tasks" :key="task.id">
    <Card :task="task" />
  </div>
</template>

<script>
import Card from "./Card.vue";
export default {
  name: "card-list",
  components: {
    Card,
  },
  props: {
    tasks: Array,
  },
  data() {
    return {
      // tasks: [
      //   { title: "task1", id: 1 },
      //   { title: "task2", id: 3 },
      //   { title: "task2", id: 3 },
      // ],
    };
  },
};
</script>

<style></style>
