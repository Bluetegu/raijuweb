<template>
  <div class="logo">
    <!--<img src="/icon.png"/>-->
  </div>
</template>

<style>
.logo {
  display: inline-block;
  animation: turn 2s linear forwards 1s;
  transform: rotateX(180deg);
  position: relative;
  overflow: hidden;
}

@keyframes turn {
  100% {
    transform: rotateX(0deg);
  }
}
</style>
