<script setup>
import { RouterLink } from 'vue-router';
</script>


<template>
    <header>
        <nav class="container">
            <div class="logo">
                <RouterLink to="/"><img src="../assets/logo.png" alt="thedream.logo" draggable="false"></RouterLink>
                <h1 to="/">Vanilla</h1>
            </div>
            <ul class="nav-routes">
            <RouterLink to="/">Home</RouterLink>
            <RouterLink to="/music">Music</RouterLink>
            <RouterLink to="/videos">Videos</RouterLink>
            <RouterLink to="/about">About</RouterLink>
            </ul>
        </nav>
    </header>

    <body>
    </body>
</template>


<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Lobster&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');
header {
  background-color: #D8D8D8;
  nav {
    display: flex;
    align-items: center;
    padding: 12px 12px;

    .logo {
      display: flex;
      align-items: center;
      gap: 8px;
      img {
        max-width: 60px;
      }

      h1 {
        font-size: 36px;
        font-family: 'Lobster', sans-serif;
      }
    }

    .nav-routes {
      display: flex;
      flex: 1;
      justify-content: flex-end;
      gap: 12px;
      list-style: none;

      a {
        font-family: 'Roboto', sans-serif;
        font-size: 18px;
        padding: 0 10px ;
        font-weight: 500;
        text-decoration: none;
        color: inherit;
      }

      a :active {
        color: blue;
      }
    }
  }
}
</style>