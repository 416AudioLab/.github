<!DOCTYPE html>
<html>
<head>
	<meta charset="UTF-8">
	<title>实验室介绍</title>
	<style>
		/* 样式表 */
		body {
			font-family: Arial, sans-serif;
			margin: 0;
			padding: 0;
		}
		header {
			background-color: #008CBA;
			color: white;
			padding: 20px;
			text-align: center;
		}
		h1 {
			margin: 0;
			font-size: 36px;
		}
		section {
			margin: 20px;
		}
		h2 {
			font-size: 24px;
			margin: 0;
		}
		ul {
			margin: 0;
			padding: 0;
			list-style: none;
		}
		li {
			margin: 5px 0;
		}
		.lang-toggle {
			display: none;
		}
		.lang-toggle.show-cn[data-lang="cn"],
		.lang-toggle.show-en[data-lang="en"] {
			display: block;
		}
	</style>
	<script>
		// 中英文切换
		function toggleLang() {
			var langEl = document.getElementById("lang-toggle");
			var contentEls = document.getElementsByClassName("lang-toggle");
			var lang = langEl.innerText.trim();
			if (lang === "中文") {
				langEl.innerText = "English";
				for (var i = 0; i < contentEls.length; i++) {
					contentEls[i].classList.remove("show-cn");
					contentEls[i].classList.add("show-en");
				}
			} else {
				langEl.innerText = "中文";
				for (var i = 0; i < contentEls.length; i++) {
					contentEls[i].classList.remove("show-en");
					contentEls[i].classList.add("show-cn");
				}
			}
		}
	</script>
</head>
<body>
	<header>
		<h1>实验室名称 / Laboratory Name</h1>
		<button onclick="toggleLang()" id="lang-toggle">English</button>
	</header>
	<main>
		<section>
			<h2>实验室介绍 / Introduction</h2>
			<p class="lang-toggle show-cn" data-lang="cn">我们是一家致力于XX领域的实验室。</p>
			<p class="lang-toggle show-en" data-lang="en">We are a laboratory dedicated to the XX field.</p>
			<p class="lang-toggle show-cn" data-lang="cn">我们通过实验和研究，开发出具有创新性和实用性的科技产品，为人们提供更好的XX体验。</p>
			<p class="lang-toggle show-en" data-lang="en">Through experimentation and research, we develop innovative and practical technology products to provide people with better XX experiences.</p>
		</section>
		<section>
			<h2>研究方向 / Research Areas</h2>
			<ul>
				<li class="lang-toggle show
