<template>
	<view class="content">
		<view>
			<text class="title" >{{title}}</text>
		</view>
		<view class="a">
		<view id="box" >
			<h1>欢迎来到论坛规则页</h1>
			<h2>规则如下：</h2>
			<h3> 一、注册ID管理规则  </h3>
			
			<ol >
				<p>  1、党和国家领导人或其他名人的真实姓名、拼音，或者与之相似、相近名；<br>
					2、冒称国家机构或其他现实机构单位、部门的名称以及有关职务的名称；<br />
					与论坛管理员、超级版主ID相似,易对网友造成混淆的。<br />
					3、蓄意与其他网友之名相近、相仿，并对其他网友发布的音乐有针对或隐含意味的人生攻击、谩骂、诋毁等行为；<br />
					4、以本人或他人的手机号码、QQ号码、群号码等含有联系方式的信息注册；<br />
					5、未经授权以某公司、团体名称注册的昵称。
		
				</p>
				
				</ol>
			
			<h3> 二、 个性签名头像管理规则 </h3>
			<h4>个性签名出现以下情况， 原创文章论坛有权对其提出警告，严重者将禁止论坛的一切活动</h4>
			<ol >
				<p>  1、党和国家领导人或其他名人的真实姓名、拼音，或者与之相似、相近名；<br>
					2、出现QQ号码、QQ群、电话号码等个人信息；<br />
					3、涉及广告、色情、猥琐、侮辱、诽谤、挑衅等主题，以及相互谩骂人身攻击等不文明语言；<br />
					4、使用受国家规定保护的图案，如国徽、国家领导人(现任、前任)照片。<br />
						
			
				</p>
				
				</ol>
			
			<h3> 三、 免责声明</h3>
			
			<ol >
				<p>  1、在论坛里发表的音乐仅代表作者本人的观点，与本论坛立场无关。
				出于遵守国家相关法规的前提，我们有权在不经作者准许的情况下删除其在论坛所发表的音乐。<br>
					2、原创音乐论坛的所有非管理员所发表的文章、内容、信息、资料等均不保证其准确性、完整性、有效性、时间性。<br />
					
						
			
				</p>
				
				</ol>
				<navigator  url="page.vue">转到首页</navigator>
		</view>
	</view>
</template>

<script>
	import mpvueEcharts from 'page.vue'

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
	
	.a{
		margin-top: 100upx;
	}
	
	.box{
				margin: 10upx  solid;
				padding: 100upx;
				margin: 10upx;
				padding: 10upx;
				text-align: center;
			}
			
			
			
			
			
			
			
			
			
			
			
</style>
