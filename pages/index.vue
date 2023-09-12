<template>
  <div>
    <div id="wrapper">

		<!-- Intro -->
		<page-header
			title="Harvard Curling"
			logo="/images/logo.svg"
      logo="/images/Goldline.png"
			intro="We got the brains and brawn. 🥌 <a href='https://www.instagram.com/harvardcurlingteam'>@harvardcurling</a>"
			img="/images/Harvard-Curling-200221-71_web.jpg"
		></page-header>

		<!-- Section -->
		<page-section title="About Us" id="about">
			<div class="content">
				<p><b>Harvard Curling</b> is a university-recognized club sport at Harvard University. We were first established in 2000 and have qualified for every USA College Championship since 2016. Most recently, we placed 4th at the 2022 USA College Curling Championship and the 2017 USA College Curling Championship.</p>

				<span class="image main"><img src="/images/Utica-College-Bonspiel-46_web.jpg" alt="" /></span>

				<p>Our season runs from October through March. During the season, we play local teams and participate in college bonspiels (tournaments) in the Northeast, accumulating points to qualify for the USA College Championship.</p>

				<p>We are always seeking new team members, so <a href="#join" class="scrolly">get in touch</a> if you are interested in curling with us. We welcome both brand new curlers and experienced curlers looking for more serious competition. Harvard Curling is open to all Harvard students. No experience is necessary to join — we’ll teach you how to curl. We practice and play at Broomstones Curling Club on Fridays from 4:00-6:00. We have transportation available, but if you have access to a car, this would also be a great help for carpooling.</p>

				<p>The club was originally established in 2000, and although it has waxed and waned through the years, we're looking forward to another 20 years of curling.</p>
			</div>
		</page-section>

		<!-- Section -->
		<!-- <section id="who">
			<header>
				<h2>Who We Are</h2>
			</header>
			<div class="content">
				<p><strong>IDK</strong> Something about who the people on the team are? Or we could just get rid of this section.</p>
				<ul class="feature-icons">
					<li class="icon solid fa-laptop">Consequat tempus</li>
					<li class="icon solid fa-bolt">Etiam adipiscing</li>
					<li class="icon solid fa-signal">Libero nullam</li>
					<li class="icon solid fa-cog">Blandit condimentum</li>
					<li class="icon solid fa-map-marker-alt">Lorem ipsum dolor</li>
					<li class="icon solid fa-code">Nibh amet venenatis</li>
				</ul>
			</div>
		</section> -->

		<page-section id="news" title="News Coverage">
			<div>
				<news
					title="Harvard Curling Club: From Learn-To-Curl to Nationals"
					link="https://www.thecrimson.com/article/2019/3/6/curling-club/"
					source="Harvard Crimson, March 2019"
					img="/images/crimson-img.jpg"
					alt="Harvard Crimson preview"
				></news>

				<news
					title="As curling grows, it finds a new target: college campuses"
					link="https://apnews.com/766049c592ea446b9e204613d132416d"
					source="AP News, March 2019"
					img="/images/ap-news-img.jpg"
					alt="AP News preview"
				></news>

				<news
					title="To compete, they let it slide"
					link="https://news.harvard.edu/gazette/story/2018/02/brooms-at-the-ready-harvards-curling-team-takes-to-the-ice/"
					source="Harvard Gazette, February 2018"
					video="https://www.youtube.com/embed/N988Kltkk0M"
				></news>
			</div>
		</page-section>

		<!-- Section -->
		<section id="photos">
			<header>
				<h2>Photos</h2>
			</header>
			<div class="content">
				<gallery
					:images="{
						'2018 Nationals in Wisconsin': '/images/1718_nationals_cheese_1-1.jpg',
						'Jack Cordes making faces': '/images/Utica-College-Bonspiel-138_web-1.jpg',
						'Lara Teich and Kristin Kiley making faces': '/images/Utica-College-Bonspiel-223_web-1.jpg',
						'Learn to curl event': '/images/1819_firstpractice_22-1.jpg'
					}"
					:orientations="['landscape', 'portrait', 'portrait', 'landscape']"
				></gallery>

				<!-- Section -->
				<page-section id="insta"
					title="Instagram"
					description="See the latest feed of what the team is up to."
					is-subsection>
					<!-- <header>
						<h3>Instagram</h3>
						<p>See the latest feed of what the team is up to.</p>
					</header> -->
					<div>
						<script src="https://assets.juicer.io/embed.js" type="text/javascript"></script>
						<link href="https://assets.juicer.io/embed.css" media="all" rel="stylesheet" type="text/css" />
						<ul class="juicer-feed"
							data-feed-id="pterosaur"
							data-per="9"
							data-gutter="15"
							data-pages="1"
							data-style="image-grid">
						</ul>
						<!-- Configuration: https://help.juicer.io/en/articles/2154872-code-customizations-for-date-range-feed-style-spacing-filtering-and-more -->
					</div>
				</page-section>

			</div>
		</section>

		<!-- Section -->
		<page-section title="Join the Team" id="join">
			<div class="content">
				<p>Interested in joining the Harvard curling team? Students in all Harvard schools are eligible to join, including the College, GSAS, HLS, HBS, etc.</p>
				<p>No experience is necessary! We host learn-to-curl events, and we will provide all of the necessary equipment and transportation. We're committed to getting new players involved, so you'll be able to play in tournaments as soon as you join.</p>
				<h3>Email us:</h3>
				<ul class="actions">
					<li><a href="mailto:harvardcurling@gmail.com" class="button primary large">harvardcurling@gmail.com</a></li>
				</ul>
			</div>
			<div slot="footer">
				<footer-links>
					<f-link
						:links="{'mailto:harvardcurling@gmail.com': 'harvardcurling@gmail.com'}"
					>Email</f-link>
					<f-link
						:links="{
							'http://collegecurlingusa.org/': 'College Curling USA',
							'https://recreation.gocrimson.com/recreation/club_sports/Club_Sports_Program': 'Harvard Club Sports'
							}"
					>Links</f-link>
					<f-link
						:social-links="{
							'twitter': 'https://twitter.com/harvardcurling/',
							'facebook-f': 'https://www.facebook.com/HarvardCurling/',
							'instagram': 'https://www.instagram.com/harvardcurling/'
						}"
					>Social Media</f-link>
				</footer-links>
			</div>
		</page-section>

		<!-- Copyright -->
		<div class="copyright">&copy; Harvard Curling Club. All rights reserved. Design: <a href="https://html5up.net">HTML5 UP</a>.</div>

	</div>

	<!-- Scripts -->
	<script src="/js/jquery.min.js"></script>
	<script src="/js/jquery.scrolly.min.js"></script>
	<script src="/js/browser.min.js"></script>
	<script src="/js/breakpoints.min.js"></script>
	<script src="/js/util.js"></script>
	<script src="/js/main.js"></script>

  </div>
</template>

<script>
import PageHeader from "~/components/PageHeader.vue";
import PageSection from "~/components/PageSection.vue";
import News from "~/components/News.vue";
import Gallery from "~/components/Gallery.vue";
import FooterLinks from "~/components/FooterLinks.vue";
import FLink from "~/components/FLink.vue";

export default {
  components: {
    PageHeader,
    PageSection,
    News,
    Gallery,
    FooterLinks,
    FLink
  }
};
</script>

<style>
</style>
