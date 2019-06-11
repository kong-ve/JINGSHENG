<template>
	<div class="block">
		<el-carousel id="img-header">
			<el-carousel-item key="1"><img src="../../assets/banner/1.jpg" class="el-carousel-img" /></el-carousel-item>
			<el-carousel-item key="2"><img src="../../assets/banner/3.jpg" class="el-carousel-img" /></el-carousel-item>
			<el-carousel-item key="3"><img src="../../assets/banner/2.jpg" class="el-carousel-img" /></el-carousel-item>
		</el-carousel>
		<h4 class="title">涵括业务</h4>
		<div style="padding-left: 10%;">
			<div align="center" style="padding-top: 50px;">
				<!-- <el-tabs v-model="activeName" @tab-click="handleClick" stretch="true">
						<el-tab-pane label="01-技术解决" name="first" class="f-t">技术解决</el-tab-pane>
						<el-tab-pane label="02-HR服务解决方案" name="second" class="f-t">HR服务解决方案</el-tab-pane>
						<el-tab-pane label="03-虚拟数字产品分销与服务" name="third"class="f-t">虚拟数字产品分销与服务</el-tab-pane>
					</el-tabs> -->
				<ul class="tab-list">
					<li :class="[first ? activeClass : '', tabCss]" @click="changeClick('first')">
						01-
						<span>技术解决</span>
					</li>
					<li :class="[two ? activeClass : '', tabCss]" @click="changeClick('two')">
						02-
						<span>HR服务解决方案</span>
					</li>
					<li :class="[three ? activeClass : '', tabCss]" @click="changeClick('three')">
						03-
						<span>虚拟数字产品分销与服务</span>
					</li>
				</ul>
			</div>
			<div class="grid-content">
				<div class="left"><img src="../../assets/image/首页_02_06.jpg.png" class="img-list" /></div>
				<div class="right alow-right">
					<div class="card-list">
						<div class="card-header"><div class="floats">技术解决</div></div>
						<div class="card-body">
							高科技类企业往往规模庞大技术需求复杂且具有多样化 京盛时代在软件技术开发领域深耕多年，拥有为国内领 先的科技公司提供技术服务的丰富经验，以及有优秀的
							技术团队保驾护航，可以为客户提供量身定制的技术解 决方案。
						</div>
						<div class="card-bottom"><span class="pages">-01</span></div>
					</div>
				</div>
			</div>
			<div class="grid-content">
				<div class="right"><img src="../../assets/image/首页_03_07.jpg.png" class="img-list" /></div>
				<div class="left alow-left">
					<div class="card-list">
						<div class="card-header"><div class="floats">HR服务解决方案</div></div>
						<div class="card-body">
							近年来许多高速成长的创新型企业面临招聘人员耗时费力 成效低、人才管理困难重重和人员流失严重等种种问题， 京盛时代依托在各领域丰富的人力资源以及国内领先的开
							发技术团队支撑，实现企业合理的人才分配机制，提升企 业运作效率，降低用工风险，充分发挥企业核心的竞争力
						</div>
						<div class="card-bottom"><span class="pages">-02</span></div>
					</div>
				</div>
			</div>
			<div class="grid-content">
				<div class="left"><img src="../../assets/image/首页_04_06.jpg.png" class="img-list" /></div>
				<div class="right alow-right">
					<div class="card-list">
						<div class="card-header"><div class="floats">虚拟数字产品分销与服务</div></div>
						<div class="card-body">
							<p>-全面覆盖虚拟品类</p>
							<p>-专业服务B端客户</p>
							<p>-专业系统平台保障</p>
							<p>-全面的数据营销功能</p>
						</div>
						<div class="card-bottom"><span class="pages">-03</span></div>
					</div>
				</div>
			</div>
		</div>
		<div id="proList">
			<div class="l_p">
				<!-- <div class="top"><h3>合作伙伴</h3></div> -->
				<div class="top_list">
					<img src="../../assets/ban.jpg" />
					<!-- <div class="top_list_card bluecat">
							<div class="card_list_title">平安科技：</div>
							<div class="card_list_body">
								平安科技通过"科技+互联网+金融"模式， 在 技术研究和储备方面，拥有超过18项新技术 及全球研究和开发AI内部的能力， 包括微表
								情、图像和语音识别及语义理解。
							</div>
						</div>
						<div class="top_list_card whitebg">
							<div class="card_list_title">陆金所：</div>
							<div class="card_list_body">
								陆金所是中国平安集团打造的网络投融资平 台，隶属于上海陆家嘴国际金融资产交易市 场股份有限公司，为企业及个人客户提供投 融资中介服务。
							</div>
						</div>
						<div class="top_list_card whitebg">
							<div class="card_list_title">中国移动：</div>
							<div class="card_list_body">中国移动目前是全球网络规模最大、客户数 量最多、盈利能力和品牌价值领先、市值排 名位居前列的电信运营企业。</div>
						</div> -->
				</div>
				<div id="logo_list">
					<div class="list_logo">
						<img src="../../assets/logolist/zgpa.png" />
						<img src="../../assets/logolist/ljs.png" />
						<img src="../../assets/logolist/ydtx.png" />
						<img src="../../assets/logolist/hej.png" />
						<img src="../../assets/logolist/cibn.png" />
					</div>
					<div class="list_logo">
						<img src="../../assets/logolist/txsp.png" />
						<img src="../../assets/logolist/iqiyi.png" />
						<img src="../../assets/logolist/shsp.png" />
						<img src="../../assets/logolist/youku.png" />
						<img src="../../assets/logolist/jd.png" />
					</div>
					<div class="list_logo">
						<img src="../../assets/logolist/hr.png" />
						<img src="../../assets/logolist/dx.png" />
						<img src="../../assets/logolist/lt.png" />
						<img src="../../assets/logolist/sn.png" />
						<img src="../../assets/logolist/yx.png" />
					</div>
					<div class="list_logo">
						<img src="../../assets/logolist/sopce.png" />
						<img src="../../assets/logolist/sy.png" />
						<img src="../../assets/logolist/xbk.png" />
						<img src="../../assets/logolist/kfc.png" />
						<img src="../../assets/logolist/qj.png" />
					</div>
				</div>
			</div>
			<el-footer class="footer" height="215px" id="footer_fix">
				<el-row :gutter="10" class="footer-alt">
					<el-col :xs="15" :sm="15" :md="15" :lg="15" :xl="15">
						<div class="bg-left-footer">
							<p>京盛集团 Ai美网</p>
							<p>免责声明 版权所有：京盛时代（北京）新媒体科技有限公司 Beijing Jingsheng Era Advertising Co. Ltd.</p>
							<p>京ICP备17028194号 增值电信业务经营许可证B2-20170400</p>
						</div>
					</el-col>
					<el-col :xs="9" :sm="9" :md="9" :lg="9" :xl="9" style="padding-right: 0;">
						<div class="bg-right-footer">
							<div class="left-footer">
								<div class="left-top-footer"><img src="../../assets/image/首页-1_05_03.jpg" class="footer-img" /></div>
								<div class="left-bottom-footer">AI美网</div>
							</div>
							<div class="right-footer">
								<div class="right-top-footer"><img src="../../assets/image/首页-1_05_05.png" class="footer-img" /></div>
								<div class="right-bottom-footer">京盛集团</div>
							</div>
						</div>
					</el-col>
				</el-row>
			</el-footer>
		</div>
	</div>
