---
title: "Home"
layout: homelay
sitemap: false
permalink: /
---

<style>
html, body {
  margin: 0;
  padding: 0;
}
#homeid {
  flex: 0 0 100%;
  max-width: 100%;
  width: 100%;
  padding-left: 0;
  padding-right: 0;
}
/* ===== Your existing image layout ===== */
.container {
  text-align: center; /* 使容器内的所有内容居中显示 */
  margin-bottom: 0px; /* 底部空间 */
}
.navbar,
.navbar.sticky-top {
  position: absolute !important;
  top: 0;
  left: 0;
  right: 0;
  width: 100%;
  background-color: transparent !important;
  border: none !important;
  box-shadow: none !important;
  z-index: 10;
  padding: 12px 24px !important;
}
.navbar-brand {
  font-size: 1.8rem;
  font-weight: 700;
}
.navbar-brand-title {
  font-size: 1.4rem;
  font-weight: 700;
}
.navbar-toggler {
  border-color: rgba(255,255,255,0.7) !important;
}
.navbar-dark .navbar-nav .nav-link,
.navbar-dark .navbar-brand,
.navbar-brand-title {
  color: #ffffff !important;
  font-size: 1.05rem;
}
.page-hero {
  position: relative;
  left: 50%;
  right: 50%;
  margin-left: -50vw;
  margin-right: -50vw;
  width: 100vw;
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  background-image: url('{{ site.url }}{{ site.baseurl }}/images/vibration.webp');
  background-size: cover;
  background-position: center;
  background-attachment: scroll;
  color: #ffffff;
  overflow: hidden;
}
@media (max-width: 767px) {
  .page-hero {
    background-image: url('{{ '/images/vibration-small.webp' | relative_url }}');
  }
}
.page-hero::before {
  content: '';
  position: absolute;
  inset: 0;
  background: linear-gradient(180deg, rgba(2, 23, 82, 0.32), rgba(2, 23, 82, 0.45));
}
.page-hero-inner {
  position: relative;
  z-index: 1;
  width: 100%;
  max-width: 980px;
  padding: 40px 28px;
  text-align: center;
}
.page-hero-logo {
  display: block;
  margin-bottom: 1.2rem;
  letter-spacing: 0.26em;
  text-transform: uppercase;
  color: #a5d8ff;
  font-weight: 700;
  font-size: 0.95rem;
}
.page-hero-title {
  margin: 0;
  font-size: clamp(3rem, 6vw, 5.2rem);
  line-height: 0.98;
}
.page-hero-copy {
  margin: 24px auto 0;
  max-width: 760px;
  font-size: clamp(1rem, 1.15vw, 1.35rem);
  line-height: 1.75;
  color: rgba(255,255,255,0.92);
}
.page-hero-note {
  margin-top: 26px;
  font-size: 0.95rem;
  color: rgba(255,255,255,0.75);
}
.welcome-frame {
  width: 100%;
  margin: 0 auto 20px auto;
  overflow: hidden;
}
.welcome-img {
  width: 100%;
  height: 500px;
  object-fit: contain;
  display: block;
}
.image-item {
  display: inline-block; /* 使图片和文本并排显示，根据内容自动调整宽度 */
  margin: 0 10px; /* 图片之间的间距 */
  vertical-align: top; /* 确保图片顶部对齐 */
}
.image-caption {
  display: block; /* 确保描述文字在图片下方 */
  margin-top: -10px; /* 图片与文字间的距离 */
}

/* ===== Featured carousel ===== */
.featured-carousel {
  position: relative;
  width: 100%;
  max-width: 1240px;
  margin: 28px auto;
  padding: 0 20px;
  box-sizing: border-box;
}

.fc-viewport {
  overflow: hidden;
  width: 100%;
  border-radius: 0;
  box-shadow: none;
  border: 1px solid rgba(0,0,0,0.08);
}

