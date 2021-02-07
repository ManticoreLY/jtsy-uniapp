<template>
	<view class="content">
		<view class="logo">
			<image src="../../static/login/256.png" mode="" style="width: 200rpx;height: 200rpx"></image>
		</view>
		<view class='input'>
			<input class="line regular-fontcolor" type="text" :value="account" placeholder="请输入手机号"/>
			<input class="line regular-fontcolor" type="password" :value="password" placeholder="输入账号密码"/>
		</view>
		<view class="icon-button">
			<label class="regular-fontcolor">
				<checkbox :value="1" /><text>记住密码</text>
			</label>
			<navigator class="regular-fontcolor" url="/pages/login/forgotPwd" style="text-decoration: underline;">忘记密码</navigator>
		</view>
		<view class="input" style="height: 200upx;">
			<button class="big" style="color: #fff;">登&nbsp;&nbsp;&nbsp;录</button>
		</view>
		<view class="bottom regular-fontcolor">
			登录即代表同意APP <navigator style="display: inline-block;text-decoration: underline;" url="">用户协议</navigator>
		</view>
	</view>
</template>

<script>
export default {
	name: 'login',
	data() {
		return {
			account: '18874136663',
			password: 'a123456'
		}
	}
}
</script>

<style lang="scss" scoped>
	@import url("../../common/common.scss");
	.logo{
		width: 100%;
		height: 400upx;
		display: flex;
		align-items: center;
		justify-content: center;
	}
	.input{
		width: 100%;
		height: 250upx;
		display: flex;
		flex-flow: column nowrap;
		justify-content: space-around;
		align-items: center;
		align-content: center;
		input{
			padding-left: 20upx;
			text-align: center;
		}
	}
	.icon-button{
		margin: 0 auto;
		width: 650upx;
		height: 100upx;
		line-height: 100upx;
		display: flex;
		flex-flow: row nowrap;
		justify-content: space-between;
	}
	.bottom {
		position: absolute;
		bottom: 60upx;
		left: 50upx;
		margin: 0 auto;
		width: 650upx;
		height: 80upx;
		line-height: 80upx;
		text-align: center;
	}
</style>
