<template>
<body>
    <div class="make-chal">
        <form class="chal-form">
            <p>챌린지명 <input type="text" name="name" class="text-field"></p>
            <p>챌린지 총 기간 <input type="text" name="period" class="text-field"></p>
            <p>기간별 할 일 <input type="text" name="todolist" class="text-field"></p>
            <div class="todo_list">
                <ul>
                    <li>부트캠프</li>
                    <li>토익</li>
                    <li>3대 500</li>
                    <li>매일 6시 기상</li>
                </ul>
            </div>
        </form>
    </div>
</body>
<footer>
    <div class="footer-right">
        <button class="makebtn"><p>챌린지 생성 완료</p></button>
    </div>
</footer>
</template>

<style scoped>
.make-chal {
    margin-right: auto;
    margin-left: 10px;
    padding: 20px;
    border: none;
}
.todolist{
    margin: auto;
    padding-right: 30%;
}
.text-field {
    font-size: 14px;
    padding: 10px;
    border: 1px solid gainsboro;
    width: 400px;
    margin-bottom: 10px;
}
footer {
    width: 98%;
    height: 80px;
    bottom: 0px;
    position: absolute;
}
.footer-right {
    border: none;
    float: right;
}
.makebtn {
    border: none;
    background-color: tomato;
    width: 200px;
    font-size: 14px;
}#search_bar {
width: 80%;
border: white solid 0px;
}
.todo_list {
    border-radius: 5%;
}
.todo_list {
border: black solid 1px;
width: 30%;
margin: auto;
text-align: left;
}
</style>
