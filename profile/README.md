<!DOCTYPE html>
<html>
<head>
	<title>中英文切换示例</title>
	<script>
		function toggleLang() {
			var langEl = document.getElementById("lang-toggle");
			var contentEls = document.getElementsByClassName("lang-toggle");
			if (langEl.innerText === "中文") {
				langEl.innerText = "English";
				for (var i = 0; i < contentEls.length; i++) {
					contentEls[i].innerText = contentEls[i].getAttribute("data-en");
				}
			} else {
				langEl.innerText = "中文";
				for (var i = 0; i < contentEls.length; i++) {
					contentEls[i].innerText = contentEls[i].getAttribute("data-cn");
				}
			}
		}
	</script>
</head>
<body>
	<header>
		<h1>中英文切换示例 / Language Toggle Example</h1>
		<button onclick="toggleLang()" id="lang-toggle">English</button>
	</header>

	<main>
		<section>
			<h2>实验室介绍 / Introduction</h2>
			<p class="lang-toggle" data-cn="我们是一家致力于XX领域的实验室。" data-en="We are a laboratory dedicated to the XX field."></p>
			<p class="lang-toggle" data-cn="我们通过实验和研究，开发出具有创新性和实用性的科技产品，为人们提供更好的XX体验。" data-en="Through experimentation and research, we develop innovative and practical technology products to provide people with better XX experiences."></p>
		</section>

		<section>
			<h2>研究方向 / Research Areas</h2>
			<ul>
				<li class="lang-toggle" data-cn="研究方向1" data-en="Research Area 1"></li>
				<li class="lang-toggle" data-cn="研究方向2" data-en="Research Area 2"></li>
				<li class="lang-toggle" data-cn="研究方向3" data-en="Research Area 3"></li>
				<li class="lang-toggle" data-cn="研究方向4" data-en="Research Area 4"></li>
			</ul>
		</section>

		<section>
			<h2>团队介绍 / Our Team</h2>
			<p class="lang-toggle" data-cn="我们的团队由一群热爱XX领域的专业人士组成，涵盖了XX领域的多个方面。" data-en="Our team consists of a group of professionals who are passionate about the XX field, covering various aspects of XX."></p>
			<p class="lang-toggle" data-cn="我们致力于将最前沿的技术应用于产品开发中，不断创新和进步。" data-en="We are committed to
