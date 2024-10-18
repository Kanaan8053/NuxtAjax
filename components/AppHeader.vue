<template>
  <header>
    <nav>
      <div class="logo-wrapper">
        <div class="logo">
          <img src="/img/Ajax-Emblema.png" alt="Ajax Logo">
        </div>
        <div class="logo-text">
          <a href="/index.html">Ajax Website</a>
          <div class="slogan">Welkom bij de mooiste club!</div>
        </div>
      </div>
      <ul class="ulcodes">
        <li class="navlist"><a href="/pages/overons.html">Over Ons</a></li>
        <li class="navlist"><a href="/pages/quiz.html">Quiz</a></li>
        <li class="navlist"><a href="/pages/contact.html">Contact</a></li>
      </ul>
    </nav>
  </header>
</template>

<script setup lang="ts">

const sayHello = () => {
  alert("Hello");
}

defineProps<{
  headerTitle: string;
}>();
</script>

<style>
.navlist {
  margin-left: 30px;
}

.navlist a {
  text-decoration: none;
  color: #d50000;
  font-size: 18px;
  padding: 10px 20px;
  border-radius: 5px;
  transition: background-color 0.3s, color 0.3s;
}

.navlist a:hover {
  background-color: #d50000;
  color: white;
}

.slogan {
  font-size: 14px;
  color: #000;
  font-weight: bold;
}

nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}

.logo-wrapper {
  display: flex;
  align-items: center;
}

.logo {
  display: flex;
  align-items: center;
  margin-right: 20px;
}

.logo img {
  width: 80px;
  height: auto;
}

.logo-text {
  display: flex;
  flex-direction: column;
}

.logo-text a {
  font-size: 24px;
  font-weight: bold;
  color: #d50000;
  text-decoration: none;
}

.ulcodes {
  list-style: none;
  display: flex;
}

header {
  background-color: #ffffff;
  padding: 20px 0;
  border-bottom: 4px solid #d50000;
}
</style>