<script>
export default {
    data() {
        return {    
            arrayLogo: ["vue", "html", "css", "javascript", "mongodb", "bootstrap","Node.js"] 
        }
    }
}
</script>
<template>
    <div class="content_skills">
        <h1>МОИ НАВЫКИ</h1>
        <nav>
            <ul>
                <li v-for="index in arrayLogo" class="ok">
                    <img v-bind:src="'src/assets/' + index + '.svg'" class="img">
                    <p>{{ index }}</p>
                </li>
            </ul>
        </nav>
    </div>
</template>
<style scoped>
.content_skills {
    justify-content: center;
    background-color: #2d3142;
    color: white;
}
nav ul {
    display: flex;
    gap: 90px;
    justify-content: center;
    text-align: center;
    text-transform: uppercase;
    font-size: 40px;
}
.content_skills {
    padding: 60px 0;
    text-align: center;
}
.content_skills h1 {
    font-size: 50px;
    padding-bottom: 50px;
}
.img:hover {
    width: 80px;
    height: 80px;
    transition: all 1s;
}
</style>