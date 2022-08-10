<template>
<div class='container'>
    <div class="search_challenge">
        <!-- <SearchBar hint="Search hint" :text="searchPhrase" @textChange="onTextChanged" @submit="onSubmit" /> -->
        <input type="text" id="search_bar"> 검색 아이콘
    </div>
    <br>
    <br>
    <div class="search_challenge_list">
        <div style="border: 3px solid black; text-align: center; border-radius: 10%;"><b>검색된 챌린지 목록</b></div>
        <ul>
            <li>부트캠프</li>
            <li>토익</li>
            <li>3대 500</li>
            <li>매일 6시 기상</li>
        </ul>
    </div>
    <!-- <span class="3-0"><router-link to="/3-0">3-0</router-link></span> -->
    </div>
</template>
<style scoped>
#search_bar {
width: 80%;
border: white solid 0px;
}
.search_challenge_list {
    border-radius: 5%;
}
.search_challenge {
border: black solid 1px;
width: 50%;
margin: auto;
}
.search_challenge_list {
border: black solid 1px;
width: 50%;
margin: auto;
text-align: left;
}
</style>
