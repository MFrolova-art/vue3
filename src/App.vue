<template>
  <div class="todoapp">
      <header class="header">
        <h1>todos</h1>

        <form>
          <input
            type="text"
            data-cy="createTodo"
            class="new-todo"
            placeholder="What needs to be done?"
          />
        </form>
      </header>

      <section class="main">
        <input
          type="checkbox"
          id="toggle-all"
          class="toggle-all"
          data-cy="toggleAll"
        />
        <label htmlFor="toggle-all">Mark all as complete</label>

        <ul class="todo-list" data-cy="todoList">
          <li>
            <div class="view">
              <input type="checkbox" class="toggle" id="toggle-view" />
              <label htmlFor="toggle-view">asdfghj</label>
              <button type="button" class="destroy" data-cy="deleteTodo" />
            </div>
            <input type="text" class="edit" />
          </li>

          <li class="completed">
            <div class="view">
              <input type="checkbox" class="toggle" id="toggle-completed" />
              <label htmlFor="toggle-completed">qwertyuio</label>
              <button type="button" class="destroy" data-cy="deleteTodo" />
            </div>
            <input type="text" class="edit" />
          </li>

          <li class="editing">
            <div class="view">
              <input type="checkbox" class="toggle" id="toggle-editing" />
              <label htmlFor="toggle-editing">zxcvbnm</label>
              <button type="button" class="destroy" data-cy="deleteTodo" />
            </div>
            <input type="text" class="edit" />
          </li>

          <li>
            <div class="view">
              <input type="checkbox" class="toggle" id="toggle-view2" />
              <label htmlFor="toggle-view2">1234567890</label>
              <button type="button" class="destroy" data-cy="deleteTodo" />
            </div>
            <input type="text" class="edit" />
          </li>
        </ul>
      </section>

      <footer class="footer">
        <span class="todo-count" data-cy="todosCounter">
          3 items left
        </span>

        <ul class="filters">
          <li>
            <a href="#/" class="selected">All</a>
          </li>

          <li>
            <a href="#/active">Active</a>
          </li>

          <li>
            <a href="#/completed">Completed</a>
          </li>
        </ul>

        <button type="button" class="clear-completed">
          Clear completed
        </button>
      </footer>
    </div>
</template>
