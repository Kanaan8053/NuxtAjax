<template>
  <nav class="flex h-12 bg-[#d50000] justify-between px-4 items-center">
    <div class="flex">
      <img src="/img/Ajax-Emblema.png" alt="Ajax Logo" class="flex items-center w-20"/>
      <div class="flex flex-col">
        <a href="index.html">Ajax Website</a>
        <div class="slogan">Welkom bij de mooiste club!</div>
      </div>
    </div>
    <div class="flex text-red-500 gap-3">
      
    <a class=""hover href="/">Home</a>
    <a href="/about">About</a>
    </div>
  </nav>
</template>

<script setup lang="ts">

const sayHello = () => {
  alert("Hello");
}

defineProps<{
  headerTitle: string;
}>();
</script>