<template>
	<view class="content">
		<view>
			<text class="title" >{{title}}</text>
				<live-player>
			<audio src="file:///C:/Users/asus/Documents/HBuilderProjects/Music/bug/王铮 - 莲花谣.mp3">莲花谣 - 王铮</audio>
			<audio src="file:///C:/Users/asus/Documents/HBuilderProjects/Music/bug/徐佳莹 - 不要再孤单.mp3">不要再孤单 - 徐佳莹</audio>
			<audio src="file:///C:/Users/asus/Documents/HBuilderProjects/Music/bug/银临 - 不老梦.mp3">不老梦 - 银临</audio>
			<audio src="file:///C:/Users/asus/Documents/HBuilderProjects/Music/bug/银临 - 浮生辞.mp3">浮生辞 - 银临</audio>
			<audio src="file:///C:/Users/asus/Documents/HBuilderProjects/Music/bug/银临 - 腐草为萤.mp3">腐草为萤 - 银临</audio>
			<audio src="file:///C:/Users/asus/Documents/HBuilderProjects/Music/bug/银临 - 棠梨煎雪.mp3">棠梨煎雪 - 银临</audio>
			<audio src="file:///C:/Users/asus/Documents/HBuilderProjects/Music/bug/银临,Aki阿杰 - 牵丝戏.mp3">牵丝戏 - 银临,Aki阿杰</audio>
			<audio src="file:///C:/Users/asus/Documents/HBuilderProjects/Music/bug/银临,云の泣 - .mp3">锦鲤抄 - 银临,云の泣</audio>
			<audio src="file:///C:/Users/asus/Documents/HBuilderProjects/Music/bug/张碧晨 - 下一秒.mp3"> 下一秒 - 张碧晨</audio>
			
			</live-player>
		</view>
		
	</view>
</template>

<script>
	export default {
		data: {
			title: 'Hello uniapp',
			
		},
		mounted() {
			
		},
		methods:{
			
		}
	}
</script>

<style>
	.content {
		margin-top: 50upx;
		text-align: center;
		height: 400upx;
	}

	.title {
		font-size: 36upx;
	}
</style>
