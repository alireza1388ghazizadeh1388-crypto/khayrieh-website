# khayrieh-website
<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>خیریه دارالاحسان</title>

<!-- فونت فارسی -->
<link href="https://fonts.googleapis.com/css2?family=Vazirmatn:wght@400;700&display=swap" rel="stylesheet">

<!-- Lightbox -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/glightbox/dist/css/glightbox.min.css" />
<script src="https://cdn.jsdelivr.net/npm/glightbox/dist/js/glightbox.min.js"></script>

<style>
* {margin:0;padding:0;box-sizing:border-box;font-family:'Vazirmatn',sans-serif;}
body {background:#fdf6ec;color:#333;line-height:1.6;}
.splash {position:fixed;top:0;left:0;width:100%;height:100%;background:#1c3d5a;color:#fff;display:flex;justify-content:center;align-items:center;font-size:2em;z-index:1000;transition:opacity 0.5s;}
header{background:#1c3d5a;color:#fff;padding:20px;text-align:center;}
header h1{font-size:2em;}
.container{padding:20px;max-width:900px;margin:auto;display:none;}
nav{display:flex;flex-direction:column;gap:15px;margin-bottom:20px;}
nav a{background:linear-gradient(90deg,#2e5984,#1c3d5a);color:#fff;padding:15px;border-radius:10px;text-decoration:none;text-align:center;font-weight:700;box-shadow:0 4px 6px rgba(0,0,0,0.2);transition:0.3s;}
nav a:hover{background:linear-gradient(90deg,#1c3d5a,#2e5984);transform:scale(1.03);}
section{display:none;margin-bottom:40px;}
section.active{display:block;}
.back-link{display:inline-block;margin-bottom:20px;padding:10px 15px;background:#2e5984;color:#fff;border-radius:8px;text-decoration:none;}
.gallery{display:flex;overflow-x:auto;gap:15px;padding-bottom:10px;}
.gallery img{height:150px;border-radius:10px;flex-shrink:0;transition:0.3s;}
.gallery img:hover{transform:scale(1.05);}
.cards .card{display:flex;justify-content:space-between;align-items:center;background:#fff;padding:10px 15px;margin-bottom:10px;border-radius:8px;box-shadow:0 2px 4px rgba(0,0,0,0.1);}
.cards .card button{background:#1c3d5a;color:#fff;border:none;padding:5px 10px;border-radius:5px;cursor:pointer;}
.mojtaba img{width:100%;border-radius:10px;margin-bottom:15px;}
a.map-link{display:inline-block;margin-top:10px;background:#1c3d5a;color:#fff;padding:10px 15px;border-radius:8px;text-decoration:none;}
footer{text-align:center;padding:20px;background:#f1f1f1;margin-top:40px;border-top:1px solid #ccc;}
</style>
</head>
<body>

<div class="splash">خیریه دارالاحسان حضرت فاطمه تقدیم می‌کند</div>

<header>
<h1>خیریه دارالاحسان</h1>
</header>

<div class="container">
<nav>
<a href="#home" data-target="home">🏠 صفحه اصلی</a>
<a href="#gallery" data-target="gallery">📸 گالری عکس‌ها</a>
<a href="#videos" data-target="videos">🎬 ویدیوها</a>
<a href="#cards" data-target="cards">💳 شماره کارت‌ها</a>
<a href="#mojtaba" data-target="mojtaba">🕊️ شهید مجتبی</a>
<a href="https://kasebamin.mydigify.app/" target="_blank">🛒 فروشگاه کاسب امین</a>
<a href="#about" data-target="about">ℹ️ درباره ما</a>
<a href="#contact" data-target="contact">📞 ارتباط با ما</a>
</nav>

<section id="home" class="active">
<h2>صفحه اصلی</h2>
<p>خیریه دارالاحسان حضرت فاطمه تقدیم می‌کند</p>
</section>

<section id="gallery">
<h2>گالری عکس‌ها</h2>
<div class="gallery">
<!-- ۳۰ عکس -->
<script>
for(let i=1;i<=30;i++){
  document.write('<a href="images/photo'+i+'.jpg" class="glightbox"><img src="images/photo'+i+'.jpg" alt="عکس '+i+'"></a>');
}
</script>
</div>
</section>

<section id="videos">
<h2>ویدیوها</h2>
<ul>
<li><a href="videos/video1.mp4" target="_blank">video1.mp4</a></li>
<li><a href="videos/video2.mp4" target="_blank">video2.mp4</a></li>
</ul>
</section>

<section id="cards">
<h2>شماره کارت‌های خیریه</h2>
<div class="cards">
<script>
const cards = [
["6037997599431443","صدقات،تمام مصارف خیریه(دارو،شیر خشک و...)"],
["5894637000163383","خریدملک حسینیه و زائرسرا مشهد"],
["5892107044557489","باقیات و صالحات فاطمی"],
["6037997599470987","نحر شتر"],
["6037997599470979","نذرقربانی هفتگی (گوشت،مرغ)"],
["6274121940107204","اطعام وافطار،مراسمات اهلبیت"],
["5894637000172434","وقف صندوق قرض الحسنه"],
["5892107044199209","مراسمات بیت الرقیه وبیت الزهرا مشهد"],
["6274121940107196","اعزام زوار به کربلا و مشهد و قم"],
["5859838800018396","نون نذری وکفاره روزه"],
["5892107044245937","رد مظالم عباد (ادای حق الناس)"],
["6274121940107188","نذر خرید زمین و مصالح،کارهای عام المنفعه"],
["6037708800050678","خیرات میوه و خرما برای اموات"],
["5859837011499171","تهیه لوازم خانگی وجهیزیه به عروس"],
["6037708800050660","سهم سادات"],
["5859838800077889","زکات مستحبی وفطریه"],
["5892107044199217","یک درصدطلایی برای مصارف مهدوی دینی(کارت برکت)"],
["5041721112361804","دوشنبه های امام حسنی( ایتام و نیازمندان)"],
["5041721112361812","نذر شنبه ام البنین(س)"],
["6037997599835221","عطای فاطمی(تهیه پوشاک و کفش و چادر)"],
["6037997599979827","هدیه به طلاب علوم دینی"]
];
cards.forEach(c=>{
  document.write('<div class="card"><span>'+c[0]+' - '+c[1]+'</span><button onclick="copyToClipboard(\''+c[0]+'\')">کپی</button></div>');
});
</script>
</div>
</section>

<section id="mojtaba">
<h2>شهید مجتبی (علیرضا) قاضی‌زاده</h2>
<div class="mojtaba">
<img src="images/mojtaba.jpg" alt="شهید مجتبی">
<p>شهید مجتبی (علیرضا) قاضی زاده، 17 ساله اهل قم<br>در ۱۳۶۴/۱۲/۲۰ در عملیات والفجر۸ به شهادت رسیدند.<br>وصیت ایشان:<br>1. نماز اول وقت<br>2. رساندن سلامش به امام حسین (ع)</p>
<a href="https://neshan.org/maps/places/7c47218b0daaa7d7e816da26a17fd97b#c34.631-50.902-15z-0p" target="_blank" class="map-link">📍 موقعیت مزار</a>
</div>
</section>

<section id="about">
<h2>درباره ما</h2>
<p>خیریه دارالاحسان حضرت فاطمه (س) فعالیت‌های خیریه خود را در زمینه کمک‌های مالی، آموزشی و فرهنگی انجام می‌دهد.</p>
</section>

<section id="contact">
<h2>ارتباط با ما</h2>
<p>آیدی ایتا: @ghazizadeh1</p>
<p>شماره تماس: 09122519350 (لطفا پیامک دهید)</p>
<a href="https://eitaa.com/ghazizadeh1" target="_blank">پیوی در ایتا</a>
</section>

<footer>© 2026 خیریه دارالاحسان</footer>

<script>
// Splash screen
setTimeout(()=>{
  const splash=document.querySelector('.splash');
  splash.style.opacity='0';
  setTimeout(()=>{
    splash.style.display='none';
    document.querySelector('.container').style.display='block';
  },500);
},2500);

// تغییر بخش‌ها
document.querySelectorAll('nav a[data-target]').forEach(link=>{
  link.addEventListener('click', e=>{
    e.preventDefault();
    const target = e.target.getAttribute('data-target');
    document.querySelectorAll('section').forEach(s=>s.classList.remove('active'));
    document.getElementById(target).classList.add('active');
  });
});

// کپی کارت‌ها
function copyToClipboard(text){
  navigator.clipboard.writeText(text).then(()=>{
    alert(text + ' در حافظه کپی شد!');
  });
}

// Lightbox
const lightbox = GLightbox({selector: '.glightbox'});
</script>

</body>
</html>
