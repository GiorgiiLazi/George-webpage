<template>
  <Navbar></Navbar>
  <Intro></Intro>
</template>

<script>
import Navbar from './components/Navbar';
import Intro from './components/Intro';

export default {
  name: 'App',
  components: {
    Navbar,
    Intro
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:ital,wght@0,200..800;1,200..800&display=swap');
body{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Plus Jakarta Sans", sans-serif;
  font-optical-sizing: auto;
  background-color: white;
}
</style>
