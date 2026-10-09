
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#075b43">
<title>MAGHRIBI | مغربي</title>
<style>
:root{
  --green:#075b43;--green2:#0b7958;--red:#c73542;
  --bg:#f5f7f5;--white:#fff;--text:#17251f;--muted:#7a8780;
  --border:#e6ece8;--gold:#f1b94a;
}
*{box-sizing:border-box}
body{margin:0;background:var(--bg);font-family:Tahoma,Arial,sans-serif;color:var(--text)}
button,input,select,textarea{font:inherit}
button{cursor:pointer}
header{background:var(--white);position:sticky;top:0;z-index:10;border-bottom:1px solid var(--border)}
.top{max-width:1200px;margin:auto;padding:13px 18px;display:flex;align-items:center;gap:15px}
.logo{font-weight:900;color:var(--green);font-size:23px;white-space:nowrap}
.logo span{color:var(--red)}
.location{font-size:12px;color:var(--muted);white-space:nowrap}
.location strong{display:block;color:var(--text);font-size:13px;margin-top:3px}
.search{flex:1;display:flex;background:#f2f5f3;border-radius:12px;padding:4px 12px;min-width:80px}
.search input{width:100%;border:0;background:transparent;outline:0;padding:10px;font-size:14px}
.iconbtn{border:0;background:#f2f6f3;border-radius:12px;padding:11px;position:relative;font-size:19px}
.count{position:absolute;top:-5px;left:-5px;background:var(--red);color:white;border-radius:50%;font-size:10px;min-width:18px;height:18px;display:grid;place-items:center}
main{max-width:1200px;margin:auto;padding:20px 18px 100px}
.hero{background:linear-gradient(120deg,#064832,#0c7957);color:white;border-radius:24px;padding:30px;display:flex;align-items:center;justify-content:space-between;overflow:hidden;min-height:200px;position:relative}
.hero:after{content:"";position:absolute;width:230px;height:230px;border:35px solid #ffffff12;border-radius:50%;left:8%;top:-70px}
.hero h1{font-size:clamp(25px,4vw,39px);margin:0 0 12px;line-height:1.4}
.hero p{color:#d8eee3;line-height:1.9;margin:0 0 18px}
.primary{background:var(--gold);border:0;border-radius:11px;padding:12px 19px;font-weight:bold;color:#2a291d}
.heroart{font-size:80px;z-index:1;filter:drop-shadow(0 10px 12px #001b13aa)}
.sectionhead{display:flex;justify-content:space-between;align-items:center;margin:27px 0 15px}
.sectionhead h2{font-size:19px;margin:0}
.subtle{font-size:12px;color:var(--muted)}
.categories{display:grid;grid-template-columns:repeat(6,1fr);gap:12px}
.cat{border:1px solid var(--border);background:white;border-radius:16px;padding:15px 5px;text-align:center;transition:.2s}
.cat:hover,.cat.active{border-color:var(--green);background:#e9f5ee}
.cat .emoji{font-size:28px;display:block;margin-bottom:8px}
.cat span:last-child{font-size:12px;font-weight:bold}
.promo{display:flex;gap:12px;margin:22px 0}
.promo div{flex:1;border-radius:15px;padding:15px;background:#fff0ef;color:#8e2b34;font-weight:bold;font-size:14px}
.promo div:nth-child(2){background:#eaf4ff;color:#215c92}
.filters{display:flex;gap:8px;flex-wrap:wrap}
.chip{border:1px solid var(--border);background:white;color:#56635c;border-radius:20px;padding:8px 14px;font-size:12px}
.chip.active{background:var(--green);color:white;border-color:var(--green)}
.sort{border:1px solid var(--border);background:white;padding:9px;border-radius:10px;font-size:12px}
.products{display:grid;grid-template-columns:repeat(4,minmax(0,1fr));gap:15px}
.product{background:white;border:1px solid var(--border);border-radius:16px;overflow:hidden;transition:transform .2s;min-width:0}
.product:hover{transform:translateY(-3px)}
.productpic{height:165px;background:#eef2ef;display:grid;place-items:center;font-size:66px;position:relative}
.tag{position:absolute;top:10px;right:10px;background:#e4f5e9;color:#17633d;border-radius:6px;padding:5px 7px;font-size:10px}
.tag.used{background:#fff0d9;color:#8a5c13}
.heart{position:absolute;top:8px;left:8px;border:0;border-radius:50%;width:32px;height:32px;background:#ffffffdd;font-size:17px}
.productbody{padding:12px}
.productname{font-size:13px;font-weight:bold;line-height:1.7;min-height:40px}
.price{font-size:17px;color:var(--green);font-weight:900;margin:8px 0}
.price small{font-size:11px}
.oldprice{font-size:11px;color:#9aa39e;text-decoration:line-through;margin-right:5px}
.seller{font-size:11px;color:var(--muted);margin-bottom:10px}
.addcart{border:1px solid var(--green);color:var(--green);background:white;width:100%;border-radius:9px;padding:9px;font-size:12px;font-weight:bold}
.addcart:hover{background:var(--green);color:white}
.empty{text-align:center;padding:35px;color:var(--muted);grid-column:1/-1}
footer{border-top:1px solid var(--border);background:white;text-align:center;padding:22px;color:var(--muted);font-size:12px;line-height:2}
.bottomnav{position:fixed;bottom:0;right:0;left:0;background:#ffffffed;backdrop-filter:blur(12px);border-top:1px solid var(--border);display:flex;justify-content:space-around;padding:8px 3px calc(8px + env(safe-area-inset-bottom));z-index:20}
.navbtn{border:0;background:transparent;color:var(--muted);font-size:10px;display:flex;flex-direction:column;align-items:center;gap:5px;min-width:52px}
.navbtn b{font-size:21px;font-weight:400}
.navbtn.active{color:var(--green);font-weight:bold}
.modal{position:fixed;inset:0;background:#061d14a8;z-index:50;display:none;align-items:center;justify-content:center;padding:15px}
.modal.show{display:flex}
.dialog{background:white;width:min(480px,100%);max-height:90vh;overflow:auto;border-radius:20px;padding:22px}
.dialoghead{display:flex;justify-content:space-between;align-items:center;margin-bottom:15px}
.dialoghead h2{font-size:19px;margin:0}
.close{border:0;background:#f0f3f1;border-radius:50%;width:35px;height:35px;font-size:19px}
.field{display:flex;flex-direction:column;gap:7px;margin:13px 0}
.field label{font-size:12px;font-weight:bold}
.field input,.field select,.field textarea{border:1px solid var(--border);border-radius:10px;padding:12px;outline-color:var(--green);background:white;width:100%}
.fullbtn{width:100%;border:0;background:var(--green);color:white;border-radius:11px;padding:13px;font-weight:bold;margin-top:8px}
.detailpic{height:190px;display:grid;place-items:center;background:#eef3ef;border-radius:14px;font-size:85px}
.toast{position:fixed;bottom:85px;left:50%;transform:translateX(-50%);background:#152a20;color:white;padding:12px 20px;border-radius:12px;z-index:100;font-size:13px;display:none;white-space:nowrap;box-shadow:0 5px 20px #0002}
.toast.show{display:block}
.panel{display:none}
.panel.show{display:block}
.panelbox{background:white;border:1px solid var(--border);border-radius:16px;padding:18px;margin-bottom:12px}
.panelbox h3{margin-top:0}
.rowitem{display:flex;justify-content:space-between;gap:12px;align-items:center;padding:13px 0;border-bottom:1px solid var(--border);font-size:13px}
.rowitem:last-child{border:0}
.smallbtn{border:1px solid var(--border);background:white;border-radius:8px;padding:7px 10px;font-size:12px}
@media(max-width:750px){
 .top{gap:8px;padding:11px 12px;flex-wrap:wrap}
 .logo{font-size:20px}.location{display:none}
 .search{order:3;flex-basis:100%}
 main{padding:13px 12px 95px}
 .hero{padding:23px 18px;min-height:180px;border-radius:19px}
 .heroart{font-size:59px}.hero p{font-size:12px}
 .categories{grid-template-columns:repeat(3,1fr);gap:8px}
 .cat{padding:12px 4px}
 .products{grid-template-columns:repeat(2,minmax(0,1fr));gap:10px}
 .productpic{height:135px;font-size:55px}
 .productbody{padding:10px}
 .productname{font-size:12px}
 .price{font-size:16px}
 .promo{gap:8px}.promo div{padding:12px;font-size:12px}
 .sectionhead h2{font-size:17px}
}
@media(min-width:751px){.bottomnav{display:none}}
</style>
</head>
<body>
<header>
  <div class="top">
    <div class="logo">MAGHRIBI<span>.</span></div>
    <div class="location">📍 التوصيل إلى<strong>الجديدة، المغرب ▾</strong></div>
    <div class="search">
      <span style="align-self:center">🔎</span>
      <input id="searchInput" placeholder="قلب على أي منتج..." oninput="renderProducts()">
    </div>
    <button class="iconbtn" onclick="openCart()" aria-label="السلة">🛒<span id="cartCount" class="count">0</span></button>
    <button class="iconbtn" onclick="openAccount()" aria-label="الحساب">👤</button>
  </div>
</header>

<main>
<section id="homePanel" class="panel show">
  <div class="hero">
    <div>
      <h1>كلشي قريب ليك 🇲🇦</h1>
      <p>بيع وشري بسهولة، اكتشف عروض جديدة<br>من محلات وبائعين من مدينتك.</p>
      <button class="primary" onclick="document.getElementById('shopSection').scrollIntoView({behavior:'smooth'})">اكتشف المنتجات ←</button>
    </div>
    <div class="heroart">🛍️</div>
  </div>

  <div class="sectionhead"><h2>تسوّق حسب الفئة</h2><span class="subtle">اختار اللي بغيتي</span></div>
  <div class="categories" id="categories">
    <button class="cat active" onclick="setCategory('الكل',this)"><span class="emoji">✨</span><span>الكل</span></button>
    <button class="cat" onclick="setCategory('إلكترونيات',this)"><span class="emoji">📱</span><span>إلكترونيات</span></button>
    <button class="cat" onclick="setCategory('ملابس',this)"><span class="emoji">👕</span><span>ملابس</span></button>
    <button class="cat" onclick="setCategory('أحذية',this)"><span class="emoji">👟</span><span>أحذية</span></button>
    <button class="cat" onclick="setCategory('المنزل',this)"><span class="emoji">🪑</span><span>المنزل</span></button>
    <button class="cat" onclick="setCategory('إكسسوارات',this)"><span class="emoji">👜</span><span>إكسسوارات</span></button>
  </div>

  <div class="promo">
    <div>🚚 عروض محلية<br><span class="subtle">اكتشف منتجات قريبة منك</span></div>
    <div>♻️ جديد ومستعمل<br><span class="subtle">اختيارات على حساب ميزانيتك</span></div>
  </div>

  <section id="shopSection">
    <div class="sectionhead"><h2 id="productsTitle">منتجات مختارة ليك</h2><span class="subtle" id="productCount"></span></div>
    <div style="display:flex;justify-content:space-between;align-items:center;gap:10px;flex-wrap:wrap;margin-bottom:14px">
      <div class="filters">
        <button class="chip active" onclick="setCondition('الكل',this)">الكل</button>
        <button class="chip" onclick="setCondition('جديد',this)">جديد</button>
        <button class="chip" onclick="setCondition('مستعمل',this)">مستعمل</button>
      </div>
      <select class="sort" id="sortSelect" onchange="renderProducts()">
        <option value="default">الترتيب الافتراضي</option>
        <option value="low">الثمن: من الأقل</option>
        <option value="high">الثمن: من الأعلى</option>
      </select>
    </div>
    <div class="products" id="products"></div>
  </section>
</section>

<section id="favoritesPanel" class="panel">
  <div class="sectionhead"><h2>❤️ المفضلة ديالي</h2></div>
  <div class="products" id="favoriteProducts"></div>
</section>

<section id="sellPanel" class="panel">
  <div class="sectionhead"><h2>🏪 بيع منتج ديالك</h2></div>
  <div class="panelbox">
    <h3>وصل منتجك للمشترين</h3>
    <p class="subtle">عمر المعلومات باش تضيف منتج تجريبي للواجهة.</p>
    <form id="sellForm">
      <div class="field"><label>اسم المنتج</label><input id="sellName" required maxlength="70" placeholder="مثلاً: سبرديلة رياضية"></div>
      <div class="field"><label>الثمن بالدرهم</label><input id="sellPrice" type="number" min="1" required placeholder="مثلاً: 149"></div>
      <div class="field"><label>الفئة</label><select id="sellCategory"><option>أحذية</option><option>إلكترونيات</option><option>ملابس</option><option>المنزل</option><option>إكسسوارات</option><option>أخرى</option></select></div>
      <div class="field"><label>حالة المنتج</label><select id="sellCondition"><option>جديد</option><option>مستعمل</option></select></div>
      <div class="field"><label>الإيموجي ديال المنتج</label><select id="sellEmoji"><option value="📦">📦 منتج عام</option><option value="👟">👟 أحذية</option><option value="📱">📱 هاتف</option><option value="👕">👕 ملابس</option><option value="👜">👜 إكسسوارات</option><option value="🪑">🪑 أثاث</option></select></div>
      <div class="field"><label>اسم البائع أو المحل</label><input id="sellSeller" required placeholder="اسمك أو اسم المحل"></div>
      <button class="fullbtn" type="submit">＋ إضافة المنتج</button>
    </form>
    <p class="subtle">ملاحظة: الإضافة حالياً تجريبية وكتبان غير فهاد النسخة.</p>
  </div>
</section>

<section id="ordersPanel" class="panel">
  <div class="sectionhead"><h2>📦 الطلبات ديالي</h2></div>
  <div class="panelbox" id="ordersList"><p class="subtle">ما عندك حتى طلب دابا.</p></div>
</section>

<section id="accountPanel" class="panel">
  <div class="sectionhead"><h2>👤 الحساب ديالي</h2></div>
  <div class="panelbox">
    <div style="font-size:48px;text-align:center">🇲🇦</div>
    <h3 style="text-align:center" id="accountName">مرحبا بك فـ مغربي</h3>
    <p class="subtle" style="text-align:center">منصة مغربية للبيع والشراء</p>
    <div class="field"><label>الاسم</label><input id="userName" placeholder="دخل الاسم ديالك"></div>
    <div class="field"><label>رقم الهاتف</label><input id="userPhone" type="tel" placeholder="06XXXXXXXX"></div>
    <div class="field"><label>المدينة</label><select id="userCity"><option>الجديدة</option><option>الدار البيضاء</option><option>الرباط</option><option>مراكش</option><option>آسفي</option><option>أكادير</option><option>طنجة</option><option>مدينة أخرى</option></select></div>
    <button class="fullbtn" onclick="saveAccount()">حفظ المعلومات التجريبية</button>
    <button class="fullbtn" style="background:#f1f4f2;color:#34483c" onclick="showPanel('sellPanel','sell')">＋ بدا البيع</button>
  </div>
  <div class="panelbox">
    <h3>على MAGHRIBI</h3>
    <p class="subtle">مغربي مشروع هدفه يسهل البيع والشراء بين الناس والمحلات فالمغرب.</p>
    <p class="subtle">النسخة الحالية للعرض والتجربة فقط؛ ما كاينش أداء إلكتروني أو إرسال حقيقي للطلبات.</p>
  </div>
</section>
</main>

<footer>
  <strong style="color:var(--green)">MAGHRIBI | مغربي 🇲🇦</strong><br>
  منصة مغربية كتجمع البائعين والمشترين.<br>
  © 2026 MAGHRIBI — نسخة تجريبية
</footer>

<nav class="bottomnav">
  <button class="navbtn active" data-nav="home" onclick="showPanel('homePanel','home')"><b>⌂</b>الرئيسية</button>
  <button class="navbtn" data-nav="favorites" onclick="showPanel('favoritesPanel','favorites')"><b>♡</b>المفضلة</button>
  <button class="navbtn" data-nav="sell" onclick="showPanel('sellPanel','sell')"><b>＋</b>بيع</button>
  <button class="navbtn" data-nav="orders" onclick="showPanel('ordersPanel','orders')"><b>▤</b>طلباتي</button>
  <button class="navbtn" data-nav="account" onclick="showPanel('accountPanel','account')"><b>☻</b>حسابي</button>
</nav>

<div class="modal" id="modal" onclick="if(event.target===this)closeModal()">
  <div class="dialog">
    <div class="dialoghead"><h2 id="modalTitle">تفاصيل</h2><button class="close" onclick="closeModal()">×</button></div>
    <div id="modalContent"></div>
  </div>
</div>
<div class="toast" id="toast"></div>

<script>
const initialProducts=[
 {id:1,name:"سبرديلة رياضية عصرية",price:149,category:"أحذية",condition:"جديد",emoji:"👟",seller:"MyShoes.ma",city:"الجديدة",desc:"سبرديلة ستايل عصري للاستعمال اليومي."},
 {id:2,name:"سماعات لاسلكية",price:119,category:"إلكترونيات",condition:"جديد",emoji:"🎧",seller:"متجر التقنية",city:"الجديدة",desc:"سماعات لاسلكية بتصميم أنيق."},
 {id:3,name:"حقيبة نسائية أنيقة",price:179,category:"إكسسوارات",condition:"جديد",emoji:"👜",seller:"Boutique Sara",city:"الجديدة",desc:"حقيبة مناسبة للاستعمال اليومي."},
 {id:4,name:"كرسي للمنزل",price:220,category:"المنزل",condition:"مستعمل",emoji:"🪑",seller:"بيع المستعمل",city:"الجديدة",desc:"كرسي مستعمل بحالة جيدة حسب وصف البائع."},
 {id:5,name:"قميص كاجوال",price:99,category:"ملابس",condition:"جديد",emoji:"👕",seller:"Style Maroc",city:"الجديدة",desc:"قميص كاجوال بسيط وأنيق."},
 {id:6,name:"هاتف ذكي مستعمل",price:850,category:"إلكترونيات",condition:"مستعمل",emoji:"📱",seller:"عالم الهواتف",city:"الجديدة",desc:"مثال تجريبي لهاتف مستعمل. تحقق من الحالة قبل الشراء."},
 {id:7,name:"ساعة يد كلاسيكية",price:135,category:"إكسسوارات",condition:"جديد",emoji:"⌚",seller:"Accessoires.ma",city:"الجديدة",desc:"ساعة بتصميم كلاسيكي."},
 {id:8,name:"حذاء يومي",price:129,category:"أحذية",condition:"مستعمل",emoji:"👞",seller:"Souk El Jadida",city:"الجديدة",desc:"حذاء مستعمل؛ التفاصيل والصور خاصها التأكيد مع البائع."}
];
let products=initialProducts.map(p=>({...p}));
let cart=[];
let favorites=new Set();
let orders=[];
let currentCategory="الكل",currentCondition="الكل",currentPanel="home";
let nextId=100;
let user={name:"",phone:"",city:"الجديدة"};

function money(n){return Number(n).toLocaleString("fr-MA")+" د.م"}
function toast(msg){
 const el=document.getElementById("toast");el.textContent=msg;el.classList.add("show");
 clearTimeout(window.toastTimer);window.toastTimer=setTimeout(()=>el.classList.remove("show"),2300);
}
function showPanel(panel,nav){
 document.querySelectorAll(".panel").forEach(p=>p.classList.remove("show"));
 document.getElementById(panel).classList.add("show");
 document.querySelectorAll(".navbtn").forEach(b=>b.classList.toggle("active",b.dataset.nav===nav));
 currentPanel=nav;
 window.scrollTo({top:0,behavior:"smooth"});
 if(panel==="favoritesPanel")renderFavorites();
 if(panel==="ordersPanel")renderOrders();
}
function setCategory(cat,el){
 currentCategory=cat;
 document.querySelectorAll(".cat").forEach(b=>b.classList.remove("active"));
 if(el)el.classList.add("active");
 document.getElementById("productsTitle").textContent=cat==="الكل"?"منتجات مختارة ليك":cat;
 renderProducts();
}
function setCondition(cond,el){
 currentCondition=cond;
 document.querySelectorAll(".filters .chip").forEach(b=>b.classList.remove("active"));
 el.classList.add("active");renderProducts();
}
function renderProducts(){
 const query=(document.getElementById("searchInput").value||"").trim().toLowerCase();
 let list=products.filter(p=>
  (currentCategory==="الكل"||p.category===currentCategory)&&
  (currentCondition==="الكل"||p.condition===currentCondition)&&
  (p.name+" "+p.category+" "+p.seller+" "+p.city).toLowerCase().includes(query)
 );
 const sort=document.getElementById("sortSelect").value;
 if(sort==="low")list.sort((a,b)=>a.price-b.price);
 if(sort==="high")list.sort((a,b)=>b.price-a.price);
 document.getElementById("productCount").textContent=list.length+" منتجات";
 const el=document.getElementById("products");
 if(!list.length){el.innerHTML='<div class="empty">🔎<br>ما لقينا حتى منتج بهاد المواصفات.</div>';return}
 el.innerHTML=list.map(p=>`
 <article class="product">
  <div class="productpic" onclick="showProduct(${p.id})">
   <span>${p.emoji}</span>
   <span class="tag ${p.condition==="مستعمل"?"used":""}">${p.condition}</span>
   <button class="heart" aria-label="المفضلة" onclick="event.stopPropagation();toggleFavorite(${p.id})">${favorites.has(p.id)?"❤️":"♡"}</button>
  </div>
  <div class="productbody">
   <div class="productname" onclick="showProduct(${p.id})">${escapeHtml(p.name)}</div>
   <div class="price">${money(p.price)}</div>
   <div class="seller">📍 ${escapeHtml(p.city||"المغرب")} · ${escapeHtml(p.seller)}</div>
   <button class="addcart" onclick="addToCart(${p.id})">＋ زيد للسلة</button>
  </div>
 </article>`).join("");
}
function escapeHtml(s){
 return String(s).replace(/[&<>"']/g,c=>({"&":"&amp;","<":"&lt;",">":"&gt;",'"':"&quot;","'":"&#39;"}[c]));
}
function toggleFavorite(id){
 if(favorites.has(id)){favorites.delete(id);toast("تحيد من المفضلة")}
 else{favorites.add(id);toast("تزاد للمفضلة ❤️")}
 renderProducts();renderFavorites();
}
function renderFavorites(){
 const list=products.filter(p=>favorites.has(p.id));
 document.getElementById("favoriteProducts").innerHTML=list.length?list.map(p=>`
 <article class="product"><div class="productpic" onclick="showProduct(${p.id})">${p.emoji}<span class="tag">${p.condition}</span></div>
 <div class="productbody"><div class="productname">${escapeHtml(p.name)}</div><div class="price">${money(p.price)}</div>
 <button class="addcart" onclick="addToCart(${p.id})">＋ زيد للسلة</button>
 <button class="smallbtn" style="width:100%;margin-top:7px" onclick="toggleFavorite(${p.id})">حيد من المفضلة</button></div></article>`).join(""):'<div class="empty">♡<br>مازال ما زدتي حتى منتج للمفضلة.</div>';
}
function addToCart(id){
 const p=products.find(x=>x.id===id);if(!p)return;
 const item=cart.find(x=>x.id===id);
 if(item)item.qty++;else cart.push({id,qty:1});
 updateCartCount();toast("تزاد "+p.name+" للسلة 🛒");
}
function updateCartCount(){
 document.getElementById("cartCount").textContent=cart.reduce((n,x)=>n+x.qty,0);
}
function openModal(title,html){
 document.getElementById("modalTitle").textContent=title;
 document.getElementById("modalContent").innerHTML=html;
 document.getElementById("modal").classList.add("show");
}
function closeModal(){document.getElementById("modal").classList.remove("show")}
function openCart(){
 let list=cart.map(i=>({...i,product:products.find(p=>p.id===i.id)})).filter(i=>i.product);
 const total=list.reduce((n,i)=>n+i.product.price*i.qty,0);
 let html=list.length?list.map(i=>`
 <div class="rowitem"><div><strong>${i.product.emoji} ${escapeHtml(i.product.name)}</strong><br><span class="subtle">${money(i.product.price)} × ${i.qty}</span></div>
 <div style="display:flex;gap:5px;align-items:center"><button class="smallbtn" onclick="changeQty(${i.id},-1)">−</button><button class="smallbtn" onclick="changeQty(${i.id},1)">＋</button></div></div>`).join("")+
 `<div style="padding:16px 0;font-weight:bold">المجموع: <span style="color:var(--green)">${money(total)}</span></div>
 <button class="fullbtn" onclick="checkout()">تأكيد الطلب التجريبي</button>`:
 '<div class="empty">🛒<br>السلة ديالك خاوية.</div>';
 openModal("سلة المشتريات",html);
}
function changeQty(id,delta){
 const item=cart.find(x=>x.id===id);if(!item)return;
 item.qty+=delta;if(item.qty<=0)cart=cart.filter(x=>x.id!==id);
 updateCartCount();openCart();
}
function checkout(){
 if(!cart.length){toast("السلة خاوية");return}
 if(!user.name){
  closeModal();showPanel("accountPanel","account");toast("دخل الاسم ديالك قبل تأكيد الطلب");return;
 }
 const items=cart.map(i=>{const p=products.find(x=>x.id===i.id);return {name:p.name,price:p.price,qty:i.qty}});
 const total=items.reduce((n,i)=>n+i.price*i.qty,0);
 orders.unshift({id:"MG"+Date.now().toString().slice(-6),items,total,date:new Date().toLocaleDateString("fr-MA"),status:"تجريبي"});
 cart=[];updateCartCount();closeModal();renderOrders();showPanel("ordersPanel","orders");
 toast("تسجل الطلب التجريبي بنجاح");
}
function renderOrders(){
 const el=document.getElementById("ordersList");
 if(!orders.length){el.innerHTML='<p class="subtle">ما عندك حتى طلب دابا.</p>';return}
 el.innerHTML=orders.map(o=>`<div class="rowitem"><div><strong>طلب #${o.id}</strong><br><span class="subtle">${o.date} · ${o.items.length} منتجات</span><br><span class="subtle">حالة الطلب: ${o.status}</span></div><strong style="color:var(--green)">${money(o.total)}</strong></div>`).join("")+
 '<p class="subtle">الطلبات هنا تجريبية، ما كيتوصل بها حتى بائع.</p>';
}
function showProduct(id){
 const p=products.find(x=>x.id===id);if(!p)return;
 openModal("تفاصيل المنتج",`
 <div class="detailpic">${p.emoji}</div>
 <div style="display:flex;justify-content:space-between;align-items:center;margin-top:16px"><strong>${escapeHtml(p.name)}</strong><span class="tag ${p.condition==="مستعمل"?"used":""}" style="position:static">${p.condition}</span></div>
 <div class="price" style="font-size:24px">${money(p.price)}</div>
 <p style="font-size:13px;line-height:1.9">${escapeHtml(p.desc||"")}</p>
 <p class="subtle">🏪 البائع: ${escapeHtml(p.seller)}<br>📍 المدينة: ${escapeHtml(p.city||"المغرب")}<br>📦 الفئة: ${escapeHtml(p.category)}</p>
 <button class="fullbtn" onclick="closeModal();addToCart(${p.id})">＋ زيد للسلة</button>
 <p class="subtle">هاد المنتج تجريبي. تأكد من معلومات المنتج والبائع قبل أي عملية شراء.</p>`);
}
function openAccount(){
 showPanel("accountPanel","account");
}
function saveAccount(){
 user.name=document.getElementById("userName").value.trim();
 user.phone=document.getElementById("userPhone").value.trim();
 user.city=document.getElementById("userCity").value;
 if(!user.name){toast("عمر الاسم ديالك أولا");return}
 document.getElementById("accountName").textContent="مرحبا "+user.name+" 👋";
 toast("تحفظات المعلومات فهاد الجلسة");
}
document.getElementById("sellForm").addEventListener("submit",function(e){
 e.preventDefault();
 const name=document.getElementById("sellName").value.trim();
 const price=Number(document.getElementById("sellPrice").value);
 const seller=document.getElementById("sellSeller").value.trim();
 if(!name||!seller||!Number.isFinite(price)||price<=0){toast("راجع المعلومات اللي دخلتي");return}
 products.unshift({
  id:nextId++,name,price,category:document.getElementById("sellCategory").value,
  condition:document.getElementById("sellCondition").value,
  emoji:document.getElementById("sellEmoji").value,seller,
  city:user.city||"الجديدة",desc:"منتج مضاف تجريبياً من طرف البائع."
 });
 this.reset();currentCategory="الكل";currentCondition="الكل";
 document.querySelectorAll(".cat").forEach(b=>b.classList.remove("active"));
 document.querySelector(".cat").classList.add("active");
 document.querySelectorAll(".filters .chip").forEach(b=>b.classList.remove("active"));
 document.querySelector(".filters .chip").classList.add("active");
 renderProducts();toast("تزاد المنتج للواجهة التجريبية");
 showPanel("homePanel","home");
});
renderProducts();
</script>
</body>
</html>