</template>

<script>
export default {
	data() {
		return {
			first: true,
			two: false,
			three: false,
			tabCss: 'tab-list-view',
			activeClass: 'active'
		};
	},
	mounted() {
		window.onresize = function temp() {
			let h = document.querySelector('.el-carousel-img').height;
			var im = document.getElementById('img-header');

			im.style.height = h + 'px';
		};
	},
	methods: {
		handleClick(tab, event) {
			console.log(tab, event);
		},
		changeClick(tab) {
			if (tab == 'first') {
				this.first = true;
				this.two = false;
				this.three = false;
			} else if (tab == 'two') {
				this.first = false;
				this.two = true;
				this.three = false;
			} else if (tab == 'three') {
				this.first = false;
				this.two = false;
				this.three = true;
			}
		}
	},
	created() {
		if(document.querySelector('.el-carousel-img')){
		let h = document.querySelector('.el-carousel-img').height;
		var im = document.getElementById('img-header');
		im.style.height = h + 'px';
		}
	}
};
</script>
<style>
.el-tabs__nav-wrap::after {
	border-bottom: 0;
	background-color: rgba(0, 0, 0, 0);
}
.el-tabs__item {
	font-size: x-large;
}
.el-tabs__active-bar {
	width: calc(7%) !important;
	left: calc(12%) !important;
}
@media only screen and (min-width: 375px) and (max-width: 700px) {
	.el-tabs__active-bar {
		width: calc(7%) !important;
		left: calc(10%) !important;
	}
	.el-tabs__item {
		font-size: 0.3rem;
		padding: 0 10px;
	}
}
@media only screen and (min-width: 700px) and (max-width: 850px) {
	.el-tabs__active-bar {
		width: calc(10%) !important;
		left: calc(5%) !important;
	}
	.el-tabs__item {
		font-size: 0.3rem;
		padding: 0 10px;
	}
	.grid-content {
		height: 5rem;
	}
}
@media only screen and (min-width: 850px) and (max-width: 1024px) {
	.el-tabs__active-bar {
		width: calc(7%) !important;
		left: calc(12%) !important;
	}
	.el-tabs__item {
		font-size: 0.3rem;
		padding: 0 10px;
	}
}
.el-carousel__container {
	height: 100%;
}
</style>
<style scoped type="text/scss" lang="scss">
	.f-t{
		font-size: x-large
	}
	.card-header{
		font-family: "微软雅黑";
		font-size: 38px;
		padding: 6px 12px;
	}
	.card-body{
		font-family: "思源黑体 CN";
		font-size: 15px;
		padding: 28.54px 35px;
	}
	.card-header .floats::after {
		content: '';
		display: inline-block;
		position: absolute;
		bottom: 0;
		left: 14px;
		width: calc(7%);
		height: 2px;
		background: #409eff;
	 }
	 .footer{
		background: #333;
	    width: 100%;
	 }
	
	.top_list{
		zoom: 1;	
	}
	.top_list::after{
		content: "";
		display: block;
		height: 0;
		visibility: hidden;
		clear: both;
	}
	.tab-list {
    width: 90%;
    text-align: center;
    height: 50px;
	.tab-list-view {
    width: 30%;
    float: left;
    color: #000;
    font-weight: 600;
    font-family: "Arial";
    font-size: 24px;
    line-height: 50px;
    padding-left: 2%;
	position: relative;
	span{
		font-family: "思源黑体 CN";
		font-size: 23px;
		font-weight: bold;
	}
}
.actives::after{
		 content: " ";
		 display: inline-block;
    position: absolute;
    bottom: 0;
    left: calc(40%);
    width: calc(30%);
    height: 3px;
    background: #24deea;
	}
	}
	.footer-alt{
		width: 100%;
		height: 100%;
		padding: 20px;
		color: #fff;
		.bg-left-footer{
			padding: 30px
		}
		.bg-right-footer{
			padding: 30px;
			.left-footer{
				width: 50%;
				float: left;
				padding-right: 0.5px;
			}
			.right-footer{
				width: 50%;
				float: right;
				padding-left: 0.5px;
				}
				img{
					max-width: 80px;
				}
				.right-top-footer{
					text-align: center;

				}
				.right-bottom-footer{
					text-align: center;

				}
				.left-top-footer{
					text-align: center;

				}
				.left-bottom-footer{
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
.block {
	margin-top: 0;
	position: relative;
}
#proList {
	background: #f6f6ff;
	position: absolute;
	text-align: center;
	width: 100%;
}
.top_list img{
	width: 100%

}
#proList .l_p {
	padding: 5%;
	padding-top: 0
}
.l_p .top h3 {
	text-align: center;
	color: #000;
	font-size: 34px;
	padding: 10px 15px;
}
.top_list .top_list_card {
	width: 25%;
	padding: .5rem;
	border-radius: 10%;
	float: left;
	text-align:left;
	margin: 2%;
	height: 100%;
}
.top_list_card .card_list_title {
	font-size: 18px;
	padding: 13px 0;
	font-weight: bold;
	text-align: left;
}
.top_list_card .card_list_body {
	font-size: 15px;
	padding: 9px 0;
	overflow: hidden;
}
.bluecat {
	background: -webkit-linear-gradient(left, #14c0fe, #3088fe);
	background: -o-linear-gradient(right, #14c0fe, #3088fe);
	background: -moz-linear-gradient(right, #14c0fe, #3088fe);
	background: linear-gradient(to right, #14c0fe, #3088fe);
}
.whitebg {
	background: #fff;
	color: #000;
}
#logo_list{
	width: 100%;
    position: relative;
    left: 0%;
	display: inline-block;
}
.list_logo {
	text-align: center;
	width: 100%;
}
.list_logo img {
	width: 13%;
}
.card-header .floats {
	text-align: left;
	padding: 16px;
	color: #23deea;
	font-size: x-large;
	font-weight: bold;
	position: relative;
}
.card-bottom {
	position: absolute;
	bottom: 0.7rem;
	color: blue;
	width: 100%;
	font-weight: bold;
}
.pages {
	position: absolute;
	right: 0.5rem;
	text-align: right;
	font-size: x-large;
}

.card-body {
	padding: 16px;
	overflow: hidden;
	font-size: 20px;
}

.grid-content {
	width: 100%;
	height: 8rem;
	padding: 20px;
	overflow: hidden;
}
.left {
	float: left;
	width: 50%;
	height: 100%;
	overflow: hidden;
	color: #000;
}
.right {
	float: right;
	width: 50%;
	height: 100%;
	overflow: hidden;
	color: #000;
}
.card-list {
	background-color: #fff;
	color: #303133;
	-webkit-transition: 0.3s;
	transition: 0.3s;
	padding: 16px 0;
	padding-left: 20px;
	height: 100%;
	position: relative;
}
.alow-left {
	-webkit-box-shadow: -4px -3px 12px 0px rgba(0, 0, 0, 0.1);
	box-shadow: -4px -3px 12px 0px rgba(0, 0, 0, 0.1);
	border: 1px solid rgba(174, 174, 174, 0.33);
}
.alow-right {
	-webkit-box-shadow: 0 5px 12px 0px rgba(0, 0, 0, 0.1);
	box-shadow: 0 5px 12px 0px rgba(0, 0, 0, 0.1);
	border: 1px solid rgba(174, 174, 174, 0.33);
}
.title {
	color: #000;
	text-align: center;
	padding-top: 50px;
	font-family: "微软雅黑";
	font-weight: bold;
	font-size: 34px;
}
.tab {
	color: #000;
}
.img-list {
	width: 100%;
	height: 100%;
	object-fit: cover;
}
.bg-purple {
	height: 100%;
}
.bg-purple-light {
	height: 100%;
}
.tab ul {
	list-style: none;
	width: 100%;
	height: 70px;
	padding: 30px 15px 15px 15px;
	text-align: center;
}

.tab ul li {
	list-style: none;
	float: left;
	font-size: xx-small;
	padding-right: 8px;
	width: 30%;
	position: relative;
}
.active {
	color: #1e6abc;
}
.active::after {
	content: ' ';
	width: 30.4px;
	height: 1.92px;
	background: #6498d1;
	position: absolute;
	bottom: -6.4px;
	left: 48%;
	-webkit-transform: translateX(-50%);
	transform: translateX(-50%);
}

.el-carousel__item:nth-child(2n) {
	background-color: #99a9bf;
}

.el-carousel__item:nth-child(2n + 1) {
	background-color: #d3dce6;
}
.el-carousel-img {
	width: 100%;
	height: auto;
	object-fit: cover;
}
.el-card {
	height: 100%;
}

@media (max-width:1280px) {

	.tab-list {
	width: 90%;
	text-align: center;
	height: 50px;
	.tab-list-view {
	width: 30%;
	float: left;
	color: #000;
	font-weight: 600;
	font-family: "Arial";
	font-size: 14px;
	line-height: 50px;
	padding-left: 2%;
	position: relative;
	span{
		font-family: "思源黑体 CN";
		font-size: 16px;
		font-weight: bold;
	}
	}
	}
	
	.footer-bottom{
		background-size: contain;
	}
}


@media (max-width: 860px) {
	.el-tabs__active-bar {
		left: calc(18%);
	}

	.tab-list {
	    width: 96%;
	    text-align: center;
	    height: 50px;
		.tab-list-view {
	    width: 30%;
	    float: left;
	    color: #000;
	    font-weight: 600;
	    font-family: "Arial";
	    font-size: 12px;
	    line-height: 50px;
	    padding-left: 2%;
		position: relative;
		span{
			font-family: "思源黑体 CN";
			font-size: 12px;
			font-weight: bold;
		}

	}
	.actives::after{
		content: " ";
		display: inline-block;
	    position: absolute;
	    bottom: 0;
	    left: calc(40%);
	    width: calc(30%);
	    height: 3px;
	    background: #24deea;
		}
	}

	.title {
		font-size: large;
	}
	.grid-content {
		height: 5rem;
	}
	.grid-content .left,.grid-content .right {
		height: 100%;
	}
	.floats {
		padding: 1px !important;
		font-size: 0.35rem !important;
	}
	.card-body {
		font-size: 0.25rem !important;
	}
	.pages{
		font-size: 0.25rem;
	}
	.floats::after {
		content: '';
		display: inline-block;
		position: absolute;
		bottom: 0;
		left: 0.05rem !important;
    width: calc(5%) !important;
		height: 2px;
		background: #23deea;
	}

	
	.grid-content .left,.grid-content .right {
		height: 100%;
	}
	.top_list .top_list_card{
		padding: .5rem;;
	}
	.top_list .top_list_card {
		width: 30% !important;
	}
	
	.top_list .top_list_card{
		padding: .5rem;;
	}
	.footer{
		.footer-alt{
			width: 100%;
			height: 100%;
			padding: 16px;
			padding-top: 51px;
			font-size: xx-small;
			.bg-left-footer{
				padding: 0.5px;
				font-size:xx-small;
			}
			.bg-right-footer{
				padding: 0.5px;
				.right-top-footer{
					text-align: center;
					font-size:xx-small;
				}
				.right-bottom-footer{
					text-align: center;
					font-size:xx-small;
				}
				.left-top-footer{
					text-align: center;
					font-size:xx-small;
				}
				.left-bottom-footer{
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

 @media (max-width: 700px) {

	.tab-list {
	width: 90%;
	text-align: center;
	height: 50px;
	.tab-list-view {
	width: 30%;
	float: left;
	color: #000;
	font-weight: 600;
	font-family: "Arial";
	font-size: 10px;
	line-height: 50px;
	padding-left: 2%;
	position: relative;
	span{
		font-family: "思源黑体 CN";
		font-size: 10px;
		font-weight: bold;
	}
	}
	}
	.footer{
		.footer-alt{
			width: 100%;
			height: 100%;
			padding: 1.6px;
			padding-top: 51px;
			font-size: xx-small;
			.bg-left-footer{
				padding: 0.5px;
				font-size:xx-small;
			}
			.bg-right-footer{
				padding-top: 20px;
				.right-top-footer{
					text-align: center;
					font-size:xx-small;
				}
				.right-bottom-footer{
					text-align: center;
					font-size:xx-small;
				}
				.left-top-footer{
					text-align: center;
					font-size:xx-small;
				}
				.left-bottom-footer{
					text-align: center;
					font-size:xx-small;
				}
			}
			
			p{
				padding-bottom: 0.5px;
				&:first-child{
					padding-bottom: 0.5px
				}
			}
		}
	}
	
	.title {
		font-size: 0.5rem;
	}
	.top_list .top_list_card{
		padding: .5rem;;
	}
	.l_p{
		padding: 0 !important;
	}
	.pages{
		font-size: 0.2rem;
	}
	.floats::after {
		content: '';
		display: inline-block;
		position: absolute;
		bottom: 0;
		left: 0.05rem !important;
        width: calc(13%) !important;
		height: 2px;
		background: #23deea;
	}
	.floats {
		padding: 1px !important;
		font-size: 0.4rem !important;
	}
	.card-body {
		font-size: 0.22rem !important;
		height: 2.645rem !important;
	}	
 }

</style>
