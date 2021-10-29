<template>
  <div id="app">
    <div id="nav">
      <!-- <router-link :to="{name: 'Home'}">Home</router-link> |
      <router-link to="/about">About</router-link> -->
      <ul>
        <li><router-link :to="{name: 'Home'}">Home </router-link></li>
        <li><router-link :to="{name: 'About'}">About</router-link></li>
        <li><router-link :to="{name: 'Contact'}">Contact us</router-link></li>
      </ul>
    </div>
    <router-view />
  </div>
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;500;600;700&display=swap');
#app {
  font-family: Poppins, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 20px;

  a {
    font-weight: 400;
    color: #3F4FD7;
    text-decoration: none;
    box-shadow: rgba(50, 50, 93, 0.25) 0px 30px 60px -12px, rgba(0, 0, 0, 0.3) 0px 18px 36px -18px;

    &.router-link-exact-active {
      color: #fff;
      background: #3F4FD7;
      padding: 14px;
      border-radius: 6px ;
    }
  }
}
ul {
  list-style-type: none;
  text-decoration: none;
  display: flex;
  flex-direction: row;
  justify-content: end;
}
li {
  padding: 30px;
}
</style>
