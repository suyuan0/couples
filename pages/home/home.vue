<template>
	<view class="container">
		<uni-notice-bar showIcon single scrollable :speed="50" text="月光亮着，夜空就不会黑暗;问候伴着，心灵就不会孤单;祝福传递，温暖送你。愿你今晚有个好梦，晚安!">
		</uni-notice-bar>
		<view class="header">
			<image src="https://blogapi.darling0.cn/public/uploads/cc804802a622f14b9123bf2bdc784f9.jpg" mode="widthFix" class="avatar" />
			2022 / 10 / 24
		</view>
		<view class="swiper-container">
			<swiper :indicator-dots="true" :autoplay="true" :interval="3000" :duration="1000">
				<swiper-item>
					<view class="swiper-item">
						<image src="https://blogapi.darling0.cn/public/uploads/微信图片_20210323132558.jpg" mode=""></image>
					</view>
				</swiper-item>
				<swiper-item>
					<view class="swiper-item">2</view>
				</swiper-item>
			</swiper>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			};
		}
	}
</script>

<style lang="scss">
.header {
	height: 300rpx;
	display: flex;
	flex-direction: column;
	align-items: center;
	justify-content: space-around;
	.avatar {
		border-radius: 50%;
		width: 200rpx;
	}
}

.swiper-container {
	.swiper-item {
		display: flex;
		justify-content: center;
		image {
			width: 90%;
		}
	}
}
</style>