.fc-track {
  display: flex;
  transition: transform 450ms ease;
  will-change: transform;
}

.fc-slide {
  min-width: 100%;
  box-sizing: border-box;
  padding: 0 10px;
}

.fc-slide h5 {
  margin: 0 0 12px;
  font-size: 1rem;
  line-height: 1.5;
  color: #111;
}

.fc-slide p {
  margin: 6px 0;
}

.fc-img {
  width: 100%;
  height: 500px;
  object-fit: contain;
  padding: 8px;
  border-radius: 6px;
}

.fc-dots {
  display: flex;
  gap: 10px;
  justify-content: center;
  margin-top: 14px;
}

.fc-dot {
  width: 10px;
  height: 10px;
  border-radius: 999px;
  background: rgba(255,255,255,0.9);
  border: 1px solid rgba(0,0,0,0.08);
  cursor: pointer;
  transition: transform 180ms ease, background-color 180ms ease;
}

.fc-dot.is-active {
  background: #1a73e8;
  transform: scale(1.15);
}

/* Full-screen homepage hero inspired by lab landing pages. */
.navbar,
.navbar.sticky-top {
  position: absolute !important;
  top: 0;
  left: 50%;
  right: auto;
  transform: translateX(-50%);
  z-index: 20;
  width: min(92vw, 1320px);
  min-height: 74px;
  padding: 10px 44px !important;
  background-color: transparent !important;
  border: 0 !important;
  box-shadow: none !important;
}
.navbar .container-fluid {
  align-items: center;
  gap: 14px;
}
.navbar-brand {
  margin-right: 0;
  padding: 0;
  line-height: 1;
}
.navbar-brand img {
  width: 42px;
  height: 42px;
}
.navbar-brand-title {
  color: #fff !important;
  flex: 0 1 auto;
  font-size: 1.08rem;
  font-weight: 700;
  letter-spacing: 0.02em;
  line-height: 1.2;
  text-shadow: 0 2px 14px rgba(0, 0, 0, 0.42);
}
.navbar-collapse {
  justify-content: flex-end;
}
.navbar-dark .navbar-nav .nav-link,
.navbar-dark .navbar-brand {
  color: #fff !important;
  text-shadow: 0 2px 14px rgba(0, 0, 0, 0.45);
}
.navbar-dark .navbar-nav .nav-link {
  padding: 0.35rem 0.72rem;
  font-size: 0.96rem;
}
.navbar .navbar-collapse.show,
.navbar .navbar-collapse.collapsing {
  margin-top: 12px;
  padding: 12px 16px;
  background: rgba(4, 21, 38, 0.76);
  backdrop-filter: blur(8px);
}
.page-hero {
  flex: 0 0 100%;
  height: 100vh;
  min-height: 640px;
  background-size: cover;
  background-position: center;
}
.page-hero::before {
  background:
    linear-gradient(180deg, rgba(0, 0, 0, 0.20) 0%, rgba(0, 0, 0, 0.18) 34%, rgba(0, 0, 0, 0.52) 100%),
    linear-gradient(90deg, rgba(7, 31, 48, 0.42), rgba(7, 31, 48, 0.12), rgba(7, 31, 48, 0.42));
}
.page-hero-inner {
  max-width: 1080px;
  padding: 118px 32px 72px;
}
.page-hero-logo {
  margin-bottom: 1.35rem;
  color: rgba(255, 255, 255, 0.88);
  font-size: 0.9rem;
  text-shadow: 0 2px 16px rgba(0, 0, 0, 0.45);
}
.page-hero-title {
  font-size: clamp(2.8rem, 5.7vw, 5.8rem);
  line-height: 1.04;
  font-weight: 800;
  text-shadow: 0 4px 24px rgba(0, 0, 0, 0.48);
}
.page-hero-copy {
  max-width: 840px;
  font-size: 1.18rem;
  text-shadow: 0 2px 16px rgba(0, 0, 0, 0.42);
}
.page-hero-note {
  letter-spacing: 0.16em;
  text-transform: uppercase;
  text-shadow: 0 2px 16px rgba(0, 0, 0, 0.42);
}
.home-white {
  flex: 0 0 100%;
  position: relative;
  left: auto;
  right: auto;
  width: 100%;
  margin-left: 0;
  margin-right: 0;
  background: #fff;
  color: #111;
  display: block;
}
.home-section {
  max-width: 1240px;
  margin: 0 auto;
  padding: 64px 24px 18px;
}
.home-section-title {
  margin: 0 0 26px;
  color: #111;
  font-size: 2rem;
  font-weight: 750;
  line-height: 1.2;
  text-align: left;
}
.news-section {
  max-width: 1240px;
  margin: 0 auto;
  padding: 40px 24px 28px;
  text-align: left;
}
.news-section h3 {
  margin-bottom: 22px;
}
.featured-carousel {
  margin: 0 auto;
  padding: 0;
}
.fc-viewport {
  border-top: 1px solid rgba(0, 0, 0, 0.10);
  border-right: 0;
  border-bottom: 1px solid rgba(0, 0, 0, 0.10);
  border-left: 0;
}
.fc-slide {
  padding: 0;
}
.fc-slide h5 {
  margin: 0 0 18px;
  font-size: 1.04rem;
  text-align: left;
}
.fc-img {
  height: min(52vw, 560px);
  min-height: 340px;
  border-radius: 0;
}
@media (max-width: 767px) {
  .navbar,
  .navbar.sticky-top {
    width: calc(100vw - 24px);
    min-height: 64px;
    padding: 10px 18px !important;
  }
  .navbar .container-fluid {
    gap: 10px;
  }
  .navbar-brand img {
    width: 36px;
    height: 36px;
  }
  .navbar-brand-title {
    max-width: calc(100vw - 150px);
    font-size: 0.9rem;
    line-height: 1.25;
  }
  .page-hero {
    min-height: 620px;
  }
  .page-hero-inner {
    padding: 104px 22px 60px;
  }
  .page-hero-logo {
    letter-spacing: 0.16em;
    font-size: 0.78rem;
  }
  .page-hero-copy {
    font-size: 1rem;
  }
  .home-section {
    padding-top: 42px;
  }
  .home-section-title {
    font-size: 1.65rem;
  }
  .fc-img {
    height: 360px;
    min-height: 300px;
  }
}

