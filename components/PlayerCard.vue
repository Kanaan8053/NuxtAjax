<template>
    <div class="player-card">
        <h3>{{ playerName }}</h3>
        <p>Positie: {{ position }}</p>
      </div>
</template>

<script setup lang="ts">

defineProps<{
 playerName: string;
 position: string;
}>();
</script>

<style>
.player-card {
    background-color: #f4f4f4;
    border: 1px solid #d50000;
    border-radius: 10px;
    padding: 20px;
    text-align: center;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}
.player-card:hover{
    cursor: pointer;
}

.player-card img {
    width: 100%;
    height: auto;
    border-radius: 0;
    margin-bottom: 10px;
}

.player-card h3 {
    color: #d50000;
    margin-bottom: 10px;
}

.player-card p {
    color: #333;
}
</style>