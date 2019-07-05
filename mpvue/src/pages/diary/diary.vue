<template>
    <div class="diary">
        <div @click="changeBtn" class="changeBtn">切换为时间胶囊</div>
        <Jia />
        <div class="content">
            <div class="top">
                <div class="date">2019/07/05</div>
                <div class="time">19:36:53记录</div>
            </div>
            <div class="word">
                <div class="content">哈哈哈,我今天很开心</div>
                <div class="iconfont icon-lajitongshanchu" @click="delItem"></div>
            </div>
        </div>
    </div>
</template>


<script>
import Jia from "@/components/jia.vue"
export default {
    data(){
        
    },
    methods:{
        delItem (){
            
        }
    },
    components:{
        Jia
    }
}
</script>

<style lang="scss" scoped>
.diary{
    width: 100%; height: 100%;
    background-image: url("http://47.102.144.31/tang/images/bj1.jpg");
    background-size:100% 100%; padding-top: 20rpx;
    .changeBtn{
        height: 80rpx; padding:0 20rpx; line-height:80rpx;
        background-color: #21aaf2; display: inline-block;
        color: white; font-size: 14px; position:fixed;
        border-bottom-left-radius:30rpx; right: 0; top: 0;
    }
    .content{
        width: 94%;background-color: #fff;
       margin-left: 3%;
        .top{
            width: 100%; height:100rpx; border-bottom: 1px solid #f6f6f6; line-height: 100rpx;
            overflow: hidden;
            .date{
                background-color: #21aaf2; color:white; line-height:50rpx;
                height:50rpx; padding:10rpx 20rpx; float: left;
                border-radius:0 7rpx 7rpx 0; margin-top: 15rpx;
            }
            .time{
                padding:0 15rpx; float: left; font-size: 12px;
            }
        }
        .word{
            position: relative; min-height: 150rpx;
            .icon-lajitongshanchu{
                position: absolute; right: 10rpx; bottom: 10rpx;
                font-size:20px;
            }
            .content{
                padding: 25rpx 25rpx; box-sizing: border-box;
                line-height: 32rpx;
            }
        }
    }
}
</style>