/* Final homepage layout reset. Keep the hero stable inside Bootstrap rows. */
body {
  overflow-x: hidden;
}
body > .container-fluid {
  width: 100% !important;
  max-width: none !important;
  margin: 0 !important;
  padding: 0 !important;
}
.container-fluid > .row {
  --bs-gutter-x: 0;
  width: 100% !important;
  max-width: none !important;
  margin-left: 0;
  margin-right: 0;
}
#homeid {
  display: block !important;
  flex: 0 0 100% !important;
  max-width: 100% !important;
  width: 100% !important;
  margin: 0 !important;
  padding: 0 !important;
}
.navbar,
.navbar.sticky-top {
  position: absolute !important;
  top: 0 !important;
  left: 0 !important;
  right: 0 !important;
  transform: none !important;
  width: 100% !important;
  max-width: none !important;
  min-height: 0 !important;
  padding: 0 !important;
  background: transparent !important;
  border: 0 !important;
  box-shadow: none !important;
  z-index: 50;
}
.navbar > .container-fluid {
  width: min(88vw, 1780px);
  max-width: none !important;
  margin: 0 auto;
  padding: 34px 0 0;
  display: flex;
  align-items: center;
  gap: 26px;
}
.navbar-brand {
  flex: 0 0 auto;
  margin: 0;
  padding: 0;
}
.navbar-brand img {
  width: 58px;
  height: 58px;
}
.navbar-brand-title {
  flex: 0 0 auto;
  margin-right: 34px;
  color: #fff !important;
  font-size: 1.2rem !important;
  font-weight: 700;
  line-height: 1.15;
  text-shadow: 0 2px 14px rgba(0, 0, 0, 0.45);
}
.navbar-collapse {
  flex-grow: 1;
  justify-content: flex-end;
}
.navbar-nav {
  width: 100%;
  justify-content: space-between;
  gap: 18px;
}
.navbar-dark .navbar-nav .nav-link {
  color: #fff !important;
  padding: 0;
  font-size: 1.24rem;
  font-weight: 500;
  letter-spacing: 0.03em;
  text-shadow: 0 2px 14px rgba(0, 0, 0, 0.45);
  white-space: nowrap;
}
.page-hero {
  left: auto !important;
  right: auto !important;
  width: 100vw !important;
  height: 100vh;
  min-height: 720px;
  margin-left: calc(50% - 50vw) !important;
  margin-right: calc(50% - 50vw) !important;
  background-size: cover;
  background-position: center center;
}
.page-hero::before {
  background:
    linear-gradient(90deg, rgba(22, 58, 88, 0.72), rgba(24, 76, 90, 0.58)),
    linear-gradient(180deg, rgba(16, 42, 70, 0.20), rgba(16, 42, 70, 0.50));
}
.page-hero-inner {
  max-width: min(88vw, 1320px);
  padding: 140px 0 88px;
}
.page-hero-title {
  font-size: clamp(3.2rem, 5.2vw, 5.4rem);
  line-height: 1.08;
  letter-spacing: 0;
}
.page-hero-copy {
  max-width: 1180px;
  font-size: clamp(1.35rem, 2vw, 1.95rem);
  line-height: 1.55;
}
.page-hero-note {
  margin-top: 74px;
  font-size: 0.9rem;
}
.home-white {
  width: 100vw !important;
  margin-left: calc(50% - 50vw) !important;
  margin-right: calc(50% - 50vw) !important;
  padding: 0;
  background: #fff;
}
.home-section,
.news-section {
  width: min(88vw, 1240px);
  max-width: none;
  margin: 0 auto;
}
.home-section {
  padding: 68px 0 20px;
}
.news-section {
  padding: 38px 0 36px;
}
@media (max-width: 991px) {
  .navbar > .container-fluid {
    width: calc(100vw - 32px);
    padding-top: 18px;
  }
  .navbar-brand img {
    width: 42px;
    height: 42px;
  }
  .navbar-brand-title {
    max-width: calc(100vw - 150px);
    margin-right: 0;
    font-size: 0.92rem !important;
  }
  .navbar-nav {
    gap: 0;
  }
  .navbar .navbar-collapse.show,
  .navbar .navbar-collapse.collapsing {
    margin-top: 12px;
    padding: 14px;
    background: rgba(15, 42, 62, 0.86);
  }
  .page-hero {
    min-height: 640px;
  }
  .page-hero-inner {
    max-width: calc(100vw - 44px);
    padding: 112px 0 70px;
  }
  .home-section,
  .news-section {
    width: calc(100vw - 36px);
  }
}

