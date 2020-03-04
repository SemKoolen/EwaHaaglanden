<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      Welcome to the first Vue-application by {{ name }}
    </p>
    <CustomerList />
    <Projects />
  </div>
</template>

<script>
import CustomerList from "./CustomerList";
import Projects from "./Projects";
export default {
  name: 'HelloWorld',
  components: {Projects, CustomerList},
  props: {
    msg: String,
    name: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
