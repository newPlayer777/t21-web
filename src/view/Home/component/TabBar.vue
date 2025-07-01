<template>
    <div class="flex flex-row justify-between items-center bg-white shadow-sm p-[24px]">
        <div class="flex flex-row justify-center items-center">
            <h1 class="text-xl font-bold text-center">T21</h1>
            <img class="size-[40px] ml-2" src="/src/assets/logo.png" />
        </div>
        <div class="flex flex-row items-center space-x-4">
            <div class="text-sm text-[#333]" v-for="(item, index) in tabList" :key="index">
                {{ item.name }}
            </div>
        </div>
    </div>
</template>

<script lang="ts" setup>
const tabList: Array<{ name: string }> = [
    { name: '首页' },
    { name: '帮助中心' },
    { name: '关于我们' },
]
</script>

<style module="TabBar" lang="less"></style>
