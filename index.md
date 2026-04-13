---
layout: page
---

# About Me

<img src="https://larrysimingdeng.github.io/dengsiming.jpg" class="floatpic">

Here is **Siming Deng (Larry Deng)**.<br>

I am a graduate student in the Department of [Electrical and Systems Engineering (ESE)](https://www.ese.upenn.edu/) at the [Penn Engineering](https://www.seas.upenn.edu/) of the **University of Pennsylvania**.<!-- advised by [Prof. XXX](放教授web，http开头), within [Internet of Everything (IoE) Group](https://ioe.eng.cam.ac.uk/).--> Prior to joining Penn, I gained valuable research experiences as a Research Assistant at Shenzhen University under the supervision of [Dr. Jun Zhang](https://www.researchgate.net/profile/Jun_Zhang93). My work focused on **Nonparametric Statistics**, **Distortion Measurement Error Models**, and **Large Sample Theory**. I developed and analyzed advanced statistical methods, conducted large-scale simulations, and applied these techniques to real-world datasets, resulting in five SCI publications.<br>

## Work Experience

<div class="timeline">
  <div class="timeline-progress" id="timeline-progress"></div>

  <div class="timeline-item">
    <div class="timeline-dot" style="background: #ffffff;">
      <img src="/images/logo/apple.svg" alt="Apple">
    </div>
    <div class="timeline-card">
      <div class="timeline-header">
        <div class="timeline-role">Software Engineer <span class="timeline-sep">|</span> <span class="timeline-company">Apple Inc.</span></div>
        <span class="timeline-time">Jan. 2026 - Present</span>
      </div>
      <div class="timeline-details">
        Developed AI agent tools for iPhone hardware testing, enhancing automated diagnostics workflows and improving large-scale test efficiency.
      </div>
    </div>
  </div>

  <div class="timeline-item">
    <div class="timeline-dot" style="background: #ffffff;">
      <img src="/images/logo/boc.svg" alt="Bank of China">
    </div>
    <div class="timeline-card">
      <div class="timeline-header">
        <div class="timeline-role">Software Engineer <span class="timeline-sep">|</span> <span class="timeline-company">Bank of China</span></div>
        <span class="timeline-time">Jun. 2025 - Sep. 2025</span>
      </div>
      <div class="timeline-details">
        Involved in the deployment and fine-tuning of large language models in internal banking systems.
      </div>
    </div>
  </div>

  <div class="timeline-item">
    <div class="timeline-dot" style="background: #ffffff;">
      <img src="/images/logo/szu.svg" alt="Shenzhen University">
    </div>
    <div class="timeline-card">
      <div class="timeline-header">
        <div class="timeline-role">Research Assistant <span class="timeline-sep">|</span> <span class="timeline-company"><a href="https://bdsc.szu.edu.cn/">Big Data Institute, Shenzhen University</a></span></div>
        <span class="timeline-time">2023 - 2024</span>
      </div>
      <div class="timeline-details">
        Supervised by Distinguished Professor <a href="https://dblp.org/pid/h/JoshuaZhexueHuang.html">Joshua Zhexue Huang</a>. Carried out optimizations on data processing and clustering algorithms by leveraging distributed approximate computing techniques.
      </div>
    </div>
  </div>

</div>

<script>
(function() {
  var timelineProgress = document.getElementById('timeline-progress');
  var timeline = document.querySelector('.timeline');
  if (!timelineProgress || !timeline) return;

  var items = timeline.querySelectorAll('.timeline-item');

  // IntersectionObserver for in-view class
  if ('IntersectionObserver' in window) {
    var observer = new IntersectionObserver(function(entries) {
      entries.forEach(function(entry) {
        if (entry.isIntersecting) {
          entry.target.classList.add('in-view');
        }
      });
    }, { rootMargin: '0px 0px -15% 0px' });

    items.forEach(function(item) { observer.observe(item); });
  } else {
    items.forEach(function(item) { item.classList.add('in-view'); });
  }

  // Scroll progress bar
  window.addEventListener('scroll', function() {
    var rect = timeline.getBoundingClientRect();
    var totalHeight = timeline.offsetHeight;
    var windowH = window.innerHeight;
    var lineTop = 30;
    var lineBottom = 30;
    var lineHeight = totalHeight - lineTop - lineBottom;

    if (rect.top < windowH && rect.bottom > 0) {
      var scrolled = Math.min(1, Math.max(0, (windowH - rect.top - lineTop) / (totalHeight - lineTop + windowH * 0.4)));
      timelineProgress.style.height = Math.min(scrolled * lineHeight, lineHeight) + 'px';
    }
  }, { passive: true });
})();
</script>

If you are interested in any aspect of me, I am always open to discussions and collaborations. Feel free to reach out to me at - siming_deng_stat [at] 163.com

**<font color="#990000">I am actively seeking a PhD position for 2025 Fall admission. If you have any information, please contact me. Thank you!</font>**

---

## Publications

<div class="publications-grid">

  <div class="publication-card">
    <div class="publication-thumb">
      <img src="/images/papers/paper1.svg" alt="Innovative covariance-based framework">
      <a href="https://www.tandfonline.com/doi/abs/10.1080/03610918.2026.2635000" class="publication-overlay" target="_blank" rel="noopener">
        <span>View Paper</span>
      </a>
    </div>
    <div class="publication-info">
      <div class="publication-title">
        <a href="https://www.tandfonline.com/doi/abs/10.1080/03610918.2026.2635000" target="_blank" rel="noopener">Innovative covariance-based framework: symmetry assessment and exponentiality testing under multiplicative distortion measurement Errors</a>
      </div>
      <div class="publication-authors"><strong class="author-highlight">Siming Deng</strong>, Jun Zhang, Jiongtao Zhong</div>
      <div class="publication-conference"><span class="pub-venue">Communications in Statistics - Simulation and Computation, 2026</span> <a href="https://www.tandfonline.com/doi/abs/10.1080/03610918.2026.2635000" target="_blank">[paper]</a></div>
      <div class="publication-details">SCI, first author</div>
    </div>
  </div>

  <div class="publication-card">
    <div class="publication-thumb">
      <img src="/images/papers/paper2.svg" alt="A New Logarithmic Multiplicative Distortion">
      <a href="https://onlinelibrary.wiley.com/doi/10.1002/sam.11708" class="publication-overlay" target="_blank" rel="noopener">
        <span>View Paper</span>
      </a>
    </div>
    <div class="publication-info">
      <div class="publication-title">
        <a href="https://onlinelibrary.wiley.com/doi/10.1002/sam.11708" target="_blank" rel="noopener">A New Logarithmic Multiplicative Distortion for Correlation Analysis</a>
      </div>
      <div class="publication-authors"><strong class="author-highlight">Siming Deng</strong>, Jun Zhang</div>
      <div class="publication-conference"><span class="pub-venue">Statistical Analysis and Data Mining, 2024</span> <a href="https://onlinelibrary.wiley.com/doi/10.1002/sam.11708" target="_blank">[paper]</a></div>
      <div class="publication-details">SCI, JCR: Q1, first author</div>
    </div>
  </div>

  <div class="publication-card">
    <div class="publication-thumb">
      <img src="/images/papers/paper3.svg" alt="A Revisit to Pearson Correlation Coefficient">
      <a href="https://www.tandfonline.com/doi/full/10.1080/03610918.2024.2333352" class="publication-overlay" target="_blank" rel="noopener">
        <span>View Paper</span>
      </a>
    </div>
    <div class="publication-info">
      <div class="publication-title">
        <a href="https://www.tandfonline.com/doi/full/10.1080/03610918.2024.2333352" target="_blank" rel="noopener">A Revisit to Pearson Correlation Coefficient under Multiplicative Distortions</a>
      </div>
      <div class="publication-authors"><strong class="author-highlight">Siming Deng</strong>, Jun Zhang, Yingcong Huang, Jiongtao Zhong & Xiaozhen Yang</div>
      <div class="publication-conference"><span class="pub-venue">Communications in Statistics - Simulation and Computation, 2024</span> <a href="https://www.tandfonline.com/doi/full/10.1080/03610918.2024.2333352" target="_blank">[paper]</a></div>
      <div class="publication-details">SCI, first author, Highly Cited Paper - Web of Science</div>
    </div>
  </div>

  <div class="publication-card">
    <div class="publication-thumb">
      <img src="/images/papers/paper4.svg" alt="Covariance Ratio under Multiplicative Distortion">
      <a href="https://www.tandfonline.com/doi/full/10.1080/03610926.2023.2295240" class="publication-overlay" target="_blank" rel="noopener">
        <span>View Paper</span>
      </a>
    </div>
    <div class="publication-info">
      <div class="publication-title">
        <a href="https://www.tandfonline.com/doi/full/10.1080/03610926.2023.2295240" target="_blank" rel="noopener">Covariance Ratio under Multiplicative Distortion Measurement Errors</a>
      </div>
      <div class="publication-authors">Jiongtao Zhong, <strong class="author-highlight">Siming Deng</strong>, Jun Zhang & Zhenghui Feng</div>
      <div class="publication-conference"><span class="pub-venue">Communications in Statistics - Theory and Methods, 2023</span> <a href="https://www.tandfonline.com/doi/full/10.1080/03610926.2023.2295240" target="_blank">[paper]</a></div>
      <div class="publication-details">SCI, 2nd-author</div>
    </div>
  </div>

  <div class="publication-card">
    <div class="publication-thumb">
      <img src="/images/papers/paper5.svg" alt="Estimation of Correlation Coefficient">
      <a href="https://www.tandfonline.com/doi/full/10.1080/03610926.2023.2288794" class="publication-overlay" target="_blank" rel="noopener">
        <span>View Paper</span>
      </a>
    </div>
    <div class="publication-info">
      <div class="publication-title">
        <a href="https://www.tandfonline.com/doi/full/10.1080/03610926.2023.2288794" target="_blank" rel="noopener">Estimation of Correlation Coefficient with Monotone Transformation and Multiplicative Distortions</a>
      </div>
      <div class="publication-authors">Jun Zhang, Xuan Yu, <strong class="author-highlight">Siming Deng</strong>, Jiongtao Zhong, Yisheng Zhou & Bingqing Lin</div>
      <div class="publication-conference"><span class="pub-venue">Communications in Statistics - Theory and Methods, 2023</span> <a href="https://www.tandfonline.com/doi/full/10.1080/03610926.2023.2288794" target="_blank">[paper]</a></div>
      <div class="publication-details">SCI, 3rd-author</div>
    </div>
  </div>

</div>

<script>
(function() {
  if ('IntersectionObserver' in window) {
    var observer = new IntersectionObserver(function(entries) {
      entries.forEach(function(entry) {
        if (entry.isIntersecting) {
          entry.target.classList.add('animate-in');
          observer.unobserve(entry.target);
        }
      });
    }, { threshold: 0.08, rootMargin: '0px 0px -40px 0px' });
    document.querySelectorAll('.publication-card').forEach(function(card) {
      observer.observe(card);
    });
  } else {
    document.querySelectorAll('.publication-card').forEach(function(card) {
      card.classList.add('animate-in');
    });
  }
})();
</script>

---

## Research Interests

- Machine Learning
- Nonparametric Statistics

My current research focuses on addressing critical challenges in measurement error modeling and unobservable variable estimation, particularly in multiplicative distortion frameworks. Through theoretical advancements in calibration methods and simulation optimization, I have contributed to improving the accuracy of correlation coefficient estimation under complex industrial scenarios.
<img src="/images/dsm1.jpg">

---

## News and Updates

<div class="news-grid">
  <div class="news-card news-card--publication">
    <div class="news-meta">
      <span class="news-date">February 2026</span>
      <span class="news-tag news-tag--publication">Publication</span>
    </div>
    <p>First-Author Paper: <a href="https://www.tandfonline.com/doi/abs/10.1080/03610918.2026.2635000"><strong>Innovative covariance-based framework: symmetry assessment and exponentiality testing under multiplicative distortion measurement Errors</strong></a> Now Officially Published in <a href="https://www.tandfonline.com/journals/lssp20">Communications in Statistics - Simulation and Computation</a></p>
  </div>

  <div class="news-card news-card--milestone">
    <div class="news-meta">
      <span class="news-date">Jan 2026</span>
      <span class="news-tag news-tag--milestone">Milestone</span>
    </div>
    <p>Excited to have received an offer from Apple!</p>
  </div>

  <div class="news-card news-card--milestone">
    <div class="news-meta">
      <span class="news-date">March 2025</span>
      <span class="news-tag news-tag--milestone">Milestone</span>
    </div>
    <p>Thrilled to have received an offer from UPenn Engineering!</p>
  </div>

  <div class="news-card news-card--publication">
    <div class="news-meta">
      <span class="news-date">August 2024</span>
      <span class="news-tag news-tag--publication">Publication</span>
    </div>
    <p>First-Author Paper: <a href="https://onlinelibrary.wiley.com/doi/10.1002/sam.11708"><strong>A New Logarithmic Multiplicative Distortion for Correlation Analysis</strong></a> Now Officially Published in <a href="https://onlinelibrary.wiley.com/journal/19321872">Statistical Analysis and Data Mining</a> (JCR Q1)</p>
  </div>
</div>

<script>
(function() {
  if ('IntersectionObserver' in window) {
    var observer = new IntersectionObserver(function(entries) {
      entries.forEach(function(entry) {
        if (entry.isIntersecting) {
          entry.target.classList.add('animate-in');
          observer.unobserve(entry.target);
        }
      });
    }, { threshold: 0.08, rootMargin: '0px 0px -60px 0px' });
    document.querySelectorAll('.news-card').forEach(function(card) {
      observer.observe(card);
    });
  } else {
    document.querySelectorAll('.news-card').forEach(function(card) {
      card.classList.add('animate-in');
    });
  }
})();
</script>

<!-- <blockquote class="twitter-tweet"><p lang="en" dir="ltr">Thrilled to be an AAAI-UC Scholar at <a href="https://twitter.com/hashtag/AAAI24?src=hash&amp;ref_src=twsrc%5Etfw">#AAAI24</a>, thanks to <a href="https://twitter.com/hashtag/AAAI?src=hash&amp;ref_src=twsrc%5Etfw">#AAAI</a> &amp; <a href="https://twitter.com/hashtag/GoogleExploreCSR?src=hash&amp;ref_src=twsrc%5Etfw">#GoogleExploreCSR</a> for the sponsorship. Grateful for the knowledge gained and new friendships formed.<br><br>Wonderful trip in Vancouver. Looking forward to staying connected with all.<a href="https://twitter.com/hashtag/AAAI24?src=hash&amp;ref_src=twsrc%5Etfw">#AAAI24</a> <a href="https://twitter.com/hashtag/Vancouver?src=hash&amp;ref_src=twsrc%5Etfw">#Vancouver</a> <a href="https://twitter.com/hashtag/GoogleExploreCSR?src=hash&amp;ref_src=twsrc%5Etfw">#GoogleExploreCSR</a> <a href="https://t.co/wUQUp8XlSM">pic.twitter.com/wUQUp8XlSM</a></p>&mdash; Hanlin CAI (seeking a PhD position 2025) (@lancecai2002) <a href="https://twitter.com/lancecai2002/status/1762210025173344260?ref_src=twsrc%5Etfw">February 26, 2024</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script> -->
