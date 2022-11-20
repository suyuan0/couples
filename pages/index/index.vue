<template>
	<view class="container">
		<uni-notice-bar showIcon single scrollable :speed="50" text="昨夜有繁星满天，今早有朝霞渐起。你看见也好，看不见也没关系，，我找到你，它们才有意义。">
		</uni-notice-bar>
		<image src="https://blogapi.darling0.cn/public/uploads/couples-index.jpg" class="couples-index"></image>
		<uni-icons type="eye" class="icon" size="30" @click="handleToHome"></uni-icons>
	</view>
</template>

<script>
	export default {
		data() {
			return {

			}
		},
		methods: {
			handleToHome() {
				uni.switchTab({
					url: '/pages/home/home'
				})
			}
		}
	}
</script>

<style lang="scss" scoped>
	.container {
		position: relative;
		height: 100vh;

		.couples-index {
			position: relative;
			z-index: 4;
			margin-top: -28rpx;
			width: 100%;
			height: calc(100vh - 84rpx);
		}

		.icon {
			position: absolute;
			z-index: 5;
			bottom: 50rpx;
			left: 50%;
			transform: translateX(-50%);
			color: #fff !important;
			background: rgba(255, 255, 255, 0.3);
			border-radius: 50%;
			padding: 20rpx;
		}
	}
</style>
