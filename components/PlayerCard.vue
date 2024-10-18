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