<template>
  <nav>
    <span class="logo"><router-link to="/">LOGO</router-link></span>
    <span class="mypage"><router-link to="/about">마이페이지</router-link></span>
    <span class="3-2"><router-link to="/3-2">3-2</router-link></span>
    <span class="3-1"><router-link to="/3-1">3-1</router-link></span>
  </nav>
  <router-view/>
  <span class="back"><button id="back">이전</button></span>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
nav{
  display: flex;
  align-items: center;
}
a{
  text-decoration: none;
}
nav {
  padding: 30px;
}
nav a {
  font-weight: bold;
  color: #2c3e50;
}
.logo{
  margin: auto;
}
.mypage{
  margin-right: 0px;
}
.back {
  position: absolute;
  bottom: 5%;
  left: 5%;
}
#back {
  height: 50px;
  width: 100px;
}
</style>
