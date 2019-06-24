<template>
	<el-container class="box">
		<el-header></el-header>
		<el-container style="height: 100%;">
			<el-aside class="lefts">
				<div class="title-content">
					<h1>Contact</h1>
					<div class="phone">877 788 70</div>
				</div>
				<div class="box-body">
					<div class="box_body_list">
						<div class="box_body_list_title">深圳·总部</div>
						<div class="box_body_list_other">
							<p>Add:广东省深圳市南山区科技南十二路迈瑞大厦4C01</p>
							<p>Tel:0755-86725691</p>
							<p>Fax:0755-86725691</p>
							<p>email:zhouh@bjjssd.net</p>
						</div>
					</div>
					<div class="box_body_list">
						<div class="box_body_list_title">北京</div>
						<div class="box_body_list_other">
							<p>Add:北京市朝阳区霄云路32号2号楼6层2603室</p>
							<p>Tel:010-87778870</p>
							<p>Fax:010-87778870</p>
							<p>email:zhouh@bjjssd.net</p>
						</div>
					</div>
					<div class="box_body_list">
						<div class="box_body_list_title">江西</div>
						<div class="box_body_list_other">
							<p>Add:江西省鹰潭市凯翔新天地1号门8栋2602</p>
							<p>email:zhouh@bjjssd.net</p>
						</div>
					</div>
					<div class="box_body_list">
						<div class="box_body_list_title">江苏</div>
						<div class="box_body_list_other">
							<p>Add:江苏省苏州市姑苏区世界贸易中心B座8楼</p>
							<p>email:zhouh@bjjssd.net</p>
						</div>
					</div>
				</div>
				<div class="box-logo">
					<img src="../../assets/cell/weibo.png" />
					<img src="../../assets/cell/weixin.png" />
					<img src="../../assets/cell/qq.png" />
					<img src="../../assets/cell/youjian.png" />
				</div>
			</el-aside>
			<el-container>
				<el-main id="main-body" style="margin-left: 10%;padding: 0;">
					<div style="padding-bottom: 5px;">
						<h1 class="main-body-header">感谢联系京盛时代</h1>
						<h8 class="main-body-title">致力于打造一个专业、高效、创新的团队是每一个京盛人的追求，为每一位客户提供最优质的服务是我们的庄重承诺</h8>
					</div>
					<div class="forms">
						<div class="forms-left">
							<input v-model="form.name" placeholder="姓名"/>
							<input v-model="form.email" placeholder="邮箱"/>
							<input v-model="form.phone" placeholder="手机"/>
							
								<textarea placeholder="需求"  v-model="remark" rows="11"></textarea>
							
							<el-button type="primary">立即提交</el-button>
						</div>
						<div class="forms-right">
							<div class="he">您希望我们</div>
							<div class="he_title">为您提供什么服务？</div>
							<div class="btn_list">
								<div style="padding: calc(2%);">
									<div class="el-button-a">hr综合服务承接</div>
									<div class="el-button-a">技术解决</div>
								</div>
								<div style="padding: calc(2%);">
									<div class="el-button-a">业务推广</div>
									<div class="el-button-a">虚拟数字产品分销与服务</div>
								</div>
							</div>
						</div>
					</div>
				</el-main>
			</el-container>
		</el-container>
		<el-footer class="footer" height="115px" id="footer_fix">
			<div class="footer-alt">
				<el-row :gutter="10">
				<el-col :xs="15" :sm="15" :md="15" :lg="15" :xl="15">
					<div class="grid-content bg-purple">
						<p>京盛集团 Ai美网</p>
						<p>免责声明 版权所有：京盛时代（北京）新媒体科技有限公司 Beijing Jingsheng Era Advertising Co. Ltd.</p>
						<p>京ICP备17028194号 增值电信业务经营许可证B2-20170400</p>
					</div>
				</el-col>
				<el-col :xs="9" :sm="9" :md="9" :lg="9" :xl="9" style="padding-right: 0;">
					<div class="grid-content bg-purple-light">
						<div class="left">
							<div class="left-top"><img src="../../assets/image/首页-1_05_03.jpg" class="footer-img" /></div>
							<div class="left-bottom">AI美网</div>
						</div>
						<div class="right">
							<div class="right-top"><img src="../../assets/image/首页-1_05_05.png" class="footer-img" /></div>
							<div class="right-bottom">京盛集团</div>
						</div>
					</div>
				</el-col>
			</el-row>
			</div>
		</el-footer>
	</el-container>
