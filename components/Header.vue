<template>
  <header class="header">
    <div class="header-inner">
      <ul class="navi">
        <li class="navi-item">
          <a href="/">HOME</a>
        </li>
        <li class="navi-item">
          <a>ABOUT ME</a>
        </li>
        <li class="navi-item">
          <nuxt-link to="/works">WORKS</nuxt-link>
        </li>
        <li class="navi-item">
          <a>SKILLS</a>
        </li>
        <li class="navi-item">
          <a>LINKS</a>
        </li>
      </ul>
    </div>
  </header>
</template>

<style>
.header {
  height: 60px;
  background-color: #eee;
}

.header-inner {
  height: 100%;
  padding: 0;
  text-align: center;
  position: relative;
}

.navi {
  display: inline-flex;
  list-style: none;
  margin: 0;
  padding: 0;
  position: absolute;
  left: 50%;
  bottom: 0;
  transform: translate(-50%, 0);
}

.navi-item > a {
  display: block;
  padding: 10px 20px;
}
</style>