/* Keep the shared navbar style on the homepage too. */
.site-navbar,
.site-navbar.sticky-top {
  position: absolute !important;
  top: 0 !important;
  left: auto !important;
  right: auto !important;
  transform: none !important;
  width: 100% !important;
  max-width: none !important;
  min-height: 0 !important;
  margin-bottom: 0 !important;
  padding: 22px 0 18px !important;
  background: transparent !important;
  border-bottom: 1px solid rgba(255, 255, 255, 0.18) !important;
  box-shadow: none !important;
  z-index: 50;
}

.site-navbar > .container-fluid {
  width: min(92vw, 1480px) !important;
  max-width: none !important;
  margin-right: auto !important;
  margin-left: auto !important;
  padding: 0 !important;
  gap: 30px;
}

.site-navbar-logos {
  gap: 16px;
}

/* Home navbar logo tuning. Adjust icon size and offset here. */
.site-navbar-logo-hkust {
  width: 230px !important;
  height: 70px !important;
}

.site-navbar-logo-sms {
  width: 300px !important;
  height: 80px !important;
  transform: translate(8px, 5px) !important;
}

.site-navbar .navbar-nav {
  justify-content: flex-end;
  gap: clamp(16px, 1.6vw, 30px);
}

.site-navbar .nav-link {
  padding: 0;
  font-size: 1.05rem;
  text-shadow: 0 2px 14px rgba(0, 0, 0, 0.35);
}

