<script>
</script>

<template>
    <header class="header">
        <div class="container">
            <div class="up_block">
                <div class="block_logo">
                    <img src="./../assets/WD.png">
                </div>
                <div class="nav_block">
                    <ul>
                        <li><a href="#">ГЛАВНАЯ</a></li>
                        <li><a href="#about_text">ОБ АВТОРЕ</a></li>
                        <li><a href="#projects">РАБОТЫ</a></li>
                        <li><a href="#footer">КОНТАКТЫ</a></li>
                    </ul>
                </div>
            </div>
            <div class="down_block">
            <div id="block_logo_bg">  
                <div class="block_logo_text">
                    <img src="./../assets/computer.png">
                </div>
            </div>
                <div class="content_block">
                    <h1>Дизайн и верстка</h1>
                <div class="bloc_text">
                    <p>Привет! 👋 Я начинающий фулстек разработчик, горящий желанием создавать качественные и функциональные веб-приложения. 
                        Моя страсть к технологиям и постоянное стремление к 
                        развитию помогают мне осваивать новые навыки и расширять горизонты. </p>
            </div>
                    <button class="button_write"><a href="#form_send">НАПИСАТЬ МНЕ</a></button>
                </div>
            </div>
        </div>
    </header>
</template>

<style scoped>
* {
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
  list-style-type: none;
  text-decoration: none;
  color: white;
}
.container {
  padding: 0px 402px;
}
.up_block {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 38px 0;
}
.nav_block > ul {
  display: flex;
}
ul > li {
  padding-left: 30px;
}
ul > li > a:hover {
  color: #20a39f;
  transition: all 0.3s;
}
.header {
  background-color: #2d3142;
  width: 100%;
  height: 100%;
}
.button_write {
  background-color: #427574;
  padding: 20px;
  border-radius: 25px;
  font-size: 15px;
  margin: 10px 0px 0px 0px ;
}
.button_write:hover {
  background-color: #20a39f;
  transition: all 0.3s;
}
.down_block {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 137px 0;
}
.content_block > h1,
.content_block > p {
  padding-bottom: 20px;
}

#block_logo_bg{
    margin: 0px 35px 0px 0px ;
}


@media screen and (min-width: 4000px) and (max-height: 2000px) {
.block_logo_text {
    margin: 0px 0px 0px 650px;
}

#block_logo_bg{
    margin: 0px;
}

.button_write{
    margin: 0px;
}

.bloc_text {
    margin: 25px 0px 25px 0px ;
}

.nav_block{
    font-size: 25px;
}

.content_block {
    font-size: 18px;
    margin: 0px 0px 0px 100px;
};

}
</style>
