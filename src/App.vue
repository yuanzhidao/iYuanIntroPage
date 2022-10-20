<script setup></script>

<template>
	<div class="card-container">
		<div class="header">
			<div class="avatar">
				<img src="https://q4.qlogo.cn/headimg_dl?dst_uin=208823829&spec=640" alt="avatar" />
			</div>
			<div class="info">
				<div class="name">iYuan</div>
				<div class="desc">😊 高一学生、前端小白一枚，未来还请多多指教！</div>
				<div class="navbar">
					<a href="https://y.ezh.ink" target="_blank" rel="noopener noreferrer"><i class="fa-solid fa-newspaper"></i>博客</a>
					<a href="https://iyuanlab.vercel.app/" target="_blank" rel="noopener noreferrer"><i class="fa-solid fa-flask"></i>实验室</a>
					<a href="https://y.ezh.ink/bber" target="_blank" rel="noopener noreferrer"><i class="fa-solid fa-comment-dots"></i>即刻</a>
					<a href="https://y.ezh.ink/about" target="_blank" rel="noopener noreferrer"><i class="fa-solid fa-mug-saucer"></i>关于</a>
				</div>
			</div>
		</div>

		<hr />

		<div class="footer">
			<div class="contact">
				<h2>📮 联系我</h2>
				<ul>
					<li>Email：<a href="mailto:yuan@iyuan.ltd">yuan@iyuan.ltd</a></li>
					<li>Github：<a href="https://github.com/yuanzhidao">@yuanzhidao</a></li>
					<li>QQ：208823829</li>
				</ul>
			</div>
			<div class="project">
				<h2>📦 项目</h2>
				<ul>
					<li><a href="https://mc-docs.vercel.app" target="_blank" rel="noopener noreferrer">Mc-docs：Minecraft 小白快速入门文档</a></li>
					<li>（咕咕咕）</li>
					<li>（咕咕咕）</li>
				</ul>
			</div>
		</div>

		<div class="copyright mt-2 mb-4">
			<p>© 2022 iYuan</p>
			<p><a href="https://beian.miit.gov.cn">沪ICP备2022026478号-3</a></p>
		</div>
	</div>
</template>

<style>
:root {
	--card-box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.5);
	--secondary: #475555;
	--transition: 0.2s ease-in-out;
}

html {
	font-family: "Noto Serif SC", serif;
}

body {
	background-image: url(/assets/img/bg.jpg);
	background-size: cover;
	background-repeat: no-repeat;
	background-position: center;
	background-attachment: fixed;
	height: 100%;
	display: flex;
	align-items: center;
	justify-content: center;
	min-height: 100vh;
	margin: 0;
}

a {
	background-color: transparent;
	color: var(--secondary);
}

a:hover {
	border-radius: 0.5rem;
	background-color: #47555536;
	transition: var(--transition);
}

.card-container {
	display: flex;
	flex-direction: column;
	align-items: center;
	background-color: rgba(255, 255, 255, 0.25);
	backdrop-filter: blur(10px);
	border: 1px solid rgba(255, 255, 255, 0.18);
	box-shadow: rgba(142, 142, 142, 0.19) 0px 6px 15px 0px;
	border-radius: 1.5rem;
	width: 720px;
	height: 27rem;
	background-color: rgba(255, 255, 255, 0.5);
}

.header {
	display: flex;
	flex-direction: row;
	height: 11rem;
	margin-top: 2rem;
	flex-wrap: nowrap;
}

.avatar img {
	max-width: none;
	height: 10rem;
	border-radius: 50%;
}

.avatar {
	border-radius: 50%;
	height: 10rem;
	width: 10rem;
	box-shadow: var(--card-box-shadow);
}

.name {
	margin-top: 0.3rem;
	margin-bottom: 0.7rem;
	font-size: 2.7rem;
	color: #475555;
	font-weight: 700;
}

.info {
	display: flex;
	flex-direction: column;
	margin-left: 4rem;
}

.navbar {
	order: 2;
	padding-top: 1.2rem;
	padding-left: 0.2rem;
	display: flex;
	flex-direction: row;
	justify-content: center;
}

.navbar a {
	text-decoration: none;
	position: relative;
	color: var(--secondary);
	font-size: 1.1rem;
	transition: var(--transition);
	margin: -0.5rem 1rem 0 -0.7rem;
	padding: 0.8rem 0.7rem 0.8rem 0.7rem;
}

.navbar > a > i {
	margin-right: 0.3rem;
}

.navbar a:hover {
	border-radius: 0.8rem;
	background-color: #47555536;
}

hr {
	width: 90%;
	color: rgba(255, 255, 255, 0.5);
	box-sizing: content-box;
	height: 0;
	overflow: visible;
	border: none;
	border-top: 1px solid rgba(80, 80, 80, 0.1);
}

.footer {
	display: flex;
	flex-direction: row;
	flex-wrap: wrap;
	margin-top: 1rem;
}

.footer h2 {
	margin-bottom: 0.5rem;
	font-size: 24px;
	color: #475555;
	font-weight: 600;
}

.footer p {
	margin-left: 0.5rem;
	margin-bottom: -0.5rem;
}

.contact p {
	width: 100%;
}

.project {
	margin-left: 5rem;
}

ul > li {
	margin-bottom: 0.5rem;
	width: 100%;
}

.copyright {
	font-size: 12px;
	color: #475555;
}

@media screen and (max-width: 720px) {
	.card-container {
		width: 95%;
		min-width: 370px;
		height: 100%;
	}
	.header {
		width: 85%;
	}
	.avatar {
		width: auto;
		height: 70%;
	}
	.avatar img {
		height: 100%;
	}
	.info {
		margin-left: 1.5rem;
	}
	.navbar {
		margin-left: -8.5rem;
		margin-right: -0.5rem;
		padding-left: 0;
	}
	.navbar a {
		font-size: 16px;
		margin-right: 0.5rem;
	}
	.name {
		margin-bottom: 0;
	}
	.desc {
		font-size: 14px;
		line-height: 1.5rem;
		margin-bottom: 0.3rem;
	}
	.footer {
		flex-direction: column;
		font-size: 15px;
	}
	.project {
		margin-left: 0;
	}
	h2 {
		font-size: 1.3rem;
	}
	.project h2 {
		margin-top: 0;
	}
}
</style>
