<template>
	<div class="mains">
		<el-container style="height: 100%;">
  <el-main style="height: 80%;position: absolute;width: 100%;">
	  <div class="main-body">
	  	<el-col :xs="1" :sm="1" :md="3" :lg="3" :xl="3"><div style="width: 100%;height: 1px;"></div></el-col>
	  	<el-col :xs="22" :sm="22" :md="18" :lg="18" :xl="18" style="height: 100%;margin-bottom: 100px;">
	  	<div class="about-title"><b>profession</b>秉持专业价值</div>
	  	<div class="about-title-small">互相激励 梦想路上你我同行</div>
	  	<div class="about-body">
	  		<div class="body-header">京盛时代概况</div>
	  		<div class="body-message">jing sheng profile</div>
	  		<div class="message-box">
	  			京盛时代（北京）新媒体科技有限公司（简称：京盛时代），
	  			2011年6月创办于北京。是一家专注于为企业在等方面提供一站式解决方案的新型科技公司。目前在上海、深圳、江西、苏州
	  		</div>
	  		<ul class="product-list-header">
	  			<li class="list-product">
	  				<p>业务推广</p>
	  				<p>Business Promotion</p>
	  			</li>
	  			<li class="list-product">
	  				<p>技术应用及开发</p>
	  				<p>Technology application and development</p>
	  			</li>
	  			<li class="list-product">
	  				<p>数字产品服务</p>
	  				<p>Digital product services</p>
	  			</li>
	  		</ul>
	  							<div class="message-box fix">
	  								<span>等地均设立分公司。</span></div>
	  		<div class="div-img">
	  			<div class="div-img-left">
	  				<img src="../../assets/about/关于我们2_17.jpg.png" alt="">
	  			</div>
	  			<div class="div-img-right">
	  				<img src="../../assets/about/关于我们2_19.jpg.png" alt="">
	  			</div>
	  		</div>
	  		<div class="progress-footer">
	  			<span>京盛时代的主营业务涵括AI智能研发，虚拟数字产品分销和服务两大模块。2018年公司与平安科技、平安金服达成战略合作协议，针对金融保险领域的AI智能研发组建团队，基于合作研发的语音识别技术，通过最前沿的深度学习技术能够快速识别客户沟通对话中表达的意图及内容，精准判断客户意向并给出准确回应，完成智能高效的人机互动。</span>
	  		</div>
	  		<!-- <div class="product-body">	
	  		</div> -->
	  	</div>
	  	</el-col>
	  	<el-col :xs="1" :sm="1" :md="3" :lg="3" :xl="3"><div style="width: 100%;height: 1px;"></div></el-col>
	  </div>
  </el-main>
  <el-footer style="padding:0;height: 15%;position: absolute;bottom: 0;width: 100%;">
	  <div class="footer-fix">
	  	<div class="footer-left">
			<img src="../../assets/about/关于我们2_09.jpg.png" style="height: 100%;float: right;">
	  		<div class="left-f-fix">
	  			<div class="btn-about">联系我们</div>
	  			<p>如有什么建议 欢迎联系我们</p>
	  		</div>
	  	</div>
	  	<div class="footer-right">
			<img src="../../assets/about/关于我们2_10.jpg.png" style="height: 100%;float: left;">
	  		<div class="right-g-fix">
	  			<div class="btn-about">欢迎入驻</div>
	  			<p>人才服务平台邀您入驻</p>
	  		</div>
	  	</div>
	  	
	  </div>
	  <img src="../../assets/about/关于我们_05.jpg" style="width: 100%;height: 50%;position: relative;bottom: 0;"/>
  </el-footer>
</el-container>
	</div>
</template>

<script>
	export default {
		data() {
			return {

			}
		}
	}
</script>

<style scoped>
	.mains {
		height: 100%;
		background: url(../../assets/about/关于我们2_02.jpg);
		background-size: cover;
		background-repeat: no-repeat;
	}
