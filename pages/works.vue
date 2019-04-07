<template>
  <section class="container">
    <div class="mask">

    </div>
  </section>
</template>

<script>
import axios from 'axios'

export default {
  async asyncData({}) {
    let data = await axios.get('https://umi-portfolio-api.herokuapp.com/api/works/?format=json')
    console.log(data)
  },
}
</script>

<style>
.container {
  min-height: calc(100vh - 60px);
  width: 100vw;
  background-image: url('~assets/image/oya_nyanko.jpg');
  background-size: cover;
  background-position: center center;
}

.mask {
  height: calc(100vh - 60px);
  width: 100%;
  background-color: rgba( 0, 0, 0, 0.5);
  display: flex;
  justify-content: center;
}

.title {
  max-width: 800px;
  width: 100%;
  object-fit: contain;

}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
