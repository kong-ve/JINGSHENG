<template>
	<div class="mains">
		<div class="main-body">
			<div class="about-title"><b>profession</b>秉持专业价值</div>
			<div class="about-title-small">互相激励 梦想路上你我同行</div>
			<div class="about-body">
				<div class="body-header">京盛时代概况</div>
				<div class="body-message">jing sheng profile</div>
				<div class="message-box">
					京盛时代（北京）新媒体科技有限公司（简称：京盛时代），
					2011年6月创办于北京。是一家专注于为企业在
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
									<div class="message-box fix"><span>等方面提供一站式解决方案的新型科技公司。目前在上海、深圳、江西、苏州等地均设立分公司。</span></div>
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
		</div>
		<div class="footer-fix">
			<div class="footer-left">
				<div class="left-f-fix">
					<div class="btn-about">联系我们</div>
					<p>如有什么建议 欢迎联系我们</p>
				</div>
			</div>
			<div class="footer-right">
				<div class="right-g-fix">
					<div class="btn-about">欢迎入驻</div>
					<p>人才服务平台邀您入驻</p>
				</div>
			</div>
			
		</div>
		<el-footer class="footer-bottom" id="footer-fix" height="80px" >
		</el-footer>
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
		width: 35%;
    float: left;
    position: absolute;
    top: calc(39%);
    left: calc(15%);
	}

	.fix {
		position: absolute;
    top: calc(40%);
    left: calc(17%);
	}

	.div-img {
		height: calc(80%);
    padding: 25px;
    position: absolute;
    top: calc(16%);
	width: 80%;
	
	}

	.div-img-right {
		width: 35%;
    float: right;
    position: absolute;
    right: calc(8%);
	top: calc(39%);
	}

	.product-list-header {
		padding: 10px;
		border-bottom: 1px solid #aeaeae;
		list-style: none;
		height: 100px;
		margin: 0 5%;
	}

	.list-product {
		float: left;
		padding: 30px;
		width: 30%;
	}

	.list-product:not(:last-child)::after {
		content: "";
		display: inline-block;
		position: absolute;
		top: calc(23%);
		left: calc(33%);
		width: 1px;
		height: 46px;
		background: #aeaeae;
	}
	
	.list-product:not(:last-child):not(:first-child)::after {
		content: "";
		display: inline-block;
		position: absolute;
		top: calc(23%);
		left: calc(60%);
		width: 1px;
		height: 46px;
		background: #aeaeae;
	}

	.main-body {
		padding: 0.5%;
		height: 100%;
	}

	.footer-fix {
		position: relative;
		bottom: 0;
		width: 100%;
		height: 135px;
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
		background: url(../../assets/about/关于我们2_09.jpg.png);
		background-size: cover;
		background-repeat: no-repeat;
		height: 100%;
		float: left;
		position: relative;
	}

	.left-f-fix {
		width: 30%;
		position: absolute;
		right: 150px;
		top: 65px;
		text-align: center;
		font-size: x-small;
	}

	.footer-right {
		width: 50%;
		background: url(../../assets/about/关于我们2_10.jpg.png);
		background-size: cover;
		background-repeat: no-repeat;
		height: 100%;
		float: right;
		position: relative;
	}

	.right-g-fix {
		width: 30%;
		position: absolute;
		left: 145px;
		top: 65px;
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
		position: relative;
		bottom: -30px;
		left: calc(-5%);
	}

	.about-body {
		background: url(../../assets/about/有阴影.jpg);
		background-size: cover;
		background-repeat: no-repeat;
		padding: 20px;
		margin-top: 2%;
		text-align: center;
		color: #000;
		height: calc(80%);
		width: calc(70%);
		position: relative;
		left: calc(15%);
		overflow: hidden;
		box-shadow: 0px 0px 12px 0px #aeaeae;
	}

	.progress-footer {
		padding-bottom: 30px;
		position: absolute;
		left: calc(8%);
		bottom: calc(2%);
		text-align: center;
		width: 80%;
		font-size: 0.3rem;
	}

	.div-img img {
		width: 80%;
	}

	.body-header {
		font-size: 0.5rem;
		font-weight: bold;
	}

	.body-message {
		font-size: 0.3rem;
		color: #aeaeae;
	}

	.message-box {
		padding-top: 5px;
		font-size: 0.3rem;
		text-align: center;

	}

	.product-body {
		height: calc(20%);
	}
	.list-product p:first-child{
		font-size: 0.5rem;
	}
	.list-product p:last-child{
		font-size: 0.2rem;
	}
	@media (min-width:980px) {
		.list-product:not(:last-child)::after {
			
			top: calc(23%);
			
		}
				
		.list-product:not(:last-child):not(:first-child)::after {
			
			top: calc(23%);
			
		}
	}
	@media (max-width:1425px) {
		.list-product p:first-child{
			font-size: 0.2rem;
		}
		.list-product p:last-child{
			font-size: 0.05rem;
			display: block;
		}
		.div-img-left {
				width: 50%;
				float: left;
				position: absolute;
				left: 15%;
				top: calc(65%);
			}
		
			.fix {
				position: absolute;
				bottom: 170px;
				left: calc(8%);
				width: 81%;
			}
		
			.div-img {
				height: calc(30%);
				padding: 5px;
				top: calc(15%);
				position: absolute;
				width: 80%;
				font-size: 0.25em;
		
			}
		
			.div-img-right {
				width: 50%;
				float: right;
				position: absolute;
				right: calc(-15%);
				top: calc(65%);
			}
		
			.product-list-header {
				padding: 10px;
				border-bottom: 1px solid #aeaeae;
				list-style: none;
				height: 100px;
				margin: 0 5%;
			}
		
			.list-product {
				float: left;
				padding: 5px;
				width: 33%;
				font-size: 0.05rem;
			}
		
			
		
			.list-product:not(:last-child)::after {
				content: "";
				display: inline-block;
				position: absolute;
				top: calc(19%);
				left: calc(35%);
				width: 1px;
				height: 36px;
				background: #aeaeae;
			}
		
			.list-product:not(:last-child):not(:first-child)::after {
				content: "";
				display: inline-block;
				position: absolute;
				top: calc(19%);
				left: calc(65%);
				width: 1px;
				height: 36px;
				background: #aeaeae;
			}
		
			.main-body {
				padding: 2%;
			}
		
			.footer-fix {
				position: relative;
				bottom: 0;
				width: 100%;
				height: 100px;
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
				background: url(../../assets/about/关于我们2_09.jpg.png);
				background-size: cover;
				background-repeat: no-repeat;
				height: 100%;
				float: left;
				position: relative;
			}
		
			.left-f-fix {
				width: 35%;
				position: absolute;
				right: 82px;
				top: 37px;
				text-align: center;
				font-size: x-small;
			}
		
			.footer-right {
				width: 50%;
				background: url(../../assets/about/关于我们2_10.jpg.png);
				background-size: cover;
				background-repeat: no-repeat;
				height: 100%;
				float: right;
				position: relative;
			}
		
			.right-g-fix {
				width: 35%;
				position: absolute;
				left: 95px;
				top: 37px;
				text-align: center;
				font-size: x-small;
			}
		
			.about-title {
				text-align: center;
				font-size: large;
			}
		
			.about-title b {
				font-size: x-large;
			}
		
			.about-title-small {
				text-align: center;
			}
		
			.about-title-small::after {
				content: "v";
				position: relative;
				bottom: -30px;
				left: calc(-16%);
			}
		
			.about-body {
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
			}
		
			.progress-footer {
				padding-bottom: 30px;
				position: absolute;
				left: calc(5%);
				bottom: calc(10%);
				text-align: center;
				width: 90%;
			}
		
			.div-img img {
				width: 80%;
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
				padding-top: 20px;
				font-size: 0.3rem;
				text-align: center;
				top: calc(25%);
		
			}
		
			.product-body {
				height: calc(58%);
			}
	}
	@media (max-width: 1319px) {
		.div-img-left {
			width: 50%;
			float: left;
			position: absolute;
			left: 5%;
			top: calc(66%);
		}
	
		.fix {
			position: absolute;
			bottom: 170px;
			left: calc(8%);
			width: 81%;
		}
	
		.div-img {
			height: calc(22%);
			padding: 5px;
			top: calc(23%);
			position: absolute;
			width: 90%;
	
		}
	
		.div-img-right {
			width: 50%;
			float: right;
			position: absolute;
			left: calc(55%);
			top: calc(65%);
		}
	
		.product-list-header {
			padding: 10px;
			border-bottom: 1px solid #aeaeae;
			list-style: none;
			height: 60px;
			margin: 0 5%;
		}
	
		.list-product {
			float: left;
			padding: 5px;
			width: 33%;
			font-size: 0.05rem;
			height: 100%;
		}
	
		
	
		.list-product:not(:last-child)::after {
			content: "";
			display: inline-block;
			position: absolute;
			top: calc(19%);
			left: calc(35%);
			width: 1px;
			height: 36px;
			background: #aeaeae;
		}
	
		.list-product:not(:last-child):not(:first-child)::after {
			content: "";
			display: inline-block;
			position: absolute;
			top: calc(19%);
			left: calc(65%);
			width: 1px;
			height: 36px;
			background: #aeaeae;
		}
	
		.main-body {
			padding: 2%;
		}
	
		.footer-fix {
			position: relative;
			bottom: 0;
			width: 100%;
			height: 100px;
			
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
			background: url(../../assets/about/关于我们2_09.jpg.png);
			background-size: cover;
			background-repeat: no-repeat;
			height: 100%;
			float: left;
			position: relative;
		}
	
		.left-f-fix {
			width: 35%;
			position: relative;
			right: 82px;
			top: 37px;
			text-align: center;
			font-size: x-small;
		}
	
		.footer-right {
			width: 50%;
			background: url(../../assets/about/关于我们2_10.jpg.png);
			background-size: cover;
			background-repeat: no-repeat;
			height: 100%;
			float: right;
			position: relative;
		}
	
		.right-g-fix {
			width: 35%;
			position: absolute;
			left: 95px;
			top: 37px;
			text-align: center;
			font-size: x-small;
		}
	
		.about-title {
			text-align: center;
			font-size: large;
		}
	
		.about-title b {
			font-size: x-large;
		}
	
		.about-title-small {
			text-align: center;
		}
	
		.about-title-small::after {
			content: "v";
			position: relative;
			bottom: -30px;
			left: calc(-16%);
		}
	
		.about-body {
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
		}
	
		.progress-footer {
			padding-bottom: 30px;
			position: absolute;
			left: calc(8%);
			bottom: calc(8%);
			text-align: center;
			width: 80%;
		}
	
		.div-img img {
			width: 80%;
		}
	
		.body-header {
			font-size: large;
			font-weight: bold;
		}
	
		.body-message {
			font-size: xx-small;
			color: #aeaeae;
		}
	
		.message-box {
			padding-top: 20px;
			font-size: 0.25rem;
			text-align: center;
	
		}
	
		.product-body {
			height: calc(20%);
		}
	}
	
	@media (max-width: 700px) {
		.list-product p:first-child{
			font-size: 0.2rem;
		}
		.list-product p:last-child{
			font-size: 0.05rem;
			display: block;
		}
		.div-img-left {
				width: 50%;
				float: left;
				position: absolute;
				left: 5%;
				top: calc(66%);
			}
		
			.fix {
				position: absolute;
				top: calc(25%);
				left: calc(8%);
				width: 81%;
			}
		
			.div-img {
				height: calc(22%);
				padding: 5px;
				top: calc(28%);
				position: absolute;
				width: 90%;
				font-size: 0.41rem;
		
			}
		
			.div-img-right {
				width: 50%;
				float: right;
				position: absolute;
				left: calc(55%);
				top: calc(65%);
			}
		
			.product-list-header {
				padding: 10px;
				border-bottom: 1px solid #aeaeae;
				list-style: none;
				height: 60px;
				margin: 0 5%;
			}
		
			.list-product {
				float: left;
				padding: 5px;
				width: 33%;
				font-size: 0.05rem;
			}
		
			
		
			.list-product:not(:last-child)::after {
				content: "";
				display: inline-block;
				position: absolute;
				top: calc(19%);
				left: calc(35%);
				width: 1px;
				height: 36px;
				background: #aeaeae;
			}
		
			.list-product:not(:last-child):not(:first-child)::after {
				content: "";
				display: inline-block;
				position: absolute;
				top: calc(19%);
				left: calc(65%);
				width: 1px;
				height: 36px;
				background: #aeaeae;
			}
		
			.main-body {
				padding: 2%;
			}
		
			.footer-fix {
				position: relative;
				bottom: 0;
				width: 100%;
				height: 100px;
				
			}
		.footer-bottom{
			background-size: contain;
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
				background: url(../../assets/about/关于我们2_09.jpg.png);
				background-size: cover;
				background-repeat: no-repeat;
				height: 100%;
				float: left;
				position: relative;
			}
		
			.left-f-fix {
				width: 35%;
				position: absolute;
				right: 82px;
				top: 37px;
				text-align: center;
				font-size: x-small;
			}
		
			.footer-right {
				width: 50%;
				background: url(../../assets/about/关于我们2_10.jpg.png);
				background-size: cover;
				background-repeat: no-repeat;
				height: 100%;
				float: right;
				position: relative;
			}
		
			.right-g-fix {
				width: 35%;
				position: absolute;
				left: 95px;
				top: 37px;
				text-align: center;
				font-size: x-small;
			}
		
			.about-title {
				text-align: center;
				font-size: large;
			}
		
			.about-title b {
				font-size: x-large;
			}
		
			.about-title-small {
				text-align: center;
			}
		
			.about-title-small::after {
				content: "v";
				position: relative;
				bottom: -30px;
				left: calc(-16%);
			}
		
			.about-body {
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
			}
		
			.progress-footer {
				padding-bottom: 30px;
				position: absolute;
				left: calc(5%);
				bottom: calc(6%);
				text-align: center;
				width: 90%;
			}
		
			.div-img img {
				width: 80%;
			}
		
			.body-header {
				font-size: large;
				font-weight: bold;
			}
		
			.body-message {
				font-size: xx-small;
				color: #aeaeae;
			}
		
			.message-box {
				padding-top: 20px;
				font-size: 0.2rem;
				text-align: center;
				top: calc(28%);
		
			}
		
			.product-body {
				height: calc(20%);
			}
	}

	
</style>
