<script setup lang="ts">
import { ref } from 'vue';
    const shakeCountWithdraw = ref<number>(8);
    const money = ref<number>(99.83);
    const shakeCount = ref<number>(5);
</script>

<template>
    <div class="main">
        <div class="tip">
            <div class="text">已获得{{money}}元</div>
            <div class="btn">再摇{{shakeCountWithdraw}}提现</div>
        </div>
        <div class="tip">
            <div>经验值</div>
            <div>再摇x次升级</div>
        </div>
        <div class="tree"></div>
        <div class="dray">
            <div class="btn">摇钱</div>
            <div class="span">还能摇{{shakeCount}}次</div>
        </div>
    </div>
</template>
<style lang="sass">
    .main
        display: flex
        flex-direction: column
        width: 100%
        height: 64%
        .tip
            margin: 0 10%
            display: flex
            flex-direction: row
            justify-content: space-around
        .tree
            width: 100%
            height: 100%
        .dray
            width: 30%
            height: 16%
            position: relative
            top: -18%
            left: 50%
            transform: translateX(-50%)
            border-radius: 20px
            display: flex
            flex-direction: column
            align-items: center
            justify-content: space-around
            .span
                font-size: 12px

</style>