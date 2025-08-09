# Index.html<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>نیازینو — دمو (دیوار‌مانند، موبایل، خوزستان، تم تیره نئونی)</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.1/font/bootstrap-icons.css" rel="stylesheet">
  <link href="https://fonts.googleapis.com/css2?family=Vazirmatn:wght@300;400;500;700&display=swap" rel="stylesheet">
  <style>
:root{
  --bg:#0d1117; --card:#121418; --panel:#14171a;
  --muted:#94a3b8; --text:#e6f7ff;
  --accent:#00f7ff; --accent-2:#33e0ff;
  --radius:12px; --gap:12px;
  --neon-shadow: 0 8px 32px rgba(0,247,255,0.06);
  --glass: rgba(255,255,255,0.03);
  --glass-strong: rgba(255,255,255,0.06);
}
*{box-sizing:border-box;}
html,body{height:100%;margin:0;padding:0;background:linear-gradient(180deg,#090b0d,#0d1117);font-family:"Vazirmatn",sans-serif;color:var(--text);-webkit-font-smoothing:antialiased;}
a{color:inherit;text-decoration:none;}
.container{max-width:430px;margin:0 auto;padding:0 12px;}
.header{position:sticky;top:0;z-index:120;background:transparent;padding:10px 0;border-bottom:1px solid rgba(255,255,255,0.03);}
.header-inner{display:flex;align-items:center;justify-content:space-between;gap:8px;}
.header-btn{width:40px;height:40px;border-radius:10px;background:var(--panel);display:flex;align-items:center;justify-content:center;color:var(--accent);font-size:1.15rem;box-shadow:var(--neon-shadow);cursor:pointer;border:none;}
.logo{display:flex;flex-direction:column;align-items:center;gap:2px;text-align:center;}
.logo .mark{width:42px;height:42px;border-radius:10px;background:linear-gradient(135deg,var(--accent),var(--accent-2));display:flex;align-items:center;justify-content:center;color:#071018;font-weight:800;font-size:18px;box-shadow:0 8px 30px rgba(0,247,255,0.08);}
.logo .title{font-weight:700;font-size:15px;color:var(--text);}
.logo .subtitle{font-size:11px;color:var(--muted);}
.search-row{display:flex;gap:8px;margin:12px 0;align-items:center;}
.search-input{flex:1;background:var(--glass);padding:10px 12px;border-radius:999px;border:1px solid rgba(255,255,255,0.02);display:flex;align-items:center;gap:8px;box-shadow:inset 0 0 8px rgba(0,247,255,0.02);}
.search-input input{background:transparent;border:0;outline:none;color:var(--text);width:100%;font-size:14px;}
.search-shortcut{width:40px;height:40px;border-radius:10px;background:var(--panel);display:flex;align-items:center;justify-content:center;color:var(--accent);font-size:1.1rem;cursor:pointer;border:none;}
.filter-bar{display:flex;gap:8px;overflow:auto;padding-bottom:8px;margin-bottom:6px;}
.filter-chip{flex:0 0 auto;padding:8px 12px;border-radius:999px;border:1px solid rgba(255,255,255,0.04);background:transparent;color:var(--muted);font-weight:600;cursor:pointer;white-space:nowrap;font-size:13px;}
.filter-chip.active{background:linear-gradient(90deg,var(--accent),var(--accent-2));color:#071018;border-color:transparent;box-shadow:0 8px 30px rgba(0,247,255,0.06);}
.list{display:flex;flex-direction:column;gap:12px;padding-bottom:140px;}
.item{display:flex;gap:12px;align-items:flex-start;background:linear-gradient(180deg,var(--card),#0f1417);padding:12px;border-radius:12px;border:1px solid rgba(255,255,255,0.02);box-shadow:var(--neon-shadow);transition:transform .12s ease;}
.item:hover{transform:translateY(-4px);}
.meta-right{width:110px;flex-shrink:0;display:flex;flex-direction:column;align-items:flex-end;gap:8px;}
.thumb{width:110px;height:82px;border-radius:8px;background:linear-gradient(135deg,#0b0c0d,#151618);display:flex;align-items:center;justify-content:center;color:var(--muted);font-size:13px;}
.info{flex:1;display:flex;flex-direction:column;gap:6px;min-width:0;}
.title{font-weight:700;color:var(--text);font-size:15px;overflow:hidden;white-space:nowrap;text-overflow:ellipsis;}
.desc{font-size:13px;color:var(--muted);overflow:hidden;display:-webkit-box;-webkit-line-clamp:2;-webkit-box-orient:vertical;}
.row-bottom{display:flex;align-items:center;justify-content:space-between;gap:8px;margin-top:6px;}
.price{color:var(--accent);font-weight:800;font-size:14px;}
.small-muted{font-size:12px;color:var(--muted);}
.icon-small{width:36px;height:36px;border-radius:8px;background:var(--panel);display:flex;align-items:center;justify-content:center;color:var(--accent);border:1px solid rgba(255,255,255,0.02);cursor:pointer;}
.panel{position:fixed;top:0;right:-100%;height:100%;width:86%;max-width:360px;background:linear-gradient(180deg,#0f1113,#161617);z-index:200;padding:12px;border-radius:12px 0 0 12px;box-shadow:0 30px 80px rgba(2,6,23,0.7);transition:right .28s ease;overflow:auto;}
.panel.open{right:0;}
.panel h4{margin:0 0 10px 0;color:var(--accent);}
.sidebar{position:fixed;left:-100%;top:0;height:100%;width:86%;max-width:360px;background:linear-gradient(180deg,#0f1113,#161617);z-index:210;padding:14px;border-radius:0 12px 12px 0;transition:left .28s ease;overflow:auto;}
.sidebar.open{left:0;}
.sidebar h4{color:var(--accent);margin:0 0 10px 0;}
.input,select{width:100%;padding:10px;border-radius:10px;background:rgba(255,255,255,0.03);border:1px solid rgba(255,255,255,0.03);color:var(--text);margin-bottom:10px;}
.bottom-fixed{position:fixed;left:12px;right:12px;bottom:12px;display:flex;gap:10px;z-index:220;}
.fab{flex:1;padding:12px;border-radius:12px;background:linear-gradient(90deg,var(--accent),var(--accent-2));color:#071018;border:none;font-weight:800;box-shadow:0 12px 40px rgba(0,247,255,0.08);cursor:pointer;}
.hidden{display:none;}
html,body{min-width:320px;max-width:430px;margin-left:auto;margin-right:auto;}
  </style>
</head>
<body>
<div class="container">
  <header class="header">
    <div class="header-inner">
      <button class="header-btn" id="openSidebarBtn"><i class="bi bi-filter"></i></button>
      <div class="logo">
        <div class="mark">ن</div>
        <div class="title">نیازینو</div>
        <div class="subtitle">خوزستان</div>
      </div>
      <div style="display:flex;gap:8px;align-items:center">
        <button class="header-btn" id="openNotifBtn"><i class="bi bi-bell"></i></button>
        <button class="header-btn" id="openChatBtn"><i class="bi bi-chat-dots"></i></button>
      </div>
    </div>
  </header>
  <div class="search-row">
    <div class="search-input">
      <i class="bi bi-search" style="color:var(--muted)"></i>
      <input id="q" type="search" placeholder="مثلاً: آیفون ۱۲، پراید...">
    </div>
    <button class="search-shortcut" id="openQuickPost"><i class="bi bi-plus-lg"></i></button>
  </div>
  <div class="filter-bar" id="filterBar"></div>
  <section class="list" id="list"></section>
  <div class="bottom-fixed">
    <button class="fab" id="postFab">ثبت آگهی</button>
  </div>
</div>
<aside class="sidebar" id="sidebar">
  <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:12px">
    <h4>فیلترها</h4>
    <button class="header-btn" id="closeSidebarBtn"><i class="bi bi-x-lg"></i></button>
  </div>
  <label>دسته‌بندی</label>
  <select id="filterCategory" class="input">
    <option value="">همه</option>
    <option value="electronics">موبایل و الکترونیک</option>
    <option value="vehicles">وسایل نقلیه</option>
    <option value="real_estate">املاک</option>
    <option value="home">خانه و آشپزخانه</option>
    <option value="services">خدمات</option>
    <option value="personal">لوازم شخصی</option>
    <option value="leisure">سرگرمی و فراغت</option>
    <option value="industrial">تجهیزات صنعتی</option>
    <option value="pets">حیوانات</option>
    <option value="jobs">استخدام و کاریابی</option>
  </select>
  <label>شهر</label>
  <select id="filterCity" class="input">
    <option value="">همه شهرها</option>
    <option>اهواز</option><option>آبادان</option><option>خرمشهر</option><option>دزفول</option>
    <option>اندیمشک</option><option>ماهشهر</option><option>شوش</option><option>شوشتر</option>
    <option>مسجدسلیمان</option><option>لالی</option><option>گتوند</option><option>ایذه</option>
    <option>حمیدیه</option><option>رامهرمز</option><option>هندیجان</option><option>بهبهان</option>
  </select>
  <label>حداکثر قیمت (تومان)</label>
  <input id="filterPrice" type="number" class="input" placeholder="مثلاً 10000000">
  <button id="applyFilterBtn" class="fab" style="margin-top:10px;">اعمال فیلتر</button>
</aside>
<aside class="panel" id="notifPanel" aria-hidden="true">
  <h4>اعلان‌ها</h4><div id="notifList"></div>
</aside>
<aside class="panel" id="chatPanel" aria-hidden="true">
  <h4>چت‌ها</h4><div id="chatList"></div>
  <div id="chatWindow" class="hidden"></div>
  <div style="display:flex;gap:8px;position:sticky;bottom:12px">
    <input id="chatInput" placeholder="پیام..." style="flex:1;padding:10px;border-radius:10px;border:none;background:rgba(255,255,255,0.03);color:var(--text)"/>
    <button id="sendChatBtn" class="header-btn"><i class="bi bi-send"></i></button>
  </div>
</aside>
<script>
const FILTERS=[{key:'all',label:'همه'},
  {key:'electronics',label:'موبایل و الکترونیک'},
  {key:'vehicles',label:'وسایل نقلیه'},
  {key:'real_estate',label:'املاک'},
  {key:'home',label:'خانه و آشپزخانه'},
  {key:'services',label:'خدمات'},
  {key:'personal',label:'لوازم شخصی'},
  {key:'leisure',label:'سرگرمی و فراغت'},
  {key:'industrial',label:'تجهیزات صنعتی'},
  {key:'pets',label:'حیوانات'},
  {key:'jobs',label:'استخدام و کاریابی'}];
const ADS=[{id:1,title:"آیفون ۱۲ پرو (تمیز)",city:"اهواز",price:85000000,cat:"electronics",posted:"2 ساعت پیش",desc:"64GB، رنگ مشکی، بدون خط و خش",photos:3},
  {id:2,title:"پژو ۲۰۶ - مدل ۹۵",city:"آبادان",price:125000000,cat:"vehicles",posted:"۵ ساعت پیش",desc:"کارکرد 120000، سرویس کامل",photos:2},
  {id:3,title:"آپارتمان ۸۰ متری - فروش",city:"دزفول",price:2100000000,cat:"real_estate",posted:"دیروز",desc:"واقع در مرکز شهر، نقشه عالی",photos:4},
  {id:4,title:"تدریس خصوصی ریاضی",city:"اهواز",price:300000,cat:"services",posted:"امروز",desc:"تجربه ۵ ساله، حضوری / آنلاین",photos:0},
  {id:5,title:"دوچرخه کوهستان نو",city:"خرمشهر",price:4500000,cat:"leisure",posted:"۳ روز پیش",desc:"مارک حرفه‌ای، رنگ قرمز",photos:1}];
let NOTIFS=[{id:1001,text:"آگهی شما تایید شد",ts:Date.now()-60000}];
let CHATS={};
const $=(s)=>document.querySelector(s), $id=(i)=>document.getElementById(i);
function renderFilterChips(){const bar=$id('filterBar');bar.innerHTML='';FILTERS.forEach(f=>{const btn=document.createElement('button');btn.className='filter-chip'+(f.key==='all'?' active':'');btn.textContent=f.label;btn.dataset.key=f.key;btn.onclick=()=>{document.querySelectorAll('.filter-chip').forEach(c=>c.classList.remove('active'));btn.classList.add('active');applyQuickFilter(f.key);} ;bar.appendChild(btn);});}
function renderList(data){const list=$id('list');list.innerHTML='';if(!data||!data.length){list.innerHTML='<div style="padding:18px;border-radius:12px;background:var(--card);color:var(--muted)">موردی یافت نشد.</div>';return;}data.forEach(ad=>{const item=document.createElement('article');item.className='item';item.innerHTML=`<div class="meta-right"><div class="thumb">${ad.photos?ad.photos+' عکس':'بی عکس'}</div><div class="small-muted">${ad.city}</div></div><div class="info"><div class="title">${ad.title}</div><div class="desc">${ad.desc}</div><div class="row-bottom"><div class="price">${ad.price?ad.price.toLocaleString('fa-IR')+' تومان':'قیمت توافقی'}</div><div style="display:flex;gap:8px;align-items:center"><button class="icon-small" title="ذخیره" onclick="toggleFav(${ad.id},this)"><i class="bi bi-heart"></i></button><button class="icon-small" title="نمایش سریع" onclick="openQuick(${ad.id})"><i class="bi bi-eye"></i></button><button class="icon-small" title="چت" onclick="openChatForAd(${ad.id})"><i class="bi bi-chat-dots"></i></button></div></div></div>`;list.appendChild(item);});}
function applyQuickFilter(key){renderList(key==='all'?ADS:ADS.filter(a=>a.cat===key));}
$id('q').addEventListener('input', e=>{const q=e.target.value.trim().toLowerCase();renderList(!q?ADS:ADS.filter(a=>(a.title+' '+(a.desc||'')).toLowerCase().includes(q)));});
function openQuick(id){const ad=ADS.find(a=>a.id===id);if(!ad) return;alert(ad.title+"\n"+(ad.price?ad.price.toLocaleString('fa-IR')+' تومان':'')+"\n"+ad.city+"\n\n"+ad.desc);}
const FAVS=new Set();function toggleFav(id,btn){if(FAVS.has(id)){FAVS.delete(id);btn.style.background='var(--panel)';btn.querySelector('i').className='bi bi-heart';}else{FAVS.add(id);btn.style.background='linear-gradient(90deg,var(--accent),var(--accent-2))';btn.querySelector('i').className='bi bi-heart-fill';}}
function renderNotifs(){const w=$id('notifList');w.innerHTML='';if(!NOTIFS.length){w.innerHTML='<div class="list-item">هیچ اعلانی نیست</div>';return;}NOTIFS.forEach(n=>{const d=document.createElement('div');d.className='list-item';d.textContent=n.text+' • '+new Date(n.ts).toLocaleTimeString();w.appendChild(d);});}
function renderChats(){const w=$id('chatList');w.innerHTML='';const keys=Object.keys(CHATS);if(!keys.length){w.innerHTML='<div class="list-item">گفتگویی نیست</div>';return;}keys.forEach(k=>{const c=CHATS[k],last=c.messages.slice(-1)[0];const d=document.createElement('div');d.className='list-item';d.textContent='فروشنده '+c.adId+' • '+(last?last.text:'');d.onclick=()=>openConv(k);w.appendChild(d);});}
function openConv(cid){const conv=CHATS[cid];if(!conv)return;const win=$id('chatWindow');win.innerHTML='';conv.messages.forEach(m=>{const p=document.createElement('div');p.textContent=(m.from==='user'?'شما: ':'فروشنده: ')+m.text;p.style.marginBottom='8px';win.appendChild(p);});win.classList.remove('hidden');}
$id('sendChatBtn').addEventListener('click', ()=>{const txt=$id('chatInput').value.trim();if(!txt) return;let cid=Object.keys(CHATS)[0];if(!cid){const adId=ADS[0].id;cid='c_'+Date.now();CHATS[cid]={id:cid,adId,messages:[{from:'user',text:txt,ts:Date.now()}],unread:false};}else CHATS[cid].messages.push({from:'user',text:txt,ts:Date.now()});$id('chatInput').value='';renderChats();openConv(cid);setTimeout(()=>{CHATS[cid].messages.push({from:'seller',text:'در اسرع وقت پاسخ می‌دهم (دمو).',ts:Date.now()});renderChats();pushNotif('پاسخ جدید از فروشنده (دمو)');},900);});
function pushNotif(text){NOTIFS.unshift({id:Date.now(),text,ts:Date.now()});renderNotifs();}
const sidebar=$id('sidebar'), notifPanel=$id('notifPanel'), chatPanel=$id('chatPanel');
$id('openSidebarBtn').onclick=()=>sidebar.classList.add('open');
$id('closeSidebarBtn').onclick=()=>sidebar.classList.remove('open');
$id('applyFilterBtn').onclick=()=>{const cat=$id('filterCategory').value,city=$id('filterCity').value,price=Number($id('filterPrice').value||0);let list=ADS.slice();if(cat)list=list.filter(a=>a.cat===cat);if(city)list=list.filter(a=>a.city===city);if(price>0)list=list.filter(a=> (a.price||0)<=price);renderList(list);sidebar.classList.remove('open');};
$id('openNotifBtn').onclick=()=>{const o=notifPanel.classList.toggle('open');if(o){renderNotifs();chatPanel.classList.remove('open');}};
$id('openChatBtn').onclick=()=>{const o=chatPanel.classList.toggle('open');if(o){renderChats();notifPanel.classList.remove('open');}};
$id('openQuickPost').onclick=()=>{
  const overlay=document.createElement('div');
  overlay.style.position='fixed';overlay.style.top=0;overlay.style.left=0;
  overlay.style.width='100%';overlay.style.height='100%';
  overlay.style.background='rgba(0,0,0,0.8)';overlay.style.zIndex=300;
  overlay.style.display='flex';overlay.style.alignItems='center';
  overlay.style.justifyContent='center';
  overlay.innerHTML=`<div style="background:var(--panel);padding:20px;border-radius:12px;text-align:center;color:var(--text);box-shadow:var(--neon-shadow);max-width:300px">
    <p>برای ثبت آگهی، ابتدا کانال یوتیوب ما را دنبال کنید:</p>
    <button id="gotoYt" style="padding:10px;border:none;border-radius:8px;background:linear-gradient(90deg,var(--accent),var(--accent-2));color:#071018;font-weight:700;margin-top:12px;cursor:pointer">
      رفتن به کانال یوتیوب
    </button>
    <div style="margin-top:10px;font-size:12px;color:var(--muted)">بعد از باز کردن لینک، دوباره اینجا زدید.</div>
  </div>`;
  document.body.appendChild(overlay);
  document.getElementById('gotoYt').onclick=()=>{
    window.open('https://www.youtube.com/@ardalan_1996','_blank');
    overlay.remove();
  };
};
document.getElementById('postFab').onclick = () => document.getElementById('openQuickPost').click();
renderFilterChips(); renderList(ADS); renderNotifs(); renderChats();
</script>
</body>
</html>
