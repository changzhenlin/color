<script setup>
import { ref } from 'vue'
const colorvalue = ref('#')
const tset = ref('w-full h-full rounded-md p-3')
</script>

<template>
    <div class="w-full flex flex-col justify-center items-center p-3 bg-pink-200">
        <h1 class="text-4xl text-center m-3">Hello World</h1>
        <span class="m-10">输入色值，查看颜色</span>
        <div class="w-full h-20 relative flex flex-col justify-center items-center p-3 bg-blue-200">
          <input :class="tset" type="text" :value="colorvalue"/>
          <div class="absolute right-6 rounded-full bg-red-200 w-10 h-10"></div>
        </div>
    </div>
</template>


