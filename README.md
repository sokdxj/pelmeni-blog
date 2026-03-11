# pelmeni-blog
<!DOCTYPE html><html lang="uk">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Блог про пельмені</title>
<style>
body{font-family:Arial,Helvetica,sans-serif;margin:0;background:#fafafa;color:#333}
header{background:linear-gradient(135deg,#d32f2f,#ff7043);color:white;padding:40px 20px;text-align:center}
header h1{margin:0;font-size:40px}
nav{background:#b71c1c;padding:10px;text-align:center}
nav a{color:white;margin:0 15px;text-decoration:none;font-weight:bold}
.container{max-width:1100px;margin:auto;padding:20px}
.search{margin:20px 0;text-align:center}
.search input{padding:12px;width:60%;max-width:400px;border-radius:25px;border:1px solid #ccc;font-size:16px}
.grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(250px,1fr));gap:20px}
.card{background:white;border-radius:15px;overflow:hidden;box-shadow:0 6px 15px rgba(0,0,0,0.1);transition:0.2s}
.card:hover{transform:translateY(-5px)}
.card img{width:100%;height:180px;object-fit:cover}
.card-content{padding:15px}
.card h3{margin-top:0}
footer{background:#222;color:white;text-align:center;padding:20px;margin-top:40px}
</style>
</head>
<body><header>
<h1>🥟 Блог про пельмені</h1>
<p>Найкращі рецепти пельменів з усього світу</p>
</header><nav>
<a href="#">Головна</a>
<a href="#">Рецепти</a>
<a href="#">Контакти</a>
</nav><div class="container"><div class="search">
<input type="text" id="search" placeholder="Пошук рецепту..." onkeyup="searchRecipes()" />
</div><div class="grid" id="recipes"><div class="card" data-name="класичні пельмені">
<img src="https://images.unsplash.com/photo-1604908812859-1b0c6c8bda0c" />
<div class="card-content">
<h3>Класичні пельмені</h3>
<p>Свинина, цибуля, спеції. Традиційний домашній рецепт.</p>
</div>
</div><div class="card" data-name="пельмені з куркою">
<img src="https://images.unsplash.com/photo-1625944525533-473f1bba1c0f" />
<div class="card-content">
<h3>Пельмені з куркою</h3>
<p>Легкі пельмені з ніжним курячим фаршем.</p>
</div>
</div><div class="card" data-name="смажені пельмені">
<img src="https://images.unsplash.com/photo-1601050690597-df0568f70950" />
<div class="card-content">
<h3>Смажені пельмені</h3>
<p>Хрусткі пельмені зі скоринкою на сковороді.</p>
</div>
</div><div class="card" data-name="пельмені з яловичиною">
<img src="https://images.unsplash.com/photo-1562967916-eb82221dfb92" />
<div class="card-content">
<h3>Пельмені з яловичиною</h3>
<p>Ситний варіант з ароматним фаршем.</p>
</div>
</div><div class="card" data-name="пельмені з грибами">
<img src="https://images.unsplash.com/photo-1603079840592-6c6b0b2df7c7" />
<div class="card-content">
<h3>Пельмені з грибами</h3>
<p>Чудовий вегетаріанський рецепт.</p>
</div>
</div><div class="card" data-name="пельмені з сиром">
<img src="https://images.unsplash.com/photo-1544025162-d76694265947" />
<div class="card-content">
<h3>Пельмені з сиром</h3>
<p>Ніжні пельмені з сирною начинкою.</p>
</div>
</div><div class="card" data-name="пельмені з індичкою">
<img src="https://images.unsplash.com/photo-1504674900247-0877df9cc836" />
<div class="card-content">
<h3>Пельмені з індичкою</h3>
<p>Дієтичний та легкий варіант.</p>
</div>
</div><div class="card" data-name="пельмені з рибою">
<img src="https://images.unsplash.com/photo-1553621042-f6e147245754" />
<div class="card-content">
<h3>Пельмені з рибою</h3>
<p>Незвичайний морський рецепт.</p>
</div>
</div><div class="card" data-name="пельмені з картоплею">
<img src="https://images.unsplash.com/photo-1585238342028-78d387f4a707" />
<div class="card-content">
<h3>Пельмені з картоплею</h3>
<p>Домашній бюджетний варіант.</p>
</div>
</div><div class="card" data-name="пельмені з бараниною">
<img src="https://images.unsplash.com/photo-1546069901-eacef0df6022" />
<div class="card-content">
<h3>Пельмені з бараниною</h3>
<p>Ароматний східний стиль.</p>
</div>
</div><div class="card" data-name="гострі пельмені">
<img src="https://images.unsplash.com/photo-1481931098730-318b6f776db0" />
<div class="card-content">
<h3>Гострі пельмені</h3>
<p>З перцем чилі та спеціями.</p>
</div>
</div><div class="card" data-name="домашні пельмені">
<img src="https://images.unsplash.com/photo-1529042410759-befb1204b468" />
<div class="card-content">
<h3>Домашні пельмені</h3>
<p>Класичний сімейний рецепт.</p>
</div>
</div></div>
</div><footer>
<p>© 2026 Блог про пельмені</p>
</footer><script>
function searchRecipes(){
const input=document.getElementById('search').value.toLowerCase();
const cards=document.querySelectorAll('.card');

cards.forEach(card=>{
const name=card.dataset.name;
if(name.includes(input)){
card.style.display='block';
}else{
card.style.display='none';
}
});
}
</script></body>
</html>
