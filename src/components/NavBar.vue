<script setup></script>

<template>
  <div class="navbar">
    <img src="/public/favicon.png" height="20px" />
    <span class="nav-item">Início</span>
    <div class="nav-drop">
      <span class="nav-item active">Itens</span>
      <i class="fas fa-angle-down drop-icon" />
    </div>
    <div class="nav-drop">
      <span class="nav-item">Sobre</span>
      <i class="fas fa-angle-down drop-icon" />
    </div>
  </div>
</template>

<style scoped>
.navbar {
  display: flex;
  flex-direction: row;
  background-color: brown;
  padding: 10px;
  gap: 30px;
}

.active {
  font-weight: 600;
}

.nav-drop {
  display: flex;
  flex-direction: row;
  gap: 5px;
  align-items: center;
}

.nav-item {
  color: white;
  font-family: "Cinzel", serif;
  font-style: normal;
  font-size: 18px;
}

.drop-icon {
  width: 12px;
  color: white;
}
</style>
