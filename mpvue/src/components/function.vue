<template>
    <div class="fn">
        <div class="iconfont icon-jiaonang" @click="dateList"></div>
        <div class="iconfont icon-tupian"></div>
        <div class="iconfont icon-dingwei1"></div>
        <div class="iconfont icon-yuyin"></div>
        <weui-picker />
    </div>
</template>

<script>
export default {
    methods:{
        dateList(){

        }
    }
}
</script>

<style lang="scss">
.fn{
    width: 100%; height: 120rpx; background: white; align-items: center;
    display: flex; justify-content: center; text-align: center;line-height: 120rpx;
    border-top: 1px solid #f6f6f6;
    .icon-jiaonang{
        display: inline-block; width: 25%; font-size:40px;
    }
    .icon-tupian{
        display: inline-block; width: 25%; font-size:40px;
    }
    .icon-dingwei1{
        display: inline-block; width: 25%; font-size:40px;
    }
    .icon-yuyin{
        display: inline-block; width: 25%; font-size:40px;
    }
}

</style>