.footer-bottom{
		background: url(../../assets/about/关于我们_05.jpg);
	position: relative;
	bottom: 0;
	width: 100%;
	background-size: cover;
	background-repeat: no-repeat;
	}
	.div-img-left {
		width: 50%;
    float: left;
    left: calc(25%);
	height: 100%;
	display: inline-block;
	}

	.fix {
    top: calc(40%);
    left: calc(17%);
	margin-bottom: 3% !important;
	}

	.div-img {
		zoom: 1;
    padding: 20px;
    top: calc(16%);
	width: 100%;
	height: auto;
	
	}
	.div-img::after{
		content: "";
		display: block;
		visibility: hidden;
		clear: both;
		height: 0;
	}

	.div-img-right {
		width: 50%;
    float: right;
    right: calc(10%);
	height: 100%;
	display: inline-block;
	}

	.product-list-header {
		padding: 10px;
		border-bottom: 1px solid #e3e3e3;
		list-style: none;
		height: auto;
		zoom: 1;
		margin: 0 5%;
		position: relative;
	}
	.product-list-header::after{
		content: " ";
		clear: both;
		visibility: hidden;
		display: block;
		height: 0;
	}
	.list-product {
		float: left;
		padding: 5px;
		width: 30%;
		position: relative;
	}

	.list-product:not(:last-child)::after {
		content: "";
		top: calc(35%);
    width: 2px;
    height: calc(45%);
    background: #000;
    position: absolute;
    right: 0%;
		background: #aeaeae;
	}
	
	/* .list-product:not(:last-child):not(:first-child)::after {
		content: "";
		top: calc(35%);
		width: 2px;
		height: 0.5rem;
		background: #000;
		position: absolute;
		right: 0%;
		background: #aeaeae;
	} */

	.main-body {
		padding: 0.5% 0 3% 0;
		height: 100%;
		padding-bottom: 100px;
		
	}

	.footer-fix {
		bottom: 0;
		width: 100%;
		height: 50%;
		zoom: 1;
		position: relative;
	}
.footer-fix::after{
	content: "";
	clear: both;
	visibility: hidden;
	height: 0;
	display: block;
}
	.footer-fix p {
		padding-top: 5px;
	}

	.btn-about {
		border: 1px solid #fff;
		display: inline-block;
		width: auto;
		height: auto;
		padding: 4px 11px;
	}

	.footer-left {
		width: 50%;
		/* background: url(../../assets/about/关于我们2_09.jpg.png);
		background-size: cover;
		background-repeat: no-repeat; */
		height: 100%;
		float: left;
		left:0;
		position: absolute;
		background: #18b5c6;
	}

	.left-f-fix {
		width: 15%;
		position: absolute;
		right: 0%;
		top: 30%;
		text-align: center;
		font-size: x-small;
	}

	.footer-right {
		width: 50%;
		/* background: url(../../assets/about/关于我们2_10.jpg.png);
		background-size: cover;
		background-repeat: no-repeat; */
		height: 100%;
		float: right;
		right: 0;
		position: absolute;
		background: #f4762c;
	}

	.right-g-fix {
		width: 15%;
		position: absolute;
		left: 0%;
		top: 30%;
		text-align: center;
		font-size: x-small;
	}

	.about-title {
		text-align: center;
		font-size: 0.6rem;
	}

	.about-title b {
		font-size: 0.8rem;
	}

	.about-title-small {
		text-align: center;
	}

	.about-title-small::after {
		content: "v";
		position: absolute;
    margin-top: 25px;
    left: calc(50%);
	}

	.about-body {
		background: url(../../assets/about/有阴影.jpg);
		background-size: cover;
		background-repeat: no-repeat;
		padding: 2%;
		margin-top: 3%;
		text-align: center;
		color: #c1c1c1;
		height: calc(95%);
		/* width: calc(70%); */
		position: relative;
		/* left: calc(15%); */
		box-shadow: 0px 0px 12px 0px #aeaeae;
	}

	.progress-footer {
		padding-top: 10px;
		text-align: center;
		width: 65%;
		font-size: 14px;
		margin-left: 15%;
	}

	.div-img-left img{
		width: 50%;
		float: right;
		margin-right: 5%;
	}
		.div-img-right img {
		width: 50%;
		float: left;
		margin-left: 5%;
	}

	.body-header {
		font-size: 24px;
		font-weight: 500;
		color: #000000;
	}

	.body-message {
		font-size: 8px;
		color: #f5f5f5;
	}

	.message-box {
		padding-top: 20px;
		font-size: 0.3rem;
		width: 70%;
		margin:0 15%;
		color: #bdbdbd;
		text-align: center;

	}

	.product-body {
		height: calc(20%);
	}
	.list-product p:first-child{
		font-size: 0.5rem;
		color: #a0a0a0;
		font-weight: 500;
	}
	.list-product p:last-child{
		font-size: 0.1rem;
		color: #e3e3e3;
	}
