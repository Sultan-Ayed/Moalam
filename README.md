
<style>
@import url('https://fonts.googleapis.com/css2?family=Tajawal:wght@300;400;500;700;900&display=swap');
*{margin:0;padding:0;box-sizing:border-box}
.p{background:#0A0A0A;font-family:'Tajawal',sans-serif;direction:rtl;color:#F5F0E8;overflow:hidden}

/* NAV */
.nav{display:flex;align-items:center;justify-content:space-between;padding:22px 48px;border-bottom:1px solid #1A1A1A;background:#0A0A0A}
.nav-logo{font-size:22px;font-weight:900;color:#fff;letter-spacing:-0.5px;display:flex;align-items:center;gap:10px}
.nav-dot{width:10px;height:10px;background:#C9913A;border-radius:50%}
.nav-links{display:flex;gap:32px}
.nav-link{font-size:13px;color:#888;font-weight:400}
.nav-link.active{color:#fff}
.nav-cta{background:#C9913A;color:#0A0A0A;font-size:13px;font-weight:700;padding:10px 22px;border-radius:6px;font-family:'Tajawal',sans-serif}

/* HERO */
.hero{padding:100px 48px 80px;position:relative;overflow:hidden;min-height:500px;display:flex;flex-direction:column;justify-content:center}
.hero-eyebrow{display:inline-flex;align-items:center;gap:8px;background:#161616;border:1px solid #2A2A2A;border-radius:20px;padding:6px 16px;font-size:12px;color:#C9913A;margin-bottom:32px;width:fit-content}
.hero-eyebrow-dot{width:6px;height:6px;background:#C9913A;border-radius:50%}
.hero-title{font-size:72px;font-weight:900;line-height:1.05;letter-spacing:-2px;max-width:700px}
.hero-title span{color:#C9913A}
.hero-sub{font-size:16px;color:#666;margin-top:24px;max-width:500px;line-height:1.8;font-weight:400}
.hero-actions{display:flex;gap:14px;margin-top:40px;align-items:center}
.btn-primary{background:#C9913A;color:#0A0A0A;font-size:14px;font-weight:700;padding:14px 28px;border-radius:8px;font-family:'Tajawal',sans-serif}
.btn-secondary{color:#888;font-size:14px;font-weight:400;display:flex;align-items:center;gap:8px}
.btn-arrow{width:32px;height:32px;border:1px solid #2A2A2A;border-radius:50%;display:inline-flex;align-items:center;justify-content:center;font-size:14px}

/* Fire BG decoration */
.hero-bg-dec{position:absolute;left:0;top:0;bottom:0;width:50%;pointer-events:none;opacity:0.04}
.circle-dec{position:absolute;border-radius:50%;border:1px solid #C9913A}

/* MARQUEE */
.marquee-wrap{border-top:1px solid #1A1A1A;border-bottom:1px solid #1A1A1A;padding:16px 0;overflow:hidden;background:#0D0D0D}
.marquee-inner{display:flex;gap:48px;white-space:nowrap;animation:scroll 18s linear infinite}
.marquee-item{font-size:13px;color:#444;font-weight:500;display:flex;align-items:center;gap:12px}
.marquee-dot{color:#C9913A;font-size:10px}
@keyframes scroll{0%{transform:translateX(0)}100%{transform:translateX(-50%)}}

/* ABOUT */
.section{padding:80px 48px}
.section-label{font-size:11px;color:#C9913A;font-weight:700;letter-spacing:3px;margin-bottom:20px;text-transform:uppercase}
.section-title{font-size:42px;font-weight:900;line-height:1.15;letter-spacing:-1px}
.section-title span{color:#C9913A}

.about-grid{display:grid;grid-template-columns:1fr 1fr;gap:40px;margin-top:48px}
.about-text{font-size:15px;color:#888;line-height:2;font-weight:400}
.about-text span{color:#F5F0E8}
.about-stats{display:grid;grid-template-columns:1fr 1fr;gap:16px}
.stat{background:#111;border:1px solid #1E1E1E;border-radius:12px;padding:24px;position:relative;overflow:hidden}
.stat::before{content:'';position:absolute;top:0;right:0;width:3px;height:100%;background:#C9913A;border-radius:0 12px 12px 0}
.stat-num{font-size:40px;font-weight:900;color:#C9913A;line-height:1}
.stat-lbl{font-size:12px;color:#555;margin-top:6px;font-weight:400}

/* TARGETS */
.targets-sec{padding:0 48px 80px}
.targets-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:1px;background:#1A1A1A;border:1px solid #1A1A1A;border-radius:16px;overflow:hidden;margin-top:40px}
.target{background:#0D0D0D;padding:40px 28px;position:relative}
.target-num{font-size:11px;color:#333;font-weight:700;letter-spacing:2px;margin-bottom:20px}
.target-icon-wrap{width:52px;height:52px;background:#161616;border:1px solid #C9913A20;border-radius:12px;display:flex;align-items:center;justify-content:center;font-size:24px;margin-bottom:20px}
.target-name{font-size:20px;font-weight:700;margin-bottom:10px}
.target-desc{font-size:13px;color:#555;line-height:1.8}
.target:hover .target-icon-wrap{background:#C9913A15;border-color:#C9913A50}

/* SERVICES */
.services-sec{padding:0 48px 80px}
.svc-list{margin-top:40px;border-top:1px solid #1A1A1A}
.svc-row{display:flex;align-items:center;justify-content:space-between;padding:28px 0;border-bottom:1px solid #1A1A1A;cursor:pointer}
.svc-left{display:flex;align-items:center;gap:20px}
.svc-num{font-size:12px;color:#333;font-weight:700;width:28px}
.svc-name{font-size:20px;font-weight:700}
.svc-tag{font-size:11px;color:#C9913A;background:#C9913A12;border:1px solid #C9913A30;padding:4px 12px;border-radius:12px}
.svc-row:hover .svc-name{color:#C9913A}

/* SUPERVISOR */
.sup-sec{padding:0 48px 80px}
.sup-card{background:#0D0D0D;border:1px solid #1E1E1E;border-radius:20px;overflow:hidden;margin-top:40px;display:grid;grid-template-columns:1fr 1fr}
.sup-left{padding:48px;border-left:1px solid #1A1A1A;display:flex;flex-direction:column;justify-content:space-between}
.sup-avatar-area{display:flex;align-items:center;gap:16px;margin-bottom:32px}
.sup-av{width:64px;height:64px;background:#161616;border:2px solid #C9913A;border-radius:16px;display:flex;align-items:center;justify-content:center;font-size:28px;font-weight:900;color:#C9913A;flex-shrink:0;font-family:'Tajawal',sans-serif}
.sup-name{font-size:20px;font-weight:700}
.sup-role{font-size:13px;color:#555;margin-top:4px}
.sup-bio{font-size:14px;color:#666;line-height:2}
.sup-bio span{color:#F5F0E8}
.sup-badge-row{display:flex;gap:8px;margin-top:24px}
.sup-badge{background:#161616;border:1px solid #2A2A2A;border-radius:6px;padding:6px 14px;font-size:12px;color:#888}
.sup-right{padding:48px;display:flex;flex-direction:column;justify-content:center;gap:16px}
.sup-r-title{font-size:13px;color:#444;margin-bottom:8px;font-weight:500}
.sup-feature{display:flex;align-items:flex-start;gap:12px;padding:16px;background:#111;border-radius:10px;border:1px solid #1E1E1E}
.sup-feature-dot{width:6px;height:6px;background:#C9913A;border-radius:50%;margin-top:6px;flex-shrink:0}
.sup-feature-text{font-size:13px;color:#666;line-height:1.7}
.sup-feature-text span{color:#F5F0E8}

/* ANNOUNCE */
.ann-sec{padding:0 48px 80px}
.ann-card{background:#C9913A;border-radius:20px;padding:56px 48px;display:flex;align-items:center;justify-content:space-between}
.ann-title{font-size:36px;font-weight:900;color:#0A0A0A;line-height:1.2;max-width:400px}
.ann-right{text-align:left}
.ann-desc{font-size:14px;color:#0A0A0A99;max-width:260px;line-height:1.8;margin-bottom:24px;text-align:right}
.ann-btn{background:#0A0A0A;color:#F5F0E8;font-size:14px;font-weight:700;padding:14px 28px;border-radius:8px;font-family:'Tajawal',sans-serif;display:inline-block}

/* FOOTER */
.footer{border-top:1px solid #1A1A1A;padding:40px 48px;display:flex;align-items:center;justify-content:space-between}
.footer-logo{font-size:18px;font-weight:900;display:flex;align-items:center;gap:8px}
.footer-center{font-size:12px;color:#444;text-align:center}
.footer-link{color:#C9913A;font-size:12px}
</style>

<div class="p">

<nav class="nav">
  <div class="nav-logo"><div class="nav-dot"></div>مُعْلَم</div>
  <div class="nav-links">
    <div class="nav-link active">عن المبادرة</div>
    <div class="nav-link">خدماتنا</div>
    <div class="nav-link">الفئات</div>
    <div class="nav-link">المشرف</div>
  </div>
  <div class="nav-cta">انضم الآن</div>
</nav>

<section class="hero">
  <div class="circle-dec" style="width:600px;height:600px;right:-100px;top:-100px;border:1px solid #C9913A"></div>
  <div class="circle-dec" style="width:400px;height:400px;right:0px;top:50px;border:1px solid #C9913A"></div>
  <div class="hero-eyebrow"><div class="hero-eyebrow-dot"></div>مبادرة تطوعية سعودية</div>
  <h1 class="hero-title">علامتُك<br><span>الأولى</span><br>في سيرتِك</h1>
  <p class="hero-sub">مبادرة مُعْلَم تُرافقك من أول خطوة حتى أعلى درجة — إرشاد مهني حقيقي، بروح تطوعية خالصة.</p>
  <div class="hero-actions">
    <div class="btn-primary">ابدأ رحلتك</div>
    <div class="btn-secondary"><div class="btn-arrow">←</div>شف خدماتنا</div>
  </div>
</section>

<div class="marquee-wrap">
  <div class="marquee-inner">
    <div class="marquee-item"><span class="marquee-dot">◆</span>سيرة ذاتية احترافية</div>
    <div class="marquee-item"><span class="marquee-dot">◆</span>إرشاد مهني</div>
    <div class="marquee-item"><span class="marquee-dot">◆</span>LinkedIn Profile</div>
    <div class="marquee-item"><span class="marquee-dot">◆</span>تحضير مقابلات</div>
    <div class="marquee-item"><span class="marquee-dot">◆</span>تمكين مهني</div>
    <div class="marquee-item"><span class="marquee-dot">◆</span>مجتمع عربي</div>
    <div class="marquee-item"><span class="marquee-dot">◆</span>100% تطوعية</div>
    <div class="marquee-item"><span class="marquee-dot">◆</span>سيرة ذاتية احترافية</div>
    <div class="marquee-item"><span class="marquee-dot">◆</span>إرشاد مهني</div>
    <div class="marquee-item"><span class="marquee-dot">◆</span>LinkedIn Profile</div>
    <div class="marquee-item"><span class="marquee-dot">◆</span>تحضير مقابلات</div>
    <div class="marquee-item"><span class="marquee-dot">◆</span>تمكين مهني</div>
    <div class="marquee-item"><span class="marquee-dot">◆</span>مجتمع عربي</div>
    <div class="marquee-item"><span class="marquee-dot">◆</span>100% تطوعية</div>
  </div>
</div>

<section class="section">
  <div class="section-label">من نحن</div>
  <h2 class="section-title">شريك مهني حقيقي<br>مو <span>بس</span> نصيحة</h2>
  <div class="about-grid">
    <p class="about-text">مبادرة مُعْلَم مبادرة تطوعية تخدم <span>الطلاب والباحثين عن العمل والموظفين</span> في تطوير مساراتهم المهنية. نؤمن إن كل شخص يستحق دعم حقيقي في بداياته — ولذلك ما نأخذ فلساً واحداً.</p>
    <div class="about-stats">
      <div class="stat"><div class="stat-num">+500</div><div class="stat-lbl">مستفيد من المبادرة</div></div>
      <div class="stat"><div class="stat-num">100%</div><div class="stat-lbl">تطوعية خالصة</div></div>
      <div class="stat"><div class="stat-num">24/7</div><div class="stat-lbl">دعم مستمر</div></div>
      <div class="stat"><div class="stat-num">+1</div><div class="stat-lbl">سنة عطاء</div></div>
    </div>
  </div>
</section>

<section class="targets-sec">
  <div class="section-label">من نخدم</div>
  <h2 class="section-title">ثلاث فئات،<br>هدف <span>واحد</span></h2>
  <div class="targets-grid">
    <div class="target">
      <div class="target-num">01</div>
      <div class="target-icon-wrap">🎓</div>
      <div class="target-name">الطلاب</div>
      <div class="target-desc">بناء الملف المهني وتطوير المهارات قبل التخرج وبعده</div>
    </div>
    <div class="target">
      <div class="target-num">02</div>
      <div class="target-icon-wrap">💼</div>
      <div class="target-name">الباحثون عن عمل</div>
      <div class="target-desc">دعم شامل للحصول على الفرصة الوظيفية المناسبة</div>
    </div>
    <div class="target">
      <div class="target-num">03</div>
      <div class="target-icon-wrap">📈</div>
      <div class="target-name">الموظفون</div>
      <div class="target-desc">التطوير المستمر والارتقاء في المسار الوظيفي</div>
    </div>
  </div>
</section>

<section class="services-sec">
  <div class="section-label">خدماتنا</div>
  <h2 class="section-title">إيش <span>نقدم</span> لك؟</h2>
  <div class="svc-list">
    <div class="svc-row">
      <div class="svc-left"><div class="svc-num">01</div><div class="svc-name">مراجعة السيرة الذاتية</div></div>
      <div class="svc-tag">CV Review</div>
    </div>
    <div class="svc-row">
      <div class="svc-left"><div class="svc-num">02</div><div class="svc-name">إرشاد مهني فردي</div></div>
      <div class="svc-tag">Mentorship</div>
    </div>
    <div class="svc-row">
      <div class="svc-left"><div class="svc-num">03</div><div class="svc-name">تحسين LinkedIn Profile</div></div>
      <div class="svc-tag">Digital Presence</div>
    </div>
    <div class="svc-row">
      <div class="svc-left"><div class="svc-num">04</div><div class="svc-name">التحضير للمقابلات</div></div>
      <div class="svc-tag">Interview Prep</div>
    </div>
  </div>
</section>

<section class="sup-sec">
  <div class="section-label">المشرف</div>
  <h2 class="section-title">بإشراف <span>م. سلطان</span></h2>
  <div class="sup-card">
    <div class="sup-left">
      <div>
        <div class="sup-avatar-area">
          <div class="sup-av">س</div>
          <div>
            <div class="sup-name">م. سلطان بن عايد</div>
            <div class="sup-role">Sultan bin Ayed — Engineer & Career Mentor</div>
          </div>
        </div>
        <p class="sup-bio">مهندس ومتخصص في التطوير المهني والتوجيه الوظيفي. أسس مبادرة مُعْلَم من إيمان بأن <span>كل شخص يستحق دعماً حقيقياً</span> في بداياته المهنية — يُشرف شخصياً على كل البرامج.</p>
        <div class="sup-badge-row">
          <div class="sup-badge">مهندس</div>
          <div class="sup-badge">Mentor</div>
          <div class="sup-badge">مؤسس</div>
        </div>
      </div>
    </div>
    <div class="sup-right">
      <div class="sup-r-title">ما يميز الإشراف</div>
      <div class="sup-feature"><div class="sup-feature-dot"></div><div class="sup-feature-text"><span>إشراف شخصي مباشر</span> على كل برامج المبادرة دون وسيط</div></div>
      <div class="sup-feature"><div class="sup-feature-dot"></div><div class="sup-feature-text"><span>خبرة هندسية ومهنية</span> تُترجَم إلى توجيه عملي وواقعي</div></div>
      <div class="sup-feature"><div class="sup-feature-dot"></div><div class="sup-feature-text"><span>روح تطوعية خالصة</span> دون مقابل مادي أو تجارة</div></div>
    </div>
  </div>
</section>

<section class="ann-sec">
  <div class="ann-card">
    <div class="ann-title">انضم لمجتمع مُعْلَم الحين!</div>
    <div class="ann-right">
      <p class="ann-desc">المبادرة تستقبل طلبات الانضمام والتطوع — سارع وكن جزءاً من رحلة التمكين المهني العربي</p>
      <div class="ann-btn">سجّل الآن</div>
    </div>
  </div>
</section>

<footer class="footer">
  <div class="footer-logo"><div class="nav-dot"></div>مُعْلَم | Moalam</div>
  <div class="footer-center">علامتُك الأولى في سيرتِك المهنية<br><span style="color:#333">© 2024 مبادرة مُعْلَم — جميع الحقوق محفوظة</span></div>
  <div class="footer-link">github.com/Moalam</div>
</footer>

</div>
