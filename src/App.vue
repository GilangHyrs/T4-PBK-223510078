<template>
  <div id="app">
    <div class="wrapper">
      <nav class="navbar">
        <ul>
          <li><router-link to="/">HOME</router-link></li>
          <li><router-link to="/post">POST</router-link></li>
          <li><router-link to="/todos">TODOS</router-link></li>
        </ul>
      </nav>
    </div>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
};
</script>

<style>
#app {
  font-family: Arial, sans-serif;
  margin: 0 auto;
  padding: 20px;
  max-width: 600px;
}

.wrapper {
  margin-bottom: 20px;
}

.navbar {
  background-color: #0f0f0f;
  overflow: hidden;
}

.navbar ul {
  list-style-type: none;
  padding: 0;
  margin: 0;
  display: flex;
}

.navbar li {
  padding: 14px 20px;
}

.navbar li a {
  color: rgb(218, 125, 63);
  text-decoration: none;
  display: block;
}

.navbar li a:hover {
  background-color: #302e2e;
}
</style>
