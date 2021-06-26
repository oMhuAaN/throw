<template>
	<view class="lsdfho">
		<view class="dsfds3">
			<view class="ldjfl3fd">{{value}}</view>
		</view>
		<view class="flkdjfe" @click="handleClick_1">
			转
		</view>
		<audio style="text-align: left" :src="current.src" :poster="current.poster" :name="current.name"
			:author="current.author" :action="audioAction" controls></audio>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				value: 6,
				poster: 'https://bjetxgzv.cdn.bspapp.com/VKCEYUGU-uni-app-doc/7fbf26a0-4f4a-11eb-b680-7980c8a877b8.png',
				name: '致爱丽丝',
				author: '暂无',
				src: 'https://bjetxgzv.cdn.bspapp.com/VKCEYUGU-hello-uniapp/2cc220e0-c27a-11ea-9dfb-6da8e309e0d8.mp3'
			}
		},
		onLoad() {

		},
		methods: {
			handleClick_1() {
				// alert('xxdfsdf')
				this.value = Math.ceil(Math.random() * 6);
			}
		}
	}
</script>

<style>
	.dsfds3 {
		font-weight: 900;
		font-size: 200rpx;
		color: #fff;
		margin-top: 300rpx;
		padding: 20rpx 50rpx;
		border: 3px solid red;
		border-radius: 10rpx;
	}

	.flkdjfe {
		font-size: 200rpx;
		color: #1AA034;
		margin-top: 200rpx;
		cursor: pointer;
		padding: 20rpx 50rpx;
		border: 3px solid yellow;
		border-radius: 10rpx;
	}

	.lsdfho {
		display: flex;
		flex-direction: column;
		align-items: center;
		background-color: #070F17;
		height: 100vh;
		position: fixed;
		left: 0rpx;
		top: 0rpx;
		width: 750rpx;
	}

	.bb {
		border: 1px solid red;
	}
</style>
