<template>
  <div class="hello">
    <h1>{{ msg }} {{ year }}</h1>
    <p @keyup="greet">
      Learning Vue 
    </p>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
    year: {
      type: String,
      required: true
    }
  },
  methods: {
    greet(){
      console.log('enter key is pressed')
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style> 
