<template>
    <view class='test1'>
        test1
        <button type="default" @click="goto('../../packageA/test1/index')">返回上一页</button>
    </view>
</template>

<script>

export default {
    components: {},
    data() {
        return {

        };
    },
    onLoad(options) {

    },
    onShow() {

    },
    onReady() {

    },
    methods: {
        goto(url) {
            uni.navigateBack()
        }

    },
    onHide() { },
    onUnload() { },
}
</script>
<style>
</style>