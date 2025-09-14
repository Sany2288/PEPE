# PEPE
<!DOCTYPE html>
<html lang="uk">
<head>
<meta charset="UTF-8">
<title>МТЗ Техніка PRO</title>
<style>
body {font-family:Arial,sans-serif;margin:0;background:linear-gradient(135deg,#003366,#0059b3);color:white;min-height:100vh;transition:background 0.5s,color 0.5s;}
body.light {background:linear-gradient(135deg,#ffffff,#dddddd);color:black;}
header{background:#002244cc;padding:10px;color:white;text-align:center;}
nav{background:#004080cc;padding:10px;display:flex;justify-content:center;gap:20px;position:sticky;top:0;z-index:1000;}
nav a{color:white;text-decoration:none;font-weight:bold;cursor:pointer;position:relative;transition:transform 0.2s;}
nav a:hover{transform:scale(1.1);}
.cart-count{position:absolute;top:-8px;right:-12px;background:red;color:white;border-radius:50%;font-size:12px;padding:2px 6px;}
.cart-count.pop{animation:pop 0.4s;}
@keyframes pop{0%{transform:scale(1);}50%{transform:scale(1.5);}100%{transform:scale(1);}}
section{padding:20px;display:none;}
section.active{display:block;}
h1,h2{color:#ffdd00;}
.controls{margin-bottom:20px;display:flex;gap:10px;flex-wrap:wrap;}
input,button,select{padding:8px;font-size:14px;cursor:pointer;}
#product-list,#cart{display:flex;flex-wrap:wrap;gap:15px;margin-top:20px;}
.product,.cart-item{background:#ffffffcc;border:1px solid #ccc;padding:10px;width:200px;text-align:center;border-radius:5px;color:black;position:relative;box-shadow:0 0 10px rgba(0,0,0,0.5);transition:transform 0.2s;}
.product:hover,.cart-item:hover{transform:scale(1.03);}
.product img,.cart-item img{width:100%;height:120px;object-fit:cover;margin-bottom:10px;}
.add-btn{background:linear-gradient(45deg,#0077ff,#00ccff);border:none;color:white;cursor:pointer;transition:transform 0.2s,box-shadow 0.2s;}
.add-btn:hover{transform:scale(1.1);box-shadow:0 0 10px #00ccff;}
.add-btn:active,.add-btn.bounce{animation:bounce 0.5s;}
@keyframes bounce{0%{transform:scale(1);}30%{transform:scale(1.3);}50%{transform:scale(0.9);}70%{transform:scale(1.1);}100%{transform:scale(1);}}
#cart-total{margin-top:20px;font-weight:bold;font-size:18px;color:yellow;}
#admin-panel{display:none;margin-bottom:20px;border:2px solid #ffdd00;padding:10px;border-radius:5px;background:#002244cc;}
#chat{border:2px solid #ffdd00;padding:10px;border-radius:5px;background:#ffffffcc;max-width:400px;color:black;}
#messages{max-height:200px;overflow-y:auto;margin-bottom:10px;border:1px solid #ccc;padding:5px;background:#f9f9f9;}
.msg{margin:5px 0;padding:5px;border-radius:5px;}
.user{background:#d9f7ff;text-align:left;}
.tato{background:#d4ffd4;text-align:right;}
.contacts{background:#ffffffcc;border:1px solid #ccc;padding:15px;border-radius:5px;max-width:400px;color:black;}
.contacts p{font-size:16px;margin:8px 0;}
.low-stock{border:2px solid red;}
.qr-code{display:block;margin:10px auto;width:100px;height:100px;border:1px solid #ccc;border-radius:5px;}
#toast{position:fixed;bottom:20px;left:50%;transform:translateX(-50%);background:#28a745;color:white;padding:12px 25px;border-radius:5px;font-weight:bold;display:none;z-index:10000;box-shadow:0 0 10px #000;}
#toast.show{display:block;animation:fadeinout 2s forwards;}
@keyframes fadeinout{0%{opacity:0;transform:translate(-50%,20px);}10%{opacity:1;transform:translate(-50%,0);}90%{opacity:1;transform:translate(-50%,0);}100%{opacity:0;transform:translate(-50%,20px);}}
</style>
</head>
<body>

<header>
<h1>🚜 МТЗ Техніка PRO</h1>
<button onclick="toggleTheme()">🌙/☀️ Тема</button>
</header>

<nav>
<a onclick="showSection('home')">Головна</a>
<a onclick="showSection('products')">Товари</a>
<a onclick="showSection('cart-section')">Кошик <span id="cartCount" class="cart-count">0</span></a>
<a onclick="showSection('chat-section')">Чат</a>
<a onclick="showSection('contacts-section')">Контакти</a>
</nav>

<section id="home" class="active">
<h2>Ласкаво просимо!</h2>
<p>Тут ви знайдете техніку МТЗ. Товар додає лише тато.</p>
<canvas id="qrCanvas"></canvas>
<p>Скануйте, щоб відкрити сайт на телефоні!</p>
</section>

<section id="products">
<div class="controls">
<input type="text" id="search" placeholder="Пошук товару...">
<button onclick="loginAdmin()">Увійти як тато</button>
</div>

<div id="admin-panel">
<h3>Додавання товару (тільки для тата)</h3>
<input type="file" id="photo">
<input type="text" id="name" placeholder="Назва товару">
<input type="number" id="price" placeholder="Ціна (грн)">
<input type="number" id="quantity" placeholder="Кількість">
<button onclick="addProduct()">Додати товар</button>
</div>

<h2>Список товарів</h2>
<div id="product-list"></div>
</section>

<section id="cart-section">
<h2>Кошик</h2>
<div id="cart"></div>
<div id="cart-total">Всього: 0 грн</div>
<label>Доставка:
<select id="delivery">
<option value="0">Самовивіз</option>
<option value="100">По області (+100 грн)</option>
<option value="200">По Україні (+200 грн)</option>
</select>
</label>
<br><br>
<button onclick="checkout()">Оформити замовлення</button>
<button onclick="clearCart()">Очистити кошик 🗑️</button>
</section>

<section id="chat-section">
<h2>Чат з татом</h2>
<div id="chat">
<div id="messages"></div>
<input type="text" id="chatInput" placeholder="Напишіть повідомлення...">
<button onclick="sendMessage()">Відправити</button>
</div>
</section>

<section id="contacts-section">
<h2>Контакти</h2>
<div class="contacts">
<p>📞 <a href="tel:+380957611689">0 (95) 761 16 89 – <b>Олександр Михайлович</b></a></p>
<p>📞 <a href="tel:+380665071920">0 (66) 507 19 20 – <b>Михайло</b></a></p>
</div>
</section>

<div id="toast"></div>

<audio id="cashSound" src="https://www.soundjay.com/misc/sounds/cash-register-01.mp3"></audio>
<audio id="msgSound" src="https://www.soundjay.com/button/sounds/button-09.mp3"></audio>
<audio id="clearSound" src="https://www.soundjay.com/button/sounds/button-10.mp3"></audio>

<script src="https://cdn.jsdelivr.net/npm/qrious/dist/qrious.min.js"></script>
<script>
let products=[], cart=[], messages=[], isAdmin=false;
const productList=document.getElementById('product-list');
const searchInput=document.getElementById('search');
const cartDiv=document.getElementById('cart');
const cartTotal=document.getElementById('cart-total');
const adminPanel=document.getElementById('admin-panel');
const messagesDiv=document.getElementById('messages');
const cartCount=document.getElementById('cartCount');
const cashSound=document.getElementById('cashSound');
const msgSound=document.getElementById('msgSound');
const clearSound=document.getElementById('clearSound');
const deliverySelect=document.getElementById('delivery');
const toast=document.getElementById('toast');

function showSection(id){document.querySelectorAll("section").forEach(sec=>sec.classList.remove("active"));document.getElementById(id).classList.add("active");}
function saveData(){localStorage.setItem("products",JSON.stringify(products));localStorage.setItem("cart",JSON.stringify(cart));localStorage.setItem("messages",JSON.stringify(messages));}
function toggleTheme(){document.body.classList.toggle("light");}

function loginAdmin(){
    const password=prompt("Введіть пароль тата:");
    if(password==="mtz123"){isAdmin=true; adminPanel.style.display="block"; alert("Ви увійшли як тато!");} else alert("Неправильний пароль!");
}

function addProduct(){
    if(!isAdmin)return alert("Тільки тато може додавати товари!");
    const photoInput=document.getElementById('photo');
    const name=document.getElementById('name').value;
    const price=document.getElementById('price').value;
    const quantity=document.getElementById('quantity').value;
    if(!name||!price||!quantity||!photoInput.files[0])return alert("Заповніть усі поля!");
    const reader=new FileReader();
    reader.onload=function(e){
        products.push({id:Date.now(),name,price:Number(price),quantity:Number(quantity),photo:e.target.result});
        saveData(); displayProducts(products);
    }
    reader.readAsDataURL(photoInput.files[0]);
}

function displayProducts(list){
    productList.innerHTML="";
    list.forEach(p=>{
        const div=document.createElement('div'); div.className='product';
        if(p.quantity<5) div.classList.add('low-stock');
        div.innerHTML=`<img src="${p.photo}" alt="${p.name}" title="Ціна: ${p.price} грн, Кількість: ${p.quantity}">
        <h3>${p.name}</h3>
        <p>Ціна: ${p.price} грн</p>
        <p>Кількість: ${p.quantity}</p>
        <button class="add-btn" onclick="addToCart(${p.id}, this)" ${p.quantity<=0?"disabled":""}>${p.quantity>0?"У кошик":"Немає в наявності"}</button>
        <br><br><img id="qr-${p.id}" class="qr-code" />`;
        productList.appendChild(div);
        new QRious({element:document.getElementById(`qr-${p.id}`),value:`https://example.com/product/${p.id}`,size:100,background:'white',foreground:'black',level:'H'});
    });
}

function addToCart(id,btn){
    const product=products.find(p=>p.id===id);
    if(!product||product.quantity<=0)return alert("Товар закінчився!");
    let item=cart.find(c=>c.id===id);
    if(item){if(item.quantity<product.quantity)item.quantity++;else return alert("Немає більше в наявності!");}
    else cart.push({...product,quantity:1});
    btn.classList.add('bounce'); setTimeout(()=>btn.classList.remove('bounce'),500);
    cartCount.classList.add('pop'); setTimeout(()=>cartCount.classList.remove('pop'),400);
    cashSound.play(); saveData(); updateCart();
}

function updateCart(){
    cartDiv.innerHTML=""; let total=0;
    cart.forEach(c=>{
        total+=c.price*c.quantity;
        const div=document.createElement('div'); div.className="cart-item";
        div.innerHTML=`<img src="${c.photo}" alt="${c.name}"><h4>${c.name}</h4><p>Ціна: ${c.price} грн</p><p>Кількість: ${c.quantity}</p><button onclick="removeFromCart(${c.id})">Видалити</button>`;
        cartDiv.appendChild(div);
    });
    total+=Number(deliverySelect.value);
    cartTotal.innerText=`Всього: ${total} грн`;
    cartCount.innerText=cart.reduce((acc,c)=>acc+c.quantity,0);
}

function removeFromCart(id){cart=cart.filter(c=>c.id!==id); saveData(); updateCart();}
function clearCart(){cart=[]; saveData(); updateCart(); clearSound.play(); showToast("Кошик очищено!");}
function checkout(){if(cart.length===0)return alert("Кошик порожній!"); showToast("Замовлення оформлено!"); cart.forEach(c=>{const prod=products.find(p=>p.id===c.id); if(prod) prod.quantity-=c.quantity;}); cart=[]; saveData(); displayProducts(products); updateCart();}
searchInput.addEventListener('input',()=>{const term=searchInput.value.toLowerCase(); displayProducts(products.filter(p=>p.name.toLowerCase().includes(term)));});

function sendMessage(){
    const text=document.getElementById('chatInput').value.trim();
    if(!text)return;
    messages.push({text,sender:"user"});
    messages.push({text:"Дякую, замовлення прийнято!",sender:"tato"});
    document.getElementById('chatInput').value="";
    renderMessages(); saveData(); msgSound.play();
}

function renderMessages(){messagesDiv.innerHTML=""; messages.forEach(m=>{const div=document.createElement('div'); div.className="msg "+(m.sender==="user"?"user":"tato"); div.innerText=m.text; messagesDiv.appendChild(div);}); messagesDiv.scrollTop=messagesDiv.scrollHeight;}
function showToast(msg){toast.innerText=msg; toast.classList.add('show'); setTimeout(()=>toast.classList.remove('show'),2000);}

displayProducts(products); updateCart(); renderMessages();
new QRious({element:document.getElementById('qrCanvas'),value:window.location.href,size:150,background:'white',foreground:'black',level:'H'});
</script>
</body>
</html>
