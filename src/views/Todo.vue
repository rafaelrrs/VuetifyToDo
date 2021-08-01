<template>
  <div class="home">
    <filed-add-task />
    <list-task v-if="$store.state.tasks.length" />
    <no-tasks v-else />
  </div>
</template>

<script>
import FieldAddTask from "@/components/Todo/FieldAddTask.vue";
import ListTasks from "@/components/Todo/ListTasks.vue";
import NoTasks from "@/components/Todo/NoTasks.vue";

export default {
  name: "Home",
  components: {
    "filed-add-task": FieldAddTask,
    "list-task": ListTasks,
    "no-tasks": NoTasks,
  },
};
</script>
