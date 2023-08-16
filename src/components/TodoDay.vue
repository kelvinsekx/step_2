<script>
export default {
  name: 'calendar-week',
  props: ['todoDay']
}
</script>

<template>
  <div class="TodoDayWrapper">
    <div class="day">{{ todoDay.day }}</div>
    <div class="todo" v-for="task in todoDay.tasks">{{ task }}</div>
  </div>
</template>

<style scope>
.TodoDayWrapper {
  border: 1px solid #444;
  width: 15rem;
}
.day {
  background-color: #444;
  color: white;
  text-align: center;
}

.todo {
  background-color: aqua;
  color: #222;
  padding: 0.4rem 0.6rem;
  width: 75%;
  margin: 0.5rem auto;
}
</style>
