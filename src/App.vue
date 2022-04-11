<script>

import Card from '/src/Card.vue';

export default {
  components: {
    Card
  }
}

</script>

<template>
  <main>
    <h1>Contactos Dr. Slump</h1>
    <Card name="Arale" hobbies="Le gusta jugar con Gachán"
      urlImage="https://i.pinimg.com/originals/f5/e8/bb/f5e8bb3e27fcfe21c94f3ddf2b1353cc.jpg"
      bgColor="rgb(230,230,250)" />
        <Card name="Gachán" hobbies="Le gusta comer coches"
      urlImage="https://lh3.googleusercontent.com/QQBkBnr_GaHLxTdvfZTFayKQrkhIbtDXwReXx9hdBJd2p7c6g52ScYzG2TUpbsaQ4Ydp9EIPBX9uQIB6hgtaM6RSGc_choZWoPuf=s0"
      bgColor="background-color: rgba(0, 255, 0, 0.5)" 
      bg-color="olive"/>
  </main>
</template>

<style>
@import './assets/base.css';

#app {
  max-width: 1280px;
  margin: 0 auto;
  padding: 2rem;

  font-weight: normal;
}

header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

a,
.green {
  text-decoration: none;
  color: hsla(160, 100%, 37%, 1);
  transition: 0.4s;
}

@media (hover: hover) {
  a:hover {
    background-color: hsla(160, 100%, 37%, 0.2);
  }
}

@media (min-width: 1024px) {
  body {
    display: flex;
  }

  #app {
    display: grid;
    grid-template-columns: 1fr 1fr;
    padding: 0 2rem;
  }

  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  .logo {
    margin: 0 2rem 0 0;
  }
}
</style>
