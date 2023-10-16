<script setup></script>


<template>
    <header>
        <nav class="container">
            <div class="logo">
                <RouterLink to="/"><img src="../assets/thedream.jpeg" alt="thedream.logo"></RouterLink>
                <h1>Into The Dream</h1>
            </div>
            <ul class="nav-routes">
            <RouterLink to="/">Home</RouterLink>
            <RouterLink to="/about">About</RouterLink>
            </ul>
        </nav>
    </header>

    <body>
    </body>
</template>


<style lang="scss" scoped>
header {
  background-color: #D8D8D8;
  nav {
    display: flex;
    align-items: center;
    padding: 25px 16px;

    .logo {
      display: flex;
      align-items: center;
      gap: 8px;
      img {
        max-width: 50px;
      }

      h1 {
        font-size: 24px;
      }
    }

    .nav-routes {
      display: flex;
      flex: 1;
      justify-content: flex-end;
      gap: 12px;
      list-style: none;

      a {
        text-decoration: none;
        color: inherit;
      }
    }
  }
}
</style>