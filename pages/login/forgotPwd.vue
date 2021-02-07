<template>
	<view class="content">
		<view style="height: 120upx"></view>
		<view class="title">设置新密码</view>
		<view class="input">
			<input class="line" placeholder="请输入手机号" :value="account" />
			<input class="line" placeholder="请输入验证码" :value="valicode" />
			<input class="line" placeholder="请输入新密码" :value="password" />
		</view>
		<view class="line-width" style="height: 100upx; line-height: 100upx;">
			<navigator class="regular-fontcolor" url="">手机号登录</navigator>
		</view>
		<view class="input" style="height: 200upx">
			<button class="big">提&nbsp;&nbsp;&nbsp;交</button>
		</view>
	</view>
</template>

<script>
	export default {
		name: 'forgotPwd',
		data () {
			return {
				account: '',
			}
		}
	}
</script>

<style lang="scss" scoped>
@import url("../../common/common.scss");
.title{
	height: 150upx;
	line-height: 150upx;
	padding-left: 100upx;
	margin-bottom: 40upx;
	font-size: 48upx;
	font-weight: bold;
}
.input{
		width: 100%;
		height: 450upx;
		display: flex;
		flex-flow: column nowrap;
		justify-content: space-around;
		align-items: center;
		align-content: center;
	}
</style>
