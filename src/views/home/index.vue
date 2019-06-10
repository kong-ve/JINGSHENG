<template>
	<el-container>
		<el-header class="headerWrapper" style="padding:0;">
			<header class="header" id="header_fix">
				<div class="container">
					<h1>
						<a href="#/home/main" class="router-link-active" @click="hangeChange('first')">
							<img src="../../assets/image/首页-1_01_02.jpg.png" alt="element-logo" class="nav-logo" />
							<img src="../../assets/image/logo.png" alt="element-logo" class="nav-logo-small" style="max-width: 30px;" />
						</a>
					</h1>
					<ul class="nav">
						<li class="nav-item"><a href="#/home/main" :class="{'active':first}" @click="hangeChange('first')">首页</a></li>
						<li class="nav-item"><a href="#/home/about" :class="{'active':two}" @click="hangeChange('two')">关于我们</a></li>
						<!---->
						<li class="nav-item"><a href="#/home/cell" :class="{'active':three}" @click="hangeChange('three')">联系我们</a></li>
						<li class="nav-item nav-versions" style="">
							<h1>
								<a href="#/home/main" class="router-link-active" @click="hangeChange('first')">
									<img src="../../assets/image/首页-1_01_10.jpg.png" alt="element-logo" class="nav-logo" />
									<img src="../../assets/image/首页-1_01_10.jpg.png" alt="element-logo" class="nav-logo-small" />
								</a>
							</h1>
						</li>
					</ul>
				</div>
			</header>
		</el-header>
		<el-main class="main main-cnt" id="main_body" :style="'height:'+cssText+'px;'"  ref="main_body">
			<div style="height:100%;">
				<router-view></router-view>
			</div>
			
		</el-main>
		
		

	</el-container>
</template>

<script>
	import { mapGetters } from 'vuex';
import SidebarItem from './SidebarItem.vue';
import { password } from '../../api/auth/login';
import { getAdminId } from '../../utils/auth';
import { constantRouterMap } from '../../router/index';
export default {
	data() {
		return {
			menuShow: false,
			levelList: null,
			first:true,
			two:false,
			three:false,
			routers: constantRouterMap,
			passwordLoading: false,
			passwordFormVisible: false,
			cssText:document.body.clientHeight-80
		};
	},
	components: {
		SidebarItem
	},
	computed: {
		// ...mapGetters({
		//     routers:"routers"
		// }),

		isCollapse() {
			return this.$store.state.app.sidebar.opened;
		}
	},
	mounted() {
		 window.onresize = function temp() {
			// window.location.reload()
		}
	},
	methods: {
		toggleSideBar() {
			this.$store.dispatch('ToggleSideBar');
		},
		showSideBar() {
			this.$store.dispatch('ShowSideBar');
		},
		hangeChange(id){
			switch(id){
				case 'first':
				this.first = true;
				this.two = false;
				this.three = false;
				break;
				case 'two':
				this.first = false;
				this.two = true;
				this.three = false;
				break;
				case 'three':
				this.first = false;
				this.two = false;
				this.three = true;
				break;
			}
		},
		
	},
	created() {
		
		let a = window.location.href.indexOf('/#/home/');
		let q = window.location.href.substr(0,a+8);
		let x = window.location.href.replace(q,'');
		
		switch(x){
			case 'main':
			this.hangeChange('first');
			break;
			case 'about':
			this.hangeChange('two');
			break;
			case 'cell':
			this.hangeChange('three');
			break;	
		}
	},
	watch: {
	}
};
</script>

<style type="text/scss" lang="scss">
	@import "../../styles/mixin";
	
