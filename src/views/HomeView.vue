<template>
  <div id="preloader">
    <div id="preloader-text">
      Dies ist die Seite, von der Schüler ihre Hausaufgaben kopieren.
    </div>
  </div>
  <main class="container">
    <div class="title">Personenbeschreibung</div>
    <button class="fancy-btn">Click me</button>
    <div class="content">
      Text Hier
    </div>
  </main>
</template>

<style>
.fancy-btn {
  padding: 16px 14px;
  color: #ffffff;
  background: linear-gradient(to bottom right, rgb(156, 44, 167), rgb(79, 12, 204));
  border-radius: 5px;
  border: none;
  cursor: pointer;
  transition: 0.25s ease-in-out;
  box-shadow: #888 -5px 5px 2px;
}

.fancy-btn:hover {
  transform: translate3d(3px, -3px, 0px);
  box-shadow: #888 -5px 5px 8px;
}

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