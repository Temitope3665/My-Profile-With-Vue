<template>
  <div class="about-wrapper">
    <h2 class="about-header">About Me</h2>
    <p class="about-me">Hi there, I'm Temitope, I'm a Software Developer, passionate about building highly scalable products to solve problems using web and mobile technologies.
    My stacks are HTML | CSS | Javascript | Vue Js 
    If i am not coding, I design and play video games.</p>

    <p class="click-here">Click here to know about <router-link :to="{name: 'AboutEnyata'}"> Enyata </router-link></p>

    <router-view />
  </div>
  
</template>

<script>
export default {

}
</script>

<style scoped>
.about-wrapper {
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.about-me {
  width: 40%;
  line-height: 20px;
  text-align: center;
  margin-top: 20px;
  margin-right: auto;
  margin-left: auto;
  line-height: 36px;
}

  a {
    font-weight: 400;
    color: #3F4FD7;
    text-decoration: none;

    /* a.router-link-exact-active {
      color: #fff;
      background: #3F4FD7;
      padding: 14px;
      border-radius: 6px ;
    } */
  }
  .about-header {
    color: #3F4FD7;
  }

</style>