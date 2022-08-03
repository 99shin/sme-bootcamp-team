<template>
        <div class="nav">
            <div class="navleft">
                <div class="navmenu"><button class="navbtn"><i class="ms-Icon ms-Icon--GlobalNavButton navicon" aria-hidden="true"></i></button></div>
                <div class="search"><button class="searchbtn" type="button"><i class="ms-Icon ms-Icon--Search searchicon" aria-hidden="true"></i></button></div>
            </div>
            
            <div class="logo">logo</div>
        </div>





<div class="container">
 <div class="item" id="movieinfo">
 <center><h4>한산 : 용의출현</h4></center>
 <img src='./assets/moviefoster.jpg' class="foster">이미지
 <div><center><button> 다른영화 선택하기</button></center></div>
 </div>
  <div>
    <form>
      <select class="item" v-model="locations" multiple @change="iflocationselected">
        <option disabled value="">지역을 선택해 주세요</option>
        <option v-for="(광역단체,i) in locations" :key="i" >{{locations[i]}}</option>
      </select>
    </form>
  </div>

  <div>
    <form>
      <select class="item" v-model="semilocations" multiple @change="ifsemilocationselected" v-if="locationselected == true">
        <option disabled value="">군/구 를 선택해주세요</option>
        <option v-for="(기초단체,i) in semilocations" :key="i" >{{semilocations[i]}}</option>
      </select>
    </form>
  </div>

  <div>
    <form>
      <select class="item"  v-model="theater" multiple v-if="semilocationselected == true">
        <option disabled value="">영화관을 선택해 주세요</option>
        <option v-for="(영화관,i) in theater" :key="i" >{{theater[i]}}</option>
      </select>
    </form>
  </div>
 
</div>
<br>
<div class="container">
  <center><h4>날짜를 선택해 주세요</h4></center>
</div>


<div class="container">
<h4>상영시간표</h4>

</div>

</template>

<script>


export default {
  name: 'App',
  data(){
    return {
    locationselected : false,
    semilocationselected : false,
    locations : ['강원도','경기도','경상남도','경상북도','광주시','대구시','대전시','부산시','서울시','세종시','울산시','인천시','전라남도','전라북도','제주도','충청남도','충청북도'],
     semilocations : ['금정구','진구','사하구','사상구'],
     theater : ['부산대 롯데시네마', '부산대 CGV', '부산대 메가박스']
    }
  },
  methods: {
     iflocationselected(){
      this.locationselected = true
     },
     ifsemilocationselected(){
      this.semilocationselected = true
     },
 
    
    },
  
  components: {
  
  },
}
</script>

<style>
h4{
  color:white;
}
html{
    background:linear-gradient( to bottom, #161722, rgb(27, 28, 35))
}

.container{
  display: flex;
  border-style: double;
  border-color: olive;
  background-color: rgb(27, 28, 35);
  margin : 15px;
}

.item {
  height: 500px;
  padding:15px;
  margin-left: 50px;
  background-color:rgb(27, 28, 35);
}

html{
    background:linear-gradient( #161722, rgb(27, 28, 35))
}
.nav{
    display: flex;
    height: 60px;
    width: calc(100vw);
    background-color:transparent;
    border-bottom: 1px solid #717171;
}
.navleft{
    display: flex;
}
.navbtn{
    height: 50px;
    width: 45px;
    border: none;
}
.navicon{
    font-size: 30px;
    color:white;
    padding-top: 6px;
}
.searchbtn{
    height: 60px;
    width: 35px;
    border: none;
}

.searchicon{
    font-size: 20px;
    color:white;
    
}
.logo{
    margin-left: 42%;
    color:white;
}
.main{
    height: calc(100vh - 50px);
}

button{
    background-color: transparent;
    color:whitesmoke;
}

.foster{
  height: 300px;
}
</style>