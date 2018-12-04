<template>
  <div>  
    <h1>Clicked {{ number }}</h1>
    <button @click="iAmClicked()">Click me!</button>
  </div>
</template>
 
<script>
    export default {
        data() {
            return {title: 'Not clicked yet' , number: 0}
        },
        methods: {
            iAmClicked() {
                this.title = 'Clicked times.';
                this.number++;
            }
        }
    };
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
