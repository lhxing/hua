<template>
	<view class="content">
		<view>
			<text class="title" >{{title}}</text>
		</view>
			<view class="a">
			
		
					<dl class="a-l">
								<dt>用户名：</dt>
								<dd><input id="user" type="text" />
								<div id="user_prompt"> 用户名由英文字母和数字组成的4-16位字符，以字母开头 </div></dd>
							</dl>
							<dl class="a-l">
								<dt>密码：</dt>
								<dd><input id="pwd" type="password"  />
								<div id="pwd_prompt"> 密码由英文字母和数字组成的4-10位字符 </div></dd>
							</dl>
							<dl class="a-l">
								<dt>确认密码：</dt>
								<dd><input id="repwd" type="password"/>
								<div id="repwd_prompt"></div></dd>
							</dl>
							<dl class="a-l">
								<dt>电子邮箱：</dt>
								<dd><input id="email" type="text"/>
								<div id="email_prompt"></div></dd>
							</dl>
							<dl class="a-l">
								<dt>手机号码：</dt>
								<dd><input id="mobile" type="text" />
								<div id="mobile_prompt"></div></dd>
							</dl>
							<dl class="a-l">
								<dt>生日：</dt>
								<dd><input id="birth" type="text"/>
								<div id="birth_prompt"></div></dd>
							</dl>
							<dl class="a-l">
								<dt>&nbsp;</dt>
								<dd>
								
								<!--  -->
								<video ></video>
								<el-button > <a href="page.vue">提交</a>  </el-button>
								</dd>
							</dl>
							</div>
							
						</form>
					
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
	$(function(){
			$("#user").blur("checkUserName");
			$("email").blur("checkEmail");
	
		$("formRegister").submit(function(){
				var flag = true;
				
				if (!checkUserName()) {
					flag = false;
				}
				if (!checkEmail()) {
					flag = false;
				}
				return false;
			});
		});
	
		function checkUserName(){
			var username = $("#fname").val();
			var reg = /^\D{6,14}$/;
			var flag = reg.test(username);
			console.log (flag);
			return flag;
	
			}
	
		function checkEmail(){
			var email = $("email").val();
			return true;
		}
		if (!flag("user")) {
			var flag = false;
			$("user_prompt").html("用户名由英文字母和数字组成的4-16位字符，以字母开头");
		}
		
		if (!flag("pwd")) {
			var flag = false;
			$("pwd_prompt").html("密码由英文字母和数字组成的4-10位字符");
		}
		
		
		
		if (!flag("user")) {
			var flag = false;
			$("user_prompt").html("√");
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
	
	
	.register{
			
			border:lightblue 1px none;
				
		}
	.box{
			margin: 10upx  solid;
			background: lightgreen;
			padding:10upx;
			margin: 10upx;
			padding: 10upx;
			text-align: center;
			
		}
		
		
		.hr_1{
			
			text-align: center;
			margin-bottom: auto;
			border-color: #666666;
			
			
		}
		
		
		
</style>