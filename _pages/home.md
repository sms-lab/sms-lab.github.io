---
title: "Home"
layout: homelay
sitemap: false
permalink: /
---

<style>
/* ===== Your existing image layout ===== */
.container {
  text-align: center; /* 使容器内的所有内容居中显示 */
  margin-bottom: 0px; /* 底部空间 */
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
  max-width: 100%;
  margin: 10px auto 16px auto;
}

.fc-viewport {
  overflow: hidden;
  width: 100%;
}

.fc-track {
  display: flex;
  transition: transform 450ms ease;
  will-change: transform;
}

.fc-slide {
  min-width: 100%;
  box-sizing: border-box;
  padding: 0 6px;
}

.fc-slide h5 {
  margin-top: 0;
  margin-bottom: 8px;
}

.fc-slide p {
  margin: 6px 0;
}

.fc-img {
  width: 100%;
  height: 500px;
  object-fit: contain;   /* 不裁剪论文图 */
  padding: 8px;
  border-radius: 6px;
}


.fc-btn {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  border: 0;
  background: rgba(0,0,0,0.45);
  color: #fff;
  width: 38px;
  height: 38px;
  border-radius: 999px;
  cursor: pointer;
  line-height: 38px;
  font-size: 22px;
  z-index: 2;
}

.fc-prev { left: 8px; }
.fc-next { right: 8px; }

.fc-btn:hover { background: rgba(0,0,0,0.6); }

.fc-dots {
  display: flex;
  gap: 8px;
  justify-content: center;
  margin-top: 10px;
}

.fc-dot {
  width: 8px;
  height: 8px;
  border-radius: 999px;
  background: rgba(0,0,0,0.25);
  border: 0;
  cursor: pointer;
}

.fc-dot.is-active {
  background: rgba(0,0,0,0.65);
}
</style>


### Welcome!
This is Smart Materials & Systems LAB at HKUST(GZ)!

<div class="container">
<img src="{{ site.url }}{{ site.baseurl }}/images/vibration.png" style="width:100%;" />
</div>

### Featured Work

<div class="featured-carousel" id="featuredCarousel">
<button class="fc-btn fc-prev" type="button" aria-label="Previous">‹</button>

<div class="fc-viewport">
<div class="fc-track">

<article class="fc-slide">
<h5><strong>Rolling Mode TENG for Ocean Wave Energy Harvesting</strong> published in <strong><i>Nature Communications, 2024, 15, 6834.</i></strong></h5>
<img src="{{ '/images/Featured IMAGE-1-NC.jpg' | relative_url }}" class="fc-img" alt="Featured work 1 image">
</article>

<article class="fc-slide">
<h5><strong>Mantis Shrimp-inspired Ultrafast Energy Transformation for Smart Surveillance</strong> published in <strong><i>Device, 2025, 100903.</i></strong></h5>
<img src="{{ '/images/Featured IMAGE-2-Device.jpg' | relative_url }}" class="fc-img" alt="Featured work 2 image">
</article>

</div>
</div>

<button class="fc-btn fc-next" type="button" aria-label="Next">›</button>
<div class="fc-dots"></div>
</div>

<script>
(function () {
  const root = document.getElementById('featuredCarousel');
  if (!root) return;

  const track = root.querySelector('.fc-track');
  const slides = Array.from(root.querySelectorAll('.fc-slide'));
  const prevBtn = root.querySelector('.fc-prev');
  const nextBtn = root.querySelector('.fc-next');
  const dotsWrap = root.querySelector('.fc-dots');

  if (!track || slides.length < 2 || !prevBtn || !nextBtn || !dotsWrap) return;

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
  function prev(userAction) { go(idx - 1, userAction); }

  function start() {
    stop();
    timer = setInterval(() => next(false), INTERVAL_MS);
  }

  function stop() {
    if (timer) clearInterval(timer);
    timer = null;
  }

  function restart() { start(); }

  prevBtn.addEventListener('click', () => prev(true));
  nextBtn.addEventListener('click', () => next(true));

  // Keyboard support (optional)
  root.setAttribute('tabindex', '0');
  root.addEventListener('keydown', (e) => {
    if (e.key === 'ArrowLeft') { e.preventDefault(); prev(true); }
    if (e.key === 'ArrowRight') { e.preventDefault(); next(true); }
  });

  // Pause on hover (optional)
  root.addEventListener('mouseenter', stop);
  root.addEventListener('mouseleave', start);

  render();
  start();
})();
</script>




### News

##### <u>2025.06.17</u> <strong>Congrats to Yihao for receiving the CSC scholarship.!
##### <u>2025.05.13</u> <strong>Congrats to TANG Hao for his first paper being accepted by SMS!
##### <u>2024.12.27</u> <strong>Congrats to Yizhou for his first paper being accepted by APL!
##### <u>2024.12.21</u> <strong>Congrats to Yihao for his first paper being accepted by MSSP!
##### <u>2023.10.17</u> [<strong>恭喜博士生王雅巍荣获IoT首届"Outstanding Student Achievement Award"奖项!</strong>](https://mp.weixin.qq.com/s/ozUS3BBVFOm_-iWpShfCrw)
##### <u>2023.10.17</u> [<strong>恭喜胡国标教授连续三年入选全球前2%顶尖科学家榜单!</strong>](https://mp.weixin.qq.com/s/iTxbsEhDPVyGQPpST_H6Fg)
##### <u>2024.08.10</u> [Congrats to Yawei! His 1st journal paper has been published in Nature Communications.>](https://www.nature.com/articles/s41467-024-51245-5)
##### <u>2023.12.13</u> [<strong>博士生王雅巍斩获INFO Open Day最佳人气奖、最佳海报奖!</strong>](https://mp.weixin.qq.com/s/L8pKpwuZ7muS8f1R5r7UVg)
##### <u>2023.10.17</u> [<strong>恭喜胡国标教授入选全球前2%顶尖科学家榜单!</strong>](https://mp.weixin.qq.com/s/aExUrw_RwpVU2Qq1FI6xxg)
##### <u>2023.09.21</u> [<strong>恭喜胡国标教授荣获ASME-SMASIS 2023最佳论文奖!</strong>](https://mp.weixin.qq.com/s/1lwVYDcNj-gWKcWwkpmNmg?poc_token=HENwrGajkJ-Tw9AO9yY3ANeL0NhV6e-b0xyFLRa9)

