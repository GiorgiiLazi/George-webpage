<template>
  <main id="main-page">
    <section id="introduction">
        <h1>Hello,</h1>
        <h1>I'M George</h1>
        <h3>Frontend Developer</h3>
    </section>
    <section id="my-img">
        <img src="../assets/photo-1.png" alt="">
    </section>
    <section id="btn">
      <button>Contact Me</button>
    </section>
  </main>

</template>

<script>
export default {
    setup(){

    }
}
</script>

<style>
#main-page{
  display: flex;
  justify-content: space-between;
  max-height: 400px;;
  background-color: black;
  background: linear-gradient(-135deg);
  color: white;
  position: relative;
  clip-path: polygon(0 0, 100% 0, 100% 90%, 50% 100%, 50% 100%, 0 90%);
}
#introduction{
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  margin-top: 150px;
  margin-left: 100px;
  width: fit-content;
}
#introduction *{
  padding: 0;
  margin: 0;
  white-space: nowrap;
  overflow: hidden;
}
#btn{
  position: absolute;
  left: 100px;
  bottom: 100px;
}
#btn button{
  width: 200px;
  border: 2px darkorange solid;
  cursor: pointer;
  background-color: transparent;
  color: darkorange;
}
#my-img{
  text-align: center;
  max-width: 90%;
}
#my-img img{
    max-height: 90%;
    height: auto;
    margin: 0;
    padding: 0;
    border-radius: 40%;
}

</style>