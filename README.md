[jadwal_ikhtibarat (2).html](https://github.com/user-attachments/files/28182515/jadwal_ikhtibarat.2.html)
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>جداول الاختبارات النهائية</title>
<link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@400;500;700;800&display=swap" rel="stylesheet">
<style>
:root {
  --indigo:   #5B6AF0;
  --indigo-d: #3A47C7;
  --indigo-l: #EEF0FD;
  --indigo-b: #C7CBFA;
  --sage:     #4BAD8A;
  --sage-d:   #2E7A61;
  --sage-l:   #E6F5F0;
  --sage-b:   #A8D9CA;
  --amber:    #D4882A;
  --amber-d:  #9A5F13;
  --amber-l:  #FDF3E3;
  --amber-b:  #F2C97A;
  --rose:     #D95F72;
  --rose-d:   #9B3249;
  --rose-l:   #FCEEF1;
  --rose-b:   #F0A8B4;
  --bg:       #F0EEE9;
  --surface:  #FAFAF7;
  --card:     #FFFFFF;
  --text:     #1A1916;
  --text2:    #5C5A53;
  --text3:    #9A9890;
  --border:   rgba(26,25,22,0.09);
  --border2:  rgba(26,25,22,0.16);
}
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
body{font-family:'Tajawal',sans-serif;background:var(--bg);color:var(--text);min-height:100vh;padding-bottom:60px}

/* ─── HERO ─── */
.hero{
  background:linear-gradient(160deg,#3A47C7 0%,#5B6AF0 55%,#7B87F5 100%);
  padding:52px 24px 86px;text-align:center;position:relative;overflow:hidden
}
.hero::after{
  content:'';position:absolute;inset:0;
  background:url("data:image/svg+xml,%3Csvg width='60' height='60' viewBox='0 0 60 60' xmlns='http://www.w3.org/2000/svg'%3E%3Ccircle cx='30' cy='30' r='1.2' fill='rgba(255,255,255,0.10)'/%3E%3C/svg%3E");
}
.hero h1{font-size:30px;font-weight:800;color:#fff;position:relative;z-index:1;margin-bottom:8px;letter-spacing:-.3px}
.hero p{font-size:14px;color:rgba(255,255,255,0.78);position:relative;z-index:1}
.hero-chip{display:inline-block;background:rgba(255,255,255,0.14);border:1px solid rgba(255,255,255,0.22);
  color:#fff;font-size:11px;font-weight:600;padding:4px 14px;border-radius:20px;margin-bottom:14px;position:relative;z-index:1;letter-spacing:.5px}

/* ─── WRAPPER ─── */
.wrap{max-width:740px;margin:-40px auto 0;padding:0 14px;position:relative}

/* ─── INFO BAR ─── */
.info-bar{background:var(--card);border-radius:14px;border:1px solid var(--border);
  padding:13px 18px;display:flex;align-items:center;gap:10px;margin-bottom:18px;
  box-shadow:0 1px 8px rgba(0,0,0,0.05)}
.info-num{width:26px;height:26px;border-radius:50%;background:var(--indigo-l);color:var(--indigo-d);
  display:flex;align-items:center;justify-content:center;font-size:12px;font-weight:800;flex-shrink:0}
.info-bar p{font-size:13px;color:var(--text2)}.info-bar strong{color:var(--text)}

/* ─── LEGEND ─── */
.legend{display:flex;flex-wrap:wrap;gap:10px;margin-bottom:18px}
.leg{display:flex;align-items:center;gap:6px;font-size:11px;font-weight:600;
  color:var(--text2);background:var(--card);border:1px solid var(--border);
  border-radius:20px;padding:5px 12px}
.leg-dot{width:8px;height:8px;border-radius:2px;flex-shrink:0}

/* ─── SCHEDULE CARDS ─── */
.schedules{display:flex;flex-direction:column;gap:14px;margin-bottom:20px}
.sc{background:var(--card);border-radius:16px;border:2px solid var(--border);overflow:hidden;
  cursor:pointer;transition:border-color .2s,box-shadow .2s,transform .15s;
  box-shadow:0 1px 6px rgba(0,0,0,0.04)}
.sc:hover{transform:translateY(-2px);box-shadow:0 5px 18px rgba(0,0,0,0.08)}
.sc.s0{border-color:var(--indigo);  box-shadow:0 0 0 4px rgba(91,106,240,.13)}
.sc.s1{border-color:var(--sage);    box-shadow:0 0 0 4px rgba(75,173,138,.13)}
.sc.s2{border-color:var(--rose);    box-shadow:0 0 0 4px rgba(217,95,114,.13)}

.ch{display:flex;align-items:center;justify-content:space-between;padding:14px 16px 10px}
.chl{display:flex;align-items:center;gap:10px}
.cnum{width:34px;height:34px;border-radius:9px;display:flex;align-items:center;justify-content:center;font-size:15px;font-weight:800;flex-shrink:0}
.n0{background:var(--indigo-l);color:var(--indigo-d)}
.n1{background:var(--sage-l);color:var(--sage-d)}
.n2{background:var(--rose-l);color:var(--rose-d)}
.ctitle{font-size:15px;font-weight:700;color:var(--text)}
.csub{font-size:11px;color:var(--text3);margin-top:2px}

.radio{width:20px;height:20px;border-radius:50%;border:2px solid var(--border2);background:var(--bg);
  display:flex;align-items:center;justify-content:center;transition:border-color .2s;flex-shrink:0}
.radio-dot{width:10px;height:10px;border-radius:50%;transform:scale(0);transition:transform .2s}
.sc.s0 .radio{border-color:var(--indigo)}.sc.s0 .radio-dot{background:var(--indigo);transform:scale(1)}
.sc.s1 .radio{border-color:var(--sage)}.sc.s1 .radio-dot{background:var(--sage);transform:scale(1)}
.sc.s2 .radio{border-color:var(--rose)}.sc.s2 .radio-dot{background:var(--rose);transform:scale(1)}

/* ─── DAYS GRID ─── */
.dgrid{display:grid;grid-template-columns:repeat(4,1fr);gap:7px;padding:0 12px 14px}
.dbox{border-radius:10px;padding:9px 5px;text-align:center;border:1px solid transparent}
.dday{font-size:10px;font-weight:600;margin-bottom:4px;opacity:.65}
.dsub{font-size:12px;font-weight:800}
.dm{background:var(--indigo-l);border-color:var(--indigo-b)}.dm .dday{color:var(--indigo-d)}.dm .dsub{color:var(--indigo-d)}
.dl{background:var(--sage-l);border-color:var(--sage-b)}.dl .dday{color:var(--sage-d)}.dl .dsub{color:var(--sage-d)}
.ds{background:var(--amber-l);border-color:var(--amber-b)}.ds .dday{color:var(--amber-d)}.ds .dsub{color:var(--amber-d)}
.de{background:var(--rose-l);border-color:var(--rose-b)}.de .dday{color:var(--rose-d)}.de .dsub{color:var(--rose-d)}

/* ─── CONFIRM ─── */
.conf-wrap{text-align:center;margin-bottom:26px}
.conf-btn{display:inline-flex;align-items:center;gap:8px;padding:13px 36px;border-radius:12px;
  font-family:'Tajawal',sans-serif;font-size:15px;font-weight:700;border:none;cursor:pointer;color:#fff;
  background:linear-gradient(135deg,var(--indigo-d),var(--indigo));
  box-shadow:0 4px 14px rgba(91,106,240,.38);transition:transform .15s,box-shadow .15s}
.conf-btn:hover{transform:translateY(-2px);box-shadow:0 7px 22px rgba(91,106,240,.42)}
.conf-btn:active{transform:scale(0.98)}
.conf-btn:disabled{opacity:.4;cursor:not-allowed;transform:none;box-shadow:none}

/* ─── RESULT ─── */
.result{display:none;background:var(--card);border-radius:16px;border:2px solid var(--border);
  overflow:hidden;margin-bottom:22px;box-shadow:0 3px 16px rgba(0,0,0,0.07);animation:up .4s ease}
@keyframes up{from{opacity:0;transform:translateY(18px)}to{opacity:1;transform:translateY(0)}}
.rbanner{padding:18px 20px;display:flex;align-items:center;gap:12px}
.ricon{width:46px;height:46px;border-radius:12px;display:flex;align-items:center;justify-content:center;font-size:22px;flex-shrink:0}
.rtext h3{font-size:17px;font-weight:800}.rtext p{font-size:12px;margin-top:2px}
.rdays{padding:0 14px 16px;display:grid;grid-template-columns:repeat(4,1fr);gap:7px}
.reset-btn{background:none;border:1px solid var(--border2);border-radius:9px;padding:7px 16px;
  font-family:'Tajawal',sans-serif;font-size:12px;color:var(--text3);cursor:pointer;transition:background .15s}
.reset-btn:hover{background:var(--bg)}

/* ─── TEACHER GATE ─── */
.teacher-gate{background:var(--card);border-radius:16px;border:1px solid var(--border);
  padding:20px 18px;margin-bottom:22px;box-shadow:0 1px 8px rgba(0,0,0,0.05)}
.gate-top{display:flex;align-items:center;gap:10px;margin-bottom:14px}
.gate-icon{width:34px;height:34px;border-radius:9px;background:var(--indigo-l);color:var(--indigo-d);
  display:flex;align-items:center;justify-content:center;font-size:16px;flex-shrink:0}
.gate-title{font-size:14px;font-weight:700;color:var(--text)}
.gate-sub{font-size:11px;color:var(--text3)}
.gate-row{display:flex;gap:8px}
.gate-input{flex:1;padding:10px 14px;border-radius:9px;border:1px solid var(--border2);
  font-family:'Tajawal',sans-serif;font-size:14px;background:var(--bg);color:var(--text);outline:none;transition:border-color .2s}
.gate-input:focus{border-color:var(--indigo)}
.gate-btn{padding:10px 20px;border-radius:9px;background:var(--indigo);color:#fff;border:none;
  font-family:'Tajawal',sans-serif;font-size:14px;font-weight:700;cursor:pointer;transition:background .15s;white-space:nowrap}
.gate-btn:hover{background:var(--indigo-d)}
.gate-err{font-size:12px;color:var(--rose-d);margin-top:6px;display:none}

/* ─── STATS ─── */
.stats{display:none;background:var(--card);border-radius:16px;border:1px solid var(--border);
  padding:20px 18px;margin-bottom:22px;box-shadow:0 1px 8px rgba(0,0,0,0.05);animation:up .35s ease}
.stats-head{display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:8px;margin-bottom:16px}
.stats-title{font-size:15px;font-weight:700;color:var(--text)}
.stats-badge{background:var(--indigo-l);color:var(--indigo-d);font-size:11px;font-weight:700;
  padding:4px 12px;border-radius:20px}
.srow{margin-bottom:13px}
.srow-top{display:flex;align-items:center;justify-content:space-between;margin-bottom:5px}
.slabel{display:flex;align-items:center;gap:7px;font-size:13px;font-weight:700;color:var(--text)}
.sdot{width:9px;height:9px;border-radius:2px;flex-shrink:0}
.snums{font-size:12px;color:var(--text3)}.snums b{color:var(--text)}
.track{background:var(--bg);border-radius:99px;height:9px;overflow:hidden}
.fill{height:9px;border-radius:99px;transition:width .65s ease}
.chart-wrap{position:relative;height:190px;width:100%;margin-top:18px}
.chart-leg{display:flex;flex-wrap:wrap;gap:12px;margin-top:10px;justify-content:center}
.cli{display:flex;align-items:center;gap:5px;font-size:11px;color:var(--text3)}
.clb{width:9px;height:9px;border-radius:2px}
.logout-btn{display:block;margin:14px auto 0;background:none;border:1px solid var(--border2);
  border-radius:9px;padding:6px 14px;font-family:'Tajawal',sans-serif;font-size:11px;color:var(--text3);
  cursor:pointer;transition:background .15s}
.logout-btn:hover{background:var(--bg)}

@media(max-width:480px){
  .hero h1{font-size:24px}.dgrid{gap:5px}.dsub{font-size:11px}.chart-wrap{height:155px}
}
</style>
</head>
<body>

<div class="hero">
  <span class="hero-chip">الفصل الدراسي الثاني</span>
  <h1>🎓 جداول الاختبارات النهائية</h1>
  <p>اقرأ الجداول الثلاثة واختر الجدول الأنسب لك</p>
</div>

<div class="wrap">

  <!-- INFO BAR -->
  <div class="info-bar">
    <div class="info-num">١</div>
    <p><strong>اختر جدولاً واحداً</strong> من الخيارات أدناه ثم اضغط تأكيد</p>
  </div>

  <!-- LEGEND -->
  <div class="legend">
    <div class="leg"><span class="leg-dot" style="background:var(--indigo)"></span>الرياضيات — ثابت</div>
    <div class="leg"><span class="leg-dot" style="background:var(--sage)"></span>لغتي</div>
    <div class="leg"><span class="leg-dot" style="background:var(--amber)"></span>العلوم</div>
    <div class="leg"><span class="leg-dot" style="background:var(--rose)"></span>الإنجليزي</div>
  </div>

  <!-- SCHEDULES -->
  <div class="schedules" id="schedules">
    <!-- J1 -->
    <div class="sc" id="c0" onclick="pick(0)">
      <div class="ch">
        <div class="chl">
          <div class="cnum n0">١</div>
          <div><div class="ctitle">الجدول الأول</div><div class="csub">لغتي &larr; العلوم &larr; الإنجليزي</div></div>
        </div>
        <div class="radio"><div class="radio-dot"></div></div>
      </div>
      <div class="dgrid">
        <div class="dbox dm"><div class="dday">الأحد</div><div class="dsub">رياضيات</div></div>
        <div class="dbox dl"><div class="dday">الاثنين</div><div class="dsub">لغتي</div></div>
        <div class="dbox ds"><div class="dday">الثلاثاء</div><div class="dsub">العلوم</div></div>
        <div class="dbox de"><div class="dday">الأربعاء</div><div class="dsub">إنجليزي</div></div>
      </div>
    </div>
    <!-- J2 -->
    <div class="sc" id="c1" onclick="pick(1)">
      <div class="ch">
        <div class="chl">
          <div class="cnum n1">٢</div>
          <div><div class="ctitle">الجدول الثاني</div><div class="csub">العلوم &larr; الإنجليزي &larr; لغتي</div></div>
        </div>
        <div class="radio"><div class="radio-dot"></div></div>
      </div>
      <div class="dgrid">
        <div class="dbox dm"><div class="dday">الأحد</div><div class="dsub">رياضيات</div></div>
        <div class="dbox ds"><div class="dday">الاثنين</div><div class="dsub">العلوم</div></div>
        <div class="dbox de"><div class="dday">الثلاثاء</div><div class="dsub">إنجليزي</div></div>
        <div class="dbox dl"><div class="dday">الأربعاء</div><div class="dsub">لغتي</div></div>
      </div>
    </div>
    <!-- J3 -->
    <div class="sc" id="c2" onclick="pick(2)">
      <div class="ch">
        <div class="chl">
          <div class="cnum n2">٣</div>
          <div><div class="ctitle">الجدول الثالث</div><div class="csub">الإنجليزي &larr; لغتي &larr; العلوم</div></div>
        </div>
        <div class="radio"><div class="radio-dot"></div></div>
      </div>
      <div class="dgrid">
        <div class="dbox dm"><div class="dday">الأحد</div><div class="dsub">رياضيات</div></div>
        <div class="dbox de"><div class="dday">الاثنين</div><div class="dsub">إنجليزي</div></div>
        <div class="dbox dl"><div class="dday">الثلاثاء</div><div class="dsub">لغتي</div></div>
        <div class="dbox ds"><div class="dday">الأربعاء</div><div class="dsub">العلوم</div></div>
      </div>
    </div>
  </div>

  <!-- CONFIRM -->
  <div class="conf-wrap" id="confWrap">
    <button class="conf-btn" id="confBtn" onclick="doConfirm()" disabled>✓ تأكيد اختياري</button>
  </div>

  <!-- RESULT -->
  <div class="result" id="result">
    <div class="rbanner" id="rbanner"></div>
    <div class="rdays" id="rdays"></div>
    <div style="text-align:center;padding-bottom:14px">
      <button class="reset-btn" onclick="doReset()">↩ تغيير الاختيار</button>
    </div>
  </div>

  <!-- TEACHER GATE -->
  <div class="teacher-gate" id="gate">
    <div class="gate-top">
      <div class="gate-icon">🔒</div>
      <div><div class="gate-title">لوحة المعلم</div><div class="gate-sub">أدخل كلمة المرور لعرض الإحصائيات</div></div>
    </div>
    <div class="gate-row">
      <input class="gate-input" type="password" id="pwInput" placeholder="كلمة المرور..." onkeydown="if(event.key==='Enter')tryLogin()">
      <button class="gate-btn" onclick="tryLogin()">دخول</button>
    </div>
    <div class="gate-err" id="gateErr">كلمة المرور غير صحيحة</div>
  </div>

  <!-- STATS (hidden until teacher logs in) -->
  <div class="stats" id="statsPanel">
    <div class="stats-head">
      <div>
        <div class="stats-title">📊 إحصائيات اختيار الطلاب</div>
      </div>
      <div class="stats-badge" id="totalBadge">إجمالي: 0 صوت</div>
    </div>

    <div class="srow">
      <div class="srow-top">
        <div class="slabel"><span class="sdot" style="background:var(--indigo)"></span>الجدول الأول</div>
        <div class="snums"><b id="cnt0">0</b> صوت · <b id="pct0">0%</b></div>
      </div>
      <div class="track"><div class="fill" id="bar0" style="width:0%;background:var(--indigo)"></div></div>
    </div>

    <div class="srow">
      <div class="srow-top">
        <div class="slabel"><span class="sdot" style="background:var(--sage)"></span>الجدول الثاني</div>
        <div class="snums"><b id="cnt1">0</b> صوت · <b id="pct1">0%</b></div>
      </div>
      <div class="track"><div class="fill" id="bar1" style="width:0%;background:var(--sage)"></div></div>
    </div>

    <div class="srow">
      <div class="srow-top">
        <div class="slabel"><span class="sdot" style="background:var(--rose)"></span>الجدول الثالث</div>
        <div class="snums"><b id="cnt2">0</b> صوت · <b id="pct2">0%</b></div>
      </div>
      <div class="track"><div class="fill" id="bar2" style="width:0%;background:var(--rose)"></div></div>
    </div>

    <div class="chart-wrap">
      <canvas id="voteChart" role="img" aria-label="رسم دائري لنسب اختيار الجداول">لا توجد بيانات.</canvas>
    </div>
    <div class="chart-leg">
      <span class="cli"><span class="clb" style="background:var(--indigo)"></span>الجدول الأول</span>
      <span class="cli"><span class="clb" style="background:var(--sage)"></span>الجدول الثاني</span>
      <span class="cli"><span class="clb" style="background:var(--rose)"></span>الجدول الثالث</span>
    </div>

    <div style="display:flex;gap:8px;justify-content:center;margin-top:14px;flex-wrap:wrap">
      <button class="logout-btn" onclick="doLogout()">🚪 تسجيل الخروج</button>
      <button class="logout-btn" onclick="clearAll()" style="color:var(--rose-d);border-color:var(--rose-b)">🗑 مسح جميع الأصوات</button>
    </div>
  </div>

</div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/4.4.1/chart.umd.js"></script>
<script>
/* ── CONFIG ─────────────────────────────────── */
const TEACHER_PASS = 'معلم2025';   /* ← غيّر كلمة المرور هنا */
const VOTES_KEY   = 'jadwal_v2_votes';
const MYVOTE_KEY  = 'jadwal_v2_mine';
const SESSION_KEY = 'jadwal_v2_sess';
/* ─────────────────────────────────────────── */

const SD = [
  { name:'الجدول الأول', c:'#5B6AF0', bg:'#EEF0FD', tc:'#3A47C7', em:'📘',
    days:[{d:'الأحد',s:'رياضيات',cl:'dm'},{d:'الاثنين',s:'لغتي',cl:'dl'},{d:'الثلاثاء',s:'العلوم',cl:'ds'},{d:'الأربعاء',s:'إنجليزي',cl:'de'}]},
  { name:'الجدول الثاني', c:'#4BAD8A', bg:'#E6F5F0', tc:'#2E7A61', em:'📗',
    days:[{d:'الأحد',s:'رياضيات',cl:'dm'},{d:'الاثنين',s:'العلوم',cl:'ds'},{d:'الثلاثاء',s:'إنجليزي',cl:'de'},{d:'الأربعاء',s:'لغتي',cl:'dl'}]},
  { name:'الجدول الثالث', c:'#D95F72', bg:'#FCEEF1', tc:'#9B3249', em:'📙',
    days:[{d:'الأحد',s:'رياضيات',cl:'dm'},{d:'الاثنين',s:'إنجليزي',cl:'de'},{d:'الثلاثاء',s:'لغتي',cl:'dl'},{d:'الأربعاء',s:'العلوم',cl:'ds'}]}
];

let sel=null, myVote=null, chart=null;

function loadV(){ try{return JSON.parse(localStorage.getItem(VOTES_KEY))||[0,0,0]}catch{return[0,0,0]} }
function saveV(v){ try{localStorage.setItem(VOTES_KEY,JSON.stringify(v))}catch{} }
function loadMine(){ try{const v=localStorage.getItem(MYVOTE_KEY);return v!==null?+v:null}catch{return null} }
function saveMine(v){ try{localStorage.setItem(MYVOTE_KEY,String(v))}catch{} }

/* ── PICK ── */
function pick(i){
  if(myVote!==null) return;
  if(sel!==null) document.getElementById('c'+sel).classList.remove('s'+sel);
  sel=i;
  document.getElementById('c'+i).classList.add('s'+i);
  document.getElementById('confBtn').disabled=false;
}

/* ── CONFIRM ── */
function doConfirm(){
  if(sel===null)return;
  const prev=myVote; myVote=sel; saveMine(myVote);
  const v=loadV(); if(prev!==null)v[prev]--; v[sel]++; saveV(v);
  showResult(sel);
  updateStats();
}

function showResult(idx){
  const s=SD[idx];
  document.getElementById('schedules').style.display='none';
  document.getElementById('confWrap').style.display='none';
  const rb=document.getElementById('rbanner');
  rb.style.background=s.bg;
  rb.innerHTML=`<div class="ricon" style="background:${s.c}">${s.em}</div>
    <div class="rtext">
      <h3 style="color:${s.tc}">اخترت ${s.name}</h3>
      <p style="color:${s.tc};opacity:.75">جدولك للاختبارات النهائية — وفقك الله ✨</p>
    </div>`;
  document.getElementById('rdays').innerHTML=s.days.map(d=>`
    <div class="dbox ${d.cl}"><div class="dday">${d.d}</div><div class="dsub">${d.s}</div></div>`).join('');
  document.getElementById('result').style.display='block';
  document.getElementById('result').scrollIntoView({behavior:'smooth',block:'center'});
}

/* ── RESET ── */
function doReset(){
  if(myVote!==null){const v=loadV();v[myVote]--;saveV(v);updateStats()}
  try{localStorage.removeItem(MYVOTE_KEY)}catch{}
  myVote=null; if(sel!==null)document.getElementById('c'+sel).classList.remove('s'+sel); sel=null;
  document.getElementById('confBtn').disabled=true;
  document.getElementById('schedules').style.display='flex';
  document.getElementById('confWrap').style.display='block';
  document.getElementById('result').style.display='none';
  window.scrollTo({top:0,behavior:'smooth'});
}

/* ── TEACHER LOGIN ── */
function tryLogin(){
  const pw=document.getElementById('pwInput').value;
  const err=document.getElementById('gateErr');
  if(pw===TEACHER_PASS){
    err.style.display='none';
    document.getElementById('pwInput').value='';
    try{sessionStorage.setItem(SESSION_KEY,'1')}catch{}
    showStats();
  } else {
    err.style.display='block';
    document.getElementById('pwInput').value='';
    document.getElementById('pwInput').focus();
  }
}

function showStats(){
  document.getElementById('gate').style.display='none';
  document.getElementById('statsPanel').style.display='block';
  if(!chart) buildChart();
  updateStats();
}

function doLogout(){
  try{sessionStorage.removeItem(SESSION_KEY)}catch{}
  document.getElementById('statsPanel').style.display='none';
  document.getElementById('gate').style.display='block';
}

/* ── UPDATE STATS ── */
function updateStats(){
  const v=loadV();
  const total=v.reduce((a,b)=>a+b,0);
  document.getElementById('totalBadge').textContent='إجمالي: '+total+' صوت';
  [0,1,2].forEach(i=>{
    const p=total>0?Math.round(v[i]/total*100):0;
    document.getElementById('cnt'+i).textContent=v[i];
    document.getElementById('pct'+i).textContent=p+'%';
    document.getElementById('bar'+i).style.width=p+'%';
  });
  if(chart){chart.data.datasets[0].data=[...v];chart.update()}
}

/* ── CHART ── */
function buildChart(){
  const v=loadV();
  chart=new Chart(document.getElementById('voteChart'),{
    type:'doughnut',
    data:{
      labels:['الجدول الأول','الجدول الثاني','الجدول الثالث'],
      datasets:[{
        data:[...v],
        backgroundColor:['#5B6AF0','#4BAD8A','#D95F72'],
        borderColor:['#3A47C7','#2E7A61','#9B3249'],
        borderWidth:2,hoverOffset:8
      }]
    },
    options:{
      responsive:true,maintainAspectRatio:false,cutout:'62%',
      plugins:{
        legend:{display:false},
        tooltip:{callbacks:{label:ctx=>{
          const t=ctx.dataset.data.reduce((a,b)=>a+b,0);
          const p=t>0?Math.round(ctx.raw/t*100):0;
          return ' '+ctx.raw+' صوت ('+p+'%)';
        }}}
      }
    }
  });
}

/* ── CLEAR ALL ── */
function clearAll(){
  if(!confirm('هل أنت متأكد من مسح جميع الأصوات؟'))return;
  try{localStorage.removeItem(VOTES_KEY);localStorage.removeItem(MYVOTE_KEY)}catch{}
  myVote=null; sel=null;
  document.getElementById('result').style.display='none';
  document.getElementById('schedules').style.display='flex';
  document.getElementById('confWrap').style.display='block';
  document.getElementById('confBtn').disabled=true;
  [0,1,2].forEach(i=>document.getElementById('c'+i).classList.remove('s'+i));
  updateStats();
}

/* ── INIT ── */
(function init(){
  myVote=loadMine();
  if(myVote!==null){sel=myVote;showResult(myVote)}
  try{if(sessionStorage.getItem(SESSION_KEY)==='1'){showStats()}}catch{}
})();
</script>
</body>
</html>
