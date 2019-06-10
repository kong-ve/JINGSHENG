<template>
	<el-container class="box">
		<el-header></el-header>
		<el-container style="height: 100%;">
			<el-aside class="lefts">
				<div class="title-content">
					<h1>Contact</h1>
					<div class="phone">
						877 788 70
					</div>
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
				<el-main id="main-body" style="padding-left: 10%;padding-right: 0;">
					<div style="padding-bottom: 30px;"><h1 class="main-body-header">感谢联系京盛时代</h1>
					<h8 class="main-body-title">致力于打造一个专业、高效、创新的团队是每一个京盛人的追求，为每一位客户提供最优质的服务是我们的庄重承诺</h8>
					</div><div class="forms">
						<el-form class="forms-left">
							<el-form-item>
								<el-input v-model="form.name" placeholder="姓名"></el-input>
							</el-form-item>
							<el-form-item>
								<el-input v-model="form.email" placeholder="邮箱"></el-input>
							</el-form-item>
							<el-form-item>
								<el-input v-model="form.phone" placeholder="手机"></el-input>
							</el-form-item>
							<el-form-item>
								<el-input type="textarea" :autosize="{ minRows: 6, maxRows: 8}" placeholder="需求" resize="none" v-model="remark">
								</el-input>
							</el-form-item>
							<el-form-item>
								<el-button type="primary">立即提交</el-button>
							</el-form-item>
						</el-form>
						<div class="forms-right">
							<div class="he">您希望我们</div>
							<div class="he_title">为您提供什么服务？</div>
						<div class="btn_list">
							<div style="padding: calc(2%);"><el-button plain>hr综合服务承接</el-button>
							<el-button plain>技术解决</el-button></div>
							<div style="padding: calc(2%);"><el-button plain>业务推广</el-button>
							<el-button plain>虚拟数字产品分销与服务</el-button></div>
						</div>
						</div>
					</div>
				</el-main>
			</el-container>
		</el-container>
		<el-footer class="footer" height="215px"  id="footer_fix">
			<el-row :gutter="10" class="footer-alt">
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
					remark: '',

				}
			}
		}
	}
</script>

<style scoped type="text/scss" lang="scss">
	.footer-bottom{
		background: url(../../assets/about/关于我们_05.jpg);
	position: relative;
	bottom: 0;
	width: 100%;
	background-size: cover;
	background-repeat: no-repeat;
	}
	
	.footer-alt{
		width: 100%;
		height: 100%;
		padding: 20px;
		.bg-purple{
			padding: 30px
		}
		.bg-purple-light{
			padding: 30px;
			.left{
				width: 50%;
				float: left;
				padding-right: 0.5px;
			}
			.right{
				width: 50%;
				float: right;
				padding-left: 0.5px;
				}
				img{
					max-width: 80px;
				}
				.right-top{
					text-align: center;
	
				}
				.right-bottom{
					text-align: center;
	
				}
				.left-top{
					text-align: center;
	
				}
				.left-bottom{
					text-align: center;
	
				}
			.footer-img{
				width:100%;
			}
		}
		p:first-child{
			padding-bottom: 30px
		}
		p{
			padding-bottom: 0.93780px;
		}
	}
	.forms{
		padding-top: 5%;
		background: #2fc5d2;
		min-height: 8rem;
		height: 70%;
	}
	.main-body{
		padding: 30px 0px 30px 30px;
	}
	.main-body-header{
		font-size: 0.8rem;
		font-weight: bold;
	}
	.main-body-title{
		font-size: 0.3rem;
	}
	.forms-left {
		width: 50%;
		padding: 20px;
		position: relative;
		float: left;
		height: 100%;
	}
	.forms-right {
		width: 50%;
		padding: 20px;
		position: relative;
		float: right;
		height: 100%;
	}
	.forms-right .el-button{
		background: rgba(0, 0, 0, 0);
    color: #fff;
    padding: 0.5rem;
    width: 5rem;
	font-size: 0.3rem;
	}
	.forms-right .el-button:active{
		background: rgba(0,0,0,0);
		color: #fff;
		border: 1px solid #DCDFE6;
	}
	.forms-right .el-button:hover{
		background: rgba(0,0,0,0);
		color: #fff;
		border: 1px solid #DCDFE6;
	}
	.el-button.is-plain:focus, .el-button.is-plain:hover{
		border: 1px solid #DCDFE6;
	}
	.box {
		height: 100%;
		background-image: url('../../assets/cell/bg.jpg');
		background-repeat: no-repeat;
		background-size: cover;
	}

	.box-logo img {
		width: .7rem;
		padding-left: 10px;
	}

	.box_body_list {
		padding-bottom: 10px;
	}
