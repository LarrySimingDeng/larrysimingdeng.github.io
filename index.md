---
layout: page
---

# About Me

<img src="/images/dengsiming.jpg" class="floatpic">

Here is **Siming Deng (Larry Deng)**.<br>

I am a graduate student in the Department of [Electrical and Systems Engineering (ESE)](https://www.ese.upenn.edu/) at the [Penn Engineering](https://www.seas.upenn.edu/) of the **University of Pennsylvania**. Currently, I build **agentic AI tools and infrastructure** for iPhone hardware testing, spanning agent runtimes (multi-agent orchestration and tool use), on-device inference with **Apple MLX**, closed-loop test optimization, and **Vision Transformers** for distribution diagnosis. Broadly, my interests lie at the intersection of **AI infrastructure, applied ML, and hardware systems**. Prior to joining Penn, I gained valuable research experiences as a Research Assistant at Shenzhen University advised by [Dr. Jun Zhang](https://www.researchgate.net/profile/Jun_Zhang93). My work focused on **Nonparametric Statistics**, **Distortion Measurement Error Models**, and **Large Sample Theory**. I developed and analyzed advanced statistical methods, conducted large-scale simulations, and applied these techniques to real-world datasets, resulting in five SCI publications.<br>

## Work Experience

<div class="timeline">
  <div class="timeline-progress" id="timeline-progress"></div>

  <div class="timeline-item timeline-item--current">
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
      <img src="/images/logo/upenn.svg" alt="UPenn">
    </div>
    <div class="timeline-card">
      <div class="timeline-header">
        <div class="timeline-role">Research Assistant <span class="timeline-sep">|</span> <span class="timeline-company">University of Pennsylvania</span></div>
        <span class="timeline-time">Nov. 2025 - Jan. 2026</span>
      </div>
      <div class="timeline-details">
        ViT-driven image geolocation.
      </div>
    </div>
  </div>

  <div class="timeline-item">
    <div class="timeline-dot" style="background: #ffffff;">
      <img src="/images/logo/sf.svg" alt="SF Express">
    </div>
    <div class="timeline-card">
      <div class="timeline-header">
        <div class="timeline-role">Software Engineer <span class="timeline-sep">|</span> <span class="timeline-company">SF Express</span></div>
        <span class="timeline-time">May. 2025 - Jul. 2025</span>
      </div>
      <div class="timeline-details">
        Delivered microservice modules for the order management system.
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
        <span class="timeline-time">Jul. 2024 - Sep. 2024</span>
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

    items.forEach(function(item, idx) {
      if (idx < 3) {
        // Reveal first 3 immediately on load (still gets the stagger transition)
        item.classList.add('in-view');
      } else {
        observer.observe(item);
      }
    });
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

**<font color="#990000">Seeking Software Engineer and Machine Learning roles — AI Infrastructure, Applied AI / Agents, and ML Systems. Feel free to reach out!</font>**

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
      <div class="publication-details">SCI, JCR: Q1, first author, Top Cited Article - WILEY 2025</div>
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

- ML Systems & AI Infrastructure
- Efficient & On-Device Inference (Apple MLX, [SGLang](https://github.com/sgl-project/sglang)<a class="sgl-badge" href="https://github.com/sgl-project/sglang" target="_blank" rel="noopener noreferrer" aria-label="SGLang on GitHub (opens in a new tab)" title="SGLang on GitHub"><img src="/images/sglang-mark.svg" alt="SGLang logo" width="22" height="25" loading="lazy"></a>)
- Agentic AI (multi-agent orchestration & tool use)
- Machine Learning
- Nonparametric Statistics

I currently work at the intersection of **AI infrastructure and applied ML**, building agent runtimes and optimizing LLM inference.

Previously, my research centered on **nonparametric statistics** and **measurement-error modeling**, unobservable-variable estimation under multiplicative distortion frameworks, where I developed calibration methods and simulation studies to improve correlation-coefficient estimation in complex industrial settings, resulting in five SCI publications.
<img src="/images/sunset.jpg">

---

## News and Updates

<div class="news-grid">
  <div class="news-card news-card--milestone news-card--feature">
    <div class="news-meta">
      <span class="news-date">September 2026</span>
      <span class="news-tag news-tag--milestone">Milestone</span>
    </div>
    <p>Apple unveils <strong>iPhone 18 Pro</strong> &amp; <strong>iPhone Duo</strong>. Proud to have contributed to the agentic hardware-testing tooling behind the launch.</p>

    <div class="milestone-gallery">
      <figure class="mtile">
        <img src="/images/milestones/apple-iphone18.jpg" alt="Siming Deng with the iPhone 18 lineup on display at Apple" loading="lazy">
      </figure>

      <!-- iPhone 18 Pro cover: a baked snapshot of apple.com's Open Graph card, links to Apple -->
      <a class="mtile mtile--link mtile--contain" href="https://www.apple.com/iphone-18-pro/" target="_blank" rel="noopener noreferrer" aria-label="iPhone 18 Pro and iPhone 18 Pro Max on apple.com (opens in a new tab)">
        <img src="/images/milestones/iphone-18-pro-cover.png" alt="iPhone 18 Pro and iPhone 18 Pro Max" loading="lazy">
        <span class="mtile__ext" aria-hidden="true">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M7 17 17 7"/><path d="M8 7h9v9"/></svg>
        </span>
        <span class="mtile__cap">
          <span class="mtile__cap-title">iPhone 18 Pro</span>
          <span class="mtile__cap-domain">apple.com</span>
        </span>
      </a>

      <!-- iPhone Duo cover: a baked snapshot of apple.com's Open Graph card, links to Apple -->
      <a class="mtile mtile--link" href="https://www.apple.com/iphone-duo/" target="_blank" rel="noopener noreferrer" aria-label="iPhone Duo on apple.com (opens in a new tab)">
        <img src="/images/milestones/iphone-duo-cover.png" alt="iPhone Duo" loading="lazy">
        <span class="mtile__ext" aria-hidden="true">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M7 17 17 7"/><path d="M8 7h9v9"/></svg>
        </span>
        <span class="mtile__cap">
          <span class="mtile__cap-title">iPhone Duo</span>
          <span class="mtile__cap-domain">apple.com</span>
        </span>
      </a>
    </div>
  </div>

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
