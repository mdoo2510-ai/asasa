<!DOCTYPE html>

<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>دليل التميز — الثانوية الثامنة بالخرج</title>
<link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700;900&display=swap" rel="stylesheet">
<style>
:root{
  --br:#8B6914; --br2:#A07C1E; --br3:#B89430;
  --bg:#FFFFFF; --bg2:#FDFAF3; --bg3:#FAF4E4; --bg4:#F2E8CC;
  --gd:#C8922A; --gd2:#E5B050;
  --nv:#3A2C0A; --tx:#4A3A18; --tx2:#8A7040; --tx3:#B09860;
  --bd:#EAE0C8; --bd2:#D8C898;
}
*{margin:0;padding:0;box-sizing:border-box;}
html,body{font-family:'Cairo',sans-serif;background:var(--bg);color:var(--tx);min-height:100vh;}

/* ── NAV ── */
.nav{
position:sticky;top:0;z-index:999;height:52px;
background:linear-gradient(135deg,var(–br) 0%,var(–br2) 100%);
display:flex;align-items:center;justify-content:space-between;
padding:0 14px;box-shadow:0 2px 10px rgba(120,90,46,.35);
}
.nl{display:flex;align-items:center;gap:9px;}
.ni{width:32px;height:32px;border-radius:8px;background:rgba(255,255,255,.18);
display:flex;align-items:center;justify-content:center;font-size:16px;}
.nn{font-size:12.5px;font-weight:700;color:#fff;line-height:1.25;}
.ns{font-size:10px;color:rgba(255,255,255,.6);}
.bc{display:flex;align-items:center;gap:5px;font-size:11.5px;color:rgba(255,255,255,.65);}
.bc a{cursor:pointer;color:rgba(255,255,255,.65);text-decoration:none;}
.bc a:hover{color:#fff;}
.bc b{color:#fff;font-weight:700;}
.bc s{opacity:.4;margin:0 1px;}

/* ── PAGES ── */
.pg{display:none;} .pg.on{display:block;}

/* ── HERO ── */
.hero{
background:linear-gradient(150deg,#C8A048 0%,#A07828 55%,#7A5810 100%);
padding:60px 20px 52px;text-align:center;
}
.ht{font-size:11px;letter-spacing:3px;color:rgba(255,248,225,.75);text-transform:uppercase;margin-bottom:14px;}
.hs{font-size:clamp(16px,3.5vw,24px);font-weight:700;color:#fff;margin-bottom:5px;}
.hm{font-size:13px;color:#FFF0B0;margin-bottom:28px;}
.hd{width:50px;height:2px;background:linear-gradient(90deg,transparent,#FFF0B0,transparent);margin:0 auto 24px;}
.hti{font-size:clamp(24px,5vw,42px);font-weight:900;color:#fff;line-height:1.25;margin-bottom:11px;}
.hti span{color:#FFF0B0;}
.hde{font-size:13.5px;color:rgba(255,248,225,.8);line-height:1.8;max-width:520px;margin:0 auto 32px;}
.hst{display:flex;justify-content:center;margin-bottom:34px;}
.hsi{padding:16px 28px;text-align:center;position:relative;}
.hsi::before{content:’’;position:absolute;right:0;top:22%;bottom:22%;width:1px;background:rgba(255,248,225,.2);}
.hsi:last-child::before{display:none;}
.hsn{font-size:34px;font-weight:900;color:#FFF0B0;line-height:1;}
.hsl{font-size:11px;color:rgba(255,248,225,.65);margin-top:4px;}
.hbtn{
display:inline-flex;align-items:center;gap:8px;padding:13px 30px;
background:linear-gradient(135deg,var(–gd),var(–gd2));color:var(–nv);
border:none;border-radius:50px;font-family:‘Cairo’,sans-serif;
font-size:14.5px;font-weight:700;cursor:pointer;
box-shadow:0 7px 22px rgba(200,146,42,.4);transition:.3s;
}
.hbtn:hover{transform:translateY(-2px);box-shadow:0 11px 30px rgba(200,146,42,.55);}
.notice{background:var(–bg3);border-top:3px solid var(–gd);padding:13px 20px;
text-align:center;font-size:12.5px;color:var(–tx2);line-height:1.7;}
.ftr{background:var(–nv);padding:32px 20px;text-align:center;margin-top:20px;}
.ft{font-size:14px;font-weight:700;color:rgba(245,237,214,.75);margin-bottom:5px;}
.fs{font-size:11.5px;color:rgba(245,237,214,.28);line-height:1.7;}
.fc{font-size:10.5px;color:rgba(245,237,214,.18);margin-top:12px;}

/* ── PAGE HEADER ── */
.pgh{background:var(–bg);border-bottom:1px solid var(–bd);padding:20px;}
.pgh h2{font-size:19px;font-weight:900;color:var(–nv);margin-bottom:3px;}
.pgh p{font-size:12.5px;color:var(–tx2);}

/* ── DOMAIN CARDS ── */
.dgr{display:grid;grid-template-columns:repeat(2,1fr);gap:13px;padding:14px;max-width:840px;margin:0 auto;}
@media(max-width:540px){.dgr{grid-template-columns:1fr;}}
.dc{
background:var(–bg);border-radius:16px;padding:22px;
border:1.5px solid var(–bd);cursor:pointer;transition:.28s;
position:relative;overflow:hidden;
}
.dc::before{content:’’;position:absolute;top:0;right:0;width:70px;height:70px;
background:radial-gradient(ellipse at top right,rgba(200,146,42,.07),transparent);
border-radius:0 16px 0 100%;}
.dc::after{content:’’;position:absolute;bottom:0;left:0;right:0;height:3px;
background:linear-gradient(90deg,var(–gd),var(–gd2));
transform:scaleX(0);transform-origin:right;transition:.28s;}
.dc:hover{border-color:var(–gd2);box-shadow:0 7px 24px rgba(120,90,46,.1);transform:translateY(-3px);}
.dc:hover::after{transform:scaleX(1);transform-origin:left;}
.dn{font-size:9.5px;font-weight:700;letter-spacing:2.5px;color:var(–br2);
text-transform:uppercase;margin-bottom:10px;display:flex;align-items:center;gap:7px;}
.dn::after{content:’’;flex:1;height:1px;background:var(–bd);}
.de{font-size:26px;margin-bottom:9px;display:block;}
.dtt{font-size:18px;font-weight:900;color:var(–nv);margin-bottom:7px;}
.dds{font-size:12.5px;color:var(–tx2);line-height:1.8;margin-bottom:14px;}
.dba{display:flex;gap:7px;flex-wrap:wrap;}
.badge{display:inline-flex;align-items:center;gap:3px;padding:4px 10px;
background:var(–bg3);border-radius:50px;font-size:10.5px;font-weight:700;color:var(–br2);}
.dgo{font-size:11.5px;font-weight:700;color:var(–gd);margin-top:12px;
display:flex;align-items:center;gap:5px;transition:gap .25s;}
.dc:hover .dgo{gap:11px;}

/* ── BACK HEAD ── */
.bkh{background:var(–bg);border-bottom:1px solid var(–bd);padding:12px 15px;
display:flex;align-items:center;gap:11px;}
.bkb{width:32px;height:32px;background:var(–bg3);border:none;border-radius:50%;
font-size:14px;color:var(–br);cursor:pointer;
display:flex;align-items:center;justify-content:center;flex-shrink:0;transition:.2s;}
.bkb:hover{background:var(–br);color:#fff;}
.bkt{font-size:15px;font-weight:900;color:var(–nv);}
.bks{font-size:11px;color:var(–tx3);}

/* ── STANDARDS ── */
.sl{padding:12px 14px;max-width:840px;margin:0 auto;display:grid;gap:9px;}
.si{background:var(–bg);border-radius:13px;border:1.5px solid var(–bd);cursor:pointer;transition:.22s;}
.si:hover{border-color:var(–gd2);box-shadow:0 3px 14px rgba(120,90,46,.07);}
.sii{display:flex;align-items:center;gap:11px;padding:14px 16px;}
.sc{width:34px;height:34px;background:linear-gradient(135deg,var(–br),var(–br2));
border-radius:50%;display:flex;align-items:center;justify-content:center;
font-size:13px;font-weight:900;color:#fff;flex-shrink:0;}
.stit{font-size:13.5px;font-weight:700;color:var(–nv);flex:1;line-height:1.5;}
.sme{font-size:10.5px;color:var(–tx3);}
.sar{font-size:12px;color:var(–gd);}

/* ── INDICATORS ── */
.il{padding:11px 13px;max-width:840px;margin:0 auto;display:grid;gap:7px;}
.ii{background:var(–bg);border-radius:11px;border:1.5px solid var(–bd);cursor:pointer;transition:.22s;}
.ii:hover{border-color:var(–gd2);box-shadow:0 3px 12px rgba(120,90,46,.07);}
.iii{display:flex;align-items:center;gap:11px;padding:12px 14px;}
.ib{width:28px;height:28px;background:var(–bg3);border-radius:8px;
display:flex;align-items:center;justify-content:center;
font-size:11.5px;font-weight:900;color:var(–br);flex-shrink:0;}
.ico{font-size:10px;color:var(–tx3);font-weight:600;margin-bottom:2px;}
.itx{font-size:12.5px;color:var(–tx);line-height:1.6;flex:1;}
.ich{display:flex;gap:5px;flex-wrap:wrap;padding:0 14px 10px;}
.chip{display:inline-flex;align-items:center;padding:3px 8px;border-radius:50px;
font-size:9.5px;font-weight:600;border:1px solid var(–bd);color:var(–tx2);background:var(–bg2);}

/* ── DETAIL ── */
.dtc{font-size:9.5px;color:var(–gd);font-weight:700;letter-spacing:1px;margin-bottom:3px;}
.dttl{font-size:14px;font-weight:900;color:var(–nv);line-height:1.45;}
.tabs{background:var(–bg);border-bottom:1px solid var(–bd);display:flex;
padding:0 14px;position:sticky;top:52px;z-index:10;overflow-x:auto;}
.tab{display:flex;flex-direction:column;align-items:center;gap:3px;
padding:11px 16px;border:none;background:transparent;font-family:‘Cairo’,sans-serif;
font-size:12.5px;font-weight:600;color:var(–tx2);cursor:pointer;
border-bottom:3px solid transparent;white-space:nowrap;transition:.2s;flex-shrink:0;}
.tab .ti{font-size:18px;}
.tab.on{color:var(–br);border-bottom-color:var(–gd);}
.tab:hover:not(.on){color:var(–tx);background:var(–bg2);}
.tp{display:none;padding:14px;} .tp.on{display:block;}
.svr{display:flex;flex-wrap:wrap;gap:6px;margin-bottom:16px;}
.svc{padding:5px 12px;border-radius:50px;border:1.5px solid var(–bd);
background:var(–bg2);font-size:11.5px;font-weight:600;color:var(–tx2);}

/* ── STEPS LIST ── */
.steps-list{display:grid;gap:10px;}
.step-item{
background:var(–bg);border:1.5px solid var(–bd);border-radius:14px;
padding:16px 18px;display:flex;align-items:flex-start;gap:14px;
transition:.2s;
}
.step-item:hover{border-color:var(–gd2);box-shadow:0 3px 14px rgba(180,140,40,.1);}
.step-num{
width:34px;height:34px;border-radius:50%;flex-shrink:0;
background:linear-gradient(135deg,var(–gd),var(–gd2));
color:#fff;font-size:14px;font-weight:900;
display:flex;align-items:center;justify-content:center;
box-shadow:0 3px 10px rgba(200,146,42,.3);
}
.step-body{flex:1;}
.step-title{font-size:14px;font-weight:700;color:var(–nv);margin-bottom:5px;line-height:1.4;}
.step-desc{font-size:12.5px;color:var(–tx2);line-height:1.75;}

/* ── DOCS/EVAL ── */
.thint{font-size:11.5px;color:var(–tx3);display:flex;align-items:center;gap:5px;margin-bottom:12px;}
.dl,.el{display:grid;gap:8px;}
.di,.ei{background:var(–bg);border-radius:10px;border:1.5px solid var(–bd);
padding:11px 14px;display:flex;align-items:center;gap:11px;transition:.2s;}
.di:hover,.ei:hover{border-color:var(–gd2);box-shadow:0 2px 10px rgba(120,90,46,.07);}
.dico{width:36px;height:36px;border-radius:8px;background:var(–bg3);
display:flex;align-items:center;justify-content:center;font-size:18px;flex-shrink:0;}
.ditt{font-size:12.5px;font-weight:700;color:var(–nv);margin-bottom:2px;}
.disb{font-size:10.5px;color:var(–tx3);}
</style>

</head>
<body>

<nav class="nav">
  <div class="nl">
    <div class="ni">🏫</div>
    <div><div class="nn">الثانوية الثامنة</div><div class="ns">الخرج — وزارة التعليم</div></div>
  </div>
  <div class="bc" id="bc"><b>الرئيسية</b></div>
</nav>

<!-- HOME -->

<div class="pg on" id="pg-home">
  <div class="hero">
    <div class="ht">وزارة التعليم — المملكة العربية السعودية</div>
    <div class="hs">الثانوية الثامنة — الخرج</div>
    <div class="hm">طلابنا اليوم.. قادة الغد</div>
    <div class="hd"></div>
    <h1 class="hti">خارطة الطريق<br><span>للتميز والاعتماد المدرسي</span></h1>
    <p class="hde">منصة تفاعلية ذكية مستندة إلى الوثيقة الرسمية لمعايير التقويم والاعتماد المدرسي الصادرة عن هيئة تقويم التعليم والتدريب</p>
    <div class="hst">
      <div class="hsi"><div class="hsn">4</div><div class="hsl">مجالات</div></div>
      <div class="hsi"><div class="hsn">11</div><div class="hsl">معياراً</div></div>
      <div class="hsi"><div class="hsn">54</div><div class="hsl">مؤشراً</div></div>
    </div>
    <button class="hbtn" onclick="goDomains()">استعرض المجالات ←</button>
  </div>
  <div class="notice">تنويه: هذه اجتهادات مبنية على الوثيقة الرسمية لمعايير التقويم والاعتماد المدرسي، وهي مساهمة من <strong>الثانوية الثامنة بالخرج</strong> لنقل أثر التميز.</div>
  <footer class="ftr">
    <div class="ft">خارطة الطريق للتميز والاعتماد المدرسي</div>
    <div class="fs">مستند إلى الوثيقة الرسمية — هيئة تقويم التعليم والتدريب<br>إعداد: الثانوية الثامنة — الخرج</div>
    <div class="fc">© جميع حقوق الملكية محفوظة — الثانوية الثامنة 2026</div>
  </footer>
</div>

<!-- DOMAINS -->

<div class="pg" id="pg-domains">
  <div class="pgh"><h2>المجالات الأربعة</h2><p>اختر المجال للاطلاع على معاييره ومؤشراته وخرائط الطريق</p></div>
  <div class="dgr" id="dgr"></div>
</div>

<!-- STANDARDS -->

<div class="pg" id="pg-stds">
  <div class="bkh">
    <button class="bkb" id="bk-stds">←</button>
    <div><div class="bkt" id="stds-t"></div><div class="bks" id="stds-s"></div></div>
  </div>
  <div class="sl" id="sl"></div>
</div>

<!-- INDICATORS -->

<div class="pg" id="pg-inds">
  <div class="bkh">
    <button class="bkb" id="bk-inds">←</button>
    <div><div class="bkt" id="inds-t"></div><div class="bks" id="inds-s"></div></div>
  </div>
  <div class="il" id="il"></div>
</div>

<!-- DETAIL -->

<div class="pg" id="pg-det">
  <div class="bkh">
    <button class="bkb" id="bk-det">←</button>
    <div><div class="dtc" id="det-code"></div><div class="dttl" id="det-title"></div></div>
  </div>
  <div class="tabs">
    <button class="tab on" data-t="map"><span class="ti">🗺️</span>خارطة الطريق</button>
    <button class="tab" data-t="docs"><span class="ti">📁</span>الوثائق المطلوبة</button>
    <button class="tab" data-t="eval"><span class="ti">🔧</span>أدوات التقويم</button>
  </div>
  <div class="tp on" id="tp-map">
    <div class="svr" id="svr"></div>
    <div class="steps-list" id="steps-list"></div>
  </div>
  <div class="tp" id="tp-docs">
    <div class="thint"><span>📎</span>الوثائق المطلوبة لإثبات تحقق هذا المؤشر</div>
    <div class="dl" id="dl"></div>
  </div>
  <div class="tp" id="tp-eval">
    <div class="thint"><span>🔬</span>أدوات التقويم المقترحة لهذا المؤشر</div>
    <div class="el" id="el"></div>
  </div>
</div>

<script>
/* ════════════════ DATA ════════════════ */
var DB=[
 {id:'d1',em:'🏫',num:'المجال الأول',ti:'الإدارة المدرسية',
  ds:'تركز عمليات الإدارة المدرسية على التأثير الفاعل في المجتمع المدرسي لتحقيق مستويات متقدمة في الأداء المتميز.',
  stds:[
   {id:'s1',num:'1',ti:'القيادة والحوكمة المدرسية',inds:[
    {id:'i1',co:'(١-١-١)',ti:'توظف البيانات والمعلومات في اتخاذ القرارات الإدارية والتربوية',
     sv:['استبانة المعلمين','استبانة المتعلمين','استبانة الأسرة','الملاحظة الصفية'],
     nd:[{id:'c',cl:'center',tx:'توظيف البيانات\nفي اتخاذ القرارات'},
         {id:'1',cl:'c1',tx:'جمع البيانات\nمن جميع المصادر',dt:'رصد بيانات التحصيل والحضور والسلوك وتغذية راجعة المعلمين والطلاب والأسر بانتظام.'},
         {id:'2',cl:'c2',tx:'تحليل البيانات\nوتفسيرها',dt:'قراءة البيانات وتحليلها كمياً ونوعياً لاستخلاص الأنماط والفجوات وفرص التحسين.'},
         {id:'3',cl:'c3',tx:'إشراك أصحاب\nالمصلحة',dt:'عرض نتائج التحليل على الفريق الإداري والمعلمين وأولياء الأمور للاستئناس بآرائهم.'},
         {id:'4',cl:'c4',tx:'اتخاذ قرارات\nمبنية على الأدلة',dt:'صياغة قرارات وإجراءات مستندة إلى نتائج التحليل ومعطيات الواقع.'},
         {id:'5',cl:'c5',tx:'توثيق القرارات\nومتابعة التنفيذ',dt:'تسجيل القرارات وجدول التنفيذ والمسؤوليات ومراجعة الأثر دورياً.'},
         {id:'6',cl:'c6',tx:'تقويم الأثر\nوالمراجعة',dt:'قياس مدى تحقق الأهداف بعد تنفيذ القرارات وإجراء التعديلات اللازمة.'}],
     eg:[['1','c'],['2','c'],['3','c'],['4','c'],['5','c'],['6','c']],
     dc:[{ic:'📊',ti:'لوحة بيانات المدرسة',sb:'تقارير تحصيل ربع سنوية'},
         {ic:'📋',ti:'محاضر اجتماعات مجلس المدرسة',sb:'قرارات مبنية على البيانات'},
         {ic:'📁',ti:'سجل القرارات الإدارية',sb:'توثيق مع مسوغات وأدلة'},
         {ic:'📈',ti:'تقرير تتبع مؤشرات الأداء',sb:'مراجعة دورية شهرية'}],
     ev:[{ic:'🔍',bg:'#F5EDD6',ti:'الملاحظة الميدانية',sb:'مراقبة ممارسات القيادة في اتخاذ القرار'},
         {ic:'📝',bg:'#EDE0C4',ti:'مراجعة الوثائق',sb:'فحص سجلات البيانات والقرارات الموثقة'},
         {ic:'💬',bg:'#FBF6EC',ti:'المقابلة المنظمة',sb:'مقابلة القيادة والمعلمين'},
         {ic:'📊',bg:'#F5EDD6',ti:'استبانة',sb:'قياس مدى توظيف البيانات في القرارات'}]},
    {id:'i2',co:'(١-١-٢)',ti:'تتبنى الإدارة ثقافة التحسين المستمر وتنعكس على الممارسات اليومية',
     sv:['استبانة المعلمين','الملاحظة الصفية'],
     nd:[{id:'c',cl:'center',tx:'ثقافة التحسين\nالمستمر'},
         {id:'1',cl:'c1',tx:'تشخيص الواقع\nوتحديد الفجوات',dt:'إجراء مسح شامل للممارسات الحالية وتحديد مجالات التطوير.'},
         {id:'2',cl:'c2',tx:'بناء رؤية\nمشتركة للتطوير',dt:'إشراك الفريق في تحديد التوجهات التطويرية وترسيخ ثقافة التحسين.'},
         {id:'3',cl:'c3',tx:'تطبيق دورة\nالتحسين PDCA',dt:'تخطيط وتنفيذ وتقييم ومراجعة دورات التحسين بشكل منتظم.'},
         {id:'4',cl:'c4',tx:'الاحتفاء بالتحسن\nومكافأته',dt:'تعزيز الإنجازات التطويرية ومكافأة المبادرين بالتحسين.'},
         {id:'5',cl:'c5',tx:'التعلم من\nالممارسات الناجحة',dt:'توثيق التجارب الناجحة ونشرها وتعميمها على المدرسة.'}],
     eg:[['1','c'],['2','c'],['3','c'],['4','c'],['5','c']],
     dc:[{ic:'📄',ti:'خطة التحسين المدرسية',sb:'أهداف وإجراءات وجداول زمنية'},
         {ic:'📝',ti:'تقارير المتابعة الشهرية',sb:'مؤشرات قياس التحسين'},
         {ic:'🏆',ti:'سجل الممارسات الجيدة',sb:'توثيق التجارب الناجحة'}],
     ev:[{ic:'👁️',bg:'#F5EDD6',ti:'الملاحظة الميدانية',sb:'رصد مؤشرات ثقافة التحسين'},
         {ic:'📝',bg:'#EDE0C4',ti:'مراجعة وثائق الخطط',sb:'فحص خطط التطوير ومتابعة تنفيذها'},
         {ic:'💬',bg:'#FBF6EC',ti:'مجموعات النقاش',sb:'حوار مع المعلمين حول ثقافة التحسين'}]},
    {id:'i3',co:'(١-١-٣)',ti:'يطبق نظام فاعل للمساءلة والمتابعة لضمان تحقيق الأهداف',
     sv:['استبانة المعلمين','مراجعة الوثائق'],
     nd:[{id:'c',cl:'center',tx:'نظام المساءلة\nوالمتابعة الفاعل'},
         {id:'1',cl:'c1',tx:'تحديد المسؤوليات\nبوضوح',dt:'توصيف واضح للأدوار والصلاحيات والمساءلة لكل عضو في الفريق.'},
         {id:'2',cl:'c2',tx:'وضع مؤشرات\nأداء واضحة',dt:'تحديد KPIs قابلة للقياس لكل مهمة وهدف مدرسي.'},
         {id:'3',cl:'c3',tx:'جدولة المتابعة\nالدورية',dt:'اجتماعات وزيارات متابعة منتظمة للتحقق من سير التنفيذ.'},
         {id:'4',cl:'c4',tx:'التغذية الراجعة\nالبنّاءة',dt:'تقديم ملاحظات بنّاءة ودعم تطويري للمتابَعين.'},
         {id:'5',cl:'c5',tx:'التوثيق والشفافية',dt:'توثيق نتائج المتابعة ومشاركتها مع الفريق بشفافية.'}],
     eg:[['1','c'],['2','c'],['3','c'],['4','c'],['5','c']],
     dc:[{ic:'📋',ti:'نماذج المتابعة الميدانية',sb:'زيارات صفية وإدارية موثقة'},
         {ic:'📊',ti:'تقرير الأداء الدوري',sb:'ربع سنوي / شهري'},
         {ic:'📁',ti:'ملفات الموظفين التطويرية',sb:'أهداف وخطط أداء فردية'}],
     ev:[{ic:'📝',bg:'#F5EDD6',ti:'مراجعة السجلات',sb:'فحص وثائق المتابعة والتقارير'},
         {ic:'💬',bg:'#EDE0C4',ti:'مقابلات القيادة',sb:'قياس مدى تطبيق نظام المساءلة'},
         {ic:'📊',bg:'#FBF6EC',ti:'استبانة المعلمين',sb:'قياس الشعور بالعدالة والوضوح'}]}
   ]},
   {id:'s2',num:'2',ti:'التخطيط الاستراتيجي',inds:[
    {id:'i4',co:'(١-٢-١)',ti:'تمتلك المدرسة خطة تطوير مدرسية قائمة على التحليل الدقيق للواقع',
     sv:['مراجعة الوثائق','استبانة المعلمين','استبانة الأسرة'],
     nd:[{id:'c',cl:'center',tx:'خطة التطوير\nالمدرسية'},
         {id:'1',cl:'c1',tx:'تحليل SWOT\nللواقع المدرسي',dt:'تحليل نقاط القوة والضعف والفرص والتحديات في البيئة المدرسية.'},
         {id:'2',cl:'c2',tx:'إشراك جميع\nالمعنيين',dt:'ورش عمل مع المعلمين وأولياء الأمور والطلاب لبناء الخطة.'},
         {id:'3',cl:'c3',tx:'صياغة أهداف\nSMART',dt:'أهداف محددة وقابلة للقياس وواقعية ومحددة زمنياً.'},
         {id:'4',cl:'c4',tx:'خطة تنفيذ\nتفصيلية',dt:'جدول زمني وموارد ومسؤوليات واضحة لكل هدف.'},
         {id:'5',cl:'c5',tx:'مراجعة سنوية\nوتحديث الخطة',dt:'تقييم الإنجازات وتحديث الخطة في ضوء المستجدات.'}],
     eg:[['1','c'],['2','c'],['3','c'],['4','c'],['5','c']],
     dc:[{ic:'📘',ti:'الخطة الاستراتيجية للمدرسة',sb:'3 سنوات مع مؤشرات قياس'},
         {ic:'📄',ti:'تقرير التحليل البيئي',sb:'SWOT مع توثيق البيانات'},
         {ic:'📋',ti:'محاضر ورش بناء الخطة',sb:'إشراك جميع الأطراف'}],
     ev:[{ic:'📝',bg:'#F5EDD6',ti:'مراجعة الخطة الاستراتيجية',sb:'جودة الأهداف والتحليل'},
         {ic:'💬',bg:'#EDE0C4',ti:'مقابلات القيادة والمعلمين',sb:'مدى الفهم المشترك للخطة'},
         {ic:'📊',bg:'#FBF6EC',ti:'قياس نسبة الإنجاز',sb:'مقارنة بمؤشرات الخطة'}]},
    {id:'i5',co:'(١-٢-٢)',ti:'تراجع الخطة وتحدث بصورة منتظمة في ضوء نتائج التقويم',
     sv:['مراجعة الوثائق','استبانة المعلمين'],
     nd:[{id:'c',cl:'center',tx:'مراجعة وتحديث\nالخطة'},
         {id:'1',cl:'c1',tx:'جمع بيانات\nالتقويم الدوري',dt:'رصد نتائج المؤشرات والتقييمات والزيارات الميدانية.'},
         {id:'2',cl:'c2',tx:'تحليل الفجوات\nوالإنجازات',dt:'مقارنة الواقع بالمستهدف وتحديد ما تحقق وما لم يتحقق.'},
         {id:'3',cl:'c3',tx:'ورشة مراجعة\nمشتركة',dt:'اجتماع الفريق القيادي لمناقشة النتائج واتخاذ القرارات التصحيحية.'},
         {id:'4',cl:'c4',tx:'تعديل الأهداف\nوالإجراءات',dt:'مراجعة الأهداف وتعديلها وفق المستجدات والمتغيرات.'},
         {id:'5',cl:'c5',tx:'توثيق التعديلات\nوإبلاغ الفريق',dt:'توثيق التغييرات وإبلاغ جميع المعنيين بالتحديثات.'}],
     eg:[['1','c'],['2','c'],['3','c'],['4','c'],['5','c']],
     dc:[{ic:'📋',ti:'تقارير مراجعة الخطة',sb:'نصف سنوي وسنوي'},
         {ic:'📝',ti:'نسخ الخطة المحدثة',sb:'مؤرخة مع سجل التعديلات'}],
     ev:[{ic:'📝',bg:'#F5EDD6',ti:'مراجعة وثائق التحديث',sb:'فحص سجلات تطور الخطة'},
         {ic:'💬',bg:'#EDE0C4',ti:'مقابلات الفريق القيادي',sb:'استيعاب آليات المراجعة'}]}
   ]},
   {id:'s3',num:'3',ti:'التنمية المهنية للمعلمين',inds:[
    {id:'i6',co:'(١-٣-١)',ti:'تبنى برامج التنمية المهنية على تشخيص الاحتياجات الفعلية للمعلمين',
     sv:['استبانة المعلمين','الملاحظة الصفية','مراجعة الوثائق'],
     nd:[{id:'c',cl:'center',tx:'برامج التنمية\nالمهنية'},
         {id:'1',cl:'c1',tx:'تشخيص احتياجات\nالمعلمين',dt:'استبانات وملاحظات صفية ومقابلات لرصد الاحتياجات التدريبية الفعلية.'},
         {id:'2',cl:'c2',tx:'تصميم برامج\nهادفة',dt:'تصميم برامج تدريبية مرتبطة مباشرة بالاحتياجات المشخصة.'},
         {id:'3',cl:'c3',tx:'تنفيذ التدريب\nبكفاءة',dt:'تقديم التدريب بأساليب متنوعة وعملية مع ضمان جودة التنفيذ.'},
         {id:'4',cl:'c4',tx:'قياس أثر التدريب\nعلى الممارسة',dt:'متابعة ميدانية بعد التدريب للتحقق من انعكاسه على الفصل الدراسي.'},
         {id:'5',cl:'c5',tx:'تحسين البرامج\nباستمرار',dt:'تطوير برامج التنمية في ضوء التغذية الراجعة ونتائج قياس الأثر.'}],
     eg:[['1','c'],['2','c'],['3','c'],['4','c'],['5','c']],
     dc:[{ic:'📊',ti:'تقرير تشخيص الاحتياجات التدريبية',sb:'بيانات كل معلم'},
         {ic:'📋',ti:'الخطة التدريبية السنوية',sb:'مرتبطة بالاحتياجات'},
         {ic:'📁',ti:'ملفات التنمية المهنية للمعلمين',sb:'سجل التدريب والأثر'}],
     ev:[{ic:'📝',bg:'#F5EDD6',ti:'استبانة المعلمين',sb:'قياس مدى ملاءمة التدريب للاحتياجات'},
         {ic:'👁️',bg:'#EDE0C4',ti:'الملاحظة الصفية',sb:'قياس أثر التدريب على التدريس'},
         {ic:'💬',bg:'#FBF6EC',ti:'مقابلات المعلمين',sb:'استيضاح تجربة التنمية المهنية'}]}
   ]},
   {id:'s4',num:'4',ti:'الشراكة مع الأسرة والمجتمع',inds:[
    {id:'i7',co:'(١-٤-١)',ti:'توجد قنوات تواصل فاعلة ومنتظمة مع أسر الطلاب',
     sv:['استبانة الأسرة','استبانة المعلمين'],
     nd:[{id:'c',cl:'center',tx:'قنوات التواصل\nمع الأسرة'},
         {id:'1',cl:'c1',tx:'تحديد قنوات\nالتواصل المناسبة',dt:'اختيار قنوات رقمية وتقليدية تناسب طبيعة الأسر وإمكاناتها.'},
         {id:'2',cl:'c2',tx:'بناء خطة\nتواصل سنوية',dt:'جدولة اللقاءات والاجتماعات والتواصل الدوري طوال العام.'},
         {id:'3',cl:'c3',tx:'تفعيل مجلس\nأولياء الأمور',dt:'اجتماعات منتظمة ومشاركة حقيقية في القرارات المدرسية.'},
         {id:'4',cl:'c4',tx:'التغذية الراجعة\nمن الأسر',dt:'استطلاع رأي الأسر دورياً وتوظيفه في التطوير.'},
         {id:'5',cl:'c5',tx:'التواصل في\nحالات الطوارئ',dt:'بروتوكولات تواصل فوري وفاعل مع الأسر عند الحاجة.'}],
     eg:[['1','c'],['2','c'],['3','c'],['4','c'],['5','c']],
     dc:[{ic:'📱',ti:'سجل قنوات التواصل',sb:'مجموعات واتساب، منصة مدرستي'},
         {ic:'📋',ti:'محاضر اجتماعات أولياء الأمور',sb:'دورية ومنتظمة'},
         {ic:'📊',ti:'نتائج استطلاع رضا الأسر',sb:'سنوي ونصف سنوي'}],
     ev:[{ic:'📊',bg:'#F5EDD6',ti:'استبانة الأسرة',sb:'قياس رضا الأسر عن التواصل'},
         {ic:'📝',bg:'#EDE0C4',ti:'مراجعة سجلات التواصل',sb:'فحص وثائق الاتصال'},
         {ic:'💬',bg:'#FBF6EC',ti:'مقابلات أولياء الأمور',sb:'آراؤهم حول فاعلية التواصل'}]}
   ]},
   {id:'s5',num:'5',ti:'حماية حقوق المتعلمين',inds:[
    {id:'i8',co:'(١-٥-١)',ti:'تطبق سياسات واضحة تصون كرامة الطلاب وحقوقهم كافة',
     sv:['استبانة المتعلمين','استبانة الأسرة','الملاحظة الصفية'],
     nd:[{id:'c',cl:'center',tx:'سياسات حماية\nحقوق المتعلمين'},
         {id:'1',cl:'c1',tx:'إعداد ميثاق\nحقوق الطالب',dt:'وثيقة واضحة تحدد حقوق الطلاب وتنشر على الجميع.'},
         {id:'2',cl:'c2',tx:'توعية الطلاب\nبحقوقهم',dt:'برامج توعية منتظمة تعرّف الطلاب بحقوقهم وواجباتهم.'},
         {id:'3',cl:'c3',tx:'آليات الإبلاغ\nعن الانتهاكات',dt:'قنوات آمنة وسرية للإبلاغ عن أي انتهاك لحقوق الطلاب.'},
         {id:'4',cl:'c4',tx:'التحقيق والمعالجة\nالسريعة',dt:'إجراءات واضحة للتحقيق في البلاغات ومعالجتها بسرعة وعدالة.'},
         {id:'5',cl:'c5',tx:'التقويم والتحسين\nالمستمر',dt:'مراجعة دورية للسياسات وتطويرها استناداً إلى الواقع والممارسة.'}],
     eg:[['1','c'],['2','c'],['3','c'],['4','c'],['5','c']],
     dc:[{ic:'📜',ti:'ميثاق حقوق الطالب',sb:'موقع ومعتمد وموزع'},
         {ic:'📁',ti:'سجل البلاغات والشكاوى',sb:'مع إجراءات المعالجة'},
         {ic:'📊',ti:'تقرير رضا الطلاب',sb:'قياس شعورهم بالأمان والعدالة'}],
     ev:[{ic:'📊',bg:'#F5EDD6',ti:'استبانة الطلاب',sb:'قياس الشعور بالأمان والعدالة'},
         {ic:'👁️',bg:'#EDE0C4',ti:'الملاحظة الميدانية',sb:'رصد التفاعلات والسلوكيات'},
         {ic:'💬',bg:'#FBF6EC',ti:'مجموعات نقاش الطلاب',sb:'استيضاح مدى معرفتهم بحقوقهم'}]}
   ]}
  ]},
 {id:'d2',em:'📚',num:'المجال الثاني',ti:'التعليم والتعلم',
  ds:'يركز هذا المجال على جودة العمليات التعليمية داخل الفصول وبناء خبرات تعلم فاعلة تلبي احتياجات جميع المتعلمين.',
  stds:[
   {id:'s6',num:'6',ti:'جودة التدريس',inds:[
    {id:'i9',co:'(٢-٦-١)',ti:'يصمم التعلم وفق أهداف واضحة مرتبطة بالمناهج الدراسية',
     sv:['الملاحظة الصفية','مراجعة الوثائق'],
     nd:[{id:'c',cl:'center',tx:'تصميم التعلم\nبأهداف واضحة'},
         {id:'1',cl:'c1',tx:'تحليل المنهج\nوتحديد المخرجات',dt:'دراسة معايير المنهج وتحديد نواتج التعلم المستهدفة بدقة.'},
         {id:'2',cl:'c2',tx:'صياغة أهداف\nSMART',dt:'كتابة أهداف محددة وقابلة للملاحظة والقياس لكل درس.'},
         {id:'3',cl:'c3',tx:'اختيار استراتيجيات\nمناسبة',dt:'انتقاء طرائق وأساليب تدريس تحقق الأهداف بأعلى كفاءة.'},
         {id:'4',cl:'c4',tx:'تصميم أنشطة\nمتنوعة ومتدرجة',dt:'أنشطة تراعي التدرج في الصعوبة وأنماط التعلم المختلفة.'},
         {id:'5',cl:'c5',tx:'بناء أدوات\nتقويم مرتبطة',dt:'ربط التقويم بالأهداف لضمان قياس ما تم تعليمه فعلاً.'}],
     eg:[['1','c'],['2','c'],['3','c'],['4','c'],['5','c']],
     dc:[{ic:'📘',ti:'خطط الدروس اليومية',sb:'أهداف واضحة وأنشطة'},
         {ic:'📋',ti:'تحضير المعلم',sb:'مرتبط بمعايير المنهج'}],
     ev:[{ic:'👁️',bg:'#F5EDD6',ti:'الملاحظة الصفية',sb:'مراقبة وضوح الأهداف في الدرس'},
         {ic:'📝',bg:'#EDE0C4',ti:'مراجعة التحضير',sb:'فحص جودة صياغة الأهداف'}]},
    {id:'i10',co:'(٢-٦-٢)',ti:'تستخدم استراتيجيات تدريس متنوعة تناسب أنماط المتعلمين المختلفة',
     sv:['الملاحظة الصفية','استبانة المتعلمين'],
     nd:[{id:'c',cl:'center',tx:'تنويع\nاستراتيجيات التدريس'},
         {id:'1',cl:'c1',tx:'تشخيص أنماط\nتعلم الطلاب',dt:'تحديد أنماط التعلم البصري والسمعي والحركي لدى الطلاب.'},
         {id:'2',cl:'c2',tx:'التعلم التعاوني\nوالتفاعلي',dt:'مجموعات العمل والنقاش والمشاريع الجماعية.'},
         {id:'3',cl:'c3',tx:'التعلم الاستقصائي\nوحل المشكلات',dt:'أنشطة تتحدى الطلاب للبحث والاستقصاء والاكتشاف.'},
         {id:'4',cl:'c4',tx:'توظيف التقنية\nوالوسائل',dt:'استخدام الفيديو والمحاكاة والتطبيقات التفاعلية.'},
         {id:'5',cl:'c5',tx:'التقويم المستمر\nللاستراتيجيات',dt:'رصد فاعلية كل استراتيجية وتعديلها حسب الحاجة.'}],
     eg:[['1','c'],['2','c'],['3','c'],['4','c'],['5','c']],
     dc:[{ic:'📋',ti:'بطاقة ملاحظة التنويع الصفي',sb:'رصد استراتيجيات التدريس'}],
     ev:[{ic:'👁️',bg:'#F5EDD6',ti:'الملاحظة الصفية',sb:'رصد تنوع الاستراتيجيات'},
         {ic:'📊',bg:'#EDE0C4',ti:'استبانة الطلاب',sb:'مدى ملاءمة الأساليب لأنماطهم'}]}
   ]},
   {id:'s7',num:'7',ti:'التقويم وتحسين نواتج التعلم',inds:[
    {id:'i11',co:'(٢-٧-١)',ti:'توظف أساليب تقويم متنوعة تشمل التقويم التكويني والختامي',
     sv:['الملاحظة الصفية','مراجعة الوثائق','استبانة المعلمين'],
     nd:[{id:'c',cl:'center',tx:'تنويع أساليب\nالتقويم'},
         {id:'1',cl:'c1',tx:'التقويم التشخيصي\nقبل التعلم',dt:'اختبارات قبلية وأسئلة استكشافية لمعرفة المستوى الأولي.'},
         {id:'2',cl:'c2',tx:'التقويم التكويني\nأثناء التعلم',dt:'أسئلة شفهية وبطاقات خروج وملاحظات فورية.'},
         {id:'3',cl:'c3',tx:'التقويم الختامي\nبعد التعلم',dt:'اختبارات وتقارير ومشاريع لقياس تحقق الأهداف.'},
         {id:'4',cl:'c4',tx:'التقويم الأدائي\nوالأصيل',dt:'ملاحظة الأداء الحقيقي في السياقات الواقعية.'},
         {id:'5',cl:'c5',tx:'تحليل النتائج\nوالعمل بها',dt:'استخدام نتائج التقويم لتعديل التدريس ودعم الطلاب.'}],
     eg:[['1','c'],['2','c'],['3','c'],['4','c'],['5','c']],
     dc:[{ic:'📊',ti:'سجل نتائج التقويم',sb:'تكويني وختامي'},
         {ic:'📋',ti:'نماذج التقويم المستخدمة',sb:'متنوعة ومرتبطة بالأهداف'}],
     ev:[{ic:'👁️',bg:'#F5EDD6',ti:'الملاحظة الصفية',sb:'رصد ممارسات التقويم'},
         {ic:'📝',bg:'#EDE0C4',ti:'مراجعة سجلات التقويم',sb:'فحص تنوع الأساليب'}]}
   ]}
  ]},
 {id:'d3',em:'🎯',num:'المجال الثالث',ti:'نواتج التعلم',
  ds:'يشمل هذا المجال مستوى تحصيل المتعلمين الأكاديمي ومدى تطورهم الشخصي والاجتماعي.',
  stds:[
   {id:'s8',num:'8',ti:'التحصيل الأكاديمي',inds:[
    {id:'i12',co:'(٣-٨-١)',ti:'يحقق الطلاب مستويات الكفاءة المتوقعة في المهارات الأساسية',
     sv:['استبانة المعلمين','مراجعة الوثائق','الملاحظة الصفية'],
     nd:[{id:'c',cl:'center',tx:'تحقيق مستويات\nالكفاءة الأساسية'},
         {id:'1',cl:'c1',tx:'تحديد مستويات\nالكفاءة المستهدفة',dt:'تحديد مستويات الإتقان المتوقعة لكل مرحلة دراسية.'},
         {id:'2',cl:'c2',tx:'قياس المستوى\nالحالي للطلاب',dt:'اختبارات تشخيصية دورية لمعرفة مستوى كل طالب.'},
         {id:'3',cl:'c3',tx:'برامج الدعم\nوالتحسين',dt:'تدخلات هادفة للطلاب دون المستوى المطلوب.'},
         {id:'4',cl:'c4',tx:'إثراء الطلاب\nالمتفوقين',dt:'أنشطة وبرامج إثرائية للطلاب المتميزين.'},
         {id:'5',cl:'c5',tx:'متابعة التقدم\nوالرفع التدريجي',dt:'رصد التحسن الفردي وتوثيقه بانتظام.'}],
     eg:[['1','c'],['2','c'],['3','c'],['4','c'],['5','c']],
     dc:[{ic:'📊',ti:'تقارير التحصيل الدراسي',sb:'مقارنة بالمعيار الوطني'},
         {ic:'📁',ti:'سجلات الدعم الفردي',sb:'خطط دعم لكل طالب محتاج'}],
     ev:[{ic:'📊',bg:'#F5EDD6',ti:'تحليل نتائج الاختبارات',sb:'مقارنة بالمعيار الوطني'},
         {ic:'📝',bg:'#EDE0C4',ti:'مراجعة سجلات الطلاب',sb:'رصد التقدم الفردي'}]}
   ]},
   {id:'s9',num:'9',ti:'التطور الشخصي والاجتماعي',inds:[
    {id:'i13',co:'(٣-٩-١)',ti:'يبدي الطلاب قيماً إيجابية وسلوكاً مسؤولاً داخل المدرسة وخارجها',
     sv:['استبانة المتعلمين','استبانة الأسرة','الملاحظة الصفية'],
     nd:[{id:'c',cl:'center',tx:'القيم الإيجابية\nوالسلوك المسؤول'},
         {id:'1',cl:'c1',tx:'تضمين القيم\nفي المنهج',dt:'دمج القيم الإسلامية والوطنية في محتوى المواد الدراسية.'},
         {id:'2',cl:'c2',tx:'النمذجة والقدوة\nمن المعلمين',dt:'التزام المعلمين بالقيم وتجسيدها أمام الطلاب.'},
         {id:'3',cl:'c3',tx:'الأنشطة التطوعية\nوالمجتمعية',dt:'مشاركة الطلاب في أعمال خير ومبادرات مجتمعية.'},
         {id:'4',cl:'c4',tx:'التعزيز الإيجابي\nللسلوك الحسن',dt:'مكافأة السلوكيات الإيجابية وتعزيزها باستمرار.'},
         {id:'5',cl:'c5',tx:'قياس السلوك\nومتابعته',dt:'رصد مؤشرات السلوك وتوثيق التحسن الملاحظ.'}],
     eg:[['1','c'],['2','c'],['3','c'],['4','c'],['5','c']],
     dc:[{ic:'📋',ti:'سجل السلوك المدرسي',sb:'إيجابيات وتصحيح'},
         {ic:'📊',ti:'تقرير الأنشطة التطوعية',sb:'مشاركة الطلاب'}],
     ev:[{ic:'👁️',bg:'#F5EDD6',ti:'الملاحظة الميدانية',sb:'رصد السلوكيات اليومية'},
         {ic:'📊',bg:'#EDE0C4',ti:'استبانة الأسرة',sb:'قياس القيم المنعكسة في البيت'}]}
   ]}
  ]},
 {id:'d4',em:'🏗️',num:'المجال الرابع',ti:'البيئة المدرسية',
  ds:'يشمل جودة المبنى المدرسي ومتطلبات الأمن والسلامة بوصفهما ركيزتين لبيئة تعلم ملائمة وآمنة.',
  stds:[
   {id:'s10',num:'10',ti:'الأمن والسلامة',inds:[
    {id:'i14',co:'(٤-١٠-١)',ti:'تتوافر اشتراطات السلامة والأمن في المبنى المدرسي وفق المعايير',
     sv:['الملاحظة الميدانية','مراجعة الوثائق'],
     nd:[{id:'c',cl:'center',tx:'اشتراطات الأمن\nوالسلامة'},
         {id:'1',cl:'c1',tx:'مسح شامل\nللمبنى',dt:'فحص جميع مرافق المدرسة وتوثيق حالة السلامة.'},
         {id:'2',cl:'c2',tx:'إزالة المخاطر\nالموجودة',dt:'معالجة فورية لجميع مصادر الخطر المرصودة.'},
         {id:'3',cl:'c3',tx:'تركيب أنظمة\nالسلامة',dt:'كاميرات وطفايات وأبواب طوارئ وإضاءة سلامة.'},
         {id:'4',cl:'c4',tx:'التدريب على\nالطوارئ',dt:'تدريبات دورية للطلاب والمعلمين على الإخلاء والطوارئ.'},
         {id:'5',cl:'c5',tx:'الصيانة الدورية\nوالمراجعة',dt:'جدولة الصيانة الوقائية ومراجعة المنظومة الأمنية دورياً.'}],
     eg:[['1','c'],['2','c'],['3','c'],['4','c'],['5','c']],
     dc:[{ic:'🏗️',ti:'تقرير السلامة السنوي',sb:'مطابقة للمعايير الوطنية'},
         {ic:'📋',ti:'سجل تمارين الإخلاء',sb:'تواريخ ونتائج'}],
     ev:[{ic:'👁️',bg:'#F5EDD6',ti:'الجولة التفتيشية',sb:'فحص مرافق السلامة'},
         {ic:'📝',bg:'#EDE0C4',ti:'مراجعة سجلات السلامة',sb:'التحقق من الامتثال للمعايير'}]}
   ]},
   {id:'s11',num:'11',ti:'جودة المرافق والموارد',inds:[
    {id:'i15',co:'(٤-١١-١)',ti:'تتوافر مرافق وموارد تعليمية كافية تدعم التعلم الفاعل',
     sv:['استبانة المعلمين','استبانة المتعلمين','مراجعة الوثائق'],
     nd:[{id:'c',cl:'center',tx:'المرافق والموارد\nالتعليمية'},
         {id:'1',cl:'c1',tx:'تقييم المرافق\nالحالية',dt:'حصر شامل للمرافق والموارد المتاحة وتقييم حالتها.'},
         {id:'2',cl:'c2',tx:'تحديد الاحتياجات\nوالفجوات',dt:'مقارنة المتاح بالمطلوب وتحديد الأولويات.'},
         {id:'3',cl:'c3',tx:'تطوير المرافق\nالقائمة',dt:'تحديث المختبرات والمكتبة وقاعات الحاسب.'},
         {id:'4',cl:'c4',tx:'توفير الموارد\nالرقمية',dt:'منصات رقمية وأجهزة ووسائل تعليمية تقنية.'},
         {id:'5',cl:'c5',tx:'صيانة المرافق\nوتطويرها',dt:'جدولة الصيانة المنتظمة وخطة الاستدامة.'}],
     eg:[['1','c'],['2','c'],['3','c'],['4','c'],['5','c']],
     dc:[{ic:'📊',ti:'كشف الموارد التعليمية',sb:'جرد سنوي شامل'},
         {ic:'📋',ti:'خطة تطوير المرافق',sb:'أولويات وجداول زمنية'}],
     ev:[{ic:'👁️',bg:'#F5EDD6',ti:'الجولة الميدانية',sb:'فحص حالة المرافق'},
         {ic:'📊',bg:'#EDE0C4',ti:'استبانة المعلمين',sb:'كفاية الموارد للعملية التعليمية'}]}
   ]}
  ]}
];

/* ════════════════ HELPERS ════════════════ */
var cD=null, cS=null;

function show(id){
  document.querySelectorAll('.pg').forEach(function(p){p.classList.remove('on');});
  document.getElementById('pg-'+id).classList.add('on');
  window.scrollTo({top:0,behavior:'smooth'});
}

function bc(html){ document.getElementById('bc').innerHTML=html; }

/* ════════════════ NAVIGATION ════════════════ */
function goHome(){
  bc('<b>الرئيسية</b>');
  show('home');
}

function goDomains(){
  bc('<a onclick="goHome()">الرئيسية</a><s>‹</s><b>المجالات</b>');
  var g=document.getElementById('dgr');
  g.innerHTML=DB.map(function(d,i){
    var tot=d.stds.reduce(function(a,s){return a+s.inds.length;},0);
    return '<div class="dc" onclick="goStds('+i+')">'
      +'<div class="dn">'+d.num+'</div>'
      +'<span class="de">'+d.em+'</span>'
      +'<div class="dtt">'+d.ti+'</div>'
      +'<div class="dds">'+d.ds+'</div>'
      +'<div class="dba"><span class="badge">📋 '+d.stds.length+' معايير</span>'
      +'<span class="badge">🎯 '+tot+' مؤشراً</span></div>'
      +'<div class="dgo">استعرض المجال ←</div>'
      +'</div>';
  }).join('');
  show('domains');
}

function goStds(di){
  cD=DB[di];
  bc('<a onclick="goHome()">الرئيسية</a><s>‹</s><a onclick="goDomains()">المجالات</a><s>‹</s><b>'+cD.ti+'</b>');
  document.getElementById('stds-t').textContent=cD.ti;
  document.getElementById('stds-s').textContent=cD.stds.length+' معايير';
  document.getElementById('bk-stds').setAttribute('onclick','goDomains()');
  document.getElementById('sl').innerHTML=cD.stds.map(function(s,i){
    return '<div class="si" onclick="goInds('+i+')">'
      +'<div class="sii">'
      +'<div class="sc">'+s.num+'</div>'
      +'<div style="flex:1"><div class="stit">'+s.ti+'</div><div class="sme">'+s.inds.length+' مؤشر</div></div>'
      +'<div class="sar">←</div>'
      +'</div></div>';
  }).join('');
  show('stds');
}

function goInds(si){
  cS=cD.stds[si];
  var di=DB.indexOf(cD);
  bc('<a onclick="goHome()">الرئيسية</a><s>‹</s><a onclick="goDomains()">المجالات</a><s>‹</s><a onclick="goStds('+di+')">'+cD.ti+'</a><s>‹</s><b>'+cS.ti+'</b>');
  document.getElementById('inds-t').textContent=cS.ti;
  document.getElementById('inds-s').textContent=cS.inds.length+' مؤشرات';
  document.getElementById('bk-inds').setAttribute('onclick','goStds('+di+')');
  document.getElementById('il').innerHTML=cS.inds.map(function(ind,i){
    return '<div class="ii" onclick="goDet('+i+')">'
      +'<div class="iii">'
      +'<div class="ib">'+(i+1)+'</div>'
      +'<div style="flex:1"><div class="ico">'+ind.co+'</div><div class="itx">'+ind.ti+'</div></div>'
      +'<div class="sar">←</div>'
      +'</div>'
      +'<div class="ich">'+ind.sv.map(function(s){return'<span class="chip">'+s+'</span>';}).join('')+'</div>'
      +'</div>';
  }).join('');
  show('inds');
}

function goDet(ii){
  var ind=cS.inds[ii];
  var di=DB.indexOf(cD), si=cD.stds.indexOf(cS);
  bc('<a onclick="goHome()">الرئيسية</a><s>‹</s>…<s>‹</s><a onclick="goInds('+si+')">'+cS.ti+'</a><s>‹</s><b>'+ind.co+'</b>');
  document.getElementById('det-code').textContent=ind.co;
  document.getElementById('det-title').textContent=ind.ti;
  document.getElementById('bk-det').setAttribute('onclick','goInds('+si+')');
  document.getElementById('svr').innerHTML=ind.sv.map(function(s){return'<span class="svc">'+s+'</span>';}).join('');
  // reset tabs
  document.querySelectorAll('.tab').forEach(function(t){t.classList.remove('on');});
  document.querySelectorAll('.tp').forEach(function(p){p.classList.remove('on');});
  document.querySelectorAll('.tab')[0].classList.add('on');
  document.getElementById('tp-map').classList.add('on');
  buildSteps(ind);
  document.getElementById('dl').innerHTML=ind.dc.map(function(d){
    return '<div class="di"><div class="dico">'+d.ic+'</div>'
      +'<div><div class="ditt">'+d.ti+'</div><div class="disb">'+d.sb+'</div></div></div>';
  }).join('');
  document.getElementById('el').innerHTML=ind.ev.map(function(e){
    return '<div class="ei"><div class="dico" style="background:'+e.bg+'">'+e.ic+'</div>'
      +'<div><div class="ditt">'+e.ti+'</div><div class="disb">'+e.sb+'</div></div></div>';
  }).join('');
  show('det');
}

/* ── TABS ── */
document.querySelectorAll('.tab').forEach(function(btn){
  btn.addEventListener('click',function(){
    document.querySelectorAll('.tab').forEach(function(t){t.classList.remove('on');});
    document.querySelectorAll('.tp').forEach(function(p){p.classList.remove('on');});
    btn.classList.add('on');
    document.getElementById('tp-'+btn.dataset.t).classList.add('on');
  });
});

/* ════════════════ STEPS LIST ════════════════ *//* ════════════════ STEPS LIST ════════════════ */
function buildSteps(ind){
  var center=null, steps=[];
  ind.nd.forEach(function(n){
    if(n.id==='c') center=n;
    else steps.push(n);
  });
  // sort by numeric id
  steps.sort(function(a,b){ return parseInt(a.id)-parseInt(b.id); });

  var html='';
  if(center){
    html+='<div style="background:linear-gradient(135deg,var(--gd),var(--gd2));border-radius:14px;padding:16px 20px;margin-bottom:16px;text-align:center;">'
      +'<div style="font-size:15px;font-weight:900;color:#fff;">'+center.tx.replace('\n',' ')+'</div>'
      +'</div>';
  }
  steps.forEach(function(s){
    html+='<div class="step-item">'
      +'<div class="step-num">'+s.id+'</div>'
      +'<div class="step-body">'
      +'<div class="step-title">'+s.tx.replace('\n',' ')+'</div>'
      +(s.dt?'<div class="step-desc">'+s.dt+'</div>':'')
      +'</div></div>';
  });
  document.getElementById('steps-list').innerHTML=html;
}
</script>

</body>
</html>