.he{
	font-size: 0.5rem;
	font-weight: bold;
}
.he_title{
	font-size: 0.8rem;
	font-weight: bolder;
}
.box-body{
	height: auto;
	padding-bottom: .3rem;
	overflow: auto;
}
	.box-body .box_body_list .box_body_list_title {
		font-size: x-large;
		font-weight: bolder;
	}

	.box_body_list_other p {
		font-size: 0.25rem;
    font-weight: bold;
	}

	.box_body_list_other p:first-child::after {
		content: url(../../assets/cell/local.png);
		padding-left: 5px;
	}

	.title-content {
		padding-bottom: 5%;
	}

	.title-content::after {
		content: "";
		display: inline-block;
		bottom: 0;
		left: calc(30%);
    width: calc(50%);
    height: 5px;
    background: #000;
	}

	.lefts {
		width: 20% !important;
		padding: 1rem 0 0 1rem;
		margin-left: 10%;
		background: #fff;
		color: #000;
	}

	.lefts h1 {
		font-size: 0.9rem;
	}

	.phone {
		padding: 5px;
		font-size: 0.8rem;
		color: #14C0FE;
	}
	@media (max-width:1024px) {
		.footer-bottom{
			background-size: contain;
		}
	}
	@media (max-width: 700px) {
		.forms-right .el-button{
			width:4rem;
		}
		.el-button+.el-button{
			margin-left: 0;
			margin-top: 0.1rem;
		}
		.forms{
			padding-top: 15px;
			background: #2fc5d2;
			min-height: 11rem;
			min-width: 13rem;
		}
		.forms-right .el-button{
			width:4rem;
		}
		.el-button+.el-button{
			margin-left: 0;
			margin-top: 0.1rem;
		}
		.lefts{
			width: 20% !important;
			padding: .5rem;
			margin-left: .6rem;
		}
		.el-button{
			margin: calc(1%);
		}
		.lefts h1 {
			font-size: xx-small;
			font-weight: bold;
		}
		.title-content::after {
			left: calc(30%);
			width: calc(50%);
		}
		.phone {
			padding: .05px;
			font-size: .05rem;
		}
		.box-body .box_body_list .box_body_list_title {
			font-size: 0.3rem;
			font-weight: bolder;
		}
		.he{
			font-size: 0.2rem;
			font-weight: bold;
		}
		.he_title{
			font-size: 0.4rem;
			font-weight: bold;
			
		}
		.footer{
			.footer-alt{
				width: 100%;
				height: 100%;
				padding: 16px;
				padding-top: 51px;
				font-size: 0.3rem;
				.bg-purple{
					padding: 0.5px;
					font-size:xx-small;
				}
				.bg-purple-light{
					padding: 0.5px;
					.right-top{
						text-align: center;
						font-size:xx-small;
					}
					.right-bottom{
						text-align: center;
						font-size:xx-small;
					}
					.left-top{
						text-align: center;
						font-size:xx-small;
					}
					.left-bottom{
						text-align: center;
						font-size:xx-small;
					}
				}
				p:first-child{
					padding-bottom: 0.5px
				}
				p{
					padding-bottom: 0.5px;
				}
			}
		}
	}
	@media only screen and(min-width:850px) and (max-width: 1945px) {
		.forms-right .el-button{
			width:4rem;
		}
		.el-button+.el-button{
			margin-left: 0.01rem;
			margin-top: 0.1rem;
		}
		.footer{
			.footer-alt{
				width: 100%;
				height: 100%;
				padding: 16px;
				padding-top: 51px;
				font-size: xx-small;
				.bg-purple{
					padding: 0.5px;
					font-size:xx-small;
				}
				.bg-purple-light{
					padding: 0.5px;
					.right-top{
						text-align: center;
						font-size:xx-small;
					}
					.right-bottom{
						text-align: center;
						font-size:xx-small;
					}
					.left-top{
						text-align: center;
						font-size:xx-small;
					}
					.left-bottom{
						text-align: center;
						font-size:xx-small;
					}
				}
				p:first-child{
					padding-bottom: 0.5px
				}
				p{
					padding-bottom: 0.5px;
				}
			}
		}
		.lefts{
			width: 20% !important;
			padding: .5rem;
			margin-left: .6rem;
		}
		.he{
			font-size: xx-small;
			font-weight: bold;
		}
		.he_title{
			font-size: x-small;
			font-weight: bold;
			
		}
		.lefts h1 {
			font-size: 0.2rem;
			font-weight: bold;
		}
		.title-content::after {
			left: calc(30%);
			width: calc(50%);
		}
		.phone {
			padding: .05px;
			font-size: 0.3rem;
		}
		.box-body .box_body_list .box_body_list_title {
			font-size: xx-small;
			font-weight: bolder;
		}
	}
	.footer{
		background: #333;
			width: 100%;
	}
</style>
