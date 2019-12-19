<template>
	<view class="content">
		<button @tap="show = true">弹出键盘</button>
		<passkeyborad :show="show" @close="close"></passkeyborad>
	</view>
</template>

<script>
	import passkeyborad from '@/components/payPassword/paykeyboard.vue';
	export default {
		components: {
			passkeyborad,
		},
		data() {
			return {
				show: false,
			}
		},
		onLoad() {

		},
		methods: {
			close() {
				this.show = false
			}
		}
	}
</script>

<style>
	.content {

	}

	.logo {
		height: 200rpx;
		width: 200rpx;
		margin-top: 200rpx;
		margin-left: auto;
		margin-right: auto;
		margin-bottom: 50rpx;
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
