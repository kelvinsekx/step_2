<script>
import TodoDay from './TodoDay.vue'
export default {
  name: 'calendar-week',
  components: {
    TodoDay
  },
  data() {
    return {
      tasksPerDay: [
        {
          day: 'Monday',
          tasks: [
            'Spent time with Nophy',
            'Eat Amala and Ewedu with David',
            'Eat scrotched egg for the first time.'
          ]
        },
        {
          day: 'Tuesday',
          tasks: [
            "David went to kiishi's house",
            'I went to see Gozinne in her office',
            'Exclusive members Merch is out 😍'
          ]
        },
        {
          day: 'Wednesday',
          tasks: ['Todo Wednesday 1', 'Todo Wednesday 2', 'Todo Wednesday 3']
        }
      ]
    }
  }
}
</script>

<template>
  <div class="calendarWeek">
    <TodoDay v-for="day in tasksPerDay" v-bind:todoDay="day" />
  </div>
</template>

<style scope>
.calendarWeek {
  display: flex;
  gap: 4rem;
}
</style>
