<template>
	<view class="">
		<u-swiper :list="list" duration="3000" :circular="true" height="200"></u-swiper>
		<u-row>
			<u-col span="12">
				<view class="bg-purple">
					<p style="margin:10px 0px"></u-icon>发证机构：深大微众金融科技学院 微众银行</p>
					<u-search 
						placeholder="请输入身份证号" 
						:showAction="false" 
						style="width: 300px;" 
						height="40" 
						v-model="searchMsg"
						@search="searchChange(searchMsg)"
						@custom="searchChange(searchMsg)"></u-search>
				</view>
		    </u-col>
		</u-row>
		<u-row>
			<u-col span="12">
				<view class="bg-purple">
					<p>由深圳大学微众金融科技学院提供技术支持</p>
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
				],
				searchMsg:''
			}
		},
		onLoad() {

		},
		methods: {
			searchChange(searchMsg){
				console.log(searchMsg)
				uni.$u.route('/pages/index/index');
			}
		}
	}
</script>

<style>
	.u-col {
		height: 300px;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}
	.bg-purple {
	    border-radius: 8px;
		background: #fff;
		margin-top: -20px;
		z-index: 1;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}
</style>
