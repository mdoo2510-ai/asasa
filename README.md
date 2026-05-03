<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
<meta name="theme-color" content="#0D4842">
<meta name="apple-mobile-app-web-app-capable" content="yes">
<meta name="apple-mobile-app-web-app-status-bar-style" content="black-translucent">
<meta name="apple-mobile-app-web-app-title" content="ثانوية الخرج 8">
<title>النظام الإداري — الثانوية الثامنة بالخرج</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@400;500;700;900&display=swap" rel="stylesheet">
<style>
:root{
--green-900:#0D4842;
--green-700:#1F6B5E;
--green-500:#2D9C87;
--green-50:#E8F4F1;
--blue-900:#1E3A8A;
--blue-700:#2563EB;
--blue-50:#EEF2FF;
--amber-700:#B45309;
--amber-50:#FEF3C7;
--rose-700:#BE123C;
--rose-50:#FFE4E6;
--ink-900:#0F172A;
--ink-700:#334155;
--ink-500:#64748B;
--ink-300:#CBD5E1;
--ink-100:#F1F5F9;
--ink-50:#F8FAFC;
--paper:#FAFAF7;
--white:#FFFFFF;
--shadow-sm:0 1px 2px rgba(15,23,42,.06);
--shadow-md:0 4px 12px rgba(15,23,42,.08);
--shadow-lg:0 10px 30px rgba(15,23,42,.12);
--radius-sm:8px;
--radius-md:14px;
--radius-lg:20px;
}
*{box-sizing:border-box;margin:0;padding:0;-webkit-tap-highlight-color:transparent}
html,body{height:100%}
body{
font-family:'Tajawal',-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif;
background:var(--paper);
color:var(--ink-900);
font-size:16px;
line-height:1.6;
overflow-x:hidden;
padding-bottom:80px;
}
/* === LOGIN SCREEN === */
.login-screen{
display:flex;
align-items:center;
justify-content:center;
min-height:100vh;
padding:20px;
background:linear-gradient(135deg, var(--green-900) 0%, var(--green-700) 100%);
}
.login-card{
background:var(--white);
border-radius:var(--radius-lg);
padding:32px 24px;
width:100%;
max-width:420px;
box-shadow:var(--shadow-lg);
}
.login-card h1{
font-size:24px;
font-weight:900;
color:var(--green-900);
text-align:center;
margin-bottom:6px;
}
.login-card .sub{
text-align:center;
font-size:13px;
color:var(--ink-500);
margin-bottom:24px;
}
.login-card .field{
margin-bottom:16px;
}
.login-card .field label{
display:block;
font-size:13px;
font-weight:700;
color:var(--ink-700);
margin-bottom:6px;
}
.login-card .field input{
width:100%;
padding:14px 14px;
border:1.5px solid var(--ink-300);
border-radius:12px;
font-family:inherit;
font-size:16px;
background:var(--white);
color:var(--ink-900);
font-weight:500;
transition:all .15s;
}
.login-card .field input:focus{
outline:none;
border-color:var(--green-700);
box-shadow:0 0 0 3px rgba(45,156,135,.15);
}
.login-error{
color:var(--rose-700);
font-size:12px;
font-weight:600;
text-align:center;
margin-top:8px;
display:none;
}
.login-error.show{display:block}
/* === TOP BAR === */
.topbar{
background:linear-gradient(135deg,var(--green-900) 0%,var(--green-700) 100%);
color:var(--white);
padding:14px 18px 16px;
box-shadow:var(--shadow-md);
position:sticky;
top:0;
z-index:50;
}
.topbar-row{
display:flex;
align-items:center;
justify-content:space-between;
gap:12px;
}
.topbar-brand{display:flex;align-items:center;gap:10px;min-width:0;flex:1}
.topbar-titles{line-height:1.3;min-width:0}
.topbar-titles .t1{font-size:14px;font-weight:700;opacity:.95;white-space:nowrap;overflow:hidden;text-overflow:ellipsis}
.topbar-titles .t2{font-size:11px;font-weight:500;opacity:.8;margin-top:2px}
.topbar-titles .t3{font-size:12px;font-weight:700;opacity:.95;white-space:nowrap;overflow:hidden;text-overflow:ellipsis}
.topbar-right{display:flex;align-items:center;gap:8px}
.topbar-settings{
width:36px;height:36px;
border-radius:10px;
background:rgba(255,255,255,.12);
border:1px solid rgba(255,255,255,.18);
color:var(--white);
cursor:pointer;
display:grid;place-items:center;
transition:background .15s;
}
.topbar-settings:hover,.topbar-settings:active{background:rgba(255,255,255,.22)}
.topbar-settings svg{width:18px;height:18px}
.topbar-date{
font-size:11px;
background:rgba(255,255,255,.12);
padding:6px 10px;
border-radius:999px;
font-weight:500;
border:1px solid rgba(255,255,255,.18);
white-space:nowrap;
}
.topbar-logout{
width:36px;height:36px;
border-radius:10px;
background:rgba(255,255,255,.12);
border:1px solid rgba(255,255,255,.18);
color:var(--white);
cursor:pointer;
display:grid;place-items:center;
font-size:14px;font-weight:700;
transition:background .15s;
}
/* === SCREEN === */
.screen{display:none;padding:18px 16px 20px;animation:fadeUp .25s ease}
.screen.active{display:block}
@keyframes fadeUp{from{opacity:0;transform:translateY(6px)}to{opacity:1;transform:none}}
.screen-head{
margin-bottom:16px;
}
.screen-head h2{
font-size:22px;font-weight:900;
color:var(--green-900);
letter-spacing:-.02em;
}
.screen-head p{
font-size:13px;color:var(--ink-500);margin-top:2px;
}
/* === FOOTER === */
.app-footer{
text-align:center;
padding:24px 18px 14px;
margin-top:8px;
}
.footer-rule{
width:48px;height:2px;
background:linear-gradient(90deg,transparent 0%,var(--green-500) 50%,transparent 100%);
margin:0 auto 14px;
border-radius:999px;
}
.footer-rights{
font-size:12px;
color:var(--ink-500);
font-weight:600;
letter-spacing:.01em;
opacity:.85;
}
/* === KPI === */
.kpi-grid{
display:grid;
grid-template-columns:repeat(2,1fr);
gap:10px;
margin-bottom:18px;
}
.kpi{
background:var(--white);
border:1px solid var(--ink-100);
border-radius:var(--radius-md);
padding:14px;
box-shadow:var(--shadow-sm);
position:relative;
overflow:hidden;
}
.kpi::before{
content:"";
position:absolute;
inset:0 auto 0 0;
width:4px;
background:var(--green-500);
}
.kpi.k-blue::before{background:var(--blue-700)}
.kpi.k-amber::before{background:#F59E0B}
.kpi.k-rose::before{background:var(--rose-700)}
.kpi-label{font-size:11px;color:var(--ink-500);font-weight:500;margin-bottom:4px}
.kpi-value{font-size:28px;font-weight:900;color:var(--ink-900);line-height:1}
.kpi-sub{font-size:11px;color:var(--ink-500);margin-top:6px}
/* === SECTION CARD === */
.panel{
background:var(--white);
border:1px solid var(--ink-100);
border-radius:var(--radius-md);
padding:16px;
margin-bottom:14px;
box-shadow:var(--shadow-sm);
}
.panel-title{
display:flex;align-items:center;justify-content:space-between;
margin-bottom:12px;
}
.panel-title h3{font-size:15px;font-weight:700;color:var(--green-900)}
.panel-title .meta{font-size:11px;color:var(--ink-500)}
/* === BAR CHART === */
.barchart{display:flex;align-items:flex-end;gap:8px;height:120px;padding-top:10px}
.bar-col{flex:1;display:flex;flex-direction:column;align-items:center;gap:6px;height:100%}
.bar-fill{
width:100%;
background:linear-gradient(180deg,var(--green-500) 0%,var(--green-700) 100%);
border-radius:6px 6px 0 0;
min-height:4px;
position:relative;
transition:height .4s ease;
}
.bar-fill .v{
position:absolute;
top:-18px;left:50%;transform:translateX(-50%);
font-size:11px;font-weight:700;color:var(--ink-700);
}
.bar-label{font-size:11px;color:var(--ink-700);font-weight:600;letter-spacing:-.01em;white-space:nowrap}
/* === LIST ITEM === */
.list-item{
display:flex;align-items:center;gap:10px;
padding:10px 0;
border-bottom:1px solid var(--ink-100);
}
.list-item:last-child{border-bottom:none}
.li-dot{
width:8px;height:8px;border-radius:50%;
background:var(--green-500);flex-shrink:0;
}
.li-dot.amber{background:#F59E0B}
.li-dot.blue{background:var(--blue-700)}
.li-dot.rose{background:var(--rose-700)}
.li-main{flex:1;min-width:0}
.li-name{font-weight:700;font-size:14px;color:var(--ink-900);white-space:nowrap;overflow:hidden;text-overflow:ellipsis}
.li-sub{font-size:11px;color:var(--ink-500);margin-top:2px}
.li-time{font-size:11px;color:var(--ink-500);font-weight:500}
.empty{
text-align:center;padding:30px 14px;
color:var(--ink-500);font-size:13px;
}
.empty-icon{
font-size:36px;margin-bottom:8px;opacity:.4;
}
/* === CARDS (Student records) === */
.student-card{
background:var(--white);
border:1px solid var(--ink-100);
border-right:4px solid var(--green-500);
border-radius:var(--radius-md);
padding:14px;
margin-bottom:10px;
box-shadow:var(--shadow-sm);
position:relative;
}
.student-card.late{border-right-color:#F59E0B}
.student-card.permission{border-right-color:var(--blue-700)}
.student-card.violation{border-right-color:var(--rose-700)}
.sc-head{
display:flex;align-items:flex-start;justify-content:space-between;
gap:10px;margin-bottom:10px;
}
.sc-name{
font-weight:900;font-size:17px;
color:var(--ink-900);
line-height:1.3;
flex:1;
}
.sc-class{
font-size:11px;
background:var(--green-50);
color:var(--green-900);
padding:3px 9px;
border-radius:999px;
font-weight:700;
white-space:nowrap;
}
.sc-class.late{background:#FEF3C7;color:var(--amber-700)}
.sc-class.permission{background:var(--blue-50);color:var(--blue-900)}
.sc-class.violation{background:var(--rose-50);color:var(--rose-700)}
.sc-meta{
display:flex;flex-wrap:wrap;gap:8px;font-size:12px;color:var(--ink-700);
}
.sc-meta-item{
display:flex;align-items:center;gap:4px;
background:var(--ink-50);
padding:4px 9px;
border-radius:8px;
}
.sc-meta-item .lbl{color:var(--ink-500);font-weight:500;font-size:11px}
.sc-meta-item .val{font-weight:700;color:var(--ink-900);font-size:12px}
.sc-counter{
display:inline-flex;align-items:center;gap:4px;
background:var(--rose-50);
color:var(--rose-700);
padding:4px 9px;
border-radius:8px;
font-size:12px;font-weight:700;
margin-top:8px;
}
.sc-counter.ok{background:var(--green-50);color:var(--green-900)}
.sc-counter.warn{background:#FEF3C7;color:var(--amber-700)}
.sc-actions{
position:absolute;top:10px;left:10px;
display:flex;gap:4px;
}
.sc-del, .sc-edit{
width:28px;height:28px;border-radius:8px;
background:var(--ink-50);color:var(--ink-500);
border:none;cursor:pointer;
display:grid;place-items:center;
font-size:14px;font-weight:700;
transition:all .15s;
}
.sc-del:hover,.sc-del:active{background:var(--rose-50);color:var(--rose-700)}
.sc-edit:hover,.sc-edit:active{background:var(--blue-50);color:var(--blue-700)}
.sc-note{
margin-top:8px;
font-size:12px;color:var(--ink-700);
background:var(--ink-50);
padding:8px 10px;
border-radius:8px;
line-height:1.5;
}
/* === FORM === */
.form-grid{display:flex;flex-direction:column;gap:12px}
.field{display:flex;flex-direction:column;gap:6px}
.field label{
font-size:13px;font-weight:700;color:var(--ink-700);
display:flex;align-items:center;gap:4px;
}
.field label .req{color:var(--rose-700);font-weight:900}
.field input,
.field select,
.field textarea{
width:100%;
padding:14px 14px;
border:1.5px solid var(--ink-300);
border-radius:12px;
font-family:inherit;
font-size:16px;
background:var(--white);
color:var(--ink-900);
transition:all .15s;
font-weight:500;
}
.field input:focus,
.field select:focus,
.field textarea:focus{
outline:none;
border-color:var(--green-700);
box-shadow:0 0 0 3px rgba(45,156,135,.15);
}
.field textarea{resize:vertical;min-height:80px;line-height:1.6}
.field-row{display:grid;grid-template-columns:1fr 1fr;gap:10px}
.helper{font-size:11px;color:var(--ink-500)}
/* === CHIPS === */
.chips{display:flex;flex-wrap:wrap;gap:8px}
.chip{
padding:10px 14px;
border:1.5px solid var(--ink-300);
border-radius:999px;
background:var(--white);
color:var(--ink-700);
font-size:13px;font-weight:600;
cursor:pointer;
transition:all .15s;
font-family:inherit;
}
.chip.active{
background:var(--green-700);color:var(--white);border-color:var(--green-700);
}
.chip.amber.active{background:var(--amber-700);border-color:var(--amber-700)}
.chip.rose.active{background:var(--rose-700);border-color:var(--rose-700)}
.chip.blue.active{background:var(--blue-700);border-color:var(--blue-700)}
.chips-list{display:flex;flex-direction:column;gap:8px}
.chips-list .chip{
border-radius:12px;
padding:12px 14px;
text-align:right;
line-height:1.5;
font-weight:500;
font-size:14px;
display:flex;align-items:center;gap:10px;
width:100%;
}
.chips-list .chip::before{
content:"";
width:18px;height:18px;border-radius:50%;
border:2px solid var(--ink-300);
background:var(--white);
flex-shrink:0;
transition:all .15s;
}
.chips-list .chip.active{
background:var(--rose-50);
color:var(--rose-700);
border-color:var(--rose-700);
font-weight:700;
}
.chips-list .chip.active::before{
border-color:var(--rose-700);
background:var(--rose-700);
box-shadow:inset 0 0 0 3px var(--white);
}
/* === BUTTONS === */
.btn{
display:inline-flex;align-items:center;justify-content:center;gap:6px;
padding:14px 18px;
border-radius:12px;
font-family:inherit;
font-size:15px;font-weight:700;
cursor:pointer;
border:none;
transition:all .15s;
text-decoration:none;
}
.btn-primary{
background:linear-gradient(135deg,var(--green-700) 0%,var(--green-900) 100%);
color:var(--white);
box-shadow:var(--shadow-md);
}
.btn-primary:hover,.btn-primary:active{transform:translateY(-1px);box-shadow:var(--shadow-lg)}
.btn-secondary{
background:var(--white);
color:var(--ink-700);
border:1.5px solid var(--ink-300);
}
.btn-secondary:hover,.btn-secondary:active{background:var(--ink-50);border-color:var(--ink-500)}
.btn-block{width:100%}
.btn-row{display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-top:6px}
/* === FAB === */
.fab{
position:fixed;
bottom:88px;
left:18px;
width:58px;height:58px;
border-radius:50%;
background:linear-gradient(135deg,var(--green-700) 0%,var(--green-900) 100%);
color:var(--white);
border:none;
cursor:pointer;
box-shadow:0 6px 20px rgba(13,72,66,.4);
font-size:28px;font-weight:300;
display:none;
align-items:center;justify-content:center;
z-index:30;
line-height:1;
transition:all .2s;
}
.fab:hover,.fab:active{transform:scale(1.05);box-shadow:0 8px 24px rgba(13,72,66,.5)}
.screen.active.has-fab + .fab,
.screen.active.has-fab ~ .fab{display:flex}
/* === BOTTOM NAV === */
.nav{
position:fixed;
bottom:0;left:0;right:0;
background:var(--white);
border-top:1px solid var(--ink-100);
box-shadow:0 -4px 20px rgba(0,0,0,.04);
z-index:40;
padding:6px 4px calc(6px + env(safe-area-inset-bottom));
display:grid;
grid-template-columns:repeat(5,1fr);
gap:2px;
}
.nav-btn{
background:none;border:none;cursor:pointer;
padding:8px 4px 6px;
display:flex;flex-direction:column;align-items:center;gap:3px;
color:var(--ink-500);
font-family:inherit;font-size:11px;font-weight:600;
transition:color .15s;
border-radius:8px;
position:relative;
}
.nav-btn.active{color:var(--green-900)}
.nav-btn.active .nav-icon{
background:var(--green-50);
}
.nav-icon{
width:32px;height:32px;border-radius:10px;
display:grid;place-items:center;
transition:background .15s;
}
.nav-icon svg{width:20px;height:20px;stroke-width:2}
.nav-badge{
position:absolute;
top:4px;
left:50%;
transform:translateX(14px);
background:var(--rose-700);color:var(--white);
font-size:9px;font-weight:700;
min-width:16px;height:16px;
border-radius:999px;
padding:0 4px;
display:grid;place-items:center;
border:2px solid var(--white);
}
/* === MODAL === */
.modal-overlay{
position:fixed;inset:0;
background:rgba(15,23,42,.5);
backdrop-filter:blur(4px);
z-index:100;
display:none;
align-items:flex-end;
animation:fadeIn .2s;
}
.modal-overlay.open{display:flex}
@keyframes fadeIn{from{opacity:0}to{opacity:1}}
.modal{
background:var(--white);
width:100%;
max-height:92vh;
border-radius:24px 24px 0 0;
overflow-y:auto;
animation:slideUp .25s cubic-bezier(.2,.9,.3,1);
-webkit-overflow-scrolling:touch;
}
@keyframes slideUp{from{transform:translateY(100%)}to{transform:none}}
.modal-handle{
width:40px;height:4px;background:var(--ink-300);
border-radius:999px;margin:10px auto 0;
}
.modal-head{
padding:14px 18px 12px;
display:flex;align-items:center;justify-content:space-between;
border-bottom:1px solid var(--ink-100);
position:sticky;top:0;
background:var(--white);
z-index:5;
}
.modal-head h3{font-size:18px;font-weight:900;color:var(--green-900)}
.modal-close{
width:36px;height:36px;border-radius:10px;
background:var(--ink-50);
border:none;cursor:pointer;
font-size:22px;font-weight:300;color:var(--ink-700);
display:grid;place-items:center;
line-height:1;
}
.modal-body{padding:18px}
.modal-foot{
padding:14px 18px;
border-top:1px solid var(--ink-100);
background:var(--ink-50);
position:sticky;bottom:0;
}
/* === FILTER ROW === */
.filter-row{
display:flex;gap:8px;
overflow-x:auto;
margin-bottom:12px;
padding-bottom:4px;
-webkit-overflow-scrolling:touch;
}
.filter-row::-webkit-scrollbar{display:none}
.filter-pill{
flex-shrink:0;
padding:7px 14px;
border-radius:999px;
border:1.5px solid var(--ink-300);
background:var(--white);
color:var(--ink-700);
font-size:12px;font-weight:600;
cursor:pointer;
font-family:inherit;
white-space:nowrap;
}
.filter-pill.active{
background:var(--green-900);color:var(--white);border-color:var(--green-900);
}
/* === SEARCH BOX === */
.search-box{
width:100%;
padding:12px 14px;
border:1.5px solid var(--ink-300);
border-radius:12px;
font-family:inherit;
font-size:14px;
background:var(--white);
color:var(--ink-900);
margin-bottom:12px;
transition:all .15s;
}
.search-box:focus{
outline:none;
border-color:var(--green-700);
box-shadow:0 0 0 3px rgba(45,156,135,.15);
}
/* === REPORT === */
.report-section{margin-top:16px}
.report-title{
font-size:14px;font-weight:900;color:var(--green-900);
margin-bottom:10px;
padding-bottom:6px;
border-bottom:2px solid var(--green-50);
}
.stat-row{
display:grid;grid-template-columns:repeat(3,1fr);gap:8px;
margin-bottom:10px;
}
.stat-mini{
background:var(--ink-50);
padding:10px;border-radius:10px;
text-align:center;
}
.stat-mini .v{font-size:20px;font-weight:900;color:var(--green-900)}
.stat-mini .l{font-size:10px;color:var(--ink-500);font-weight:500;margin-top:2px}
table.report-table{
width:100%;border-collapse:collapse;
font-size:12px;
}
table.report-table th{
background:var(--green-900);color:var(--white);
padding:8px 6px;font-weight:700;text-align:right;
font-size:11px;
}
table.report-table th:first-child{border-radius:0 8px 0 0}
table.report-table th:last-child{border-radius:8px 0 0 0}
table.report-table td{
padding:8px 6px;border-bottom:1px solid var(--ink-100);
text-align:right;
}
table.report-table tr:nth-child(even) td{background:var(--ink-50)}
/* === AUDIT LOG === */
.audit-entry{
font-size:11px;
padding:8px 10px;
border-bottom:1px solid var(--ink-100);
color:var(--ink-700);
display:flex;justify-content:space-between;
gap:8px;
}
.audit-entry .time{color:var(--ink-500);white-space:nowrap}
/* === TOAST === */
.toast{
position:fixed;
bottom:100px;
left:50%;
transform:translateX(-50%) translateY(20px);
background:var(--green-900);color:var(--white);
padding:12px 20px;
border-radius:12px;
font-size:13px;font-weight:600;
box-shadow:var(--shadow-lg);
z-index:200;
opacity:0;
transition:all .25s;
pointer-events:none;
max-width:90%;
}
.toast.show{opacity:1;transform:translateX(-50%) translateY(0)}
/* === PRINT === */
@media print{
@page{size:A4;margin:14mm}
body{
background:var(--white)!important;
padding:0!important;
font-size:11pt;
}
.topbar,.nav,.fab,.modal-overlay,.btn-row,.filter-row,.app-footer,.search-box,.no-print,.sc-actions,.topbar-logout{
display:none!important;
}
.screen{display:none!important;padding:0!important}
.screen.active{display:block!important}
.panel,.kpi,.student-card{
box-shadow:none!important;
border:1px solid var(--ink-300)!important;
page-break-inside:avoid;
}
.student-card{margin-bottom:6px;padding:8px}
.sc-name{font-size:12pt}
.kpi-grid{grid-template-columns:repeat(4,1fr)!important}
.kpi-value{font-size:18pt}
.barchart{display:none}
table.report-table{font-size:10pt}
}
@media(min-width:720px){
body{padding-bottom:0;max-width:880px;margin:0 auto;box-shadow:var(--shadow-lg);min-height:100vh;background:var(--paper)}
.nav{position:sticky;top:auto;bottom:0;max-width:880px;margin:0 auto;left:auto;right:auto}
.kpi-grid{grid-template-columns:repeat(4,1fr)}
.stat-row{grid-template-columns:repeat(6,1fr)}
}
</style>
</head>
<body>

<!-- ====== LOGIN SCREEN ====== -->
<div class="login-screen" id="loginScreen">
<div class="login-card">
<h1>🔐 النظام الإداري</h1>
<div class="sub">الثانوية الثامنة بالخرج</div>
<div class="field">
<label>اسم المستخدم</label>
<input type="text" id="loginUser" placeholder="أدخلي اسم المستخدم" autocomplete="off">
</div>
<div class="field">
<label>كلمة المرور</label>
<input type="password" id="loginPass" placeholder="أدخلي كلمة المرور">
</div>
<button class="btn btn-primary btn-block" id="btnLogin" style="margin-top:8px">دخول</button>
<div class="login-error" id="loginError">اسم المستخدم أو كلمة المرور غير صحيحة</div>
<div style="margin-top:16px;font-size:11px;color:var(--ink-500);text-align:center">
<details>
<summary style="cursor:pointer;font-weight:600">بيانات الدخول الافتراضية</summary>
<div style="margin-top:8px;text-align:right">
<div>👤 المستخدم: <b>admin</b></div>
<div>🔑 المرور: <b>123456</b></div>
<div style="margin-top:4px;color:var(--rose-700)">⚠️ يُنصح بتغييرها فوراً من الإعدادات</div>
</div>
</details>
</div>
</div>
</div>

<!-- ====== TOP BAR ====== -->
<header class="topbar" id="topbar" style="display:none">
<div class="topbar-row">
<div class="topbar-brand">
<div class="topbar-titles">
<div class="t1">الثانوية الثامنة بالخرج</div>
<div class="t2" id="currentUserDisplay">المساعد الإداري</div>
<div class="t3">غزيل الشمراني</div>
</div>
</div>
<div class="topbar-right">
<button class="topbar-settings" id="btnSettings" aria-label="الإعدادات" title="الإعدادات">
<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="3"/><path d="M19.4 15a1.7 1.7 0 00.34 1.87l.06.06a2 2 0 11-2.83 2.83l-.06-.06a1.7 1.7 0 00-1.87-.34 1.7 1.7 0 00-1.03 1.56V21a2 2 0 11-4 0v-.09a1.7 1.7 0 00-1.11-1.56 1.7 1.7 0 00-1.87.34l-.06.06a2 2 0 11-2.83-2.83l.06-.06a1.7 1.7 0 00.34-1.87 1.7 1.7 0 00-1.56-1.03H3a2 2 0 110-4h.09A1.7 1.7 0 004.65 8.6a1.7 1.7 0 00-.34-1.87l-.06-.06a2 2 0 112.83-2.83l.06.06a1.7 1.7 0 001.87.34H9a1.7 1.7 0 001.03-1.56V2.6a2 2 0 014 0v.09a1.7 1.7 0 001.03 1.56 1.7 1.7 0 001.87-.34l.06-.06a2 2 0 112.83 2.83l-.06.06a1.7 1.7 0 00-.34 1.87V9a1.7 1.7 0 001.56 1.03H21a2 2 0 110 4h-.09a1.7 1.7 0 00-1.51 1.03z" stroke-linecap="round" stroke-linejoin="round"/></svg>
</button>
<button class="topbar-logout" id="btnLogout" title="تسجيل الخروج">🚪</button>
<div class="topbar-date" id="todayHijri">—</div>
</div>
</div>
</header>

<!-- ====== HOME ====== -->
<section class="screen active" id="screen-home" style="display:none">
<div class="screen-head">
<h2>اليوم</h2>
<p id="todayGreg">—</p>
</div>

<div class="kpi-grid">
<div class="kpi k-amber">
<div class="kpi-label">تأخر صباحي</div>
<div class="kpi-value" id="k-late">0</div>
<div class="kpi-sub">حالة اليوم</div>
</div>
<div class="kpi k-blue">
<div class="kpi-label">استئذان</div>
<div class="kpi-value" id="k-perm">0</div>
<div class="kpi-sub">حالة اليوم</div>
</div>
<div class="kpi k-rose">
<div class="kpi-label">مخالفات</div>
<div class="kpi-value" id="k-vio">0</div>
<div class="kpi-sub">حالة اليوم</div>
</div>
<div class="kpi">
<div class="kpi-label">حالات متكررة</div>
<div class="kpi-value" id="k-repeat">0</div>
<div class="kpi-sub">طالبات تحتاج متابعة</div>
</div>
</div>

<div class="panel">
<div class="panel-title">
<h3>الأسبوع الحالي</h3>
<span class="meta" id="weekRange">—</span>
</div>
<div class="barchart" id="weekChart"></div>
</div>

<div class="panel">
<div class="panel-title">
<h3>آخر السجلات</h3>
<span class="meta meta-action">
<button class="btn btn-secondary no-print" style="padding:6px 12px;font-size:12px" id="btnExportAll">تصدير الكل</button>
<button class="btn btn-secondary no-print" style="padding:6px 12px;font-size:12px;margin-right:4px" id="btnBackup">نسخ احتياطي</button>
</span>
</div>
<div id="recentList"></div>
</div>
</section>

<!-- ====== LATE ====== -->
<section class="screen has-fab" id="screen-late" style="display:none">
<div class="screen-head">
<h2>التأخر الصباحي</h2>
<p>سجل الطالبات المتأخرات — يحسب التكرار تلقائياً</p>
</div>
<input type="text" class="search-box" id="searchLate" placeholder="🔍 بحث باسم الطالبة..." autocomplete="off">
<div class="filter-row">
<button class="filter-pill active" data-filter="today">اليوم</button>
<button class="filter-pill" data-filter="week">الأسبوع</button>
<button class="filter-pill" data-filter="month">الشهر</button>
<button class="filter-pill" data-filter="all">الكل</button>
</div>
<div id="lateList"></div>
<div class="btn-row no-print" style="margin-top:14px">
<button class="btn btn-secondary" data-print="late">طباعة</button>
<button class="btn btn-secondary" data-export="late">تصدير</button>
</div>
</section>

<!-- ====== PERMISSION ====== -->
<section class="screen has-fab" id="screen-perm" style="display:none">
<div class="screen-head">
<h2>الاستئذان</h2>
<p>تسجيل وتوثيق طلبات الاستئذان خلال اليوم</p>
</div>
<input type="text" class="search-box" id="searchPerm" placeholder="🔍 بحث باسم الطالبة..." autocomplete="off">
<div class="filter-row">
<button class="filter-pill active" data-filter="today">اليوم</button>
<button class="filter-pill" data-filter="week">الأسبوع</button>
<button class="filter-pill" data-filter="month">الشهر</button>
<button class="filter-pill" data-filter="all">الكل</button>
</div>
<div id="permList"></div>
<div class="btn-row no-print" style="margin-top:14px">
<button class="btn btn-secondary" data-print="perm">طباعة</button>
<button class="btn btn-secondary" data-export="perm">تصدير</button>
</div>
</section>

<!-- ====== VIOLATION ====== -->
<section class="screen has-fab" id="screen-vio" style="display:none">
<div class="screen-head">
<h2>المخالفات السلوكية</h2>
<p>رصد المخالفات مع عداد تراكمي تلقائي لكل طالبة</p>
</div>
<input type="text" class="search-box" id="searchVio" placeholder="🔍 بحث باسم الطالبة..." autocomplete="off">
<div class="filter-row">
<button class="filter-pill active" data-filter="today">اليوم</button>
<button class="filter-pill" data-filter="week">الأسبوع</button>
<button class="filter-pill" data-filter="month">الشهر</button>
<button class="filter-pill" data-filter="all">الكل</button>
</div>
<div id="vioList"></div>
<div class="btn-row no-print" style="margin-top:14px">
<button class="btn btn-secondary" data-print="vio">طباعة</button>
<button class="btn btn-secondary" data-export="vio">تصدير</button>
</div>
</section>

<!-- ====== REPORT ====== -->
<section class="screen" id="screen-report" style="display:none">
<div class="screen-head">
<h2>التقرير الأسبوعي</h2>
<p>يُسحب تلقائياً من البيانات المحفوظة</p>
</div>

<div class="panel no-print">
<div class="field">
<label>الفترة</label>
<select id="reportRange">
<option value="week">الأسبوع الحالي</option>
<option value="lastweek">الأسبوع السابق</option>
<option value="month">الشهر الحالي</option>
<option value="custom">فترة مخصصة</option>
</select>
</div>
<div class="field-row" id="customRange" style="display:none;margin-top:10px">
<div class="field">
<label>من</label>
<input type="date" id="rFrom">
</div>
<div class="field">
<label>إلى</label>
<input type="date" id="rTo">
</div>
</div>
<button class="btn btn-primary btn-block" id="btnGenReport" style="margin-top:12px">توليد التقرير</button>
</div>

<div id="reportOutput" style="display:none">
<div class="panel">
<div class="panel-title">
<h3 id="reportPeriod">—</h3>
</div>
<div class="stat-row">
<div class="stat-mini"><div class="v" id="r-late">0</div><div class="l">تأخر</div></div>
<div class="stat-mini"><div class="v" id="r-perm">0</div><div class="l">استئذان</div></div>
<div class="stat-mini"><div class="v" id="r-vio">0</div><div class="l">مخالفات</div></div>
</div>
<div class="stat-row" style="margin-top:8px">
<div class="stat-mini"><div class="v" id="r-st-1">0</div><div class="l">أول ثانوي</div></div>
<div class="stat-mini"><div class="v" id="r-st-2">0</div><div class="l">ثاني ثانوي</div></div>
<div class="stat-mini"><div class="v" id="r-st-3">0</div><div class="l">ثالث ثانوي</div></div>
</div>
</div>

<div class="panel">
<div class="report-title">الحالات المتكررة (تحتاج متابعة)</div>
<div id="r-repeat-list"></div>
</div>
<div class="panel">
<div class="report-title">تفاصيل التأخر</div>
<div id="r-late-details"></div>
</div>
<div class="panel">
<div class="report-title">تفاصيل الاستئذان</div>
<div id="r-perm-details"></div>
</div>
<div class="panel">
<div class="report-title">تفاصيل المخالفات</div>
<div id="r-vio-details"></div>
</div>

<div class="btn-row no-print" style="margin-top:16px">
<button class="btn btn-primary" id="btnPrintReport">طباعة / حفظ PDF</button>
<button class="btn btn-secondary" id="btnExportReport">تصدير CSV</button>
</div>
</div>
</section>

<!-- ====== FOOTER ====== -->
<footer class="app-footer" id="appFooter" style="display:none">
<div class="footer-rule"></div>
<div class="footer-rights">© جميع الحقوق محفوظة لـ غزيل الشمراني</div>
</footer>

<!-- ====== FAB ====== -->
<button class="fab" id="fab" aria-label="إضافة" style="display:none">+</button>

<!-- ====== BOTTOM NAV ====== -->
<nav class="nav" id="bottomNav" style="display:none">
<button class="nav-btn active" data-screen="home">
<span class="nav-icon">
<svg viewBox="0 0 24 24" fill="none" stroke="currentColor"><path d="M3 12l9-9 9 9M5 10v10h14V10" stroke-linecap="round" stroke-linejoin="round"/></svg>
</span>
الرئيسية
</button>
<button class="nav-btn" data-screen="late">
<span class="nav-icon">
<svg viewBox="0 0 24 24" fill="none" stroke="currentColor"><circle cx="12" cy="12" r="9"/><path d="M12 7v5l3 2" stroke-linecap="round"/></svg>
<span class="nav-badge" id="badge-late" style="display:none">0</span>
</span>
تأخر
</button>
<button class="nav-btn" data-screen="perm">
<span class="nav-icon">
<svg viewBox="0 0 24 24" fill="none" stroke="currentColor"><path d="M9 21H5a2 2 0 01-2-2V5a2 2 0 012-2h4M16 17l5-5-5-5M21 12H9" stroke-linecap="round" stroke-linejoin="round"/></svg>
<span class="nav-badge" id="badge-perm" style="display:none">0</span>
</span>
استئذان
</button>
<button class="nav-btn" data-screen="vio">
<span class="nav-icon">
<svg viewBox="0 0 24 24" fill="none" stroke="currentColor"><path d="M12 9v4M12 17h.01M10.29 3.86L1.82 18a2 2 0 001.71 3h16.94a2 2 0 001.71-3L13.71 3.86a2 2 0 00-3.42 0z" stroke-linecap="round" stroke-linejoin="round"/></svg>
<span class="nav-badge" id="badge-vio" style="display:none">0</span>
</span>
مخالفات
</button>
<button class="nav-btn" data-screen="report">
<span class="nav-icon">
<svg viewBox="0 0 24 24" fill="none" stroke="currentColor"><path d="M9 17V7M14 17v-5M19 17v-3M4 17V4h16v13M3 21h18" stroke-linecap="round" stroke-linejoin="round"/></svg>
</span>
تقارير
</button>
</nav>

<!-- ====== MODAL ====== -->
<div class="modal-overlay" id="modal">
<div class="modal">
<div class="modal-handle"></div>
<div class="modal-head">
<h3 id="modalTitle">إضافة جديد</h3>
<button class="modal-close" id="modalClose">×</button>
</div>
<div class="modal-body" id="modalBody"></div>
<div class="modal-foot">
<button class="btn btn-primary btn-block" id="modalSave">حفظ</button>
</div>
</div>
</div>

<!-- ====== TOAST ====== -->
<div class="toast" id="toast"></div>

<script>
(function(){
'use strict';

/* ============= SECURITY & CONFIG ============= */
const APP_VERSION = '2.0.0';
const STORAGE_KEY = 'thanaweya8_admin_v2';
const SETTINGS_KEY = 'thanaweya8_settings_v2';
const AUTH_KEY = 'thanaweya8_auth_v2';
const AUDIT_KEY = 'thanaweya8_audit_v2';
const MAX_LOGIN_ATTEMPTS = 5;
const LOCKOUT_DURATION = 15 * 60 * 1000; // 15 دقيقة
const SESSION_TIMEOUT = 60 * 60 * 1000; // ساعة واحدة
const AUTO_SAVE_INTERVAL = 30000; // 30 ثانية

// تشفير بسيط (AES-like باستخدام btoa لتوضيح المبدأ)
const ENCRYPTION_SALT = 'Thanaweya8_Secure_Salt_2024';

function simpleEncrypt(text) {
try {
const salted = text + ENCRYPTION_SALT;
return btoa(unescape(encodeURIComponent(salted)));
} catch(e) {
return btoa(text);
}
}

function simpleDecrypt(encoded) {
try {
const decoded = decodeURIComponent(escape(atob(encoded)));
if (decoded.endsWith(ENCRYPTION_SALT)) {
return decoded.slice(0, -ENCRYPTION_SALT.length);
}
return atob(encoded);
} catch(e) {
return atob(encoded);
}
}

// تعقيم HTML لمنع XSS
function sanitizeHTML(str) {
if (str === null || str === undefined) return '';
const div = document.createElement('div');
div.appendChild(document.createTextNode(String(str)));
return div.innerHTML;
}

// التحقق من صحة المدخلات
function validateName(name) {
name = name.trim();
if (!name) return { valid: false, error: 'الاسم مطلوب' };
if (name.length < 4) return { valid: false, error: 'الاسم قصير جداً (4 أحرف على الأقل)' };
if (name.length > 100) return { valid: false, error: 'الاسم طويل جداً (100 حرف كحد أقصى)' };
if (/[<>]/.test(name)) return { valid: false, error: 'الاسم يحتوي على رموز غير مسموحة' };
return { valid: true };
}

function validatePhone(phone) {
if (!phone) return { valid: true }; // اختياري
if (!/^05\d{8}$/.test(phone)) return { valid: false, error: 'صيغة الجوال غير صحيحة (05xxxxxxxx)' };
return { valid: true };
}

function validateFutureDate(date) {
const d = new Date(date);
const today = new Date();
today.setHours(23, 59, 59, 999);
if (d > today) return { valid: false, error: 'لا يمكن إدخال تاريخ مستقبلي' };
return { valid: true };
}

// توليد معرف فريد أكثر أماناً
function generateUID() {
const timestamp = Date.now().toString(36);
const randomPart = crypto.getRandomValues(new Uint32Array(2));
const random1 = randomPart[0].toString(36);
const random2 = randomPart[1].toString(36);
return `${timestamp}-${random1}-${random2}`;
}

const DEFAULT_SETTINGS = {
schoolStart: '06:45',
adminUser: 'admin',
adminPass: simpleEncrypt('123456'),
autoBackup: true,
sessionTimeout: SESSION_TIMEOUT
};

let settings = Object.assign({}, DEFAULT_SETTINGS);
let authState = { isLoggedIn: false, username: '', loginTime: 0, attempts: 0, lockUntil: 0 };
let sessionTimer = null;

const GRADES = [
{ id: '1', label: 'أول ثانوي', sections: [
{ value:'1/1', label:'أول ثانوي / ١' },
{ value:'1/2', label:'أول ثانوي / ٢' },
{ value:'1/3', label:'أول ثانوي / ٣' },
{ value:'1/4', label:'أول ثانوي / ٤' },
{ value:'1/5', label:'أول ثانوي / ٥' },
{ value:'1/6', label:'أول ثانوي / ٦' }
]},
{ id: '2', label: 'ثاني ثانوي', sections: [
{ value:'2/1', label:'ثاني ثانوي / ١' },
{ value:'2/2', label:'ثاني ثانوي / ٢' },
{ value:'2/3', label:'ثاني ثانوي / ٣' },
{ value:'2/4', label:'ثاني ثانوي / ٤' },
{ value:'2/5', label:'ثاني ثانوي / ٥' },
{ value:'2/6', label:'ثاني ثانوي / ٦' }
]},
{ id: '3', label: 'ثالث ثانوي', sections: [
{ value:'3/1', label:'ثالث ثانوي / ١' },
{ value:'3/2', label:'ثالث ثانوي / ٢' },
{ value:'3/3', label:'ثالث ثانوي / ٣' },
{ value:'3/4', label:'ثالث ثانوي / ٤' },
{ value:'3/5', label:'ثالث ثانوي / ٥' },
{ value:'3/صحي', label:'ثالث ثانوي / مسار الصحة والحياة' }
]}
];

const VIOLATION_TYPES = [
'التأخر الصباحي',
'عدم حضور الاصطفاف الصباحي',
'التأخر عن الاصطفاف الصباحي أو العبث أثناءه',
'التأخر في الدخول إلى الحصص',
'إعاقة سير الحصص الدراسية',
'النوم داخل الفصل',
'تكرار الخروج والدخول من البوابة قبل الحضور والانصراف',
'التجمهر أمام بوابة المدرسة',
'عدم حضور الحصة الدراسية أو الهروب منها',
'الدخول أو الخروج من الفصل دون استئذان',
'دخول فصل آخر دون استئذان',
'إثارة الفوضى داخل الفصل أو المدرسة أو في وسائل النقل'
];

const VIOLATION_ACTIONS = [
'تنبيه شفهي',
'إنذار كتابي',
'استدعاء ولي الأمر',
'تعهد خطي',
'حسم درجات',
'تحويل للإدارة العليا'
];

const PERMISSION_TYPES = [
'مرضي',
'طارئ عائلي',
'موعد رسمي',
'شخصي',
'وفاة',
'أخرى'
];

/* ============= STATE ============= */
let state = { late: [], perm: [], vio: [] };
let auditLog = [];
let currentScreen = 'home';
let currentForm = null;
let currentFilter = { late:'today', perm:'today', vio:'today' };
let editingId = null;

/* ============= AUDIT LOG ============= */
function addAuditEntry(action, details) {
auditLog.push({
timestamp: new Date().toISOString(),
user: authState.username,
action: action,
details: details
});
// الاحتفاظ بآخر 500 سجل فقط
if (auditLog.length > 500) auditLog = auditLog.slice(-500);
saveAudit();
}

function saveAudit() {
try {
localStorage.setItem(AUDIT_KEY, simpleEncrypt(JSON.stringify(auditLog)));
} catch(e) { console.warn('Audit save failed', e); }
}

function loadAudit() {
try {
const raw = localStorage.getItem(AUDIT_KEY);
if (raw) {
auditLog = JSON.parse(simpleDecrypt(raw)) || [];
}
} catch(e) { auditLog = []; }
}

/* ============= STORAGE WITH ENCRYPTION ============= */
function load(){
try{
const raw = localStorage.getItem(STORAGE_KEY);
if(raw){
const decrypted = simpleDecrypt(raw);
const parsed = JSON.parse(decrypted);
state = Object.assign(state, parsed);
}
const sraw = localStorage.getItem(SETTINGS_KEY);
if(sraw){
const sparsed = JSON.parse(simpleDecrypt(sraw));
settings = Object.assign({}, DEFAULT_SETTINGS, sparsed);
}
} catch(e) {
console.warn('Load failed', e);
// محاولة تحميل النسخة الاحتياطية
tryLoadBackup();
}
loadAuth();
loadAudit();
}

function save(){
try{
const encrypted = simpleEncrypt(JSON.stringify(state));
localStorage.setItem(STORAGE_KEY, encrypted);
// حفظ نسخة احتياطية تلقائية
if (settings.autoBackup) {
localStorage.setItem(STORAGE_KEY + '_backup', encrypted);
}
} catch(e) {
console.warn('Save failed', e);
toast('تنبيه: فشل الحفظ. قد تكون مساحة التخزين ممتلئة.');
}
}

function saveSettings(){
try{
const encrypted = simpleEncrypt(JSON.stringify(settings));
localStorage.setItem(SETTINGS_KEY, encrypted);
} catch(e) { console.warn('Settings save failed', e); }
}

function tryLoadBackup() {
try {
const backup = localStorage.getItem(STORAGE_KEY + '_backup');
if (backup) {
const decrypted = simpleDecrypt(backup);
const parsed = JSON.parse(decrypted);
state = Object.assign(state, parsed);
save();
toast('تم استعادة البيانات من النسخة الاحتياطية');
addAuditEntry('استعادة نسخة احتياطية', 'تم الاستعادة تلقائياً');
}
} catch(e) { console.warn('Backup load failed', e); }
}

function createBackup() {
try {
const encrypted = simpleEncrypt(JSON.stringify(state));
localStorage.setItem(STORAGE_KEY + '_backup_manual_' + Date.now(), encrypted);
// أيضاً تصدير كملف
const exportData = {
version: APP_VERSION,
timestamp: new Date().toISOString(),
user: authState.username,
data: state,
audit: auditLog.slice(-100)
};
const blob = new Blob([JSON.stringify(exportData, null, 2)], {type: 'application/json'});
const url = URL.createObjectURL(blob);
const a = document.createElement('a');
a.href = url;
a.download = 'thanaweya8_backup_' + new Date().toISOString().slice(0,10) + '.json';
document.body.appendChild(a);
a.click();
document.body.removeChild(a);
setTimeout(() => URL.revokeObjectURL(url), 1000);
addAuditEntry('نسخ احتياطي', 'تم إنشاء نسخة احتياطية وتصديرها');
toast('تم إنشاء النسخة الاحتياطية بنجاح');
} catch(e) {
toast('فشل في إنشاء النسخة الاحتياطية');
}
}

function importBackup(file) {
const reader = new FileReader();
reader.onload = function(e) {
try {
const imported = JSON.parse(e.target.result);
if (!imported.data || !imported.data.late) {
throw new Error('ملف غير صالح');
}
if (confirm('سيتم استبدال جميع البيانات الحالية بالنسخة المستوردة. هل أنت متأكد؟')) {
state = imported.data;
save();
addAuditEntry('استيراد نسخة احتياطية', 'تم استيراد البيانات من ملف');
rerender();
toast('تم استيراد البيانات بنجاح');
}
} catch(err) {
toast('فشل في استيراد الملف: الملف غير صالح');
}
};
reader.readAsText(file);
}

/* ============= AUTH ============= */
function loadAuth() {
try {
const raw = localStorage.getItem(AUTH_KEY);
if (raw) {
const decrypted = simpleDecrypt(raw);
const parsed = JSON.parse(decrypted);
authState = Object.assign(authState, parsed);

// التحقق من انتهاء الجلسة
if (authState.isLoggedIn) {
const elapsed = Date.now() - authState.loginTime;
if (elapsed > settings.sessionTimeout) {
logout(false);
}
}
}
} catch(e) { /* ignore */ }
}

function saveAuth() {
try {
const encrypted = simpleEncrypt(JSON.stringify(authState));
localStorage.setItem(AUTH_KEY, encrypted);
} catch(e) { console.warn('Auth save failed', e); }
}

function login(username, password) {
// التحقق من القفل
if (authState.lockUntil > Date.now()) {
const remaining = Math.ceil((authState.lockUntil - Date.now()) / 60000);
toast(`الحساب مقفل. يرجى المحاولة بعد ${remaining} دقيقة`);
return false;
}

const decryptedPass = simpleDecrypt(settings.adminPass);

if (username === settings.adminUser && password === decryptedPass) {
authState.isLoggedIn = true;
authState.username = username;
authState.loginTime = Date.now();
authState.attempts = 0;
authState.lockUntil = 0;
saveAuth();

addAuditEntry('تسجيل دخول', `المستخدم: ${username}`);
// بدء مؤقت الجلسة
startSessionTimer();

showApp();
return true;
} else {
authState.attempts++;

if (authState.attempts >= MAX_LOGIN_ATTEMPTS) {
authState.lockUntil = Date.now() + LOCKOUT_DURATION;
saveAuth();
addAuditEntry('قفل الحساب', `تجاوز عدد المحاولات: ${authState.attempts}`);
toast('تم قفل الحساب لمدة 15 دقيقة لكثرة المحاولات الخاطئة');
} else {
saveAuth();
const remaining = MAX_LOGIN_ATTEMPTS - authState.attempts;
toast(`محاولة خاطئة. متبقي ${remaining} محاولات`);
}

return false;
}
}

function logout(showToast = true) {
authState.isLoggedIn = false;
authState.loginTime = 0;
saveAuth();

if (sessionTimer) clearTimeout(sessionTimer);

hideApp();
if (showToast) {
addAuditEntry('تسجيل خروج', '');
toast('تم تسجيل الخروج');
}
}

function startSessionTimer() {
if (sessionTimer) clearTimeout(sessionTimer);
sessionTimer = setTimeout(() => {
logout(true);
toast('انتهت الجلسة. يرجى إعادة تسجيل الدخول');
}, settings.sessionTimeout);
}

function resetSessionTimer() {
if (!authState.isLoggedIn) return;
authState.loginTime = Date.now();
saveAuth();
startSessionTimer();
}

function showApp() {
document.getElementById('loginScreen').style.display = 'none';
document.getElementById('topbar').style.display = 'block';
document.getElementById('screen-home').style.display = 'block';
document.getElementById('appFooter').style.display = 'block';
document.getElementById('bottomNav').style.display = 'grid';
document.getElementById('currentUserDisplay').textContent =
authState.username === 'admin' ? 'المساعد الإداري' : authState.username;

renderTopDate();
rerender();
}

function hideApp() {
document.getElementById('loginScreen').style.display = 'flex';
document.getElementById('topbar').style.display = 'none';
document.getElementById('screen-home').style.display = 'none';
document.getElementById('appFooter').style.display = 'none';
document.getElementById('bottomNav').style.display = 'none';
document.getElementById('fab').style.display = 'none';
// إخفاء جميع الشاشات
document.querySelectorAll('.screen').forEach(s => s.classList.remove('active'));
document.getElementById('screen-home').classList.add('active');
currentScreen = 'home';
}

/* ============= UTIL ============= */
function pad(n){ return String(n).padStart(2,'0'); }
function todayISO(){
const d = new Date();
return d.getFullYear() + '-' + pad(d.getMonth()+1) + '-' + pad(d.getDate());
}
function nowHM(){
const d = new Date();
return pad(d.getHours()) + ':' + pad(d.getMinutes());
}
function fmtHijri(date){
try{
const fmt = new Intl.DateTimeFormat('ar-SA-u-ca-islamic-umalqura',{
day:'numeric',month:'long',year:'numeric'
});
const out = fmt.format(date).replace(/\s*هـ\s*$/,'').trim();
return out + ' هـ';
}catch(e){ return ''; }
}
function fmtGreg(date){
try{
const fmt = new Intl.DateTimeFormat('ar-EG',{
weekday:'long',day:'numeric',month:'long',year:'numeric'
});
return fmt.format(date);
}catch(e){ return date.toISOString().slice(0,10); }
}
function fmtShortDate(iso){
if(!iso) return '';
const d = new Date(iso);
if (isNaN(d.getTime())) return iso;
return pad(d.getDate())+'/'+pad(d.getMonth()+1)+'/'+d.getFullYear();
}
function diffMinutes(from, to){
const [fh,fm] = from.split(':').map(Number);
const [th,tm] = to.split(':').map(Number);
if (isNaN(fh) || isNaN(fm) || isNaN(th) || isNaN(tm)) return 0;
return Math.max(0, (th*60+tm) - (fh*60+fm));
}
function fmtDuration(mins){
if(mins <= 0) return '٠ د';
if(mins < 60) return mins + ' د';
const h = Math.floor(mins/60), m = mins%60;
return m ? h+' س '+m+' د' : h+' س';
}
function startOfWeek(d){
const dt = new Date(d);
const day = dt.getDay();
dt.setDate(dt.getDate() - day);
dt.setHours(0,0,0,0);
return dt;
}
function endOfWeek(d){
const s = startOfWeek(d);
s.setDate(s.getDate()+6);
s.setHours(23,59,59,999);
return s;
}
function inFilter(item, filter){
const today = todayISO();
if(filter==='today') return item.date === today;
const d = new Date(item.date);
if (isNaN(d.getTime())) return false;
const now = new Date();
if(filter==='week'){
return d >= startOfWeek(now) && d <= endOfWeek(now);
}
if(filter==='month'){
return d.getFullYear()===now.getFullYear() && d.getMonth()===now.getMonth();
}
return true;
}
function inDateRange(item, from, to){
if (!from || !to) return true;
return item.date >= from && item.date <= to;
}
function gradeFromSec(sec){
if(!sec) return '';
return sec.split('/')[0];
}
function gradeLabel(id){
const g = GRADES.find(x=>x.id===id);
return g ? g.label : '';
}
function secLabel(value){
for(const g of GRADES){
const s = g.sections.find(x=>x.value===value);
if(s) return s.label;
}
return value || '';
}
function shortSec(value){
if(!value) return '';
const [g,s] = value.split('/');
if(s==='انتساب') return gradeLabel(g)+' / انتساب';
if(s==='صحي') return 'صحي';
return gradeLabel(g)+' / فصل '+s;
}
function toast(msg){
const t = document.getElementById('toast');
t.textContent = msg;
t.classList.add('show');
setTimeout(()=>t.classList.remove('show'), 2500);
}
function countByName(category, name, beforeDate){
if(!name) return 0;
const normalizedName = name.trim().replace(/\s+/g, ' ');
const list = state[category] || [];
return list.filter(x =>
(x.name || '').trim().replace(/\s+/g, ' ') === normalizedName &&
(!beforeDate || x.date <= beforeDate)
).length;
}

/* ============= AUTO SAVE ============= */
let autoSaveTimer = null;
function startAutoSave() {
if (autoSaveTimer) clearInterval(autoSaveTimer);
autoSaveTimer = setInterval(() => {
save();
resetSessionTimer();
}, AUTO_SAVE_INTERVAL);
}

/* ============= HEADER DATE ============= */
function renderTopDate(){
const now = new Date();
document.getElementById('todayHijri').textContent = fmtHijri(now);
const gregEl = document.getElementById('todayGreg');
if (gregEl) gregEl.textContent = fmtGreg(now);
}

/* ============= HOME ============= */
function renderHome(){
const today = todayISO();
const lateToday = state.late.filter(x=>x.date===today);
const permToday = state.perm.filter(x=>x.date===today);
const vioToday = state.vio.filter(x=>x.date===today);
document.getElementById('k-late').textContent = lateToday.length;
document.getElementById('k-perm').textContent = permToday.length;
document.getElementById('k-vio').textContent = vioToday.length;

const cutoff = new Date(); cutoff.setDate(cutoff.getDate()-30);
const cutoffISO = cutoff.toISOString().slice(0,10);
const map = {};
['late','perm','vio'].forEach(cat=>{
state[cat].forEach(r=>{
if(r.date >= cutoffISO){
const k = (r.name || '').trim().replace(/\s+/g, ' ');
if(!k) return;
map[k] = (map[k]||0)+1;
}
});
});
const repeats = Object.values(map).filter(v=>v>=3).length;
document.getElementById('k-repeat').textContent = repeats;

const wStart = startOfWeek(new Date());
const days = ['الأحد','الإثنين','الثلاثاء','الأربعاء','الخميس'];
const chart = document.getElementById('weekChart');
chart.innerHTML = '';
let maxV = 1;
const dayCounts = [];
for(let i=0;i<5;i++){
const dt = new Date(wStart); dt.setDate(wStart.getDate()+i);
const iso = dt.getFullYear()+'-'+pad(dt.getMonth()+1)+'-'+pad(dt.getDate());
const c = state.late.filter(x=>x.date===iso).length +
state.perm.filter(x=>x.date===iso).length +
state.vio.filter(x=>x.date===iso).length;
dayCounts.push(c);
if(c>maxV) maxV=c;
}
dayCounts.forEach((c,i)=>{
const h = c===0 ? 4 : Math.max(8, (c/maxV)*100);
const col = document.createElement('div');
col.className = 'bar-col';
col.innerHTML =
'<div style="flex:1;display:flex;align-items:flex-end;width:100%">' +
'<div class="bar-fill" style="height:'+h+'%">' +
(c>0 ? '<span class="v">'+c+'</span>' : '') +
'</div>' +
'</div>' +
'<div class="bar-label">'+days[i]+'</div>';
chart.appendChild(col);
});

const we = endOfWeek(new Date());
document.getElementById('weekRange').textContent =
pad(wStart.getDate())+'/'+pad(wStart.getMonth()+1)+' — '+pad(we.getDate())+'/'+pad(we.getMonth()+1);

const all = [
...state.late.map(x=>({...x,_t:'late',_label:'تأخر'})),
...state.perm.map(x=>({...x,_t:'perm',_label:'استئذان'})),
...state.vio.map(x=>({...x,_t:'vio',_label:'مخالفة'}))
].sort((a,b)=>(b.createdAt||0)-(a.createdAt||0)).slice(0,8);

const rl = document.getElementById('recentList');
if(all.length===0){
rl.innerHTML = '<div class="empty"><div class="empty-icon">📋</div>لا توجد سجلات بعد. ابدئي بإضافة من شريط القائمة السفلي.</div>';
} else {
rl.innerHTML = all.map(r=>{
const cls = r._t==='late'?'amber':r._t==='perm'?'blue':'rose';
return '<div class="list-item">'+
'<span class="li-dot '+cls+'"></span>'+
'<div class="li-main">'+
'<div class="li-name">'+sanitizeHTML(r.name||'—')+'</div>'+
'<div class="li-sub">'+r._label+' · '+sanitizeHTML(shortSec(r.section))+' · '+fmtShortDate(r.date)+'</div>'+
'</div>'+
'</div>';
}).join('');
}

updateBadges();
}

function updateBadges(){
const today = todayISO();
[['late','badge-late'],['perm','badge-perm'],['vio','badge-vio']].forEach(([k,id])=>{
const c = state[k].filter(x=>x.date===today).length;
const b = document.getElementById(id);
if (!b) return;
if(c>0){ b.textContent = c; b.style.display='grid'; }
else { b.style.display='none'; }
});
}

/* ============= RENDER LISTS ============= */
function renderLate(){
const filter = currentFilter.late;
const searchTerm = (document.getElementById('searchLate')?.value || '').trim().toLowerCase();
let list = state.late
.filter(x=>inFilter(x, filter))
.sort((a,b)=>(b.createdAt||0)-(a.createdAt||0));

if (searchTerm) {
list = list.filter(x => (x.name || '').toLowerCase().includes(searchTerm));
}

const root = document.getElementById('lateList');
if(list.length===0){
root.innerHTML = '<div class="empty"><div class="empty-icon">⏰</div>' +
(searchTerm ? 'لا توجد نتائج للبحث' : 'لا توجد حالات تأخر في هذه الفترة') +
'</div>';
return;
}
root.innerHTML = list.map(r=>{
const dur = r.arrival ? diffMinutes(settings.schoolStart, r.arrival) : 0;
const totalForName = countByName('late', r.name);
const ctrCls = totalForName>=4 ? '' : (totalForName>=2 ? 'warn' : 'ok');
return '<div class="student-card late" data-id="'+sanitizeHTML(r.id)+'">'+
'<div class="sc-actions">'+
'<button class="sc-edit" data-act="edit-late" data-id="'+sanitizeHTML(r.id)+'" title="تعديل">✎</button>'+
'<button class="sc-del" data-act="del-late" data-id="'+sanitizeHTML(r.id)+'" title="حذف">×</button>'+
'</div>'+
'<div class="sc-head">'+
'<div class="sc-name">'+sanitizeHTML(r.name||'—')+'</div>'+
'<div class="sc-class late">'+sanitizeHTML(shortSec(r.section))+'</div>'+
'</div>'+
'<div class="sc-meta">'+
'<div class="sc-meta-item"><span class="lbl">الوصول</span><span class="val">'+sanitizeHTML(r.arrival||'—')+'</span></div>'+
'<div class="sc-meta-item"><span class="lbl">المدة</span><span class="val">'+fmtDuration(dur)+'</span></div>'+
'<div class="sc-meta-item"><span class="lbl">التاريخ</span><span class="val">'+fmtShortDate(r.date)+'</span></div>'+
'</div>'+
'<span class="sc-counter '+ctrCls+'">المرة رقم ' + totalForName + ' للطالبة</span>'+
(r.note ? '<div class="sc-note">'+sanitizeHTML(r.note)+'</div>' : '')+
'</div>';
}).join('');
}

function renderPerm(){
const filter = currentFilter.perm;
const searchTerm = (document.getElementById('searchPerm')?.value || '').trim().toLowerCase();
let list = state.perm
.filter(x=>inFilter(x, filter))
.sort((a,b)=>(b.createdAt||0)-(a.createdAt||0));

if (searchTerm) {
list = list.filter(x => (x.name || '').toLowerCase().includes(searchTerm));
}

const root = document.getElementById('permList');
if(list.length===0){
root.innerHTML = '<div class="empty"><div class="empty-icon">🚪</div>' +
(searchTerm ? 'لا توجد نتائج للبحث' : 'لا توجد طلبات استئذان في هذه الفترة') +
'</div>';
return;
}
root.innerHTML = list.map(r=>{
return '<div class="student-card permission" data-id="'+sanitizeHTML(r.id)+'">'+
'<div class="sc-actions">'+
'<button class="sc-edit" data-act="edit-perm" data-id="'+sanitizeHTML(r.id)+'" title="تعديل">✎</button>'+
'<button class="sc-del" data-act="del-perm" data-id="'+sanitizeHTML(r.id)+'" title="حذف">×</button>'+
'</div>'+
'<div class="sc-head">'+
'<div class="sc-name">'+sanitizeHTML(r.name||'—')+'</div>'+
'<div class="sc-class permission">'+sanitizeHTML(shortSec(r.section))+'</div>'+
'</div>'+
'<div class="sc-meta">'+
'<div class="sc-meta-item"><span class="lbl">النوع</span><span class="val">'+sanitizeHTML(r.ptype||'—')+'</span></div>'+
'<div class="sc-meta-item"><span class="lbl">الخروج</span><span class="val">'+sanitizeHTML(r.outTime||'—')+'</span></div>'+
'<div class="sc-meta-item"><span class="lbl">ولي الأمر</span><span class="val">'+sanitizeHTML(r.guardian||'—')+'</span></div>'+
'<div class="sc-meta-item"><span class="lbl">التاريخ</span><span class="val">'+fmtShortDate(r.date)+'</span></div>'+
'</div>'+
(r.reason ? '<div class="sc-note"><b>السبب:</b> '+sanitizeHTML(r.reason)+'</div>' : '')+
'</div>';
}).join('');
}

function renderVio(){
const filter = currentFilter.vio;
const searchTerm = (document.getElementById('searchVio')?.value || '').trim().toLowerCase();
let list = state.vio
.filter(x=>inFilter(x, filter))
.sort((a,b)=>(b.createdAt||0)-(a.createdAt||0));

if (searchTerm) {
list = list.filter(x => (x.name || '').toLowerCase().includes(searchTerm));
}

const root = document.getElementById('vioList');
if(list.length===0){
root.innerHTML = '<div class="empty"><div class="empty-icon">⚠️</div>' +
(searchTerm ? 'لا توجد نتائج للبحث' : 'لا توجد مخالفات في هذه الفترة') +
'</div>';
return;
}
root.innerHTML = list.map(r=>{
const totalForName = countByName('vio', r.name);
const ctrCls = totalForName>=3 ? '' : (totalForName>=2 ? 'warn' : 'ok');
return '<div class="student-card violation" data-id="'+sanitizeHTML(r.id)+'">'+
'<div class="sc-actions">'+
'<button class="sc-edit" data-act="edit-vio" data-id="'+sanitizeHTML(r.id)+'" title="تعديل">✎</button>'+
'<button class="sc-del" data-act="del-vio" data-id="'+sanitizeHTML(r.id)+'" title="حذف">×</button>'+
'</div>'+
'<div class="sc-head">'+
'<div class="sc-name">'+sanitizeHTML(r.name||'—')+'</div>'+
'<div class="sc-class violation">'+sanitizeHTML(shortSec(r.section))+'</div>'+
'</div>'+
'<div class="sc-meta">'+
'<div class="sc-meta-item"><span class="lbl">المخالفة</span><span class="val">'+sanitizeHTML(r.vtype||'—')+'</span></div>'+
'<div class="sc-meta-item"><span class="lbl">الإجراء</span><span class="val">'+sanitizeHTML(r.action||'—')+'</span></div>'+
'<div class="sc-meta-item"><span class="lbl">التاريخ</span><span class="val">'+fmtShortDate(r.date)+'</span></div>'+
'</div>'+
'<span class="sc-counter '+ctrCls+'">المخالفة رقم ' + totalForName + ' للطالبة</span>'+
(r.note ? '<div class="sc-note">'+sanitizeHTML(r.note)+'</div>' : '')+
'</div>';
}).join('');
}

/* ============= MODAL FORMS ============= */
function buildSectionOptions(selectedValue){
let html = '<option value="">اختاري الفصل</option>';
GRADES.forEach(g=>{
html += '<optgroup label="'+sanitizeHTML(g.label)+'">';
g.sections.forEach(s=>{
const sel = selectedValue === s.value ? ' selected' : '';
html += '<option value="'+sanitizeHTML(s.value)+'"'+sel+'>'+sanitizeHTML(s.label)+'</option>';
});
html += '</optgroup>';
});
return html;
}

function openSettings(){
if (authState.username !== 'admin') {
toast('فقط المسؤول يمكنه تغيير الإعدادات');
return;
}
currentForm = 'settings';
editingId = null;
document.getElementById('modalTitle').textContent = 'الإعدادات';
document.getElementById('modalBody').innerHTML =
'<div class="form-grid">'+
'<div class="field">'+
'<label>وقت بداية الدوام <span class="req">*</span></label>'+
'<input type="time" name="schoolStart" value="'+sanitizeHTML(settings.schoolStart)+'">'+
'<span class="helper">يُستخدم لحساب مدة التأخر تلقائياً</span>'+
'</div>'+
'<div class="field">'+
'<label>اسم المستخدم الجديد</label>'+
'<input type="text" name="adminUser" value="'+sanitizeHTML(settings.adminUser||'')+'">'+
'</div>'+
'<div class="field">'+
'<label>كلمة المرور الجديدة</label>'+
'<input type="password" name="adminPass" placeholder="اتركيه فارغاً لعدم التغيير">'+
'</div>'+
'<div class="field">'+
'<label style="display:flex;align-items:center;gap:8px;cursor:pointer">'+
'<input type="checkbox" name="autoBackup" '+(settings.autoBackup?'checked':'')+' style="width:auto">'+
'نسخ احتياطي تلقائي'+
'</label>'+
'</div>'+
'<div class="field" style="margin-top:6px">'+
'<label>إدارة البيانات</label>'+
'<div style="display:flex;flex-direction:column;gap:8px;margin-top:6px">'+
'<button type="button" class="btn btn-secondary" id="btnImport" style="font-size:13px">'+
'📥 استيراد بيانات من ملف'+
'</button>'+
'<button type="button" class="btn btn-secondary" id="btnClearAll" style="font-size:13px;color:var(--rose-700)">'+
'🗑️ حذف جميع السجلات (لا رجعة)'+
'</button>'+
'</div>'+
'</div>'+
'<div class="field" style="margin-top:4px">'+
'<details>'+
'<summary style="cursor:pointer;font-weight:600;font-size:13px">📋 سجل التدقيق (آخر العمليات)</summary>'+
'<div style="max-height:200px;overflow-y:auto;margin-top:8px;border:1px solid var(--ink-100);border-radius:8px">'+
(auditLog.slice(-20).reverse().map(e =>
'<div class="audit-entry"><span>'+sanitizeHTML(e.action)+'</span><span class="time">'+fmtShortDate(e.timestamp.slice(0,10))+'</span></div>'
).join('') || '<div class="empty" style="padding:10px">لا توجد سجلات</div>')+
'</div>'+
'</details>'+
'</div>'+
'</div>';
document.getElementById('modal').classList.add('open');

const clr = document.getElementById('btnClearAll');
const imp = document.getElementById('btnImport');
if(clr){
clr.addEventListener('click',()=>{
if(confirm('تحذير: سيتم حذف جميع سجلات التأخر والاستئذان والمخالفات. هل أنتِ متأكدة؟')){
if(confirm('تأكيد نهائي: لا يمكن التراجع عن هذا الإجراء.')){
state = { late:[], perm:[], vio:[] };
save();
addAuditEntry('حذف جميع البيانات', '');
closeModal();
rerender();
toast('تم الحذف الكامل لجميع السجلات');
}
}
});
}
if(imp){
imp.addEventListener('click',()=>{
const input = document.createElement('input');
input.type = 'file';
input.accept = '.json';
input.onchange = (e) => {
if (e.target.files[0]) importBackup(e.target.files[0]);
};
input.click();
});
}
}

function saveSettingsForm(){
const inpTime = document.querySelector('#modalBody input[name="schoolStart"]');
const inpUser = document.querySelector('#modalBody input[name="adminUser"]');
const inpPass = document.querySelector('#modalBody input[name="adminPass"]');
const inpBackup = document.querySelector('#modalBody input[name="autoBackup"]');

if(!inpTime || !inpTime.value){ toast('الرجاء تحديد الوقت'); return; }

settings.schoolStart = inpTime.value;
if (inpUser && inpUser.value.trim()) {
settings.adminUser = inpUser.value.trim();
}
if (inpPass && inpPass.value.trim()) {
if (inpPass.value.length < 4) {
toast('كلمة المرور يجب أن تكون 4 أحرف على الأقل');
return;
}
settings.adminPass = simpleEncrypt(inpPass.value);
}
settings.autoBackup = inpBackup ? inpBackup.checked : true;

saveSettings();
addAuditEntry('تحديث الإعدادات', 'تم تغيير إعدادات النظام');
closeModal();
rerender();
toast('تم حفظ الإعدادات بنجاح');
}

function openModal(type, prefill){
currentForm = type;
editingId = prefill ? prefill.id : null;
const titles = { late:'تسجيل تأخر', perm:'تسجيل استئذان', vio:'تسجيل مخالفة' };
document.getElementById('modalTitle').textContent = (prefill?'تعديل ':'') + titles[type];
const body = document.getElementById('modalBody');
if(type==='late'){
body.innerHTML = renderLateForm(prefill);
} else if(type==='perm'){
body.innerHTML = renderPermForm(prefill);
} else if(type==='vio'){
body.innerHTML = renderVioForm(prefill);
}
bindFormEvents();
document.getElementById('modal').classList.add('open');
setTimeout(()=>{
const f = document.querySelector('#modalBody input[name="name"]');
if(f) f.focus();
}, 250);
}

function closeModal(){
document.getElementById('modal').classList.remove('open');
currentForm = null;
editingId = null;
}

function renderLateForm(p){
p = p || {};
return '' +
'<div class="form-grid">'+
'<div class="field">'+
'<label>اسم الطالبة <span class="req">*</span></label>'+
'<input type="text" name="name" value="'+sanitizeHTML(p.name||'')+'" placeholder="اكتبي الاسم الرباعي" autocomplete="off" inputmode="text" maxlength="100">'+
'<span class="helper">4-100 حرف</span>'+
'</div>'+
'<div class="field">'+
'<label>الصف والفصل <span class="req">*</span></label>'+
'<select name="section">'+buildSectionOptions(p.section)+'</select>'+
'</div>'+
'<div class="field-row">'+
'<div class="field">'+
'<label>التاريخ</label>'+
'<input type="date" name="date" value="'+sanitizeHTML(p.date||todayISO())+'" max="'+todayISO()+'">'+
'</div>'+
'<div class="field">'+
'<label>وقت الوصول <span class="req">*</span></label>'+
'<input type="time" name="arrival" value="'+sanitizeHTML(p.arrival||nowHM())+'">'+
'</div>'+
'</div>'+
'<div class="field">'+
'<label>ملاحظة (اختياري)</label>'+
'<textarea name="note" placeholder="سبب التأخر، ملاحظات المعلمة..." maxlength="500">'+sanitizeHTML(p.note||'')+'</textarea>'+
'<span class="helper">500 حرف كحد أقصى</span>'+
'</div>'+
'</div>';
}

function renderPermForm(p){
p = p || {};
const types = PERMISSION_TYPES.map(t=>
'<button type="button" class="chip blue '+(p.ptype===t?'active':'')+'" data-chip="ptype" data-val="'+sanitizeHTML(t)+'">'+sanitizeHTML(t)+'</button>'
).join('');
return '' +
'<div class="form-grid">'+
'<div class="field">'+
'<label>اسم الطالبة <span class="req">*</span></label>'+
'<input type="text" name="name" value="'+sanitizeHTML(p.name||'')+'" placeholder="اكتبي الاسم الرباعي" autocomplete="off" maxlength="100">'+
'</div>'+
'<div class="field">'+
'<label>الصف والفصل <span class="req">*</span></label>'+
'<select name="section">'+buildSectionOptions(p.section)+'</select>'+
'</div>'+
'<div class="field">'+
'<label>نوع الاستئذان <span class="req">*</span></label>'+
'<div class="chips" data-chips="ptype">'+types+'</div>'+
'<input type="hidden" name="ptype" value="'+sanitizeHTML(p.ptype||'')+'">'+
'</div>'+
'<div class="field-row">'+
'<div class="field">'+
'<label>التاريخ</label>'+
'<input type="date" name="date" value="'+sanitizeHTML(p.date||todayISO())+'" max="'+todayISO()+'">'+
'</div>'+
'<div class="field">'+
'<label>وقت الخروج</label>'+
'<input type="time" name="outTime" value="'+sanitizeHTML(p.outTime||nowHM())+'">'+
'</div>'+
'</div>'+
'<div class="field-row">'+
'<div class="field">'+
'<label>ولي الأمر</label>'+
'<input type="text" name="guardian" value="'+sanitizeHTML(p.guardian||'')+'" placeholder="اسم المستلِم" maxlength="100">'+
'</div>'+
'<div class="field">'+
'<label>الجوال</label>'+
'<input type="tel" name="phone" value="'+sanitizeHTML(p.phone||'')+'" placeholder="05xxxxxxxx" inputmode="tel" maxlength="10" pattern="05[0-9]{8}">'+
'<span class="helper">مثال: 0512345678</span>'+
'</div>'+
'</div>'+
'<div class="field">'+
'<label>سبب الاستئذان</label>'+
'<textarea name="reason" placeholder="السبب أو الموعد..." maxlength="300">'+sanitizeHTML(p.reason||'')+'</textarea>'+
'</div>'+
'</div>';
}

function renderVioForm(p){
p = p || {};
const types = VIOLATION_TYPES.map(t=>
'<button type="button" class="chip rose '+(p.vtype===t?'active':'')+'" data-chip="vtype" data-val="'+sanitizeHTML(t)+'">'+sanitizeHTML(t)+'</button>'
).join('');
const acts = VIOLATION_ACTIONS.map(a=>
'<button type="button" class="chip amber '+(p.action===a?'active':'')+'" data-chip="action" data-val="'+sanitizeHTML(a)+'">'+sanitizeHTML(a)+'</button>'
).join('');
return '' +
'<div class="form-grid">'+
'<div class="field">'+
'<label>اسم الطالبة <span class="req">*</span></label>'+
'<input type="text" name="name" value="'+sanitizeHTML(p.name||'')+'" placeholder="اكتبي الاسم الرباعي" autocomplete="off" maxlength="100">'+
'</div>'+
'<div class="field">'+
'<label>الصف والفصل <span class="req">*</span></label>'+
'<select name="section">'+buildSectionOptions(p.section)+'</select>'+
'</div>'+
'<div class="field">'+
'<label>نوع المخالفة <span class="req">*</span></label>'+
'<div class="chips-list" data-chips="vtype">'+types+'</div>'+
'<input type="hidden" name="vtype" value="'+sanitizeHTML(p.vtype||'')+'">'+
'</div>'+
'<div class="field">'+
'<label>الإجراء المتخذ</label>'+
'<div class="chips" data-chips="action">'+acts+'</div>'+
'<input type="hidden" name="action" value="'+sanitizeHTML(p.action||'')+'">'+
'</div>'+
'<div class="field">'+
'<label>التاريخ</label>'+
'<input type="date" name="date" value="'+sanitizeHTML(p.date||todayISO())+'" max="'+todayISO()+'">'+
'</div>'+
'<div class="field">'+
'<label>تفاصيل المخالفة</label>'+
'<textarea name="note" placeholder="وصف ما حدث، شهود، إلخ..." maxlength="500">'+sanitizeHTML(p.note||'')+'</textarea>'+
'</div>'+
'</div>';
}

function bindFormEvents(){
document.querySelectorAll('#modalBody .chip').forEach(c=>{
c.addEventListener('click', function(){
const group = this.parentNode.getAttribute('data-chips');
const val = this.getAttribute('data-val');
this.parentNode.querySelectorAll('.chip').forEach(b=>b.classList.remove('active'));
this.classList.add('active');
const hidden = document.querySelector('#modalBody input[name="'+group+'"]');
if(hidden) hidden.value = val;
});
});
if(editingId){
const rec = (state[currentForm]||[]).find(x=>x.id===editingId);
if(rec){
const sel = document.querySelector('#modalBody select[name="section"]');
if(sel) sel.value = rec.section || '';
}
}
}

function saveForm(){
if(currentForm === 'settings'){
saveSettingsForm();
return;
}
const body = document.getElementById('modalBody');
const data = {};
body.querySelectorAll('input,select,textarea').forEach(el=>{
if(el.name){ data[el.name] = (el.value||'').trim(); }
});

// التحقق من صحة البيانات
const nameValidation = validateName(data.name);
if (!nameValidation.valid) { toast(nameValidation.error); return; }
if (!data.section){ toast('الرجاء اختيار الصف والفصل'); return; }

// التحقق من التاريخ
if (data.date) {
const dateValidation = validateFutureDate(data.date);
if (!dateValidation.valid) { toast(dateValidation.error); return; }
}

if(currentForm==='late' && !data.arrival){ toast('الرجاء إدخال وقت الوصول'); return; }
if(currentForm==='perm'){
if (!data.ptype){ toast('الرجاء اختيار نوع الاستئذان'); return; }
if (data.phone) {
const phoneValidation = validatePhone(data.phone);
if (!phoneValidation.valid) { toast(phoneValidation.error); return; }
}
}
if(currentForm==='vio' && !data.vtype){ toast('الرجاء اختيار نوع المخالفة'); return; }

if(editingId){
const idx = state[currentForm].findIndex(x=>x.id===editingId);
if(idx>=0){
const oldData = {...state[currentForm][idx]};
state[currentForm][idx] = Object.assign({}, oldData, data);
addAuditEntry('تعديل '+currentForm, 'تم تعديل سجل للطالبة: '+data.name);
}
} else {
data.id = generateUID();
data.createdAt = Date.now();
state[currentForm].push(data);
addAuditEntry('إضافة '+currentForm, 'تم إضافة سجل للطالبة: '+data.name);
}
save();
closeModal();
rerender();
toast(editingId ? 'تم التعديل بنجاح' : 'تم الحفظ بنجاح');
}

/* ============= NAVIGATION ============= */
function goTo(scr){
document.querySelectorAll('.screen').forEach(s=>s.classList.remove('active'));
document.querySelectorAll('.nav-btn').forEach(b=>b.classList.remove('active'));
const screen = document.getElementById('screen-'+scr);
if(screen) screen.classList.add('active');
const nav = document.querySelector('.nav-btn[data-screen="'+scr+'"]');
if(nav) nav.classList.add('active');
currentScreen = scr;
const fab = document.getElementById('fab');
fab.style.display = ['late','perm','vio'].includes(scr) ? 'flex' : 'none';
rerender();
window.scrollTo({top:0,behavior:'instant'});
}

function rerender(){
resetSessionTimer();
if(currentScreen==='home') renderHome();
else if(currentScreen==='late') renderLate();
else if(currentScreen==='perm') renderPerm();
else if(currentScreen==='vio') renderVio();
updateBadges();
}

/* ============= EXPORT CSV ============= */
function exportCSV(category, period){
let rows = [];
let headers = [];
let filename = '';
let data = state[category] || [];
if(period && period!=='all'){
data = data.filter(x=>inFilter(x, period));
}
if(category==='late'){
headers = ['الاسم','الصف والفصل','التاريخ','وقت الوصول','مدة التأخر (د)','رقم المرة','ملاحظة'];
filename = 'tardies_';
rows = data.map(r=>[
r.name, secLabel(r.section), r.date, r.arrival||'',
r.arrival ? diffMinutes(settings.schoolStart, r.arrival) : '',
countByName('late', r.name),
r.note||''
]);
} else if(category==='perm'){
headers = ['الاسم','الصف والفصل','التاريخ','نوع الاستئذان','وقت الخروج','ولي الأمر','الجوال','السبب'];
filename = 'permissions_';
rows = data.map(r=>[
r.name, secLabel(r.section), r.date, r.ptype||'', r.outTime||'',
r.guardian||'', r.phone||'', r.reason||''
]);
} else if(category==='vio'){
headers = ['الاسم','الصف والفصل','التاريخ','نوع المخالفة','الإجراء','رقم المخالفة','تفاصيل'];
filename = 'violations_';
rows = data.map(r=>[
r.name, secLabel(r.section), r.date, r.vtype||'', r.action||'',
countByName('vio', r.name),
r.note||''
]);
} else if(category==='all'){
const lines = [];
lines.push('=== التأخر الصباحي ===');
const h1 = ['الاسم','الصف','التاريخ','الوصول','المدة','المرة','ملاحظة'];
lines.push(h1.join(','));
state.late.forEach(r=>{
const row = [
r.name, secLabel(r.section), r.date, r.arrival||'',
r.arrival?diffMinutes(settings.schoolStart,r.arrival):'',
countByName('late', r.name), r.note||''
];
lines.push(row.map(csvEscape).join(','));
});
lines.push('');
lines.push('=== الاستئذان ===');
lines.push(['الاسم','الصف','التاريخ','النوع','الخروج','ولي الأمر','الجوال','السبب'].join(','));
state.perm.forEach(r=>{
lines.push([r.name,secLabel(r.section),r.date,r.ptype||'',r.outTime||'',r.guardian||'',r.phone||'',r.reason||''].map(csvEscape).join(','));
});
lines.push('');
lines.push('=== المخالفات ===');
lines.push(['الاسم','الصف','التاريخ','المخالفة','الإجراء','المرة','تفاصيل'].join(','));
state.vio.forEach(r=>{
lines.push([r.name,secLabel(r.section),r.date,r.vtype||'',r.action||'',countByName('vio',r.name),r.note||''].map(csvEscape).join(','));
});
downloadCSV(lines.join('\n'), 'all_records_'+todayISO()+'.csv');
addAuditEntry('تصدير CSV', 'تصدير جميع السجلات');
return;
}

const csv = [headers, ...rows].map(r=>r.map(csvEscape).join(',')).join('\n');
downloadCSV(csv, filename + todayISO() + '.csv');
addAuditEntry('تصدير CSV', 'تصدير '+category+' - الفترة: '+period);
}

function csvEscape(v){
if(v==null) return '';
const s = String(v);
if(/[",\n\r]/.test(s)) return '"' + s.replace(/"/g,'""') + '"';
return s;
}

function downloadCSV(content, filename){
const BOM = '\uFEFF';
const blob = new Blob([BOM + content], {type:'text/csv;charset=utf-8'});
const url = URL.createObjectURL(blob);
const a = document.createElement('a');
a.href = url; a.download = filename;
document.body.appendChild(a);
a.click();
document.body.removeChild(a);
setTimeout(()=>URL.revokeObjectURL(url), 1000);
toast('تم تصدير الملف');
}

/* ============= REPORT ============= */
function generateReport(){
const rng = document.getElementById('reportRange').value;
let from, to, label;
const now = new Date();
if(rng==='week'){
const s = startOfWeek(now), e = endOfWeek(now);
from = isoFromDate(s); to = isoFromDate(e);
label = 'الأسبوع الحالي ('+fmtShortDate(from)+' — '+fmtShortDate(to)+')';
} else if(rng==='lastweek'){
const s = startOfWeek(new Date(now.getTime() - 7*86400000));
const e = endOfWeek(s);
from = isoFromDate(s); to = isoFromDate(e);
label = 'الأسبوع السابق ('+fmtShortDate(from)+' — '+fmtShortDate(to)+')';
} else if(rng==='month'){
from = now.getFullYear()+'-'+pad(now.getMonth()+1)+'-01';
const lastDay = new Date(now.getFullYear(), now.getMonth()+1, 0).getDate();
to = now.getFullYear()+'-'+pad(now.getMonth()+1)+'-'+pad(lastDay);
label = 'شهر '+pad(now.getMonth()+1)+'/'+now.getFullYear();
} else {
from = document.getElementById('rFrom').value;
to = document.getElementById('rTo').value;
if(!from || !to){ toast('الرجاء تحديد الفترة'); return; }
if (from > to) { toast('تاريخ البداية يجب أن يكون قبل تاريخ النهاية'); return; }
label = fmtShortDate(from)+' — '+fmtShortDate(to);
}
const lateF = state.late.filter(x=>inDateRange(x,from,to));
const permF = state.perm.filter(x=>inDateRange(x,from,to));
const vioF = state.vio.filter(x=>inDateRange(x,from,to));

document.getElementById('reportPeriod').textContent = label;
document.getElementById('r-late').textContent = lateF.length;
document.getElementById('r-perm').textContent = permF.length;
document.getElementById('r-vio').textContent = vioF.length;

const byGrade = (arr)=>({
'1': arr.filter(r=>gradeFromSec(r.section)==='1').length,
'2': arr.filter(r=>gradeFromSec(r.section)==='2').length,
'3': arr.filter(r=>gradeFromSec(r.section)==='3').length
});
const t1 = byGrade(lateF), t2 = byGrade(permF), t3 = byGrade(vioF);
document.getElementById('r-st-1').textContent = t1['1']+t2['1']+t3['1'];
document.getElementById('r-st-2').textContent = t1['2']+t2['2']+t3['2'];
document.getElementById('r-st-3').textContent = t1['3']+t2['3']+t3['3'];

const repeatMap = {};
[...lateF.map(x=>({...x,_t:'تأخر'})),
...permF.map(x=>({...x,_t:'استئذان'})),
...vioF.map(x=>({...x,_t:'مخالفة'}))].forEach(r=>{
const k = (r.name || '').trim().replace(/\s+/g, ' ');
if(!k) return;
if(!repeatMap[k]) repeatMap[k] = { name:k, section:r.section, late:0, perm:0, vio:0, total:0 };
if(r._t==='تأخر') repeatMap[k].late++;
else if(r._t==='استئذان') repeatMap[k].perm++;
else repeatMap[k].vio++;
repeatMap[k].total++;
});
const repeats = Object.values(repeatMap).filter(r=>r.total>=3).sort((a,b)=>b.total-a.total);
const rl = document.getElementById('r-repeat-list');
if(repeats.length===0){
rl.innerHTML = '<div class="empty" style="padding:14px"><em>لا توجد حالات متكررة في هذه الفترة (٣ حالات أو أكثر)</em></div>';
} else {
rl.innerHTML = '<table class="report-table"><thead><tr>'+
'<th>الاسم</th><th>الفصل</th><th>تأخر</th><th>استئذان</th><th>مخالفات</th><th>المجموع</th>'+
'</tr></thead><tbody>'+
repeats.map(r=>'<tr>'+
'<td>'+sanitizeHTML(r.name)+'</td>'+
'<td>'+sanitizeHTML(shortSec(r.section))+'</td>'+
'<td>'+r.late+'</td><td>'+r.perm+'</td><td>'+r.vio+'</td><td><b>'+r.total+'</b></td>'+
'</tr>').join('')+
'</tbody></table>';
}

document.getElementById('r-late-details').innerHTML = renderTable(lateF, ['name','section','date','arrival','note'],
['الاسم','الفصل','التاريخ','الوصول','ملاحظة']);
document.getElementById('r-perm-details').innerHTML = renderTable(permF, ['name','section','date','ptype','outTime','reason'],
['الاسم','الفصل','التاريخ','النوع','الخروج','السبب']);
document.getElementById('r-vio-details').innerHTML = renderTable(vioF, ['name','section','date','vtype','action','note'],
['الاسم','الفصل','التاريخ','المخالفة','الإجراء','تفاصيل']);

document.getElementById('reportOutput').style.display = 'block';
document.getElementById('reportOutput').scrollIntoView({behavior:'smooth',block:'start'});
addAuditEntry('توليد تقرير', 'الفترة: '+label);
}

function isoFromDate(d){
return d.getFullYear()+'-'+pad(d.getMonth()+1)+'-'+pad(d.getDate());
}

function renderTable(arr, fields, labels){
if(arr.length===0) return '<div class="empty" style="padding:14px"><em>لا توجد بيانات في هذه الفترة</em></div>';
let html = '<div style="overflow-x:auto"><table class="report-table"><thead><tr>';
labels.forEach(l=>html+='<th>'+sanitizeHTML(l)+'</th>');
html += '</tr></thead><tbody>';
arr.sort((a,b)=>(a.date||'').localeCompare(b.date||'')).forEach(r=>{
html += '<tr>';
fields.forEach(f=>{
let v = r[f]||'';
if(f==='section') v = shortSec(v);
if(f==='date') v = fmtShortDate(v);
html += '<td>'+sanitizeHTML(v)+'</td>';
});
html += '</tr>';
});
html += '</tbody></table></div>';
return html;
}

function exportReport(){
const rng = document.getElementById('reportRange').value;
let from, to, label;
const now = new Date();
if(rng==='week'){
from = isoFromDate(startOfWeek(now)); to = isoFromDate(endOfWeek(now));
label = 'week_'+from;
} else if(rng==='lastweek'){
const s = startOfWeek(new Date(now.getTime() - 7*86400000));
from = isoFromDate(s); to = isoFromDate(endOfWeek(s));
label = 'lastweek_'+from;
} else if(rng==='month'){
from = now.getFullYear()+'-'+pad(now.getMonth()+1)+'-01';
const ld = new Date(now.getFullYear(), now.getMonth()+1, 0).getDate();
to = now.getFullYear()+'-'+pad(now.getMonth()+1)+'-'+pad(ld);
label = 'month_'+from.slice(0,7);
} else {
from = document.getElementById('rFrom').value;
to = document.getElementById('rTo').value;
label = 'custom_'+from+'_'+to;
}
const lateF = state.late.filter(x=>inDateRange(x,from,to));
const permF = state.perm.filter(x=>inDateRange(x,from,to));
const vioF = state.vio.filter(x=>inDateRange(x,from,to));
const lines = [];
lines.push('التقرير الإداري - الثانوية الثامنة بالخرج');
lines.push('الفترة: '+from+' إلى '+to);
lines.push('المساعد الإداري: غزيل الشمراني');
lines.push('');
lines.push('=== التأخر الصباحي ('+lateF.length+') ===');
lines.push(['الاسم','الفصل','التاريخ','الوصول','المدة (د)','المرة','ملاحظة'].join(','));
lateF.forEach(r=>{
lines.push([r.name,secLabel(r.section),r.date,r.arrival||'',
r.arrival?diffMinutes(settings.schoolStart,r.arrival):'',
countByName('late',r.name),r.note||''].map(csvEscape).join(','));
});
lines.push('');
lines.push('=== الاستئذان ('+permF.length+') ===');
lines.push(['الاسم','الفصل','التاريخ','النوع','الخروج','ولي الأمر','الجوال','السبب'].join(','));
permF.forEach(r=>{
lines.push([r.name,secLabel(r.section),r.date,r.ptype||'',r.outTime||'',r.guardian||'',r.phone||'',r.reason||''].map(csvEscape).join(','));
});
lines.push('');
lines.push('=== المخالفات ('+vioF.length+') ===');
lines.push(['الاسم','الفصل','التاريخ','المخالفة','الإجراء','المرة','تفاصيل'].join(','));
vioF.forEach(r=>{
lines.push([r.name,secLabel(r.section),r.date,r.vtype||'',r.action||'',countByName('vio',r.name),r.note||''].map(csvEscape).join(','));
});
downloadCSV(lines.join('\n'), 'report_'+label+'.csv');
addAuditEntry('تصدير تقرير CSV', 'الفترة: '+label);
}

/* ============= EVENT BINDING ============= */
function bindEvents(){
// Login
document.getElementById('btnLogin').addEventListener('click', () => {
const user = document.getElementById('loginUser').value.trim();
const pass = document.getElementById('loginPass').value;
if (login(user, pass)) {
document.getElementById('loginError').classList.remove('show');
} else {
document.getElementById('loginError').classList.add('show');
}
});

// Enter key for login
document.getElementById('loginPass').addEventListener('keypress', (e) => {
if (e.key === 'Enter') {
document.getElementById('btnLogin').click();
}
});

// Logout
document.getElementById('btnLogout').addEventListener('click', () => logout(true));

// Settings
document.getElementById('btnSettings').addEventListener('click', openSettings);

// Navigation
document.querySelectorAll('.nav-btn').forEach(b=>{
b.addEventListener('click',()=>goTo(b.getAttribute('data-screen')));
});

// FAB
document.getElementById('fab').addEventListener('click',()=>{
if(currentScreen==='late') openModal('late');
else if(currentScreen==='perm') openModal('perm');
else if(currentScreen==='vio') openModal('vio');
});

// Modal
document.getElementById('modalClose').addEventListener('click', closeModal);
document.getElementById('modal').addEventListener('click',(e)=>{
if(e.target.id==='modal') closeModal();
});
document.getElementById('modalSave').addEventListener('click', saveForm);

// Delete & Edit (delegated)
document.body.addEventListener('click',(e)=>{
const delBtn = e.target.closest('[data-act^="del-"]');
const editBtn = e.target.closest('[data-act^="edit-"]');

if (delBtn) {
const act = delBtn.getAttribute('data-act');
const id = delBtn.getAttribute('data-id');
const cat = act.slice(4);
if(confirm('هل تريدين حذف هذا السجل؟ (يمكن التراجع فقط باستعادة النسخة الاحتياطية)')){
const removed = state[cat].find(x=>x.id===id);
state[cat] = state[cat].filter(x=>x.id!==id);
save();
addAuditEntry('حذف '+cat, 'حذف سجل: '+(removed?.name||''));
rerender();
toast('تم الحذف');
}
}

if (editBtn) {
const act = editBtn.getAttribute('data-act');
const id = editBtn.getAttribute('data-id');
const cat = act.slice(5);
const rec = state[cat].find(x=>x.id===id);
if (rec) {
openModal(cat, rec);
}
}
});

// Filters
document.querySelectorAll('.filter-row').forEach(row=>{
row.addEventListener('click',(e)=>{
const pill = e.target.closest('.filter-pill');
if(!pill) return;
row.querySelectorAll('.filter-pill').forEach(p=>p.classList.remove('active'));
pill.classList.add('active');
const filter = pill.getAttribute('data-filter');
currentFilter[currentScreen] = filter;
rerender();
});
});

// Search
['searchLate','searchPerm','searchVio'].forEach(id => {
const el = document.getElementById(id);
if (el) {
el.addEventListener('input', () => {
if (currentScreen === 'late' && id === 'searchLate') renderLate();
else if (currentScreen === 'perm' && id === 'searchPerm') renderPerm();
else if (currentScreen === 'vio' && id === 'searchVio') renderVio();
});
}
});

// Print buttons
document.querySelectorAll('[data-print]').forEach(b=>{
b.addEventListener('click',()=>window.print());
});

// Export buttons
document.querySelectorAll('[data-export]').forEach(b=>{
b.addEventListener('click',()=>exportCSV(b.getAttribute('data-export'), currentFilter[currentScreen]));
});
document.getElementById('btnExportAll').addEventListener('click',()=>exportCSV('all'));
document.getElementById('btnBackup').addEventListener('click', createBackup);

// Report
document.getElementById('reportRange').addEventListener('change',(e)=>{
document.getElementById('customRange').style.display = e.target.value==='custom' ? 'grid' : 'none';
});
document.getElementById('btnGenReport').addEventListener('click', generateReport);
document.getElementById('btnPrintReport').addEventListener('click',()=>window.print());
document.getElementById('btnExportReport').addEventListener('click', exportReport);

// Click anywhere to reset session timer
document.addEventListener('click', resetSessionTimer);
document.addEventListener('keypress', resetSessionTimer);
}

/* ============= INIT ============= */
function init(){
load();
loadAudit();

if (authState.isLoggedIn) {
const elapsed = Date.now() - authState.loginTime;
if (elapsed < settings.sessionTimeout) {
showApp();
startSessionTimer();
} else {
logout(false);
}
}

renderTopDate();
setInterval(renderTopDate, 60000);
bindEvents();
startAutoSave();
// التحقق من وجود نسخة احتياطية قديمة
const lastBackup = localStorage.getItem(STORAGE_KEY + '_backup');
if (!lastBackup && (state.late.length > 0 || state.perm.length > 0 || state.vio.length > 0)) {
save(); // إنشاء نسخة احتياطية أولى
}
}

if(document.readyState==='loading'){
document.addEventListener('DOMContentLoaded', init);
} else {
init();
}
})();
</script>

</body>
</html>
