<template>
	<view>
		<!-- <view wx:if="{{canIUse}}"> -->
		<view class='header'>
			<div class="header_bg">
				<image class="avatar" :src="avatarUrl"></image>
				<div class="name">{{nickName}}</div>
			</div>
		</view>
		<!-- #ifdef MP-WEIXIN -->
		<button class='bottom' type='primary' open-type="getUserInfo" lang="zh_CN" @getuserinfo="getUserInfo" withCreadentials="true" v-show="login">授权登录</button>
		<!-- #endif -->
	</view>
</template>

<script>
	export default {
		data() {
			return {
				login:true,
				avatarUrl:'../../static/images/avatar.jpg',
				nickName: '未登录'
			}
		},
		onLoad() {

		},
		methods: {
			getUserInfo(res){
				console.log('点击了授权按钮',res)
				if(res.detail.errMsg==='getUserInfo:ok'){
					//console.log(res.detail.userInfo.avatarUrl)
					this.avatarUrl = res.detail.userInfo.avatarUrl;
					this.nickName = res.detail.userInfo.nickName;
					this.login = false;
					//授权成功后，跳转进入小程序首页
					wx.switchTab({
						url: '/pages/index/index'  
					})
				}else{
					uni.showToast({
						title:"授权失败，请重试！",
						icon:"none"
					});
					return false;					
				}
				
				if(!res.detail.iv){
					uni.showToast({
						title:"你取消了授权，登录失败",
						icon:"none"
					});
					return false;
				}
			}
		}
	}
</script>

<style>
/* 	*{
		box-sizing: border-box;
	} */
	.header_bg{
		width: 100%;
		min-height: 200px;
		background: #FFFFFF;
		text-align: center;
	}
	
	.avatar{
		height: 80px;
		width: 80px;
		border-radius: 50%;
		/* background: #4CD964; */
		margin-top: 20px;
	}
	.name{
		font-size: 20px;
		color: #000000;
		font-family: "SimHei";
		margin-top: 10px;
	}
	
	.content {
		display: flex;
		flex-wrap: wrap;
		justify-content: center;
		/* background: white; */
		
		position: relative;
		top: -50px;
		
		text-align: center;
	}
	
	.content div{
		margin: 10px;
		background: rgb(251,251,251);
		width: 40%;
		height: 400rpx;
		border-radius: 10px;
		box-shadow: 0 1px 1px -0.5px #00000070;
	}
	
	.content div image{
		padding: 20px;
		width: 50px;
		height: 50px;
	}
	
	.text{
		font-size: 10px;
		font-family: "SimHei";
		letter-spacing: 1px;
	}
</style>
