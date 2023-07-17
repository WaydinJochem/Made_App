<template>
    <img src="https://i.postimg.cc/j2KJ84K0/Png-Item-2690030.png">
</template>
<script>
export default {

}
</script>
<style>
img {
    height: 150px;
    width: 50dvh;
    position: fixed;
    bottom: 85px;
    left: 600px;
    /* border: 5px black solid; */
    animation: ride 3.3s ease infinite;
}

@keyframes ride {

    0%,
    100% {
        bottom: 10px;
        left: 600px;
    }
    /* 25% {
        bottom: -10px;
        left: 650px;
    } */
    50% {
        bottom: 60px;
        left: 650px;
    }
}</style>