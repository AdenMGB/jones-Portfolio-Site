<script setup>
import { RouterLink } from "vue-router";
</script>

<template>
  <div class="content-wrap">
    <h1 class="name-title arcade-title">Arcade</h1>

    <p class="arcade-subtitle">
      A collection of modern and classic browser games.
    </p>

    <div class="arcade-row-1">
      <div class="arcade-card">
        <div class="arcade-card-top">
          <span class="arcade-icon">🧱</span>
          <h3 class="arcade-name">Tetris</h3>
        </div>
        <RouterLink to="/arcade/tetris" class="arcade-card-bottom red-btn">
          Play Now
        </RouterLink>
      </div>

      <div class="arcade-card">
        <div class="arcade-card-top">
          <span class="arcade-icon">🏓</span>
          <h3 class="arcade-name">Pong</h3>
        </div>
        <RouterLink to="/arcade/pong" class="arcade-card-bottom blue-btn">
          Play Now
        </RouterLink>
      </div>

      <div class="arcade-card">
        <div class="arcade-card-top">
          <span class="arcade-icon">💣</span>
          <h3 class="arcade-name">Minesweeper</h3>
        </div>
        <RouterLink
          to="/arcade/minesweeper"
          class="arcade-card-bottom green-btn"
        >
          Play Now
        </RouterLink>
      </div>

      <div class="arcade-card">
        <div class="arcade-card-top">
          <span class="arcade-icon">🪝</span>
          <h3 class="arcade-name">Stickman Hook</h3>
        </div>
        <RouterLink
          to="/arcade/stickman-hook"
          class="arcade-card-bottom red-btn"
        >
          Play Now
        </RouterLink>
      </div>
    </div>

    <div class="arcade-row-2">
      <div class="arcade-card">
        <div class="arcade-card-top">
          <span class="arcade-icon">🧍</span>
          <h3 class="arcade-name">Hangman</h3>
        </div>
        <RouterLink to="/arcade/hangman" class="arcade-card-bottom green-btn">
          Play Now
        </RouterLink>
      </div>

      <div class="arcade-card">
        <div class="arcade-card-top">
          <span class="arcade-icon">⭕</span>
          <h3 class="arcade-name">Noughts & Crosses</h3>
        </div>
        <RouterLink
          to="/arcade/noughts-and-crosses"
          class="arcade-card-bottom red-btn"
        >
          Play Now
        </RouterLink>
      </div>

      <div class="arcade-card">
        <div class="arcade-card-top">
          <span class="arcade-icon">🔢</span>
          <h3 class="arcade-name">2048</h3>
        </div>
        <RouterLink to="/arcade/2048" class="arcade-card-bottom blue-btn">
          Play Now
        </RouterLink>
      </div>
    </div>
  </div>
</template>

<style scoped>
.arcade-title {
  margin-top: 20px;
  margin-bottom: 4px;
  font-size: 72px;
}

.arcade-subtitle {
  color: #94a3b8;
  font-size: 1.05rem;
  margin-bottom: 24px;
  font-weight: 400;
}

.arcade-row-1,
.arcade-row-2 {
  display: grid;
  gap: 21px;
  width: 100%;
  max-width: 900px;
  justify-content: center;
  margin: 0 auto 6px auto;
}

.arcade-row-1 {
  grid-template-columns: repeat(4, 250px);
}

.arcade-row-2 {
  grid-template-columns: repeat(3, 250px);
}

.arcade-card {
  background: rgba(255, 255, 255, 0.03);
  border: 1px solid rgba(255, 255, 255, 0.08);
  border-radius: 16px;
  overflow: hidden;
  display: flex;
  flex-direction: column;
  height: 210px;
  transition: all 0.3s ease;
  backdrop-filter: blur(0px);
  -webkit-backdrop-filter: blur(12px);
}

.arcade-card:hover {
  transform: translateY(-4px);
  border-color: rgba(255, 255, 255, 0.2);
}

.arcade-card-top {
  flex: 1;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 8px;
  padding: 12px;
}

.arcade-icon {
  font-size: 2.5rem;
}

.arcade-name {
  color: white;
  font-size: 1.25rem;
  font-weight: 700;
  margin: 0;
}

.arcade-card-bottom {
  height: 50px;
  display: flex;
  align-items: center;
  justify-content: center;
  text-decoration: none !important;
  font-weight: 800;
  font-size: 0.75rem;
  text-transform: uppercase;
  letter-spacing: 1px;
  border-top: 1px solid rgba(255, 255, 255, 0.05);
  transition: all 0.3s ease;
}

.red-btn {
  background: rgba(255, 71, 87, 0.05);
  color: #ff4757;
}

.red-btn:hover {
  background: #ff4757;
  color: white;
}

.blue-btn {
  background: rgba(0, 162, 255, 0.05);
  color: #00a2ff;
}

.blue-btn:hover {
  background: #00a2ff;
  color: white;
}

.yellow-btn {
  background: rgba(255, 215, 0, 0.05);
  color: #ffd700;
}

.yellow-btn:hover {
  background: #ffd700;
  color: black;
}

.green-btn {
  background: rgba(46, 213, 115, 0.05);
  color: #2ed573;
}

.green-btn:hover {
  background: #2ed573;
  color: white;
}

@media (max-width: 600px) {
  .arcade-row-1,
  .arcade-row-2 {
    grid-template-columns: 1fr;
  }
}
</style>
