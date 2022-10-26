<script setup>
import { ref } from 'vue'

function test(){
  alert("Кнопка работает! ")
}

defineProps({
})

const count = ref(0)
</script>

<template>
    <div class="container-box">
    <img src="/img/logo.png"  class="logo" alt="logo"/>
    <h3>VUE приложение</h3>
    <button @click="test">Открыть</button>
  </div>
</template>

<style scoped>
h3{
    color: red;
    font-size: 40px;
    position: relative;
    left: 8%;
    bottom: 10px;
}
h3:hover {
  filter: drop-shadow(0 0 2em rgba(117, 78, 249));
}
.container-box{
    box-shadow: 10px 5px 5px rgba(117, 78, 249);
    width: 50%;
    margin: 0 auto;
    background-color: #fff;

}
.container-box{
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 30px;
}

.logo {
    width: 25%;
    padding: 5px;
}
.logo:hover {
  filter: drop-shadow(0 0 2em rgba(117, 78, 249));
}
button{
    color: white;
    position: relative;
    top: 50px;
    right: 150px;
    background: #754EF9;
    color: white;
    font-size: 10px;
    padding: 10px;
    padding-left: 35px;
    padding-right: 35px;
    border-radius: 30px;
    transition: 1s;
}
button:hover{
	background: #2ECC71;
	color: #fff;
	opacity: 0.7;

}
button{
    transition: 1s;
    transition: 1s;
    position: relative;
    top: 45px;
    right: 30%;
  }
button:hover {
    transform: scale(1.2);
}

</style>
