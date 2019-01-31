<template>
  <section class="container">
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
      <div class="links">
      </div>
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
  padding-top: 30px;
  font-size: 24px;
  font-weight: 300;
  color: #526488;
}

.links {
  padding-top: 15px;
}
</style>
