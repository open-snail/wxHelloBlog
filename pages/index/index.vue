<template>
	<view class="view__body">
		
		<view class="view__item" v-for="(item, index) in dataList" :key="index">
			<view class="view__item-title">{{ item.title }}</view>
			<view class="view__item-author">{{ item.author }}</view>
			<view class="view__item-icon"> 
			{{ item.collect }}
			 <text class="iconfont icon icon-collected"></text>
			 {{ item.like }}
			 <text class="iconfont icon icon-like"></text>
			</view>
		</view>
	</view>
</template>

<script>
export default {
	data() {
		return {
			title: 'Hello',
			dataList: [
				{ title: 'i let Blank Notebook Censor Me', collect: 155, like: 235, author: 'alen walker' },
				{ title: 'i let Blank Notebook Censor Me', collect: 155, like: 235, author: 'alen walker' },
				{ title: 'i let Blank Notebook Censor Me', collect: 155, like: 235, author: 'alen walker' },
				{ title: 'i let Blank Notebook Censor Me', collect: 155, like: 235, author: 'alen walker' },
				{ title: 'i let Blank Notebook Censor Me', collect: 155, like: 235, author: 'alen walker' },
				{ title: 'i let Blank Notebook Censor Me', collect: 155, like: 235, author: 'alen walker' },
			]
		};
	},
	onLoad() {},
	methods: {}
};
</script>

<style>
	@font-face {
		font-family:'iconfont';
		src: url('https://at.alicdn.com/t/font_1491397_y8j40in8dg.css');
	}
.view__body {
	background-color: rgb(45, 78, 138);
}
.view__item {
	margin: 10rpx;
	background: #4CD964;
	border-radius: 5px;
	height: 300upx;
	width:98%;
}
.view__item-title{
	padding-top: 40upx;
	text-align: center;
}
.view__item-author{
	text-align: center;
}
.view__item-icon{
	text-align: center;
}
.view__item-like-img{
	font-size: 1rpx;
}
</style>
