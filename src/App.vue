<template>
  <div>
    <input v-model="name">
    <p>{{ name }}</p>
    <Hello :name="name"></Hello>
  </div>
</template>

<script>
import Hello from './components/Hello'

export default {
  data () {
    return {
      name: 'test'
    }
  },
  components: {
    Hello
  },
  mounted () {
    $(this.$el)
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
