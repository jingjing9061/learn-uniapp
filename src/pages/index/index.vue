<template>
    <view class="content">
        <image class="logo" src="/static/logo.png"></image>
        <view>
            <text class="title">{{title}}</text>
            <button type="default" @click="goto('../../packageA/test1/index')">通过方法跳转到分包packageA/test页面</button>
        </view>
    </view>
</template>

<script>
export default {
    data() {
        return {
            title: 'Hello'
        }
    },
    onLoad() {

    },
    methods: {
        goto(url) {
            console.log(url)
            uni.navigateTo({
                url: url
            })
        }
    }
}
</script>

<style>
.content {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

.logo {
    height: 200rpx;
    width: 200rpx;
    margin: 200rpx auto 50rpx auto;
}

.text-area {
    display: flex;
    justify-content: center;
}

.title {
    font-size: 36rpx;
    color: #8f8f94;
}
</style>