@media (max-width: 991px) {
  .site-navbar > .container-fluid {
    width: calc(100vw - 32px) !important;
  }

  .site-navbar-logos {
    gap: 10px;
  }

  .site-navbar-logo-hkust {
    width: 150px !important;
    height: 48px !important;
  }

  .site-navbar-logo-sms {
    width: 104px !important;
    height: 48px !important;
    transform: translate(5px, 3px) !important;
  }
}
</style>


{::nomarkdown}
<div class="page-hero">
<div class="page-hero-inner">
<h1 class="page-hero-title">This is Smart Materials & Systems Lab</h1>
<p class="page-hero-copy">We advance battery-free IoT by integrating intelligent materials and structures, ambient energy harvesting, low-power sensing, and wireless communication.</p>
<p class="page-hero-note">JOIN US IN BUILDING A CONNECTED WORLD POWERED BY AMBIENT ENERGY.</p>
</div>
</div>

<main class="home-white">
<section class="home-section">
<h2 class="home-section-title">Featured Work</h2>

<div class="featured-carousel" id="featuredCarousel">
<div class="fc-viewport">
<div class="fc-track">

<article class="fc-slide">
<h5><strong>Rolling Mode TENG for Ocean Wave Energy Harvesting</strong> published in <strong><i>Nature Communications, 2024, 15, 6834.</i></strong></h5>
<img src="{{ '/images/featured-nc.webp' | relative_url }}" srcset="{{ '/images/featured-nc-small.webp' | relative_url }} 960w, {{ '/images/featured-nc.webp' | relative_url }} 1920w" sizes="(max-width: 1409px) 88vw, 1240px" width="1920" height="1080" loading="lazy" decoding="async" class="fc-img" alt="Featured work 1 image">
</article>

<article class="fc-slide">
<h5><strong>Mantis Shrimp-inspired Ultrafast Energy Transformation for Smart Surveillance</strong> published in <strong><i>Device, 2025, 100903.</i></strong></h5>
<h5><strong>Selected as Front Cover</strong></h5>
<img src="{{ '/images/featured-device.webp' | relative_url }}" srcset="{{ '/images/featured-device-small.webp' | relative_url }} 960w, {{ '/images/featured-device.webp' | relative_url }} 1920w" sizes="(max-width: 1409px) 88vw, 1240px" width="1920" height="996" loading="lazy" decoding="async" class="fc-img" alt="Featured work 2 image">
</article>

<article class="fc-slide">
<h5><strong>Origami-TENG for Energy and Information Co-Harvesting</strong> published in <strong><i>Joule, 2026, 10(5), 102338.</i></strong></h5>
<h5><strong>Selected as Front Cover</strong></h5>
<img src="{{ '/images/featured-joule.webp' | relative_url }}" srcset="{{ '/images/featured-joule-small.webp' | relative_url }} 960w, {{ '/images/featured-joule.webp' | relative_url }} 1920w" sizes="(max-width: 1409px) 88vw, 1240px" width="1920" height="1015" loading="lazy" decoding="async" class="fc-img" alt="Featured work 3 image">
</article>

</div>
</div>
<div class="fc-dots"></div>
</div>

