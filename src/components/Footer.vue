<script>
export default {
    data() {
        return {
            arraySites: ["telegram", "vk", "whatsapp"],
        }
    }
}
</script>
<template>
    <footer class="footer" id="footer">
        <div class="left_block">
            <h1>Зайцев Константин</h1>
            <p>(с) 2024. Все права защищены</p>
        </div>
        <div class="right_block">
            <ul>
                <li v-for="index in arraySites">
                    <a href="https://t.me/+QTKuypFG3LNiYTZi" target="_blank"><img v-bind:src="'src/assets/' +  index  + '.svg'" class="img"></a>
                </li>
            </ul>
        </div>
    </footer>
</template>
<style scoped>
.footer {
    display: flex;
    justify-content: space-between;
    padding: 100px 402px;
}
.right_block ul {
    display: flex;
    gap: 30px;
}
.img:hover {
    width: 80px;
    height: 80px;
}
</style>