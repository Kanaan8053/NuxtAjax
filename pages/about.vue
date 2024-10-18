<template>
  <section>
    <section class="players-section">
      <h2>Huidige Spelers van Ajax</h2>
      <div class="players-grid">
        <PlayerCard 
          v-for="(player, index) in players" 
          :key="index" 
          :position="player.position" 
          :playerName="player.playerName" 
        />
      </div>
    </section>
  </section>
</template>

<script setup lang="ts">
interface Player {
  playerName: string;
  position: string;
}


const players: Player[] = [
  // Doelmannen
  { playerName: "Remko Pasveer", position: "Doelman" },
  { playerName: "Diant Ramaj", position: "Doelman" },
  { playerName: "Jay Gorter", position: "Doelman" },
  { playerName: "Charlie Setford", position: "Doelman" },

  // Verdedigers
  { playerName: "Daniele Rugani", position: "Verdediger" },
  { playerName: "Owen Wijndal", position: "Verdediger" },
  { playerName: "Josip Sutalo", position: "Verdediger" },
  { playerName: "Gaston Avila", position: "Verdediger" },
  { playerName: "Devyne Rensch", position: "Verdediger" },
  { playerName: "Ahmetcan Kaplan", position: "Verdediger" },
  { playerName: "Youri Baas", position: "Verdediger" },
  { playerName: "Jorrel Hato", position: "Verdediger" },
  { playerName: "Anton Gaaei", position: "Verdediger" },
  { playerName: "Dies Janse", position: "Verdediger" },
  { playerName: "Jorthy Mokio", position: "Verdediger" },

  // Middenvelders
  { playerName: "Jordan Henderson", position: "Middenvelder" },
  { playerName: "Branco van den Boomen", position: "Middenvelder" },
  { playerName: "Sivert Mannsverk", position: "Middenvelder" },
  { playerName: "Kenneth Taylor", position: "Middenvelder" },
  { playerName: "Kristian Hlynsson", position: "Middenvelder" },
  { playerName: "Kian Fitz Jim", position: "Middenvelder" },
  { playerName: "Benjamin Tahirovic", position: "Middenvelder" },

  // Aanvallers
  { playerName: "Steven Berghuis", position: "Aanvaller" },
  { playerName: "Chuba Akpom", position: "Aanvaller" },
  { playerName: "Bertrand Traore", position: "Aanvaller" },
  { playerName: "Wout Weghorst", position: "Aanvaller" },
  { playerName: "Brian Brobbey", position: "Aanvaller" },
  { playerName: "Christian Rasmussen", position: "Aanvaller" },
  { playerName: "Amourricho van Axel Dongen", position: "Aanvaller" },
  { playerName: "Julian Rijkhoff", position: "Aanvaller" },
  { playerName: "Jaydon Banel", position: "Aanvaller" },
  { playerName: "Mika Godts", position: "Aanvaller" }
];
</script>

<style>
.players-section{
    text-align: center;
}

.players-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr); 
    gap: 20px;
    justify-content: center;
}
</style>