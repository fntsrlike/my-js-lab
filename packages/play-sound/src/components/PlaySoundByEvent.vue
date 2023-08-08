<template>
    <div></div>
</template>
<script setup lang="ts">
import sound from '../assets/bell-ring.wav'; // 聲音檔案的路徑可能根據你的專案配置有所不同

const playAudioInBackground = function () {
    console.log('playAudio')
    const audio = new Audio(sound)
    audio.play();
}

setInterval(playAudioInBackground, 1000);
</script>
