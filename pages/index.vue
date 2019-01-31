<template>
  <section class="container">
    <div class="bg" />
    <div class="lightning flashit" />
    <div>
      <logo />
      <h1 class="title">
        Raiju
      </h1>
      <h2 class="subtitle">
        Lightning Network
      </h2>
      <div class="contact">
        Contact: info at raiju.io
      </div>
      <div class="links" />
    </div>
  </section>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.bg {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: url(/images/seaside.jpg);
  background-position: center center;
  background-origin: content-box;
  background-size: cover;
  background-attachment: fixed;
  z-index: -2;
}

.lightning {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: url(/images/seaside.jpg);
  background-position: center center;
  background-origin: content-box;
  background-size: cover;
  background-attachment: fixed;
  -webkit-filter: brightness(3);
  filter: brightness(3);
  -o-filter: brightness(3);
  -moz-filter: brightness(3);
  z-index: -1;
}

/*Now just a opacity animation*/
.flashit {
  -webkit-animation: flash ease-out 7s infinite;
  -moz-animation: flash ease-out 7s infinite;
  animation: flash ease-out 7s infinite;
  animation-delay: 2s;
}

@-webkit-keyframes flash {
  from {
    opacity: 0;
  }
  92% {
    opacity: 0;
  }
  93% {
    opacity: 0.6;
  }
  94% {
    opacity: 0.2;
  }
  96% {
    opacity: 0.9;
  }
  to {
    opacity: 0;
  }
}

@keyframes flash {
  from {
    opacity: 0;
  }
  92% {
    opacity: 0;
  }
  93% {
    opacity: 0.6;
  }
  94% {
    opacity: 0.2;
  }
  96% {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
  padding-top: 15px;
}

.contact {
  padding-top: 140px;
  font-size: 24px;
  font-weight: 300;
  color: #526488;
}

.links {
  padding-top: 15px;
}
</style>