</template>

<script>
export default {
	data() {
		return {
			form: {
				name: '',
				phone: '',
				email: '',
				remark: ''
			}
		};
	}
};
</script>

<style scoped type="text/scss" lang="scss">
	html{-webkit-text-size-adjust:none;}
	.el-button--primary {
    color: #000;
    background-color: #ffffff;
    border-color: #d4d4d4;
}
	.el-header{
		height: 2% !important;
	}
	.el-button-a{
		overflow: hidden;
white-space: nowrap;
text-overflow:ellipsis;

	}
	input,textarea{
		width:100%;
		margin-bottom: 1%;
		line-height: 10px;
		padding: 5px;
	}
	
.footer-bottom {
	background: url(../../assets/about/关于我们_05.jpg);
	position: relative;
	bottom: 0;
	width: 100%;
	background-size: contain;
	background-repeat: no-repeat;
}
.footer{
	width: 100%;
	height: auto !important;
}
.footer-alt {
	width: 100%;
	height: 100%;
	padding: 0px;
	font-family: '微软雅黑';
	font-size: 18px;
	color: #fff;
	.bg-left-footer {
		padding: 30px;
	}
	.bg-right-footer {
		padding: 10px;
		.left-footer {
			width: 50%;
			float: left;
			padding-right: 0.5px;
		}
		.right-footer {
			width: 50%;
			float: right;
			padding-left: 0.5px;
		}
		img {
			max-width: 80px;
		}
		.right-top-footer {
			text-align: center;
		}
		.right-bottom-footer {
			text-align: center;
		}
		.left-top-footer {
			text-align: center;
		}
		.left-bottom-footer {
			text-align: center;
		}
		.footer-img {
			width: 100%;
		}
	}
	p:first-child {
		padding-bottom: 30px;
	}
	p {
		padding-bottom: 0.9378px;
	}
}
.footer-alt {
	width: 100%;
	height: 100%;
	padding: 0px;
	.bg-purple {
		padding: 30px;
	}
	.bg-purple-light {
		padding: 30px;
		zoom:1;
		&::after{
			content: "";
			clear: both;
			display: block;
			height: 0;
			visibility: hidden;
		}
		.left {
			width: 50%;
			float: left;
			padding-right: 0.5px;
		}
		.right {
			width: 50%;
			float: right;
			padding-left: 0.5px;
		}
		img {
			max-width: 80px;
		}
		.right-top {
			text-align: center;
		}
		.right-bottom {
			text-align: center;
		}
		.left-top {
			text-align: center;
		}
		.left-bottom {
			text-align: center;
		}
		.footer-img {
			width: 100%;
		}
	}
	p:first-child {
		padding-bottom: 30px;
	}
	p {
		padding-bottom: 0.9378px;
	}
}
.forms {
	padding-top: 1%;
	background: #2fc5d2;
	zoom: 1;
}
.forms::after {
	content: '';
	clear: both;
	height: 0;
	visibility: hidden;
	display: block;
}
.main-body {
	padding: 30px 0px 30px 30px;
}
.main-body-header {
	font-size: 15px;
	font-weight: bold;
	
}
.main-body-title {
	font-size: 6px;
	
}
.forms-left {
	width: 40%;
	padding: 20px;
	position: relative;
	float: left;
	height: 100%;
}
.forms-right {
	width: 40%;
	padding: 20px;
	position: relative;
	float: left;
	height: 100%;
}
.forms-right .el-button-a {
	background: rgba(0, 0, 0, 0);
	color: #fff;
	padding: 0.2rem;
	width: 48%;
	margin-left: 0.1rem;
	display: inline-block;
	border: 1px #fff solid;
	min-width: 45%;
	font-size: 14px;
	text-align: center;
}
.forms-right .el-button-a:active {
	background: rgba(0, 0, 0, 0);
	color: #fff;
	border: 1px solid #dcdfe6;
}
.forms-right .el-button-a:hover {
	background: rgba(0, 0, 0, 0);
	color: #fff;
	border: 1px solid #dcdfe6;
}

