<template>
    <div class="ocean">
        <div class="wave"></div>
        <div class="wave"></div>
        <div class="wave"></div>
    </div>
</template>
<script>
export default {

}
</script>
<style scoped>
.ocean {
    height: 2%;
    width: 100%;
    position: absolute;
    bottom: 0;
    left: 0;
    /* background: #015871; */
}

.wave {
    background: url("https://s3-us-west-2.amazonaws.com/s.cdpn.io/85486/wave.svg") repeat-x;
    position: absolute;
    top: -110px;
    width: 3400px;
    height: 200px;
    animation: wave 3.3s cubic-bezier(0.36, 0.45, 0.63, 0.53) infinite, swell 4s ease -1.25s infinite;
    transform: translate3d(0, 0, 0);
}

.wave:nth-of-type(2) {
    top: -100px;
    left: 320px;
    animation: wave 3s cubic-bezier(0.36, 0.45, 0.63, 0.53) -.125s infinite, swell 6s ease -1.25s infinite;
    opacity: 0.8;
}

.wave:nth-of-type(3) {
    top: -120px;
    left: -320px;
    animation: wave 5s cubic-bezier(0.36, 0.45, 0.63, 0.53) -.125s infinite, swell 5s ease -1.25s infinite;
    opacity: 0.7;
}

@keyframes wave {
    0% {
        margin-left: 0;
    }

    100% {
        margin-left: -1600px;
    }
}

@keyframes swell {

    0%,
    100% {
        transform: translate3d(0, -10px, 0);
    }

    50% {
        transform: translate3d(50px, -5px, 0);
    }
}
</style>