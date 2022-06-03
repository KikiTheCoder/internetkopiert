<template>
  <div id="preloader">
    <div id="preloader-text">
      Dies ist die Seite, von der Schüler ihre Hausaufgaben kopieren.
    </div>
  </div>
  <main class="container">
    <div class="title">Personenbeschreibung</div>
    <div class="content">
      Text Hier
    </div>
  </main>
</template>

<style>
#preloader {
  height: 100vh;
  width: 100vw;
  background-color: #1a1a1a;
  position: absolute;
  top: 0px;
  left: 0px;
  text-align: center;
  color: #ffffff;
  display: flex;
  animation: moveup 1.5s 3s ease-in-out forwards;
}

#preloader-text {
  margin: auto;
  font-size: 58px;
  max-width: 80vw;
  font-weight: 300;
  font-family: 'Lobster', cursive;
  animation: fadeout 1.5s 2.25s ease-in-out forwards;
}

@keyframes fadeout {
  to {
    opacity: 0%;
    visibility: hidden;
  }
}

@keyframes moveup {
  to {
    height: 0px;
  }
}

@media only screen and (min-width: 768px) {
  #preloader-text {
    font-size: 80px;
  }
}
</style>