.box {
	height: 100%;
	background-image: url('../../assets/cell/bg.jpg');
	background-repeat: no-repeat;
	background-size: cover;
}

.box-logo img {
	width: 20%;
	padding-left: 10px;
	max-width: 60px;
}

.box_body_list {
	padding-bottom: 5px;
}
.he {
	font-size: 25px;
	font-family: "微软雅黑";
	font-weight: 400;
}
.he_title {
	font-size: 23px;
	font-family: "微软雅黑";
	font-weight: bold;
}
.box-body {
	height: auto;
	padding-bottom: 0.3rem;
	overflow: auto;
}
.box-body .box_body_list .box_body_list_title {
	font-size: 23px;
	font-weight: bolder;
}

.box_body_list_other p {
	font-size: 12px;
	font-weight: 400;
}

.box_body_list_other p:first-child::after {
	content: '';
	background: url(../../assets/cell/local.png);
	background-repeat: no-repeat;
	background-size: contain;
	position: relative;
	padding-left: 15px;
}

.title-content {
	padding-bottom: 5%;
}

.title-content::after {
	content: '';
	display: inline-block;
	bottom: 0;
	left: calc(30%);
	width: calc(30%);
	height: 5px;
	background: #000;
}

.lefts {
	width: 20% !important;
	padding: 0.2rem;
	margin-left: 10%;
	background: #fff;
	color: #000;
	height: 100%;
}

.lefts h1 {
	font-size: 38px;
}

.phone {
	padding: 5px;
	font-size: 40px;
	color: #14c0fe;
}
@media (max-width:1550px){
	.lefts h1 {
		font-size: 0.4rem;
	}
	
	.phone {
		padding: 5px;
		font-size: 0.4rem;
		color: #14c0fe;
	}
	.box-body .box_body_list .box_body_list_title {
    font-size: 0.3rem;
    font-weight: bolder;
}
.box_body_list_other p {
    font-size: 0.25rem;
    font-weight: 400;
}
}