.headerWrapper {
    height:80px
}.header {
    height:80px;
    background-color:#fff;
    color:#fff;
    top:0;
    left:0;
    width:100%;
    line-height:80px;
    z-index:100;
    position:relative
}.header .container {
    height:100%;
    box-sizing:border-box;
    border-bottom:1px solid #dcdfe6;
}.header .nav-lang-spe {
    color:#888
}.header h1 {
    margin:0;
    float:left;
    font-size:32px;
    font-weight:400;
}.header h1 a {
    color:#333;
    text-decoration:none;
    display:block;
}.header h1 span {
    font-size:12px;
    display:inline-block;
    width:34px;
    height:18px;
    border:1px solid hsla(0, 0%, 100%, .5);
    text-align:center;
    line-height:18px;
    vertical-align:middle;
    margin-left:10px;
    border-radius:3px;
}.header .nav {
    float:right;
    height:100%;
    line-height:80px;
    background:transparent;
    padding:0;
    margin:0;
}
.header .nav:after,
.header .nav:before {
    display:table;
    content:"";
}.header .nav:after {
    clear:both;
}.header .nav-gap {
    position:relative;
    width:1px;
    height:80px;
    padding:0 20px;
}.header .nav-gap:before {
    content:"";
    position:absolute;
    top:calc(50%-8px);
    width:1px;
    height:16px;
    background:#ebebeb;
}
.header .nav-logo-small,
.header .nav-logo {
    vertical-align:sub;
}
.header .nav-logo-small {
    display:none
}.header .nav-item {
    margin:0;
    float:left;
    list-style:none;
    position:relative;
    cursor:pointer;
}.header .nav-item.nav-algolia-search {
    cursor:default
}.header .nav-item.lang-item,
.header .nav-item:last-child {
    cursor:'default';
    margin-left:34px;
}
.header .nav-item.lang-item span,
.header .nav-item:last-child span {
    opacity:.8
}.header .nav-item.lang-item.nav-lang,
.header .nav-item:last-child.nav-lang {
    cursor:pointer;
    display:inline-block;
    height:100%;
    color:#888;
}.header .nav-item.lang-item .nav-lang:hover,
.header .nav-item:last-child .nav-lang:hover {
    color:#409eff;
}.header .nav-item.lang-item .nav-lang.active,
.header .nav-item:last-child .nav-lang.active {
    font-weight:700;
    color:#409eff;
}.header .nav-item a {
    text-decoration:none;
    color:#1989fa;
    opacity:.5;
    display:block;
    padding:0 22px;
}.header .nav-item a.active,
.header .nav-item a:hover {
    opacity:1;
}.header .nav-item a.active:after {
    content:"";
    display:inline-block;
    position:absolute;
    bottom:0;
    left:calc(30%);
    width:30px;
    height:2px;
    background:#409eff;
}.nav-dropdown {
    margin-bottom:6px;
    padding-left:18px;
    width:100%;
}.nav-dropdown span {
    display:block;
    width:100%;
    font-size:16px;
    color:#888;
    line-height:40px;
    transition:.2s;
    padding-bottom:6px;
    user-select:none;
}.nav-dropdown span:hover {
    cursor:pointer
}.nav-dropdown i {
    transition:.2s;
    font-size:12px;
    color:#979797;
    transform:translateY(-2px)
}.nav-dropdown .is-active i,
.nav-dropdown .is-active span {
    color:#409eff
}.nav-dropdown .is-active i {
    transform:rotate(180deg) translateY(3px)
}.nav-dropdown:hover i,
.nav-dropdown:hover span {
    color:#409eff;
}.nav-dropdown-list {
    width:auto
}
@media(max-width:1024px){
	
	.list_logo {
    text-align: right;
    width: 83%;
}
.title {
    font-size: 1rem;
}
}
@media(max-width:850px) {
	.header .nav-logo {
        display:none;
    }.header .nav-logo-small {
        display:inline-block;
    }.header .nav-item {
        margin-left:6px;
    }.header .nav-item .lang-item,
    .header .nav-item:last-child {
        margin-left:10px;
    }.header .nav-item a {
        padding:0 5px;
    }.header .nav-algolia-search,
    .header .nav-theme-switch  {
        display:none
    }
	#app.is-component .main-cnt {
	    padding: 0;
    // height: 848px !important;
	}
	
}
@media(max-width:700px) {
	
	.header .container {
        padding:0 12px
    }.header .nav-item a {
        font-size:12px;
        vertical-align:top
    }.header .nav-item .lang-item {
        height:100%
    }.header .nav-item .lang-item .nav-lang {
        display:flex;
        align-items:center
    }.header .nav-item .lang-item .nav-lang span {
        padding-bottom:0;
    }.header .nav-dropdown {
        padding:0;
    }.header .nav-dropdown span {
        font-size:12px;
    }.header .nav-gap {
        padding:0 8px;
    }.header .nav-versions {
        display:none
    }
	#app.is-component .main-cnt {
	    padding: 0;
	    // margin-top: 10% !important;
	    // height: 651.4px;


	}
	
}

#app.is-component .main-cnt {
    padding: 0;
    margin-top: 80px;
    // height:460px;
}
@media(max-width:1024px) {
.main-cnt::-webkit-scrollbar {
 width: 8px;
}
 .main-cnt::-webkit-scrollbar-track {
 background-color:rgba(0,0,0,0);
 -webkit-border-radius: 1px;
 -moz-border-radius: 1px;
 border-radius:1px;
}
 .main-cnt::-webkit-scrollbar-thumb {
	 background-color:rgba(0,0,0,0.5);
 -webkit-border-radius: 1px;
 -moz-border-radius: 1px;
 border-radius:1px;
}
}
#app.is-component .headerWrapper {
    position: fixed;
    width: 100%;
    left: 0;
    top: 0;
    z-index: 1500;
}
</style>
