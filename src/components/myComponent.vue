<script>
export default {
  name: 'my-component',
  data() {
    return {
      getGreeting: 'Hello Kelvin'
    }
  },
  computed: {
    reversedGreeting() {
      const str = this.getGreeting
      let nonsense = str.split('').reverse().join('')
      return nonsense
    }
  }
}
</script>

<template>
  <h2>{{ reversedGreeting }}</h2>
  <p>This is the Hello World component.</p>
</template>
