<template>
    <div class="page">
        <SideBar />
        <Content/>
    </div>
</template>

<style lang="scss">
body {
    background-color: $color-primary;
    width: 100%;
    height: 100vh;
}

.page {
    display: flex;
    justify-content: space-between;
    align-items: center;
}
</style>

<script setup>
import SideBar from '@/components/navigation/SideBar.vue';
import Content from '@/components/content/Content.vue';
</script>