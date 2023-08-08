<template>
    <p>按下以下按鈕後會撥放音樂。</p>
    <button :onclick="playAudio">播放</button>
</template>
<script setup lang="ts">
import sound from '../assets/alert.wav'; // 聲音檔案的路徑可能根據你的專案配置有所不同

const playAudio = function () {
    console.log('playAudio by clicking button')
    const audio = new Audio(sound)
    audio.play();
}
</script>