@media only screen and(min-width:241px) and(max-width: 700px) {
	.lefts {
		width: 100% !important;
		padding: 0.2rem;
		position: relative;	
		bottom: 215px;
		margin-left: 0.2rem;
	}
	.forms-left,.forms-right{
		width: 100%;
		float: none;
	}
	.main-body{
		width: 100%;
	}
	.el-button.el-button--primary{
		padding: 4px;
	}
	.title-content::after{
		width: calc(40%);
		height:2px;
	}
	.lefts h1{
		font-size: 8px;
	}
	.phone{
		font-size: 8px;
	}
	html,body{-webkit-text-size-adjust:none;}
	.forms-right .el-button-a {
		min-width: 45%;
		width: 40%;
	}
	.footer-alt .bg-purple{
		padding: 15px;
		font-size: 8px;
	}
	.footer-alt .bg-purple-light{
		font-size: 7px;
	}
	.footer-alt p:first-child{
		padding-bottom: 3%;
	}
	.forms-right .el-button-a {
		font-size: 6px;
	}
	.box-body .box_body_list .box_body_list_title {
		font-size: 10px;
		font-weight: 600;
	}
	.el-button-a{
		font-size:3px 
	}
	.box_body_list_other p {
		font-size: 5px;
		font-weight: 500;
	}
	.he_title{
		font-size: 12px;
	}
	.he{
		font-size: 10px;
	}
	.forms-right{
		width:55%;
	}
	.footer-alt{
		font-size: 10px;
	}
	.forms-left{
			padding: 5px;
			width: 45%;
		}
		textarea{
			margin-bottom: 3%;
			height: 65px;
		}
}
@media only screen and(min-width:701px) and (max-width: 849px) {
	.forms-right .el-button-a {
		width: 45%;
		font-size: 7px;
	}
	
	#main-body {
		overflow-y: auto !important;
		padding-top: 1% !important;
	}
	.box-body .box_body_list .box_body_list_title {
		font-size: 12px;
		font-weight: 600;
	}
	.box_body_list_other p {
		font-size: 7px;
		font-weight: 500;
	}
	.el-button-a + .el-button-a {
		margin-left: 0;
		margin-top: 0.1rem;
	}
	.forms {
		padding-top: 15px;
		background: #2fc5d2;
	}
	.el-button-a + .el-button-a {
		margin-left: 0;
		margin-top: 0.1rem;
	}
	.lefts {
		width: 20% !important;
		padding: 0.2rem;
		margin-left: 0.6rem;
	}
	.el-button-a {
		margin: calc(1%);
	}
	.lefts h1 {
		font-size: 14px;
		font-weight: bold;
	}
	.title-content::after {
		left: calc(30%);
		width: calc(50%);
	}
	.phone {
		padding: 0.05px;
		font-size: 13px;
	}
	.box-body .box_body_list .box_body_list_title {
		font-size: 10px;
		font-weight: bolder;
	}
	.he {
		font-size: 12px;
		font-weight: 400;
	}
	.he_title {
		font-size:14px;
		font-weight: bold;
	}
	.footer {
		
		.footer-alt {
			width: 100%;
			height: 100%;
			padding: 16px;
			padding-top: 11%;
			font-size: 15px;
			.bg-purple {
				padding: 0.5px;
			}
			.bg-purple-light {
				padding: 0.5px;
				.right-top {
					text-align: center;
				}
				.right-bottom {
					text-align: center;
				}
				.left-top {
					text-align: center;
				}
				.left-bottom {
					text-align: center;
				}
			}
			p:first-child {
				padding-bottom: 0.5px;
			}
			p {
				padding-bottom: 0.5px;
			}
		}
	}
	#main-body {
		overflow-y: auto !important;
		padding-top: 1% !important;
	}
	.forms-left,.forms-right{
		width: 100%;
		float: none;
	}
}
@media only screen and(min-width:850px) and (max-width: 1450px) {
	@media (max-width: 1433px) {
		.el-button-a + .el-button-a {
			margin-left: 0.1rem;
			margin-top: 0.1rem;
		}
	}
	@media (max-width: 1024px) {
		.footer-bottom {
			background-size: contain;
		}
		#main-body {
			overflow-y: auto !important;
		}
	}
	#main-body {
		overflow-y: auto !important;
		padding-top: 1% !important;
	}
	.forms-right .el-button-a {
		min-width: 40%;
		width: 40%;
	}
	.forms-right .el-button-a {
		font-size: 10px;
	}
	.el-button-a + .el-button-a {
		margin-left: 0.1rem;
		margin-top: 0.1rem;
	}
	.footer {
		.footer-alt {
			width: 100%;
			height: 100%;
			padding: 16px;
			font-size: 10px;
			padding-top: 10%;
			.bg-purple {
				padding: 0.5px;
			}
			.bg-purple-light {
				padding: 0.5px;
				.right-top {
					text-align: center;
				}
				.right-bottom {
					text-align: center;
				}
				.left-top {
					text-align: center;
				}
			}
			p:first-child {
				padding-bottom: 0.5px;
			}
			p {
				padding-bottom: 0.5px;
			}
		}
	}
	.lefts {
		width: 25% !important;
		padding: 0.2rem;
		margin-left: 0.2rem;
	}

	.lefts h1 {
		font-size: 18px;
		font-weight: bold;
	}
	.title-content::after {
		left: calc(30%);
		width: calc(35%);
	}
	
	.phone {
		padding: 0.05px;
		font-size: 17px;
	}
	
	.box-body .box_body_list .box_body_list_title {
		font-size: 12px;
		font-weight: 600;
	}
	.box_body_list_other p {
		font-size: 10px;
		font-weight: 500;
	}
	.he_title{
		font-size: 12px;
	}
	.he{
		font-size: 10px;
	}
}


.footer {
	background: #333;
	width: 100%;
}
</style>
