<template>
	<view class="content">
		<u-navbar :is-back="false" title="证书"></u-navbar>
		<u-row>
			<u-col span="12">
				<u-image class="image_bg" src="../../static/980272f97804a081599612948437d22.png" height="350px"
					width="100%">
				</u-image>
				<u-image class="image_cert" src="../../static/58d3638623fd767c2cfb033ec88ab50.png"></u-image>
				<!-- 				<u-swiper height="300">
					
				</u-swiper> -->
			</u-col>
		</u-row>
		<u-row>
			<u-col span=" 12">
				<view class="row-content">
					<p><span>证书名称</span>第十二届职工技术创新运动会深圳市技能大赛</p>
					<p><span>奖项</span>二等奖</p>
					<p><span>赛道</span>区块链工程技术人员技能</p>
					<p><span>姓名</span>张宇豪</p>
					<p><span>参数团队</span>个人</p>
					<p><span>发证机构</span>深圳市职工技术创新运动会</p>
					<p><span>获取时间</span>2023年4月</p>
					<p><span>上链哈希</span>976s786ad8797asdc93bab0e5e859dfbc6b9sd88fded892e78a</p>
				</view>
			</u-col>
		</u-row>
		<u-row>
			<u-col span="12">
				<view class="bg-purple">
					<span>
						<u-image src="../../static/logo.jpg" width="20" height="20">
						</u-image>
					</span> 微众区块链
					<div style="margin-left: 10px;"></div>
					</span>
					<span>
						<u-image src="../../static/logo-title.png" width="20" height="20">
						</u-image>
					</span>
					深圳职业技术大学
				</view>
				<span style="color: gray;font-size: 10px;text-align: center;">由微众银行区块链、深圳职业技术大学提供技术支持</span>
			</u-col>
		</u-row>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				list: [
					'https://fintechthon.fisco.com.cn/assets/bg-certificate.25e79aeb.png'
				]
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style lang="less">
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

	.row-content p {
		width: 300px;
		display: inline-block;
		margin-top: 12px;
		margin-left: 50px;
		word-break: break-all;
	}

	.row-content span {
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

	.image_bg {
		margin-top: 40px;
		background-size: 100% 100%;
	}

	.image_cert {
		position: absolute;
		top: 14%;
		left: 12%;
		background-size: 90% 90%;
	}
</style>
