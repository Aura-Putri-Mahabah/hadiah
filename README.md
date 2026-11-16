# hadiah
hadiah untuk kalian wahai teman-teman

<html lang="id">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Hadiah Ulang Tahun</title>
<link href="https://fonts.googleapis.com/css2?family=Fredoka:wght@400;500;600&family=Nunito:wght@400;600;700&display=swap" rel="stylesheet">
<style>
:root{--bg:#fbf6ff;--card:#ffffff;--ink:#4a3f5c;--soft:#8a7f9c;--lilac:#e0d4f5;--mint:#d3eee1;--peach:#ffdfcf;--butter:#fff1bd;--sky:#d3e7f8;--pink:#fbd5e4;--line:#ece3f7;--accent:#b79ae6;
box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
@media (prefers-color-scheme:dark){:root:not([data-theme="light"]){color-scheme:dark;--bg:#241d30;--card:#322a41;--ink:#f1eafb;--soft:#b9aed0;--lilac:#4a3d68;--mint:#2f4d44;--peach:#5a4137;--butter:#585032;--sky:#34495e;--pink:#5b3a49;--line:#46395a;--accent:#b79ae6}}
:root[data-theme="dark"]{color-scheme:dark;--bg:#241d30;--card:#322a41;--ink:#f1eafb;--soft:#b9aed0;--lilac:#4a3d68;--mint:#2f4d44;--peach:#5a4137;--butter:#585032;--sky:#34495e;--pink:#5b3a49;--line:#46395a}
*{box-sizing:border-box}
html{scroll-padding-top:env(safe-area-inset-top,0px)}
body{margin:0;min-height:100vh;background:var(--bg);color:var(--ink);font:400 16px/1.55 Nunito,system-ui,sans-serif;
background-image:radial-gradient(circle at 12% 8%,var(--pink) 0,transparent 32%),radial-gradient(circle at 90% 20%,var(--sky) 0,transparent 30%),radial-gradient(circle at 70% 95%,var(--mint) 0,transparent 32%);background-attachment:fixed}
main{max-width:560px;margin:0 auto;padding:28px 18px 60px}
h1,h2{font-family:Fredoka,Nunito,sans-serif;font-weight:600;margin:0;line-height:1.2}
h1{font-size:30px}h2{font-size:24px;margin-bottom:6px}
.dots{display:flex;gap:6px;margin:0 0 18px}
.dots i{flex:1;height:7px;border-radius:9px;background:var(--line);transition:background .3s}
.dots i.on{background:var(--accent)}
.card{background:var(--card);border-radius:28px;padding:26px 22px;border:2px solid var(--line);box-shadow:0 14px 40px -22px var(--accent);animation:pop .35s ease}
@keyframes pop{from{transform:scale(.97);opacity:.4}to{transform:none;opacity:1}}
p.sub{color:var(--soft);margin:0 0 18px}
input[type=text],input[type=date]{width:100%;font:600 18px Nunito,sans-serif;padding:14px 16px;border-radius:18px;border:2px solid var(--line);background:var(--bg);color:var(--ink)}
input:focus,button:focus-visible{outline:3px solid var(--accent);outline-offset:2px}
.btn{font:500 18px Fredoka,sans-serif;border:0;border-radius:18px;padding:13px 26px;cursor:pointer;background:var(--accent);color:#2f2540;margin-top:18px}
.btn.ghost{background:transparent;color:var(--soft);border:2px solid var(--line);margin-left:8px}
.btn:disabled{opacity:.45;cursor:not-allowed}
.grid{display:grid;gap:10px}
.opt{font:600 17px Nunito,sans-serif;text-align:left;padding:14px 16px;border-radius:18px;border:2px solid var(--line);background:var(--bg);color:var(--ink);cursor:pointer;transition:transform .15s,border-color .15s}
.opt:hover{transform:translateY(-2px);border-color:var(--accent)}
.opt small{display:block;font-weight:400;color:var(--soft)}
.c0{background:var(--lilac)}.c1{background:var(--peach)}.c2{background:var(--mint)}.c3{background:var(--butter)}
.chips{display:flex;flex-wrap:wrap;gap:8px;max-height:340px;overflow-y:auto;padding:2px}
.chip{font:600 15px Nunito,sans-serif;padding:9px 14px;border-radius:99px;border:2px solid transparent;background:var(--lilac);color:var(--ink);cursor:pointer}
.chip.sel{border-color:var(--ink);transform:scale(1.05)}
.big{font:600 15px Nunito,sans-serif;background:var(--butter);border-radius:20px;padding:14px 16px;margin-top:14px;text-align:center}
.big b{font:600 22px Fredoka,sans-serif;display:block}
.age{display:grid;grid-template-columns:repeat(3,1fr);gap:8px;margin-top:14px}
.age div{background:var(--lilac);border-radius:16px;padding:10px 4px;text-align:center}
.age div:nth-child(2n){background:var(--mint)}
.age b{display:block;font:600 24px Fredoka,sans-serif}
.age span{font-size:13px;color:var(--soft)}
.slot{font:600 26px Fredoka,sans-serif;text-align:center;padding:34px 10px;border-radius:22px;background:var(--pink);min-height:110px;display:flex;align-items:center;justify-content:center}
.result{text-align:center}
.animal{font-size:96px;line-height:1;margin:8px 0;animation:bob 2.4s ease-in-out infinite}
@keyframes bob{50%{transform:translateY(-8px) rotate(-3deg)}}
.sum{text-align:left;background:var(--bg);border-radius:20px;padding:14px 18px;margin-top:14px}
.sum div{display:flex;justify-content:space-between;gap:12px;padding:4px 0}
.sum span{color:var(--soft)}
.sum b{text-align:right}
@media (prefers-reduced-motion:reduce){*{animation:none!important;transition:none!important}}
</style>
</head>
<body>
<main>
<div class="dots" id="dots"></div>
<section class="card" id="stage"></section>
</main>
<script>
var S={name:'',dob:'',mode:'',cat:'',scent:'',q5:'',q6:''};
var STEPS=['name','dob','hello','mode','scent','q5','q6','result'];
var cur=0,timer=null;
var SC={
Bunga:'Bunga 7 Rupa|Bunga Cempaka|Bunga Cempaka Keraton|Bunga Jasmin|Bunga Jasmin Royal|Bunga Kenanga|Bunga Lavender|Bunga Mawar Bali|Bunga Mawar Keraton|Bunga Melati|Bunga Melati Keraton|Bunga Rose|Bunga Sedap Malam|Bunga Tanjung|Bunga Terompet',
Buah:'Buah Anggur|Buah Apel|Buah Arbei|Buah Ceri|Buah Cranberry|Buah Green Apple|Buah Green Pear|Buah Guava “Jambu”|Buah Jeruk|Buah Jeruk New|Buah Jeruk Sunkis|Buah Lemon|Buah Mangga|Buah Melon|Buah Melon Muda|Buah Papaya|Buah Papaya Mangga|Buah Peach “Persik”|Buah Strawberry|Cucumber “Ketimun”|Fruits Glam|Mix Fruit|Orange Fruit|Passion Fruit|Strawberry Candy',
Laundry:'Akasia|Downy Antibacteria|Downy Black|Downy Blue|Kispray|Leaf Oil Essential|Life Boy|Masterbar|Pantai Kuta Bali|Pond’s|Snapy|White Tea',
Gourmand:'Black Coffee|Black Coffee “Kapal Api”|Butterscotch|Cappuchino|Cappuchino New|Caramel|Cheese Cream|Chiffon Cake|Chocolate Hot|Chocolate Orange|Chocolate Swiss|Cocopandan|Coffee|Coffee Espresso|Coffee Hazelnut|Coffee Luwak|Coklat (Chocolate)|Coklat Cappuchino|Coklat Essence (Essence Chocolate)|Coklat Manis (Sweet Chocolate)|Pie Crusty|Roti Buoy|Vanilla|Vanilla Bitter|Vanilla Butter Milk|Vanilla Cake|Vanilla Coffee|Vanilla Mango|Vanilla Mango New|Vanilla Pleasure|Vanilla Susu|White Cake'};
Object.keys(SC).forEach(function(k){SC[k]=SC[k].split('|')});
var ALL=[].concat(SC.Bunga,SC.Buah,SC.Laundry,SC.Gourmand);
var stage=document.getElementById('stage');
function esc(t){return String(t).replace(/[&<>"]/g,function(c){return {'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;'}[c]})}
function dots(){document.getElementById('dots').innerHTML=STEPS.map(function(_,i){return '<i class="'+(i<=cur?'on':'')+'"></i>'}).join('')}
function go(n){cur=n;clearInterval(timer);dots();render();window.scrollTo(0,0)}
function age(){
  var b=new Date(S.dob+'T00:00:00'),n=new Date();
  var y=n.getFullYear()-b.getFullYear(),m=n.getMonth()-b.getMonth(),d=n.getDate()-b.getDate();
  if(d<0){m--;d+=new Date(n.getFullYear(),n.getMonth(),0).getDate()}
  if(m<0){y--;m+=12}
  return [y,m,d,n.getHours(),n.getMinutes(),n.getSeconds()];
}
function two(x){return x<10?'0'+x:x}
function render(){
  var s=STEPS[cur],h='';
  if(s=='name'){
    h='<h1>Halo, selamat datang</h1><p class="sub">Ada hadiah kecil yang menunggu. Isi dulu ya.</p><label for="n"><h2>Siapa nama kamu?</h2></label><input type="text" id="n" maxlength="40" placeholder="Tulis namamu di sini" value="'+esc(S.name)+'"><button class="btn" id="nx">Lanjut</button>';
    stage.innerHTML=h;var i=document.getElementById('n'),b=document.getElementById('nx');
    var chk=function(){b.disabled=!i.value.trim()};chk();i.oninput=chk;
    b.onclick=function(){S.name=i.value.trim();go(1)};i.onkeydown=function(e){if(e.key=='Enter'&&!b.disabled)b.click()};
  }else if(s=='dob'){
    h='<label for="d"><h2>Kapan kamu keluar dari rahim ibu/mamah/mommy/bunda/umi/baginda ratu?</h2></label><p class="sub">Pilih tanggal lahirmu di kalender.</p><input type="date" id="d" value="'+S.dob+'" max="'+new Date().toISOString().slice(0,10)+'"><button class="btn" id="nx">Lanjut</button><button class="btn ghost" id="bk">Kembali</button>';
    stage.innerHTML=h;var d=document.getElementById('d'),b=document.getElementById('nx');
    var chk=function(){b.disabled=!d.value||new Date(d.value)>new Date()};chk();d.oninput=chk;
    b.onclick=function(){S.dob=d.value;go(2)};document.getElementById('bk').onclick=function(){go(0)};
  }else if(s=='hello'){
    var a=age();
    h='<div class="result"><div class="animal" style="font-size:64px">🎂</div><h1>Selamat ulang tahun, '+esc(S.name)+'!</h1><p class="sub">Kamu sudah hidup selama</p></div><div class="age"><div><b id="a0">0</b><span>tahun</span></div><div><b id="a1">0</b><span>bulan</span></div><div><b id="a2">0</b><span>hari</span></div><div><b id="a3">0</b><span>jam</span></div><div><b id="a4">0</b><span>menit</span></div><div><b id="a5">0</b><span>detik</span></div></div><button class="btn" id="nx">Lanjut ke hadiah</button><button class="btn ghost" id="bk">Kembali</button>';
    stage.innerHTML=h;
    var tick=function(){var v=age();for(var i=0;i<6;i++)document.getElementById('a'+i).textContent=i>2?two(v[i]):v[i]};
    tick();timer=setInterval(tick,1000);
    document.getElementById('nx').onclick=function(){go(3)};document.getElementById('bk').onclick=function(){go(1)};
  }else if(s=='mode'){
    h='<h2>Kamu mau racik sendiri atau gacha?</h2><p class="sub">Pilih cara dapat aroma hadiahmu.</p><div class="grid"><button class="opt c0" data-m="racik">Racik sendiri<small>Pilih kategori, lalu pilih aroma favoritmu</small></button><button class="opt c1" data-m="gacha">Gacha<small>Biar semesta yang memilihkan aromamu</small></button></div><button class="btn ghost" id="bk" style="margin-left:0">Kembali</button>';
    stage.innerHTML=h;
    [].forEach.call(stage.querySelectorAll('[data-m]'),function(b){b.onclick=function(){S.mode=b.dataset.m;S.scent='';S.cat='';go(4)}});
    document.getElementById('bk').onclick=function(){go(2)};
  }else if(s=='scent'){
    if(S.mode=='racik')racik();else gacha();
  }else if(s=='q5'||s=='q6'){
    var five=s=='q5',opts=five?['Arya','Ara']:['Arya','Caca'];
    h='<p class="sub">Bayangkan dulu ya…</p><h2>'+(five?'IMAGINE dalam match IDP, kamu lebih percaya diselamatkan sama siapa?':'IMAGINE lagi dalam match IDP, siapa penyebab kamu ketangkep HUNTER?')+'</h2><div class="grid" style="margin-top:16px">'+opts.map(function(o,i){return '<button class="opt c'+(i?2:3)+'" data-o="'+o+'">'+o+'</button>'}).join('')+'</div><button class="btn ghost" id="bk" style="margin-left:0">Kembali</button>';
    stage.innerHTML=h;
    [].forEach.call(stage.querySelectorAll('[data-o]'),function(b){b.onclick=function(){if(five)S.q5=b.dataset.o;else S.q6=b.dataset.o;go(cur+1)}});
    document.getElementById('bk').onclick=function(){go(cur-1)};
  }else{
    var an,em;
    if(S.q5=='Arya'&&S.q6=='Arya'){an='Ular';em='🐍'}
    else if(S.q5=='Ara'&&S.q6=='Caca'){an='Kucing';em='🐱'}
    else{an='Kapibara';em='🦫'}
    S.animal=an;
    h='<div class="result"><p class="sub">Hasil untuk '+esc(S.name)+'</p><div class="animal">'+em+'</div><h1>Kamu adalah '+an+'!</h1></div><div class="sum"><div><span>Nama</span><b>'+esc(S.name)+'</b></div><div><span>Aroma hadiah</span><b>'+esc(S.scent)+'</b></div><div><span>Cara memilih</span><b>'+(S.mode=='racik'?'Racik sendiri':'Gacha')+'</b></div><div><span>Hewan</span><b>'+an+'</b></div></div><button class="btn" id="cp">Salin hasil</button><button class="btn ghost" id="rs">Ulangi</button><p class="sub" id="msg" style="margin:10px 0 0"></p>';
    stage.innerHTML=h;
    document.getElementById('cp').onclick=function(){
      var t='Nama: '+S.name+'\nAroma: '+S.scent+' ('+(S.mode=='racik'?'racik sendiri':'gacha')+')\nHewan: '+an;
      var m=document.getElementById('msg');
      try{navigator.clipboard.writeText(t).then(function(){m.textContent='Tersalin. Kirim ke pembuat hadiah ya!'},function(){m.textContent='Gagal menyalin. Screenshot layar ini saja ya.'})}catch(e){m.textContent='Gagal menyalin. Screenshot layar ini saja ya.'}
    };
    document.getElementById('rs').onclick=function(){S={name:'',dob:'',mode:'',cat:'',scent:'',q5:'',q6:''};go(0)};
  }
}
function racik(){
  var h='<h2>Pilih kategori aromamu</h2><div class="chips" id="cats" style="margin:12px 0">'+Object.keys(SC).map(function(k,i){return '<button class="chip c'+(i%4)+(S.cat==k?' sel':'')+'" data-c="'+k+'">'+k+'</button>'}).join('')+'</div><div id="list"></div><button class="btn" id="nx" disabled>Pilih aroma ini</button><button class="btn ghost" id="bk">Kembali</button>';
  stage.innerHTML=h;
  var nx=document.getElementById('nx');
  function list(){
    var el=document.getElementById('list');
    if(!S.cat){el.innerHTML='<p class="sub">Pilih salah satu kategori di atas dulu.</p>';return}
    el.innerHTML='<p class="sub" style="margin-bottom:8px">'+SC[S.cat].length+' aroma '+S.cat.toLowerCase()+'</p><div class="chips">'+SC[S.cat].map(function(x){return '<button class="chip'+(S.scent==x?' sel':'')+'" data-s="'+esc(x)+'">'+esc(x)+'</button>'}).join('')+'</div>';
    [].forEach.call(el.querySelectorAll('[data-s]'),function(b){b.onclick=function(){S.scent=b.dataset.s;nx.disabled=false;[].forEach.call(el.querySelectorAll('.chip'),function(c){c.classList.toggle('sel',c==b)})}});
  }
  list();nx.disabled=!S.scent;
  [].forEach.call(document.querySelectorAll('[data-c]'),function(b){b.onclick=function(){S.cat=b.dataset.c;S.scent='';[].forEach.call(document.querySelectorAll('[data-c]'),function(c){c.classList.toggle('sel',c==b)});nx.disabled=true;list()}});
  nx.onclick=function(){go(5)};document.getElementById('bk').onclick=function(){go(3)};
}
function gacha(){
  stage.innerHTML='<h2>Gacha aroma</h2><p class="sub">Tekan tombolnya dan lihat aroma apa yang keluar.</p><div class="slot" id="slot">?</div><button class="btn" id="roll">Putar gacha</button><button class="btn ghost" id="nx" style="display:none">Pakai aroma ini</button><button class="btn ghost" id="bk">Kembali</button>';
  var slot=document.getElementById('slot'),roll=document.getElementById('roll'),nx=document.getElementById('nx');
  roll.onclick=function(){
    roll.disabled=true;nx.style.display='none';
    var n=0,pick=ALL[Math.floor(Math.random()*ALL.length)];
    var iv=setInterval(function(){n++;slot.textContent=ALL[Math.floor(Math.random()*ALL.length)];
      if(n>22){clearInterval(iv);S.scent=pick;slot.textContent=pick;roll.disabled=false;roll.textContent='Putar lagi';nx.style.display='inline-block'}},75);
  };
  nx.onclick=function(){go(5)};document.getElementById('bk').onclick=function(){go(3)};
}
dots();render();
</script>
</body>
</html>
