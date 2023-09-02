<template>
	<view class="content">
		<u-navbar :is-back="false" title="证书"></u-navbar>
		<u-row>
			<u-col span="12">
				<u-swiper :list="list" height="300" ></u-swiper>
		    </u-col>
		</u-row>
		<u-row>
			<u-col span="12">
				<view class="row-content">
					<p><span>证书名称</span>2022深圳国际金融科技大赛获奖证书</p>
					<p><span>奖项</span>一等奖</p>
					<p><span>赛道</span>区块链</p>
					<p><span>姓名</span>张宇豪</p>
					<p><span>参数团队</span>TIDAL</p>
					<p><span>发证机构</span>深大微众金融科技学院 微众银行</p>
					<p><span>获取时间</span>2022年12月1日</p>
					<p><span>上链哈希</span>627d8f5b4574f5438c93bab0e5e859dfbc6b707a6e7fded892e78a43e65e609f</p>
				</view>
		    </u-col>
		</u-row>
		<u-row>
			<u-col span="12">
				<view class="bg-purple">
					由微众区块链、深大微众金融科技学院、深圳职业技术大学提供技术支持
				</view>
		    </u-col>
		</u-row>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				list:[
					'https://fintechthon.fisco.com.cn/assets/banner-search.0a78e40b.jpg'
				]
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style>
	.content {
		height: 100vh;
		background: #F0F0F0;
	}
	.row-content {
		border-radius: 8px;
		margin-top: -20px;
		z-index: 1;
		height: 260px;
		font-size: 12px;
		background-color: #fff;
		color: #000;
	}
	.row-content p{
		width: 300px;
		display: inline-block;
		margin-top: 12px;
		margin-left: 50px;
		word-break: break-all;
	}
	.row-content span{
		display: inline-block;
		width: 60px;
		text-align: left;
	}
	.bg-purple {
		width: 300px;
		z-index: 1;
		color: #BABABA;
		font-size: 12px;
		height: 50px;
		margin: auto;
		display: flex;
		justify-content: center;
		align-items: center;
		text-align: center;
	}
</style>
