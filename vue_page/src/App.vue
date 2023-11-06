<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header>
    <img alt="Profile Pic" class="logo" src="@/assets/logo.png" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="Hello my name is Artem Rudenko"/>
      <nav>
        <ul>
          <li><RouterLink to="/">Home</RouterLink></li>
          <li><RouterLink to="/about">About</RouterLink></li>
          <li><RouterLink to="/project0">Project 0</RouterLink></li>
        </ul>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav ul {
    list-style: none; /* Remove default list styles */
    padding: 0;
    margin: 0;
  }

  nav li {
    margin-bottom: 10px; /* Add space between the list items */
  }

  nav li:last-child {
    margin-bottom: 0; /* Remove margin for the last item to prevent extra spacing at the bottom */
  }

  nav a {
    text-decoration: none; /* Remove underline from links */
    color: #333; /* Set link color */
    display: block; /* Make the links fill the width of the list item */
    padding: 5px 0; /* Add some padding for better clickability */
  }

  nav a:hover {
    color: #007bff; /* Change color on hover */
    background-color: #f8f9fa; /* Optional: Add a background color on hover */
  }

  /* Add some padding and possibly a border to the nav element if you like */
  nav {
    padding: 20px;
    border-right: 1px solid #ddd; /* Optional: Add a right border */
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
