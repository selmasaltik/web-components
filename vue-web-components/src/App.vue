<template>
  <div class="App">
    <input placeholder="Enter your name" v-model="name" />

    <div class="greeting">Hello {{ name }}!</div>

    <search-result v-bind:name-attribute="name"></search-result>
  </div>
</template>

<script>
//import our Web Component
import './web-components/search-result';

export default {
  data() {
    return {
      name: '',
    };
  },
};
</script>

<style>
.App {
  margin-top: 30px;
  text-align: center;
}
.greeting {
  margin-top: 20px;
}
</style>