@media (max-width:1550px) {
	.message-box {
		font-size: 10px;
	}
	.progress-footer {
		font-size: 10px;
	}
	.list-product p:first-child{
		font-size: 14px;
		font-weight: 500;
	}
	.list-product p:last-child{
		font-size: 5px;
	}
	.list-product{
		padding: 0.1%;
	}
	.list-product:not(:last-child)::after{
		height: calc(75%);
    top: calc(15%);
	}
	.fix{
		margin-bottom: 1% !important;
	}
	.progress-footer {
		/* padding-bottom: 30px; */
		text-align: center;
		/* width: 90%; */
		font-size: 10px;
	}
	.div-img {
		width: 100%;
		padding-top: 0.2%;
		padding-bottom: 0.2%;
	}
	.div-img img {
		width: 40%;
	}
	.message-box{
		font-size: 12px;
	}
	.fix{
		margin-bottom: 1% !important;
	}
}
@media (max-width:1425px) {
		.list-product p:first-child{
			font-size: 16px;
			font-weight: 500;
		}
		.list-product p:last-child{
			font-size: 9px;
			display: block;
		}
		.div-img-left {
				/* width: 50%;
				float: left;
				left: 15%;
				top: calc(65%); */
				display: inline-block;
			}
		
			
		
			.div-img {
				/* padding: 5px;
				top: calc(15%);
				width: 80%; */
				font-size: 0.25em;
		
			}
		
			.div-img-right {
				/* width: 50%;
				float: right;
				right: calc(-15%);
				top: calc(65%); */
				display: inline-block;
			}
		
			.product-list-header {
				/* padding: 10px;
				border-bottom: 1px solid #aeaeae;
				list-style: none;
				height: 100px;
				margin: 0 5%; */
			}
		
			.list-product {
				/* float: left;
				padding: 5px;
				width: 33%; */
				padding: 0.1%;
				font-size: 0.05rem;
			}
		
			
		
			
		
			.main-body {
				/* padding: 2%; */
			}
		
			.footer-fix {
				/* bottom: 0; */
				width: 100%;
				/* height: 100px; */
			}
		
			.footer-fix p {
				padding-top: 5px;
			}
		
			.btn-about {
				/* border: 1px solid #fff;
				display: inline-block;
				width: auto;
				height: auto; */
				padding: 4px 11px;
			}
		
			.footer-left {
				width: 50%;
				
			}
		
			.left-f-fix {
				width: 25%;
				font-size: 0.1rem;
				/* position: absolute;
				text-align: center; */
				/* font-size: x-small; */
			}
		
			.footer-right {
				width: 50%;
				
			}
		
			.right-g-fix {
				width: 25%;
				font-size: 0.1rem;
				/* position: absolute;
				text-align: center; */
				/* font-size: x-small; */
			}
		
			.about-title {
				/* text-align: center; */
				font-size: large;
			}
		
			.about-title b {
				font-size: x-large;
			}
		
			.about-title-small {
				text-align: center;
			}
		
			/* .about-title-small::after {
				content: "v";
				position: relative;
				bottom: -30px;
				left: calc(-16%);
			} */
		
			/* .about-body {
				background: url(../../assets/about/有阴影.jpg);
				background-size: cover;
				background-repeat: no-repeat;
				padding: 20px;
				padding: 5px;
				margin-top: 8%;
				text-align: center;
				color: #000;
				height: calc(80%);
				width: calc(70%);
				position: relative;
				left: calc(15%);
				overflow: auto;
				-webkit-box-shadow: 0px 0px 12px 0px #aeaeae;
				box-shadow: 0px 0px 12px 0px #aeaeae;
			} */
		
			.progress-footer {
				/* padding-bottom: 30px; */
				/* text-align: center; */
				/* width: 90%; */
				font-size: 12px;
			}
		
			.div-img img {
				width: 50%;
			}
		
			.body-header {
				font-size: large;
				font-weight: bold;
			}
		
			.body-message {
				font-size: 0.25rem;
				color: #aeaeae;
			}
		
			.message-box {
				/* padding-top: 20px; */
				font-size: 14px;
				/* text-align: center; */
				/* top: calc(25%); */
		
			}
		
			/* .product-body {
				height: calc(58%);
			} */
	}

