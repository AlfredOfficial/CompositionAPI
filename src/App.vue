<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <div>
      <nav>
        <RouterLink to="/" class="nav-link">Home</RouterLink>
        <RouterLink to="/add-post" class="nav-link">Add Post</RouterLink>
      </nav>
    </div>
  </header>
  <RouterView />
</template>

<style lang="scss" scoped>
nav {
  padding: 1rem 2rem;
  background-color: #90caf9;
  border-bottom: 1px solid #90caf9;
  .nav-link {
    color: #fff;
    padding: 5px 15px;
    border-radius: 5px;
    transition: all 0.2s ease-in-out;
    margin-right: 1rem;
    &:hover {
      background-color: #90caf9;
    }
  }
}
</style>
