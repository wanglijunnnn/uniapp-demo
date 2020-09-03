<template>
	 <view class="index_view">
		 <view class="search_view">
			 <uni-search-bar bgColor="rgba(255,255,255,.3)" placeholder="搜索你想要的模板" color="#fff" radius="100" @confirm="search"></uni-search-bar>
		 </view>
		<view class="edit_resume_view">
			<view class="inner">
<!-- 				<text>职场精英都在用的专业简历</text>
				<text>快速生成优秀简历，敲定高新Offer</text>
				<button>立即制作</button> -->
				<text class="t1">xxxxxxxx</text>
				<text class="t2">xxxxxxxxxxxxxxxxxxxxx</text>
				<button>立即制作</button>
			</view>
		</view>
		<view class="service_view">
			<uni-grid :column="4" :showBorder="false">
				<uni-grid-item>
					<view class="icon"><image :src="src"></image></view>
					<text class="text">文本</text>
				</uni-grid-item>
				<uni-grid-item>
					<view class="icon"><image :src="src"></image></view>
					<text class="text">文本</text>
				</uni-grid-item>
				<uni-grid-item>
					<view class="icon"><image :src="src"></image></view>
					<text class="text">文本</text>
				</uni-grid-item>
				<uni-grid-item>
					<view class="icon"><image :src="src"></image></view>
					<text class="text">文本</text>
				</uni-grid-item>
			</uni-grid>
		</view>
		<view class="list_view edit_list_view">
			<view class="list_head_view">
				<text class="h3">在线模板</text>
				<text class="more">更多</text>
			</view>
			<view class="list_body_view">
				<view class="list_ul">
					<view class="list_li">
						<image src="../../static/uni.png"></image>
						<text>电动蝶阀丰富的接口和打飞机</text>
					</view>
					<view class="list_li">
						<image src="../../static/uni.png"></image>
						<text>电动蝶阀丰富的接口和打飞机</text>
					</view>
					<view class="list_li">
						<image src="../../static/uni.png"></image>
						<text>电动蝶阀丰富的接口和打飞机</text>
					</view>
					<view class="list_li">
						<image src="../../static/uni.png"></image>
						<text>电动蝶阀丰富的接口和打飞机</text>
					</view>
					<view class="list_li">
						<image src="../../static/uni.png"></image>
						<text>电动蝶阀丰富的接口和打飞机</text>
					</view>
					<view class="list_li">
						<image src="../../static/uni.png"></image>
						<text>电动蝶阀丰富的接口和打飞机</text>
					</view>
					<view class="list_li">
						<image src="../../static/uni.png"></image>
						<text>电动蝶阀丰富的接口和打飞机</text>
					</view>

				</view>
			</view>
		</view>
	</view>

</template>

<script>
	import uniSearchBar from '@/components/uni-search-bar/uni-search-bar.vue'
	import uniGrid from "@/components/uni-grid/uni-grid.vue"
	import uniGridItem from "@/components/uni-grid-item/uni-grid-item.vue"
	export default {
		components: {uniSearchBar,uniGrid,uniGridItem},
		data() {
			return {
				src:'https://ss1.bdstatic.com/70cFuXSh_Q1YnxGkpoWK1HF6hhy/it/u=1617835772,224556771&fm=26&gp=0.jpg'
			}
		},
		methods: {

		}
	}
</script>

<style lang="scss" scoped>
	.index_view{
		padding: 0 0 200rpx 0;
	}
	.search_view{
		padding: 8px 8px 15px 8px;
		background: #007AFF;
	}
	.edit_resume_view{
		padding:0 30rpx;
		background: #007AFF;
		height: 180rpx;
		.inner{
			padding:20px 20rpx 50rpx 20rpx;
			background: #fff;
			box-shadow: 0px 4px 10px 0px rgba(201,201,201,.1 );
			border-radius: 8px;
		}
		text{
			line-height: 1.2;
			display: block;
			text-align: center;
			color: #000;
		}
		.t1{
			font-size: 40px;
		}
		.t2{
			font-size: 20px;
			color: #454545;
		}
		button{
			margin-top: 50rpx;
			width: 50%;
			height: 80rpx;
			line-height: 80rpx;
			border-radius: 80rpx;
			background: #4CD964;
			border:none;
			color: #fff;
		}
	}
	.service_view{
		padding: 220rpx 30rpx 0 30rpx;
		text-align: center;
		.icon{
			margin: 0 auto;
			width: 120rpx;
			height: 120rpx;
			background: #66AAFF;
			border-radius: 120rpx;
			image{
				width: 100%;
				height: 100%;
			}
		}
		text{
			font-size: 32rpx;
		}
	}
	.list_view{
		padding: 0 15rpx;
		.list_head_view{
			padding: 0 0 0 10rpx;
		}
		.list_body_view{
			.list_ul{
				.list_li{
					width: 45%;
					display: inline-block;
					border: 1px solid #ccc;
					margin: 0 2%;
					image{
						width: 100%;
						display: block;
					}
					text{
						display: block;
					}
				}
			}
		}

	}
</style>
