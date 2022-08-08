<template>
  <nav>
    <span class="logo"><router-link to="/">LOGO</router-link></span>
    <span class="mypage"><router-link to="/about">마이페이지</router-link></span>
    <span class="3-2"><router-link to="/3-2">3-2</router-link></span>
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
.logo{
  margin: auto;
}
.mypage{
  margin-right: 0px;
}
.container{
  padding: 5%;
  flex-direction: column;
  padding-right: 20%;
  padding-left: 20%;
}
.account_section{
  float: left;
  margin-left: 10%;
}
.remind_section{
  float: right;
  margin-right: 10%;
}
.challenging_section{
  float: left;
  margin-left: 10%;
}
.finish_section{
  float: right;
  margin-right: 10%;
}
.top{
  height: 250px;
}
.bottom{
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
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
.search_challenge {
  border: black solid 1px;
  width: 50%;
  margin: auto;
}
#search_bar {
  width: 80%;
  border: white solid 0px;
}
.search_challenge_list {
  border: black solid 1px;
  width: 50%;
  margin: auto;
  text-align: left;
}
</style>
