<template>
  <AppHeader />

  <AppFilters />

  <main class="app-main">
    <AppTodoList />

    <section class="add-todo">
      <button class="add-todo__show-form-button">
        <i class="bi bi-plus-lg"></i>
      </button>
      <form class="add-todo__form">
        <button class="close-button" type="button">
          <i class="bi bi-x"></i>
        </button>
        <div class="text-input text-input--focus">
          <input class="input" />
        </div>
        <button class="button button--filled">Add task</button>
      </form>
    </section>
  </main>

  <footer class="app-footer">2 more to do, 1 done</footer>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import AppHeader from "./components/AppHeader.vue";
import AppFilters from "./components/AppFilters.vue";
import AppTodoList from "./components/AppTodoList.vue";

export default defineComponent({
  components: {
    AppHeader,
    AppFilters,
    AppTodoList
  }
})
</script>