@media (max-width: 1319px) {
		.div-img-left {
			width: 50%;
			/* float: left; */
			/* left: 5%; */
			/* top: calc(66%); */
		}
	
		
	
		.div-img {
			padding: 5px;
			/* top: calc(23%); */
			/* width: 90%; */
	
		}
	
		.div-img-right {
			width: 50%;
			/* float: right;
			left: calc(55%);
			top: calc(65%); */
		}
	
		.product-list-header {
			padding: 10px;
			/* border-bottom: 1px solid #aeaeae;
			list-style: none;
			height: 60px;
			margin: 0 5%; */
		}
	
		.list-product {
			/* float: left;
			padding: 5px; */
			/* width: 33%; */
			font-size: 0.05rem;
			padding: 0.1%;;
			/* height: 100%; */
		}
	
		
	
		
	
		.main-body {
			padding: auto;
		}
	
		.footer-fix {
			bottom: 0;
			width: 100%;
			/* height: 100px; */
			
		}
	
		.footer-fix p {
			padding-top: 5px;
		}
	
		.btn-about {
			/* border: 1px solid #fff;
			display: inline-block;
			width: auto;
			height: auto; */
			padding: 4px 11px;
		}
	
		.footer-left {
			width: 50%;
			
		}
	
		.left-f-fix {
			width: 35%;
			/* position: absolute;
			text-align: center; */
			/* font-size: x-small; */
		}
	
		.footer-right {
			width: 50%;
			
			
		}
	
		.right-g-fix {
			width: 35%;
			/* position: absolute;
			text-align: center; */
			/* font-size: x-small; */
		}
	
		.about-title {
			text-align: center;
			font-size: 12px;
		}
	
		.about-title b {
			font-size: 16px;
		}
	
		.about-title-small {
			text-align: center;
			font-size: 10px;
		}
	
		.about-title-small::after {
			left: calc(50%);
    margin-top: 20px;
		}
	
		.about-body {
			/* background: url(../../assets/about/有阴影.jpg);
			background-size: cover;
			background-repeat: no-repeat;
			padding: 20px;
			padding: 5px;
			margin-top: 8%;
			text-align: center;
			color: #000;
			height: calc(80%);
			width: calc(70%);
			position: relative;
			left: calc(15%);
			overflow: auto; */
			-webkit-box-shadow: 0px 0px 12px 0px #aeaeae;
			box-shadow: 0px 0px 12px 0px #aeaeae;
		}
	
		.progress-footer {
			/* padding-top: 10px; */
			/* text-align: center;
			width: 80%; */
			font-size: 10px;
		}
	
		.div-img img {
			width: 80%;
		}
	
		.body-header {
			font-size: large;
			font-weight: bold;
		}
	
		.body-message {
			font-size: 10px;
			color: #aeaeae;
		}
	
		.message-box {
			/* padding-top: 20px; */
			font-size: 10px;
			/* text-align: center; */
	
		}
		.div-img img{
			width: 50%;
		}
		.product-body {
			height: calc(20%);
		}
		.fix{
			padding-top: 0.1%;
		}
	}
	@media (max-width: 980px) {
		.about-body{
			margin: 2%;
		}
			.list-product p:first-child{
				font-size: 0.15rem;
				font-weight: bold;
			}
			.list-product p:last-child{
				font-size: 0.09rem;
			}
	        .progress-footer{
		     bottom: calc(30%);
		     font-size: 0.15rem;
	       }
		   .message-box {
			   font-size: 0.15rem;
		   }
	}
	@media (max-width: 700px) {
		.progress-footer {
			font-size: 0.15rem;
		}
		.list-product p:first-child{
			font-size: 0.2rem;
		}
		.list-product p:last-child{
			font-size: 0.1rem;
			display: block;
		}
		.div-img-left {
				width: 50%;
				left: 5%;
			}
		
			
		
			.div-img {
				/* padding: 5px;
				top: calc(28%);
				width: 90%; */
				font-size: 0.41rem;
		
			}
		
			.div-img-right {
				width: 50%;
				left: calc(55%);
			}
		
			.product-list-header {
			/* 	padding: 10px;
				border-bottom: 1px solid #aeaeae;
				list-style: none; */
				/* height: 60px; */
				margin: 0 5%;
			}
		
			.list-product {
				/* float: left;
				padding: 5px;
				width: 33%; */
				font-size: 9px;
			}
		
			
		
			
		
			.main-body {
				/* padding: 2%; */
			}
		
			.footer-fix {
				/* bottom: 0; */
				width: 100%;
				/* height: 100px; */
				
			}
		.footer-bottom{
			background-size: contain;
		}
			.footer-fix p {
				padding-top: 5px;
			}
		
			.btn-about {
				/* border: 1px solid #fff;
				display: inline-block;
				width: auto;
				height: auto; */
				padding: 2%;
			}
		
			.footer-left {
				width: 50%;
				
				
			}
		
			.left-f-fix {
				width: 55%;
				/* position: absolute;
				text-align: center; */
				font-size: 0.1rem;
			}
		
			.footer-right {
				width: 50%;
				
			}
		
			.right-g-fix {
				width: 55%;
				/* position: absolute;
				text-align: center; */
				font-size: 0.1rem;
			}
		
			.about-title {
				text-align: center;
				font-size: 0.2rem;
			}
		
			.about-title b {
				font-size: 0.25rem;
			}
		
			.about-title-small {
				text-align: center;
				font-size: 0.1rem;
			}
		
			.about-title-small::after {
				/* content: "v";
				position: relative;
				bottom: -30px; */
				/* left: calc(-16%); */
			}
		
			/* .about-body {
				background: url(../../assets/about/有阴影.jpg);
				background-size: cover;
				background-repeat: no-repeat;
				padding: 20px;
				padding: 5px;
				margin-top: 8%;
				text-align: center;
				color: #000;
				height: calc(80%);
				width: calc(70%);
				position: relative;
				left: calc(15%);
				overflow: auto;
				-webkit-box-shadow: 0px 0px 12px 0px #aeaeae;
				box-shadow: 0px 0px 12px 0px #aeaeae;
			} */
		
			.progress-footer {
				
				width: 75%;
				font-size: 0.25rem;
				margin: 0 12%;
			}
		
			.div-img img {
				width:75%;
			}
		
			.body-header {
				font-size: 0.25rem;
				font-weight: bold;
			}
		
			.body-message {
				font-size: 0.15rem;
				color: #aeaeae;
			}
		
			.message-box {
				/* padding-top: 20px;
				font-size: 9px;
				text-align: center; */
				top: calc(28%);
				font-size: 0.25rem;
		
			}
		
			.product-body {
				height: calc(20%);
			}
			.list-product p:first-child{
				font-size: 0.2rem;
				font-weight: 500;
			}
			.list-product p:last-child{
				font-size: 0.1rem;
			}
	}

	
</style>
