<script setup>
function buscar() {
  const termo = document.getElementById('search').value;
  alert('Você pesquisou por: ' + termo);
}
</script>

<template>
  <header>
    <nav>
      <div class="topo">
        <div class="logo">
          <h1>IFbooks</h1>
          <p>apreço a<br>leitura</p>
        </div>
        <div class="search">
          <input type="text" id="search" placeholder="Digite sua pesquisa...">
          <button @click="buscar">
            <i class="fas fa-search"></i>
          </button>
        </div>
        <div class="paginas">
          <p>Termos</p>
          <p>Equipe</p>
          <p>Envio</p>
          <p>Devoluções</p>
        </div>
        <div class="icons">
          <p><i class="fa-solid fa-cart-shopping"></i></p>
          <p><i class="fa-solid fa-heart"></i></p>
          <p><i class="fa-solid fa-user"></i></p>
        </div>
      </div>
    </nav>
  </header>
</template>

<style scoped>
div.topo {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px;
}

.logo {
  display: flex;
  flex-direction: column;
}

.paginas {
  display: flex;
  gap: 10px;
}

.search {
  display: flex;
  align-items: center;
  gap: 5px;
}

input[type="text"] {
  padding: 10px;
  width: 300px;
  font-size: 16px;
}

button {
  padding: 10px 15px;
  font-size: 16px;
  cursor: pointer;
  background-color: #007bff;
  color: white;
  border: none;
}

button i {
  pointer-events: none;
}
</style>