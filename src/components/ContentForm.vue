<script>
export default {
    data() {
        return {
            name: "",
            email: "",
            text: "",
        }
    },
    methods: {
        sendPost() {
            if(this.name == "" || this.email == "" || this.text == "" || this.email.indexOf("@") < 0) {
                alert("Ошибка! Вы ничего не ввели! Или пропустили @");
            } else {
                alert("Сообщение отправлено");
                this.name = "";
                this.text = "";
                this.email = "";
            }
        }
    }
}
</script>
<template>
    <div class="content_form">
        <h1>Хотите веб-сайт?</h1>
        <form>
            <div id="form_send">
                <input v-model="name" type="name" placeholder="Ваше имя" class="form">
                <input v-model="email" type="email" placeholder="Ваш e-mail" class="form">
            </div>
            <textarea v-model="text" placeholder="Сообщение" class="form"></textarea><br/>
            <button class="button_send" v-on:click="sendPost"><a href="!#">Отправить</a></button>
        </form>
    </div>
</template>
<style scoped>
.content_form h1, .content_form form {
    text-align: center;
    margin: 20px 0; 
}
.content_form {
    background-color: #2d3142;
    color: white;
    padding: 50px;
}
textarea {
    width: 370px;
    height: 108px;
    margin-top: 20px;
}
div input {
    margin: 0 15px;
}
.button_send {
    padding: 5px 30px;
    margin-top: 20px;
    background-color: #427574;
    border-radius: 15px;
}
.button_send:hover {
    background-color: #20a39f;
    transition: all 0.3s;
}
.button_send a {
    color: white;
}
.form:hover {
    border: 3px solid #20a39f;
    transition: all 0.2s;
}
</style>