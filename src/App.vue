<template>
  <AppHeader />

  <AppFilters />

  <main class="app-main">
    <AppTodoList />

    <AppAddTodo />
  </main>

  <footer class="app-footer">2 more to do, 1 done</footer>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import AppHeader from "./components/AppHeader.vue";
import AppFilters from "./components/AppFilters.vue";
import AppTodoList from "./components/AppTodoList.vue";
import AppAddTodo from "./components/AppAddTodo.vue";

export default defineComponent({
  components: {
    AppHeader,
    AppFilters,
    AppTodoList,
    AppAddTodo
  }
})
</script>