<template>
  <div class="about">
    <h1>Contato</h1>
    <div class="itens">
      <div class="item-icon">
        <img class="icon" src="@/assets/logos/github.svg">
      </div>
      <p class="item-text">
        <a href="https://github.com/gabrielsantos19">@gabrielsantos19</a>
      </p>
      
      <div class="item-icon">
        <svg class="icon" viewBox="0 0 36 27" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M2.45453 26.9996H8.18176V13.0939L0 6.95898V24.5456C0 25.9014 1.0984 26.9996 2.45453 26.9996Z" fill="#4285F4"></path>
          <path d="M27.8182 26.9996H33.5455C34.9016 26.9996 36 25.9014 36 24.5456V6.95898L27.8182 13.0939V26.9996Z" fill="#34A853"></path>
          <path d="M27.8182 2.46056V13.0943L36 6.95947V3.68754C36 0.654864 32.5371 -1.07722 30.1091 0.742797L27.8182 2.46056Z" fill="#FBBC04"></path>
          <path fill-rule="evenodd" clip-rule="evenodd" d="M8.18182 13.0947V2.46094L17.9999 9.82279L27.818 2.46094V13.0947L17.9999 20.4566L8.18182 13.0947Z" fill="#EA4335"></path>
          <path d="M0 3.68754V6.95947L8.18176 13.0943V2.46056L5.89087 0.742797C3.46293 -1.07722 0 0.654864 0 3.68754Z" fill="#C5221F"></path>
        </svg>
      </div>
      <p class="item-text">
        <a href="mailto:gabrielos@dcomp.ufs.br">gabrielos@dcomp.ufs.br</a>
      </p>

      <div class="item-icon">
        <img class="icon" src="@/assets/logos/freelancer.png">
      </div>
      <p class="item-text">
        <a href="https://www.freelancer.com/u/gabrielsantos19">@gabrielsantos19</a>
      </p>

      <div class="item-icon">
        <img class="icon" src="@/assets/logos/telegram.png">
      </div>
      <p class="item-text">
        <a href="https://t.me/gabrielsantos19">@gabrielsantos19</a>
      </p>

      <div class="item-icon">
        <img class="icon" src="@/assets/logos/LI-Logo.png">
      </div>
      <p class="item-text">
        <a href="https://www.linkedin.com/in/gabrielsantos19/">@gabrielsantos19</a>
      </p>
    </div>
  </div>
</template>

<style scoped>
.about {
  flex: 1;
  display: flex;
  flex-flow: column;
  align-items: center;
}
.itens {
  display: grid;
}
.item-icon {
  display: flex;
  flex-flow: row nowrap;
  justify-content: flex-end;
}
.item-text {
  grid-column: 2;
  display: flex;
  flex-flow: row nowrap;
  align-items: center;
}
.icon {
  height: 30px;
  margin: 5px 10px;
  grid-column: 1;
}
.item {
  align-self: flex-start;
  display: flex;
  flex-flow: row nowrap;
  align-items: center;
}
</style>
