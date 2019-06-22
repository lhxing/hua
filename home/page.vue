<template>
	<view class="content">
		<view>
			<text class="title" >{{title}}</text>
		</view>
		<view class="a">
			
		
			<view class="a-2">
				 <view class="big_right">
				    
				      <view class="right_d1" >
							
				          <view class="d1_erji1" >
				              <h2>音乐世界</h2>
				          </view>
				      </view>
				      <view class="right_d2" 
				          
				          <view class="d1_erji1" >
				              <h2>音乐收藏</h2>
				          </view>
				      </view>
				      <view class="right_d3" >
				         
				          <view class="d1_erji1">
				              <h2>喜欢的音乐</h2>
				          </view>
				      </view>
				      
				      </view>
				      <view class="right_d4" >
				         
				          <view class="d1_erji1" >
				              <h2>返回顶部</h2>
				          </view>
				      </view>
				  </view>
			</view>
			
			<view class="a-3"> 
				 <view class="weizhi" >请您登录
				        <view class="shou">下拉</view>
				        <view class="erji1">
				            <view class="erji1_tu">
				                <img src="images/front/20.jpg">
								
				            </view>
				            <view class="hai">hai!@我是原创音乐</view>
				            <form action="">
				                <input type="text" class="i1" name="username" placeholder="请输入您的账号"><br>
				                <input type="text" class="i3" name="password" placeholder="请输入您的密码"><br>
				                <input type="button"class="i2" name="" value="登录">
				            </form>
				        </view>
				    </view>
				   
				    <view class="daohang" >
				        <ul>
				            <ul class="l1">
								<a href="#" id="register">音乐库</a>
								<navigator url="libary.vue"></navigator>
								<script>
									import mpvueEcharts from 'library.vue'
								</script>
								</ul>
								
				            <ul class="l2"><a href="#">
							
				                    <form>
				                        <input type="submit" name="" value="签到">
				                    </form>
				                </view>
				            </ul>
				            <ul class="l3">
								<navigator  url="rules.vue"> 音乐规则页</navigator></ul>
							<script>
								import mpvueEcharts from 'rules.vue'
							</script>
				            <ul class="l4"><a href="#">我的音乐▼</a>
				                <view class="erji3">
				                    <view class="erji3_div1">
				                        <a href="#">音乐收藏(0)</a></view>
				                    <view class="erji3_div2"><a href="#">音乐收藏(0)</a></view>
				                    <view class="erji3_div3"><a href="#">音乐足迹(0)</a></view>
					
				                </view>
				            </ul>
				            
				         
				           
				        </ul>
				    	</view>
		
					</view>
				<section>
				    <view classs="section_header">
				        <view class="header_div1">
				           <image src="img/1740.png_300.png"></image>
				        </view>
				        <view class="header_div2">
				           
							<image class="c-service-img" src="img/d2.jpg" mode="widthFix"></image>
				        </view>
				        <!-- 搜索框 -->
				        <view class="c-search-form">
				            <input class="c-search-input "  placeholder="大家都在搜：银临"   type="text">
				            <a class="c-search-button" href="###">
				                <span class="c-search-icon"></span>
				            </a>
				        </view>
				  
			</view>
			
			<navigator  url="page.vue"></navigator>
			
			</view>
	</view>
	</view>
</template>
<script type="text/javascript"></script>
<script>

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
	.a{
		display: flex;
		margin-top: -10upx;
		width: 100%;
		height: 500upx;
		background: #F4F4F4;
		justify-content: center;
	}
</style>