<script>
(function () {
  const root = document.getElementById('featuredCarousel');
  if (!root) return;

  const track = root.querySelector('.fc-track');
  const slides = Array.from(root.querySelectorAll('.fc-slide'));
  const dotsWrap = root.querySelector('.fc-dots');

  if (!track || slides.length < 2 || !dotsWrap) return;

  let idx = 0;
  let timer = null;
  const INTERVAL_MS = 5000;

  // Build dots
  const dots = slides.map((_, i) => {
    const b = document.createElement('button');
    b.type = 'button';
    b.className = 'fc-dot' + (i === 0 ? ' is-active' : '');
    b.setAttribute('aria-label', 'Go to featured work ' + (i + 1));
    b.addEventListener('click', () => go(i, true));
    dotsWrap.appendChild(b);
    return b;
  });

  function render() {
    track.style.transform = `translateX(-${idx * 100}%)`;
    dots.forEach((d, i) => d.classList.toggle('is-active', i === idx));
  }

  function go(i, userAction) {
    idx = (i + slides.length) % slides.length;
    render();
    if (userAction) restart();
  }

  function next(userAction) { go(idx + 1, userAction); }
  function start() {
    stop();
    timer = setInterval(() => next(false), INTERVAL_MS);
  }

  function stop() {
    if (timer) clearInterval(timer);
    timer = null;
  }

  function restart() { start(); }

  // Pause on hover (optional)
  root.addEventListener('mouseenter', stop);
  root.addEventListener('mouseleave', start);

  render();
  start();
})();
</script>




</section>
{:/nomarkdown}

<section class="news-section">
<h3>News</h3>

##### <u>2026.03.14</u> [<strong>Congrats to Yawei! His 2nd journal paper has been published in Joule.</strong>](https://www.cell.com/joule/fulltext/S2542-4351(26)00022-X)
##### <u>2025.06.17</u> <strong>Congrats to Yihao on receiving the CSC scholarship!
##### <u>2025.05.13</u> <strong>Congrats to Hao on his first paper being accepted by SMS!
##### <u>2024.12.27</u> <strong>Congrats to Yizhou on his first paper being accepted by APL!
##### <u>2024.12.21</u> <strong>Congrats to Yihao on his first paper being accepted by MSSP!
##### <u>2023.10.17</u> [<strong>恭喜博士生王雅巍荣获IoT首届"Outstanding Student Achievement Award"奖项!</strong>](https://mp.weixin.qq.com/s/ozUS3BBVFOm_-iWpShfCrw)
##### <u>2023.10.17</u> [<strong>恭喜胡国标教授连续三年入选全球前2%顶尖科学家榜单!</strong>](https://mp.weixin.qq.com/s/iTxbsEhDPVyGQPpST_H6Fg)
##### <u>2024.08.10</u> [<strong>Congrats to Yawei! His 1st journal paper has been published in Nature Communications.</strong>](https://www.nature.com/articles/s41467-024-51245-5)
##### <u>2023.12.13</u> [<strong>博士生王雅巍斩获INFO Open Day最佳人气奖、最佳海报奖!</strong>](https://mp.weixin.qq.com/s/L8pKpwuZ7muS8f1R5r7UVg)
##### <u>2023.10.17</u> [<strong>恭喜胡国标教授入选全球前2%顶尖科学家榜单!</strong>](https://mp.weixin.qq.com/s/aExUrw_RwpVU2Qq1FI6xxg)
##### <u>2023.09.21</u> [<strong>恭喜胡国标教授荣获ASME-SMASIS 2023最佳论文奖!</strong>](https://mp.weixin.qq.com/s/1lwVYDcNj-gWKcWwkpmNmg?poc_token=HENwrGajkJ-Tw9AO9yY3ANeL0NhV6e-b0xyFLRa9)

</section>
{::nomarkdown}
</main>
{:/nomarkdown}
