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
        <!-- Logo + Apreço -->
        <div class="logo-container">
          <div class="logo">
            <h1>IFbooks</h1>
          </div>
          <div class="apreco">
            <p>apreço a<br>leitura</p>
          </div>
        </div>

        <!-- Campo de busca -->
        <div class="search">
          <input
            type="text"
            id="search"
            placeholder="Digite sua pesquisa..."
          />
          <button @click="buscar">
            <i class="fas fa-search"></i>
          </button>
        </div>

        <!-- Navegação -->
        <div class="paginas">
          <p><a href="#">Termos</a></p>
          <p><a href="#">Equipe</a></p>
          <p><a href="#">Envio</a></p>
          <p><a href="#">Devoluções</a></p>
        </div>

        <!-- Ícones -->
        <div class="icons">
          <p><i class="fa-solid fa-cart-shopping"></i></p>
          <p><i class="fa-solid fa-heart"></i></p>
          <p><i class="fa-solid fa-user"></i></p>
        </div>
      </div>
    </nav>
  </header>
  <main>
    <section class="destaques">
<div class="livro">
  <div>
    <p>Autor de Abril</p>
    <h1>Eric-Emanuel Schmitt </h1>
    <p>Eric-Emmanuel Schmitt has been awarded more than 20<br>literary prizes and distinctions, and in 2001 he received the<br>title of Chevalier des Arts et des Lettres. His books have been<br>translated into over 40 languages.</p>
    <button>Acessar página do livro</button>
  </div>
  <div>
    <img src="/public/img/book.png" alt="">
    <p>*within the stock limit</p>
  </div>
</div>
    </section>

  </main>
</template>

<style scoped>
/* Header */
header {
  color: white;
}

/* Container principal */
.topo {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px;
  margin: 1vw 0 1vw 2vw;
}

/* Logo + Apreço */
.logo-container {
  display: flex;
  align-items: center;
  gap: 10px;
}

.logo h1 {
  margin: 0;
}

.apreco {
  display: flex;
  margin: 0;
}

.apreco p {
  margin: 0;
  font-size: 14px;
}

/* Campo de busca */
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

/* Links da navegação */
.paginas {
  display: flex;
  gap: 10px;
}

a {
  text-decoration: none;
}

/* Ícones */
.icons {
  display: flex;
  gap: 10px;
}
div.livro{
  display: flex;
}
</style>
