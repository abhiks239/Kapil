<html lang="hi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Mindo Pickles – घर जैसा स्वाद</title>
<link href="https://fonts.googleapis.com/css2?family=Baloo+2:wght@600;700;800&family=Poppins:wght@400;500;600;700&display=swap" rel="stylesheet">
<style>
  :root{
    --green:#1f5d2b; --green-dark:#123b1b; --red:#c9271f; --gold:#f0b429;
    --cream:#fff8ea; --dark:#2b1a10;
    --shadow-sm:0 2px 8px rgba(43,26,16,.08);
    --shadow-md:0 10px 30px rgba(43,26,16,.12);
    --shadow-lg:0 20px 50px rgba(43,26,16,.18);
  }
  *{box-sizing:border-box;margin:0;padding:0}
  html{scroll-behavior:smooth}
  body{font-family:'Poppins',sans-serif;background:var(--cream);color:var(--dark);line-height:1.6;
    background-image:
      radial-gradient(circle at 15% 20%, rgba(240,180,41,.08) 0%, transparent 40%),
      radial-gradient(circle at 85% 80%, rgba(31,93,43,.08) 0%, transparent 40%);
    background-attachment:fixed;
  }
  h1,h2,h3,h4{font-family:'Baloo 2',sans-serif;line-height:1.2}
  img{max-width:100%;display:block}
  a{text-decoration:none;color:inherit}
  .container{width:min(1180px,92%);margin:auto}

  /* Header */
  header{position:sticky;top:0;z-index:100;background:rgba(255,255,255,.9);backdrop-filter:blur(12px);border-bottom:1px solid rgba(43,26,16,.06);box-shadow:var(--shadow-sm)}
  .nav{display:flex;align-items:center;justify-content:space-between;padding:14px 0;gap:20px}
  .logo{font-family:'Baloo 2',sans-serif;font-size:2rem;font-weight:800;color:var(--green);letter-spacing:-1px}
  .logo span{color:var(--gold);display:inline-block;transform:rotate(-8deg)}
  nav{display:flex;align-items:center;gap:28px}
  nav a{font-weight:600;font-size:.95rem;position:relative;padding:4px 0;transition:color .2s}
  nav a:hover{color:var(--red)}
  .btn{display:inline-flex;align-items:center;gap:8px;justify-content:center;background:linear-gradient(135deg,var(--red),#e6392f);color:#fff;padding:12px 28px;border-radius:50px;font-weight:700;font-size:.95rem;border:0;cursor:pointer;transition:.25s;box-shadow:0 6px 18px rgba(201,39,31,.35);font-family:inherit}
  .btn:hover{transform:translateY(-3px);box-shadow:0 10px 26px rgba(201,39,31,.45)}
  .btn.green{background:linear-gradient(135deg,#25a244,#1c7e34);box-shadow:0 6px 18px rgba(37,162,68,.35)}
  .btn.ghost{background:transparent;color:var(--green);border:2px solid var(--green);box-shadow:none}
  .btn.ghost:hover{background:var(--green);color:#fff}
  .btn.sm{padding:8px 16px;font-size:.85rem}
  .btn:disabled{opacity:.5;cursor:not-allowed;transform:none!important}

  /* Hero */
  .hero{position:relative;overflow:hidden;color:#fff;padding:90px 0 100px;text-align:center;background:linear-gradient(135deg,#123b1b 0%, #1f5d2b 45%, #3f8d4b 100%)}
  .hero::before,.hero::after{content:'';position:absolute;border-radius:50%;filter:blur(60px);opacity:.5}
  .hero::before{width:400px;height:400px;background:var(--gold);top:-100px;left:-100px}
  .hero::after{width:400px;height:400px;background:#7dd87d;bottom:-150px;right:-100px}
  .hero .container{position:relative;z-index:2}
  .hero .tagline{display:inline-block;background:rgba(255,255,255,.15);border:1px solid rgba(255,255,255,.3);padding:8px 20px;border-radius:50px;font-size:.85rem;font-weight:600;letter-spacing:.5px;margin-bottom:20px;backdrop-filter:blur(6px)}
  .hero h1{font-size:clamp(2.2rem,6vw,4rem);margin-bottom:12px;text-shadow:0 4px 20px rgba(0,0,0,.2)}
  .hero h2{font-size:clamp(1.2rem,3vw,1.8rem);color:var(--gold);font-weight:600;margin-bottom:22px}
  .hero p{max-width:640px;margin:0 auto 32px;opacity:.95;font-size:1.05rem}
  .hero .btn{background:linear-gradient(135deg,var(--gold),#f5c445);color:var(--dark);box-shadow:0 8px 24px rgba(240,180,41,.4)}
  .float{position:absolute;font-size:3rem;opacity:.35;animation:float 6s ease-in-out infinite}
  .float.f1{top:20%;left:8%}
  .float.f2{top:60%;left:12%;animation-delay:1s;font-size:2.5rem}
  .float.f3{top:25%;right:8%;animation-delay:2s}
  .float.f4{top:70%;right:12%;animation-delay:1.5s;font-size:2.5rem}
  @keyframes float{0%,100%{transform:translateY(0) rotate(0)}50%{transform:translateY(-20px) rotate(8deg)}}

  /* Badges & Sections */
  .badges{display:flex;flex-wrap:wrap;gap:14px;justify-content:center;padding:40px 0 20px}
  .badge{display:inline-flex;align-items:center;gap:8px;background:#fff;border:2px solid rgba(31,93,43,.15);color:var(--green);padding:12px 22px;border-radius:50px;font-weight:600;font-size:.9rem;box-shadow:var(--shadow-sm);transition:.25s}
  .badge:hover{transform:translateY(-3px);border-color:var(--green);box-shadow:var(--shadow-md)}
  section{padding:70px 0}
  .title{text-align:center;margin-bottom:48px}
  .title .sub{color:var(--red);font-weight:700;font-size:.85rem;letter-spacing:2px;text-transform:uppercase}
  .title h2{font-size:clamp(1.8rem,4vw,2.6rem);color:var(--green);margin:8px 0 10px}
  .title p{color:#6b5b4e;max-width:560px;margin:auto}

  /* Products */
  .grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(260px,1fr));gap:30px}
  .card{position:relative;background:#fff;border-radius:24px;overflow:hidden;box-shadow:var(--shadow-md);transition:.35s;display:flex;flex-direction:column}
  .card:hover{transform:translateY(-8px);box-shadow:var(--shadow-lg)}
  .card .pic{position:relative;height:260px;display:flex;align-items:center;justify-content:center;font-size:6rem;background:linear-gradient(135deg,#fff3d6,#ffe4b3);overflow:hidden}
  .card .pic img{width:100%;height:100%;object-fit:cover;transition:transform .5s}
  .card:hover .pic img{transform:scale(1.08)}
  .card .pic .emoji{font-size:6rem}
  .card .ribbon{position:absolute;top:14px;left:-6px;background:var(--red);color:#fff;padding:6px 16px;font-size:.72rem;font-weight:700;letter-spacing:1px;text-transform:uppercase;border-radius:4px;box-shadow:var(--shadow-sm);z-index:2}
  .card .body{padding:22px;display:flex;flex-direction:column;flex:1;gap:6px}
  .card h3{font-size:1.2rem;color:var(--green)}
  .card .hi{color:var(--red);font-weight:600;font-size:.95rem}
  .card .tag{font-size:.9rem;color:#7a6b5c;margin-bottom:14px;flex:1;line-height:1.5}
  .row{display:flex;justify-content:space-between;align-items:center;margin-bottom:14px}
  .price{font-size:1.5rem;font-weight:800;color:var(--red);font-family:'Baloo 2',sans-serif}
  .price small{font-size:.75rem;color:#999;font-weight:500;text-decoration:line-through;margin-left:6px}
  .wt{background:linear-gradient(135deg,#eef6ef,#dff0e1);color:var(--green);padding:4px 12px;border-radius:20px;font-size:.8rem;font-weight:700}
  .card .btn{width:100%;padding:12px}

  /* See All Card */
  .see-all-card{display:flex;align-items:center;justify-content:center;background:var(--cream);border:3px dashed var(--gold);cursor:pointer;transition:0.3s}
  .see-all-card:hover{background:#ffefd0;transform:translateY(-8px)}
  .see-all-card .inner{text-align:center;padding:20px}
  .see-all-card .plus{font-size:4rem;color:var(--green);line-height:1;margin-bottom:10px}
  .see-all-card h3{color:var(--green);font-size:1.4rem}

  /* Extra Sections */
  .why{background:linear-gradient(180deg,#fff 0%, #fdf6e7 100%)}
  .why .grid{grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:24px}
  .why .item{background:#fff;border-radius:22px;text-align:center;padding:32px 22px;box-shadow:var(--shadow-sm);transition:.3s;border:2px solid transparent}
  .why .item:hover{transform:translateY(-6px);border-color:var(--gold);box-shadow:var(--shadow-md)}
  .why .ico{font-size:3rem;margin-bottom:12px}
  .why h4{margin-bottom:6px;color:var(--green);font-size:1.15rem}
  .why p{color:#7a6b5c;font-size:.9rem}
  .ingr{background:linear-gradient(135deg,var(--green-dark),var(--green));color:#fff;text-align:center;position:relative;overflow:hidden}
  .ingr h2{color:var(--gold);margin-bottom:14px}
  .ingr p{max-width:820px;margin:auto;opacity:.95;line-height:1.8}
  .testi{background:#fff}
  .testi .grid{grid-template-columns:repeat(auto-fit,minmax(280px,1fr));gap:24px}
  .tcard{background:linear-gradient(135deg,#fff8ea,#fdf2d8);border-radius:22px;padding:28px;box-shadow:var(--shadow-sm);transition:.3s;border:1px solid rgba(240,180,41,.2)}
  .tcard:hover{transform:translateY(-4px);box-shadow:var(--shadow-md)}
  .tcard .quote{font-size:2.5rem;color:var(--gold);line-height:1;font-family:Georgia,serif}
  .tcard p{margin:8px 0 16px;color:#4a3a2c;font-style:italic}
  .tcard .who{display:flex;align-items:center;gap:12px}
  .tcard .av{width:44px;height:44px;border-radius:50%;background:linear-gradient(135deg,var(--green),var(--gold));color:#fff;display:flex;align-items:center;justify-content:center;font-weight:700}
  .tcard .nm{font-weight:700;color:var(--green)}
  .tcard .lo{font-size:.8rem;color:#8a7b6c}

  /* Contact & Footer */
  .contact{text-align:center}
  .contact .box{background:#fff;border-radius:26px;padding:40px;box-shadow:var(--shadow-lg);max-width:680px;margin:auto;border-top:6px solid var(--gold)}
  .contact p{margin:10px 0}
  .contact p a{color:var(--red);font-weight:600}
  .contact .btns{margin-top:24px;display:flex;gap:14px;justify-content:center;flex-wrap:wrap}
  .lic{display:inline-block;margin-top:14px;background:#eef6ef;color:var(--green);padding:8px 18px;border-radius:20px;font-size:.85rem;font-weight:600}
  footer{background:linear-gradient(135deg,#1a0e07,#2b1a10);color:#d9cbb9;text-align:center;padding:36px 0 30px;font-size:.9rem}
  footer .brand{color:var(--gold);font-weight:700;font-family:'Baloo 2',sans-serif;font-size:1.3rem;margin-bottom:6px}
  footer .tag{margin-bottom:12px;opacity:.8}

  /* Floating Buttons */
  .wa{position:fixed;right:20px;bottom:20px;background:linear-gradient(135deg,#25a244,#1c7e34);color:#fff;width:62px;height:62px;border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:1.9rem;box-shadow:0 8px 26px rgba(37,162,68,.5);z-index:99;transition:.25s}
  .wa:hover{transform:scale(1.1)}
  
  /* Cart Floating Button */
  .cart-btn-float{position:fixed;right:20px;bottom:95px;background:linear-gradient(135deg,var(--gold),#f5c445);color:var(--dark);width:62px;height:62px;border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:1.8rem;box-shadow:0 8px 26px rgba(240,180,41,.5);z-index:99;transition:.25s;cursor:pointer}
  .cart-btn-float:hover{transform:scale(1.1)}
  .cart-badge{position:absolute;top:-4px;right:-4px;background:var(--red);color:#fff;width:24px;height:24px;border-radius:50%;font-size:.75rem;font-weight:700;display:flex;align-items:center;justify-content:center;border:2px solid #fff}

  .admin-btn{position:fixed;left:16px;bottom:16px;width:36px;height:36px;border-radius:50%;background:rgba(43,26,16,.15);color:rgba(43,26,16,.5);border:0;cursor:pointer;font-size:1.1rem;display:flex;align-items:center;justify-content:center;transition:.3s;z-index:98;backdrop-filter:blur(6px)}
  .admin-btn:hover{background:var(--green);color:#fff;transform:rotate(45deg) scale(1.15)}

  /* Modals & Forms */
  .modal{display:none;position:fixed;inset:0;background:rgba(0,0,0,.65);backdrop-filter:blur(4px);z-index:200;align-items:flex-start;justify-content:center;padding:20px;overflow-y:auto}
  .modal.active{display:flex}
  .modal-box{background:#fff;border-radius:22px;max-width:560px;width:100%;margin:auto;position:relative;padding:30px;box-shadow:0 20px 60px rgba(0,0,0,.4);animation:popIn .3s}
  .modal-box.wide{max-width:900px}
  @keyframes popIn{from{transform:scale(.9);opacity:0}to{transform:scale(1);opacity:1}}
  .modal-close{position:absolute;top:14px;right:14px;width:34px;height:34px;border-radius:50%;background:#f3ede3;color:var(--dark);border:0;cursor:pointer;font-size:1.4rem;display:flex;align-items:center;justify-content:center;line-height:1;transition:.2s;z-index:10}
  .modal-close:hover{background:var(--red);color:#fff}
  .modal h2{color:var(--green);margin-bottom:6px;font-size:1.6rem}
  .modal .subtitle{color:#7a6b5c;font-size:.9rem;margin-bottom:20px}

  .form-group{margin-bottom:14px}
  .form-group label{display:block;font-size:.85rem;font-weight:600;color:var(--dark);margin-bottom:6px}
  .form-group input,.form-group textarea,.form-group select{width:100%;padding:11px 14px;border:2px solid #e5ddd0;border-radius:10px;font-family:inherit;font-size:.95rem;transition:.2s;background:#fff}
  .form-group input:focus,.form-group textarea:focus,.form-group select:focus{outline:none;border-color:var(--green);box-shadow:0 0 0 3px rgba(31,93,43,.1)}
  .form-group textarea{resize:vertical;min-height:70px}
  .form-row{display:grid;grid-template-columns:1fr 1fr;gap:12px}

  /* Cart Modal Specific */
  .cart-item{display:flex;align-items:center;gap:14px;padding:12px 0;border-bottom:1px dashed #e5ddd0}
  .cart-item:last-child{border-bottom:0}
  .cart-item .ci-pic{width:60px;height:60px;border-radius:10px;background:#ffe4b3;display:flex;align-items:center;justify-content:center;font-size:2rem;overflow:hidden;flex-shrink:0}
  .cart-item .ci-pic img{width:100%;height:100%;object-fit:cover}
  .cart-item .ci-info{flex:1}
  .cart-item .ci-info h4{font-size:1rem;color:var(--green);margin-bottom:4px}
  .cart-item .ci-price{font-weight:700;color:var(--red);font-size:.95rem}
  .qty-controls{display:flex;align-items:center;gap:8px;background:#f3ede3;border-radius:20px;padding:2px 8px}
  .qty-controls button{background:transparent;border:0;font-size:1.2rem;font-weight:700;color:var(--dark);cursor:pointer;padding:0 4px}
  .qty-controls span{font-weight:700;font-size:.9rem;min-width:20px;text-align:center}
  .remove-btn{background:transparent;border:0;color:#ccc;font-size:1.2rem;cursor:pointer;transition:.2s}
  .remove-btn:hover{color:var(--red)}

  .qr-section{text-align:center;margin-top:20px;padding-top:20px;border-top:2px dashed #e5ddd0}
  .qr-section h4{color:var(--green);margin-bottom:12px}
  .qr-img{width:180px;height:180px;margin:0 auto 12px;border-radius:12px;border:3px solid var(--gold);padding:6px;background:#fff;object-fit:contain}
  .upi-box{background:#fff8ea;padding:10px;border-radius:10px;font-family:monospace;font-size:.95rem;display:inline-block;margin:6px 0;font-weight:600}
  .total-row{display:flex;justify-content:space-between;padding:14px 0;border-top:2px solid #e5ddd0;margin-top:14px;font-size:1.1rem;font-weight:700}
  .total-row .amt{color:var(--red);font-family:'Baloo 2',sans-serif;font-size:1.5rem}
  
  .success-box{text-align:center;padding:20px}
  .success-box .check{font-size:4rem;color:#25a244;margin-bottom:10px}
  .success-box h3{color:var(--green);margin-bottom:10px;font-size:1.5rem}
  .success-box .oid{background:#fff8ea;padding:8px 16px;border-radius:10px;font-family:monospace;font-size:.9rem;display:inline-block;margin:10px 0;font-weight:700}
  .success-box p{color:#7a6b5c;margin-bottom:16px}

  /* Admin Dashboard */
  .admin-tabs{display:flex;gap:6px;margin-bottom:20px;border-bottom:2px solid #f3ede3;overflow-x:auto}
  .admin-tab{padding:10px 18px;background:transparent;border:0;cursor:pointer;font-weight:600;font-size:.9rem;color:#7a6b5c;border-bottom:3px solid transparent;margin-bottom:-2px;transition:.2s;white-space:nowrap;font-family:inherit}
  .admin-tab.active{color:var(--green);border-bottom-color:var(--green)}
  .admin-tab:hover{color:var(--green)}
  .admin-panel{display:none}
  .admin-panel.active{display:block}
  .admin-header{display:flex;justify-content:space-between;align-items:center;margin-bottom:14px;gap:10px;flex-wrap:wrap}
  .admin-header h3{color:var(--green);font-size:1.15rem}
  .order-list{display:flex;flex-direction:column;gap:12px;max-height:60vh;overflow-y:auto;padding-right:6px}
  .order-item{background:#fff8ea;border:2px solid #f3ede3;border-radius:14px;padding:14px;transition:.2s}
  .order-item.delivered{background:#eef6ef;border-color:#c8e6cc}
  .order-item .ohead{display:flex;justify-content:space-between;align-items:flex-start;gap:10px;margin-bottom:8px;flex-wrap:wrap}
  .order-item .oname{font-weight:700;color:var(--dark);font-size:.95rem}
  .order-item .ostatus{font-size:.7rem;font-weight:700;padding:3px 10px;border-radius:20px;text-transform:uppercase;letter-spacing:.5px}
  .ostatus.pending{background:#fff3cd;color:#856404}
  .ostatus.delivered{background:#d4edda;color:#155724}
  .order-item .oinfo{font-size:.82rem;color:#6b5b4e;line-height:1.6}
  .order-item .oitems{background:#fff;padding:8px 10px;border-radius:8px;margin:8px 0;font-size:.8rem;color:#4a3a2c}
  .order-item .oactions{display:flex;gap:8px;margin-top:8px;flex-wrap:wrap}
  .product-admin-item{display:flex;justify-content:space-between;align-items:center;gap:10px;padding:12px;background:#fff8ea;border-radius:10px;margin-bottom:8px;border:1px solid #f3ede3}
  .product-admin-item .pai-info{flex:1;min-width:0}
  .product-admin-item .pai-name{font-weight:700;color:var(--dark);font-size:.9rem}
  .product-admin-item .pai-meta{font-size:.78rem;color:#7a6b5c}
  .product-admin-item .pai-actions{display:flex;gap:6px}
  .icon-btn{width:32px;height:32px;border-radius:8px;border:0;cursor:pointer;font-size:1rem;display:flex;align-items:center;justify-content:center;transition:.2s;background:#f3ede3;color:var(--dark)}
  .icon-btn:hover{background:var(--red);color:#fff}
  .icon-btn.edit:hover{background:var(--green)}
  .empty-state{text-align:center;padding:40px 20px;color:#7a6b5c}
  .empty-state .ico{font-size:3rem;margin-bottom:10px;opacity:.5}
  .toast{position:fixed;bottom:90px;left:50%;transform:translateX(-50%) translateY(100px);background:var(--dark);color:#fff;padding:12px 24px;border-radius:30px;font-size:.9rem;font-weight:600;box-shadow:0 8px 24px rgba(0,0,0,.3);z-index:999;transition:.3s;opacity:0}
  .toast.show{transform:translateX(-50%) translateY(0);opacity:1}
  .toast.error{background:var(--red)}
  .toast.success{background:#25a244}

  @media(max-width:768px){
    nav{display:none}
    .hero{padding:70px 0 80px}
    section{padding:50px 0}
    .contact .box{padding:28px 20px}
    .float{display:none}
    .form-row{grid-template-columns:1fr}
    .modal-box{padding:22px 18px}
  }
</style>
</head>
<body>

<header>
  <div class="container nav">
    <a href="#" class="logo">m<span>i</span>ndo</a>
    <nav>
      <a href="#products">Products</a>
      <a href="#why">Why Mindo</a>
      <a href="#testi">Reviews</a>
      <a href="#contact">Contact</a>
    </nav>
    <a class="btn green" href="https://wa.me/918383050500?text=Namaste%2C%20mujhe%20Mindo%20pickle%20order%20karna%20hai" target="_blank" rel="noopener">🛒 Order Now</a>
  </div>
</header>

<div class="hero">
  <span class="float f1">🌶️</span>
  <span class="float f2">🥭</span>
  <span class="float f3">🫙</span>
  <span class="float f4">🍋</span>
  <div class="container">
    <div class="tagline">🌿 शुद्ध सरसों तेल • 100% Homemade</div>
    <h1>घर जैसा स्वाद…</h1>
    <h2>दादी-नानी की याद दिलाए</h2>
    <p>शुद्ध सरसों तेल में बने, हाथों से तैयार, पारंपरिक अचार। न कोई केमिकल, न कोई प्रिज़र्वेटिव – सिर्फ़ प्यार और मसाले।</p>
    <a href="#products" class="btn">हमारे अचार देखें →</a>
  </div>
</div>

<div class="container badges">
  <div class="badge">🌿 100% Natural</div>
  <div class="badge">🚫 No Chemical Preservatives</div>
  <div class="badge">🏠 Homemade Traditional Taste</div>
  <div class="badge">☀️ Sun Dried in Barnis</div>
</div>

<section id="products">
  <div class="container">
    <div class="title">
      <div class="sub">Our Pickle Range</div>
      <h2>हमारे अचार</h2>
      <p>सभी अचार 450g जार में उपलब्ध • शुद्ध सरसों तेल में तैयार</p>
    </div>
    <div class="grid" id="productGrid">
      <div class="empty-state"><div class="ico">⏳</div>Loading products...</div>
    </div>
  </div>
</section>

<!-- Other sections remain same -->
<section class="why" id="why">
  <div class="container">
    <div class="title"><div class="sub">Why Choose Us</div><h2>Mindo क्यों?</h2></div>
    <div class="grid">
      <div class="item"><div class="ico">🫙</div><h4>शुद्ध सरसों तेल</h4><p>हर अचार शुद्ध सरसों तेल में बना।</p></div>
      <div class="item"><div class="ico">🌶️</div><h4>स्पेशल मसाले</h4><p>सौंफ, अजवाइन और राई से भरपूर।</p></div>
      <div class="item"><div class="ico">🧼</div><h4>Hygienically Handmade</h4><p>साफ़-सफ़ाई के साथ हाथों से तैयार।</p></div>
      <div class="item"><div class="ico">❤️</div><h4>दादी-नानी की याद</h4><p>वही पुराना घर जैसा स्वाद।</p></div>
    </div>
  </div>
</section>

<section class="ingr">
  <div class="container">
    <h2>🌾 Ingredients</h2>
    <p>Green Chilli, Iodised Salt, Mustard Oil, Red Chilli, Cumin, Saunf, Ajwain, Turmeric, Asafoetida, Black Pepper, Spices and Condiments.</p>
  </div>
</section>

<section class="testi" id="testi">
  <div class="container">
    <div class="title"><div class="sub">Happy Customers</div><h2>लोग क्या कहते हैं</h2></div>
    <div class="grid">
      <div class="tcard"><div class="quote">"</div><p>बिल्कुल घर जैसा स्वाद! लाल मिर्च का अचार तो कमाल का है – माँ के हाथ का याद आ गया।</p><div class="who"><div class="av">R</div><div><div class="nm">Rohit Sharma</div><div class="lo">Delhi</div></div></div></div>
      <div class="tcard"><div class="quote">"</div><p>मिक्स अचार में 9 रंगों का स्वाद – सच में unique! पूरे परिवार को पसंद आया।</p><div class="who"><div class="av">P</div><div><div class="nm">Priya Verma</div><div class="lo">Noida</div></div></div></div>
      <div class="tcard"><div class="quote">"</div><p>शुद्ध सरसों तेल की खुशबू से ही पता चल जाता है – असली अचार है। दोबारा ज़रूर मंगवाऊँगा।</p><div class="who"><div class="av">A</div><div><div class="nm">Amit Kumar</div><div class="lo">Gurgaon</div></div></div></div>
    </div>
  </div>
</section>

<section class="contact" id="contact">
  <div class="container">
    <div class="title"><div class="sub">Get In Touch</div><h2>Order / संपर्क करें</h2></div>
    <div class="box">
      <p><strong>📞 Order &amp; Feedback:</strong> <a href="tel:+918383050500">8383 0505 00</a></p>
      <p><strong>✉️ Email:</strong> <a href="mailto:sanatan.ent500@gmail.com">sanatan.ent500@gmail.com</a></p>
      <p><strong>📍 Address:</strong> Sanatan Enterprises, F Block, School Road, Khanpur, South Delhi – 110062</p>
      <span class="lic">✅ FSSAI Lic. No.: 23325002004226</span>
      <div class="btns">
        <a class="btn green" href="https://wa.me/918383050500" target="_blank" rel="noopener">💬 WhatsApp पर Order करें</a>
        <a class="btn" href="tel:+918383050500">📞 Call करें</a>
      </div>
    </div>
  </div>
</section>

<footer>
  <div class="container">
    <div class="brand">mindo</div>
    <div class="tag">घर जैसा स्वाद, हर जार में ❤️</div>
    <div>© <span id="yr"></span> Mindo – Manufactured &amp; Marketed by Sanatan Enterprises. All rights reserved.</div>
  </div>
</footer>

<!-- Floating Buttons -->
<a class="wa" href="https://wa.me/918383050500" target="_blank" rel="noopener" aria-label="WhatsApp">💬</a>
<div class="cart-btn-float" onclick="openCart()" title="View Cart">
  🛒
  <span class="cart-badge" id="cartBadge" style="display:none;">0</span>
</div>
<button class="admin-btn" onclick="openAdmin()" title="Admin Panel">⚙️</button>

<!-- Cart Modal -->
<div id="cartModal" class="modal">
  <div class="modal-box">
    <button class="modal-close" onclick="closeModal('cartModal')">×</button>
    <div id="cartContent"></div>
  </div>
</div>

<!-- Admin Modal -->
<div id="adminModal" class="modal">
  <div class="modal-box wide">
    <button class="modal-close" onclick="closeModal('adminModal')">×</button>
    <div id="adminContent"></div>
  </div>
</div>

<div id="toast" class="toast"></div>

<!-- Firebase SDKs -->
<script src="https://www.gstatic.com/firebasejs/9.23.0/firebase-app-compat.js"></script>
<script src="https://www.gstatic.com/firebasejs/9.23.0/firebase-database-compat.js"></script>
<script src="https://www.gstatic.com/firebasejs/9.23.0/firebase-auth-compat.js"></script>

<script>
/* ============================================================
   🔥 आपका FIREBASE CONFIG
   ============================================================ */
const firebaseConfig = {
  apiKey: "AIzaSyAKe_cHTWNYerJCo6drMPn2wOi59HJR8XQ",
  authDomain: "kapilmindo-3c257.firebaseapp.com",
  databaseURL: "https://kapilmindo-3c257-default-rtdb.firebaseio.com",
  projectId: "kapilmindo-3c257",
  storageBucket: "kapilmindo-3c257.firebasestorage.app",
  messagingSenderId: "280067203318",
  appId: "1:280067203318:web:98bd3da14eee3a2f900cd7",
  measurementId: "G-CHRK14YN6D"
};

const IMG_BASE = "./";
const PHONE = "918383050500";

/* ============================================================
   STATE & INIT
   ============================================================ */
let db = null;
let auth = null;
let firebaseReady = false;
let products = [];
let cart = JSON.parse(localStorage.getItem("mindo_cart")) || [];
let paymentSettings = { qrCode:"", upiId:"" };
let isAdmin = false;
let adminTab = "orders";
let showAllProducts = false;

async function init(){
  localStorage.removeItem("mindo_products");

  try {
    if (firebaseConfig.databaseURL && firebaseConfig.databaseURL !== "YOUR_DATABASE_URL"){
      firebase.initializeApp(firebaseConfig);
      db = firebase.database();
      auth = firebase.auth();
      firebaseReady = true;

      auth.onAuthStateChanged(user => {
        if (user) {
          isAdmin = true;
          if (document.getElementById("adminModal").classList.contains("active")) renderAdminDashboard();
        } else {
          isAdmin = false;
          if (document.getElementById("adminModal").classList.contains("active")) renderAdminLogin();
        }
      });
    }
  } catch(e){ console.warn("Firebase init failed:", e); }

  await loadProducts();
  await loadPaymentSettings();
  renderProducts();
  updateCartBadge();
  document.getElementById("yr").textContent = new Date().getFullYear();
}

/* ============================================================
   PRODUCTS
   ============================================================ */
async function loadProducts(){
  if (firebaseReady){
    try {
      const snapshot = await db.ref('products').once('value');
      const data = snapshot.val();
      products = data ? Object.keys(data).map(key => ({ id: key, ...data[key] })) : [];
    } catch(e){ products = []; }
  } else {
    const cached = localStorage.getItem("mindo_products_new");
    products = cached ? JSON.parse(cached) : [];
  }
}

function renderProducts(){
  const grid = document.getElementById("productGrid");
  
  if (!products.length){
    grid.innerHTML = '<div class="empty-state" style="grid-column: 1/-1;"><div class="ico">🫙</div>अभी कोई प्रोडक्ट नहीं है। कृपया एडमिन पैनल से प्रोडक्ट जोड़ें।</div>';
    return;
  }

  const displayProducts = showAllProducts ? products : products.slice(0, 5);

  let html = displayProducts.map((p) => {
    const imgUrl = p.img ? (p.img.startsWith("http") || p.img.startsWith("data:") ? p.img : IMG_BASE + p.img) : "";
    return `
      <div class="card">
        ${p.bestseller ? '<span class="ribbon">⭐ Bestseller</span>' : ''}
        <div class="pic">
          ${imgUrl ? `<img src="${imgUrl}" alt="${p.name}" loading="lazy" onerror="this.outerHTML='<span class=emoji>${p.emoji||"🫙"}</span>'">` : `<span class="emoji">${p.emoji||"🫙"}</span>`}
        </div>
        <div class="body">
          <h3>${p.name}</h3>
          <div class="hi">${p.hi||""}</div>
          <div class="tag">${p.tag||""}</div>
          <div class="row">
            <span class="price">₹${p.price}${p.mrp ? `<small>₹${p.mrp}</small>` : ''}</span>
            <span class="wt">450g</span>
          </div>
          <button class="btn green" onclick='addToCart(${JSON.stringify(p).replace(/'/g,"&#39;")})'>🛒 कार्ट में जोड़ें</button>
        </div>
      </div>`;
  }).join("");

  if (!showAllProducts && products.length > 5) {
    html += `
      <div class="card see-all-card" onclick="showAllProducts = true; renderProducts();">
        <div class="inner">
          <div class="plus">➕</div>
          <h3>See All Products</h3>
          <p style="color:#7a6b5c">देखें सभी ${products.length} प्रोडक्ट्स</p>
        </div>
      </div>`;
  }
  grid.innerHTML = html;
}

/* ============================================================
   CART FLOW
   ============================================================ */
function addToCart(p){
  const existing = cart.find(item => item.name === p.name);
  if(existing) {
    existing.qty += 1;
  } else {
    cart.push({ ...p, qty: 1 });
  }
  saveCart();
  updateCartBadge();
  toast("✅ कार्ट में जोड़ दिया गया!", "success");
}

function saveCart(){
  localStorage.setItem("mindo_cart", JSON.stringify(cart));
}

function updateCartBadge(){
  const badge = document.getElementById("cartBadge");
  const count = cart.reduce((sum, item) => sum + item.qty, 0);
  if(count > 0){
    badge.textContent = count;
    badge.style.display = "flex";
  } else {
    badge.style.display = "none";
  }
}

function updateQty(index, change){
  cart[index].qty += change;
  if(cart[index].qty <= 0){
    cart.splice(index, 1);
  }
  saveCart();
  updateCartBadge();
  renderCartContent();
}

function removeFromCart(index){
  cart.splice(index, 1);
  saveCart();
  updateCartBadge();
  renderCartContent();
}

function openCart(){
  document.getElementById("cartModal").classList.add("active");
  document.body.style.overflow = "hidden";
  renderCartContent();
}

function renderCartContent(){
  const c = document.getElementById("cartContent");
  
  if(cart.length === 0){
    c.innerHTML = `
      <h2>🛒 आपका कार्ट</h2>
      <div class="empty-state" style="padding:30px 10px">
        <div class="ico">🛒</div>
        <p>आपका कार्ट खाली है।</p>
        <button class="btn green" style="margin-top:15px" onclick="closeModal('cartModal')">प्रोडक्ट देखें</button>
      </div>`;
    return;
  }

  let itemsHtml = cart.map((item, index) => {
    const imgUrl = item.img ? (item.img.startsWith("http") || item.img.startsWith("data:") ? item.img : IMG_BASE + item.img) : "";
    return `
      <div class="cart-item">
        <div class="ci-pic">${imgUrl ? `<img src="${imgUrl}" alt="">` : (item.emoji||"🫙")}</div>
        <div class="ci-info">
          <h4>${item.name}</h4>
          <div class="ci-price">₹${item.price}</div>
        </div>
        <div class="qty-controls">
          <button onclick="updateQty(${index}, -1)">−</button>
          <span>${item.qty}</span>
          <button onclick="updateQty(${index}, 1)">+</button>
        </div>
        <button class="remove-btn" onclick="removeFromCart(${index})">×</button>
      </div>`;
  }).join("");

  const total = cart.reduce((sum, item) => sum + (item.price * item.qty), 0);
  
  const qrHtml = paymentSettings.qrCode
    ? `<div class="qr-section">
        <h4>💳 Payment / भुगतान</h4>
        <img src="${paymentSettings.qrCode}" alt="QR" class="qr-img">
        ${paymentSettings.upiId ? `<div>UPI ID: <span class="upi-box">${paymentSettings.upiId}</span></div>` : ""}
      </div>` : "";

  c.innerHTML = `
    <h2>🛒 आपका कार्ट</h2>
    <div style="max-height: 30vh; overflow-y:auto; padding-right:10px; margin-bottom:15px">
      ${itemsHtml}
    </div>
    
    <form id="cartOrderForm" onsubmit="submitCartOrder(event)">
      <div class="total-row" style="margin-top:0; padding-top:10px; border-top:2px dashed #e5ddd0">
        <span>Total:</span><span class="amt">₹${total}</span>
      </div>
      
      <div style="margin-top:15px" class="form-group"><label>आपका नाम *</label><input type="text" name="customerName" required placeholder="Full name"></div>
      <div class="form-row">
        <div class="form-group"><label>Phone *</label><input type="tel" name="phone" required pattern="[0-9]{10}" placeholder="10 digit mobile" maxlength="10"></div>
      </div>
      <div class="form-group"><label>पूरा Address *</label><textarea name="address" required placeholder="House, Street, Area, City, Pincode"></textarea></div>
      <div class="form-group"><label>Note (optional)</label><input type="text" name="note" placeholder="कोई special instruction"></div>
      
      ${qrHtml}
      
      <button type="submit" class="btn green" style="width:100%;margin-top:18px" id="submitCartBtn">✅ Order Place करें (₹${total})</button>
    </form>`;
}

async function submitCartOrder(e){
  e.preventDefault();
  const btn = document.getElementById("submitCartBtn");
  btn.disabled = true;
  btn.textContent = "⏳ Placing order...";

  const fd = new FormData(e.target);
  const total = cart.reduce((sum, item) => sum + (item.price * item.qty), 0);
  
  const orderData = {
    customerName: fd.get("customerName").trim(),
    phone: fd.get("phone").trim(),
    address: fd.get("address").trim(),
    note: fd.get("note").trim(),
    items: cart.map(item => ({ name: item.name, price: item.price, qty: item.qty, emoji: item.emoji||"🫙" })),
    total,
    status: "pending"
  };

  try {
    let orderId;
    if (firebaseReady){
      const ref = db.ref('orders').push();
      await ref.set({ ...orderData, createdAt: firebase.database.ServerValue.TIMESTAMP });
      orderId = ref.key.slice(-6).toUpperCase();
    } else {
      orderId = "LOCAL" + Date.now().toString().slice(-6);
      const orders = JSON.parse(localStorage.getItem("mindo_orders") || "[]");
      orders.push({ id: orderId, ...orderData, createdAt: Date.now() });
      localStorage.setItem("mindo_orders", JSON.stringify(orders));
    }

    const itemsString = cart.map(item => `${item.name} (x${item.qty})`).join(", ");
    const waMsg = encodeURIComponent(
      `Namaste Mindo! Order placed\n\n👤 ${orderData.customerName}\n📞 ${orderData.phone}\n📦 ${itemsString}\n💰 Total: ₹${total}\n📍 ${orderData.address}\n\nOrder ID: ${orderId}`
    );
    
    document.getElementById("cartContent").innerHTML = `
      <div class="success-box">
        <div class="check">✅</div>
        <h3>Order Place हो गया!</h3>
        <p>हम जल्द ही WhatsApp/Call पर confirm करेंगे।</p>
        <div class="oid">Order ID: ${orderId}</div>
        <p style="font-size:.85rem;margin-top:16px">Turant confirmation के लिए WhatsApp पर message भेजें:</p>
        <a class="btn green" href="https://wa.me/${PHONE}?text=${waMsg}" target="_blank" style="margin-top:8px;margin-bottom:10px">💬 WhatsApp पर Confirm करें</a>
        <button class="btn ghost" onclick="cart = []; saveCart(); updateCartBadge(); closeModal('cartModal'); renderProducts();">Continue Shopping</button>
      </div>`;
  } catch(err){
    console.error(err);
    toast("Order failed: " + err.message, "error");
    btn.disabled = false;
    btn.textContent = `✅ Order Place करें (₹${total})`;
  }
}

/* ============================================================
   PAYMENT SETTINGS
   ============================================================ */
async function loadPaymentSettings(){
  if (!firebaseReady) {
    const cached = localStorage.getItem("mindo_payment");
    if (cached) paymentSettings = JSON.parse(cached);
    return;
  }
  try {
    const snapshot = await db.ref('settings/payment').once('value');
    if (snapshot.exists()) paymentSettings = snapshot.val();
  } catch(e){ console.warn("Settings load failed:", e); }
}

/* ============================================================
   ADMIN PANEL (Auth & Logic)
   ============================================================ */
function openAdmin(){
  document.getElementById("adminModal").classList.add("active");
  document.body.style.overflow = "hidden";
  if (isAdmin) renderAdminDashboard();
  else renderAdminLogin();
}

function renderAdminLogin(){
  document.getElementById("adminContent").innerHTML = `
    <h2>🔐 Admin Login</h2>
    <p class="subtitle">कृपया अपना ईमेल और पासवर्ड डालें</p>
    <form onsubmit="adminLogin(event)">
      <div class="form-group">
        <label>Email</label>
        <input type="email" id="adminEmail" required placeholder="admin@example.com" autofocus>
      </div>
      <div class="form-group">
        <label>Password</label>
        <input type="password" id="adminPass" required placeholder="********">
      </div>
      <button type="submit" class="btn green" style="width:100%" id="loginBtn">Login</button>
    </form>`;
}

function adminLogin(e){
  e.preventDefault();
  const email = document.getElementById("adminEmail").value;
  const pass = document.getElementById("adminPass").value;
  const btn = document.getElementById("loginBtn");
  
  btn.disabled = true;
  btn.textContent = "⏳ Checking...";

  auth.signInWithEmailAndPassword(email, pass)
    .then(() => toast("Welcome, Admin! 👋", "success"))
    .catch(err => {
      toast("Login Failed: " + err.message, "error");
      btn.disabled = false;
      btn.textContent = "Login";
    });
}

function renderAdminDashboard(){
  const c = document.getElementById("adminContent");
  c.innerHTML = `
    <div class="admin-header">
      <h2>⚙️ Admin Dashboard</h2>
      <button class="btn ghost sm" onclick="adminLogout()">Logout</button>
    </div>
    <div class="admin-tabs">
      <button class="admin-tab ${adminTab==='orders'?'active':''}" onclick="switchTab('orders')">📦 Orders</button>
      <button class="admin-tab ${adminTab==='products'?'active':''}" onclick="switchTab('products')">🛍️ Products</button>
      <button class="admin-tab ${adminTab==='payment'?'active':''}" onclick="switchTab('payment')">💳 Payment</button>
    </div>
    <div id="adminPanel" class="admin-panel active"></div>`;
  renderAdminPanel();
}

function switchTab(tab){ adminTab = tab; renderAdminDashboard(); }

async function renderAdminPanel(){
  const panel = document.getElementById("adminPanel");
  if (adminTab === "orders") return renderOrdersPanel(panel);
  if (adminTab === "products") return renderProductsPanel(panel);
  if (adminTab === "payment") return renderPaymentPanel(panel);
}

/* ---- Orders Admin ---- */
async function renderOrdersPanel(panel){
  panel.innerHTML = `<div class="empty-state">⏳ Loading orders...</div>`;
  let orders = [];
  
  if (firebaseReady){
    try {
      const snapshot = await db.ref('orders').once('value');
      const data = snapshot.val() || {};
      orders = Object.keys(data).map(key => ({ id: key, ...data[key] }));
      orders.sort((a,b) => (b.createdAt || 0) - (a.createdAt || 0));
    } catch(e){ toast("Error loading orders.", "error"); }
  } else {
    orders = JSON.parse(localStorage.getItem("mindo_orders") || "[]");
    orders.reverse();
  }

  if (!orders.length){
    panel.innerHTML = `<div class="empty-state"><div class="ico">📭</div>अभी कोई order नहीं आया।</div>`;
    return;
  }

  const pending = orders.filter(o => o.status !== "delivered").length;
  panel.innerHTML = `
    <div class="admin-header">
      <h3>📦 Orders (${orders.length} total • ${pending} pending)</h3>
      <button class="btn sm" onclick="renderAdminPanel()">🔄 Refresh</button>
    </div>
    <div class="order-list">${orders.map(o => renderOrderCard(o)).join("")}</div>`;
}

function renderOrderCard(o){
  const date = new Date(o.createdAt || Date.now());
  const dateStr = date.toLocaleString("en-IN", { day:"2-digit", month:"short", year:"numeric", hour:"2-digit", minute:"2-digit" });
  const idShort = (o.id||"").slice(-6).toUpperCase();
  const itemsHtml = (o.items||[]).map(it => `🔸 ${it.name} × ${it.qty} = ₹${it.price*it.qty}`).join("<br>");
  const isDel = o.status === "delivered";

  return `
    <div class="order-item ${isDel?'delivered':''}">
      <div class="ohead">
        <div>
          <div class="oname">${o.customerName} • #${idShort}</div>
          <div class="oinfo">📞 ${o.phone} &nbsp;•&nbsp; ${dateStr}</div>
        </div>
        <span class="ostatus ${o.status||'pending'}">${o.status||'pending'}</span>
      </div>
      <div class="oitems">${itemsHtml}</div>
      <div class="oinfo">📍 ${o.address}${o.note ? `<br>📝 ${o.note}` : ""}</div>
      <div class="oinfo" style="margin-top:6px;font-weight:700;color:var(--red)">Total: ₹${o.total}</div>
      <div class="oactions">
        ${!isDel ? `<button class="btn green sm" onclick="markDelivered('${o.id}')">✅ Mark Delivered</button>` : `<button class="btn ghost sm" onclick="markPending('${o.id}')">↩ Undo</button>`}
        <a class="btn ghost sm" href="https://wa.me/91${o.phone}?text=${encodeURIComponent('Namaste '+o.customerName+', your Mindo order #'+idShort+' is confirmed!')}" target="_blank">💬 WhatsApp</a>
        <a class="btn ghost sm" href="tel:${o.phone}">📞 Call</a>
      </div>
    </div>`;
}

async function markDelivered(id){
  try {
    if (firebaseReady){
      await db.ref('orders/' + id).update({ status:"delivered", deliveredAt: firebase.database.ServerValue.TIMESTAMP });
    } else {
      const orders = JSON.parse(localStorage.getItem("mindo_orders") || "[]");
      const o = orders.find(x => x.id === id);
      if (o) o.status = "delivered";
      localStorage.setItem("mindo_orders", JSON.stringify(orders));
    }
    toast("✅ Marked delivered", "success");
    renderAdminPanel();
  } catch(e){ toast("Failed: " + e.message, "error"); }
}

async function markPending(id){
  try {
    if (firebaseReady){
      await db.ref('orders/' + id).update({ status:"pending" });
    } else {
      const orders = JSON.parse(localStorage.getItem("mindo_orders") || "[]");
      const o = orders.find(x => x.id === id);
      if (o) o.status = "pending";
      localStorage.setItem("mindo_orders", JSON.stringify(orders));
    }
    toast("↩ Marked pending");
    renderAdminPanel();
  } catch(e){ toast("Failed: " + e.message, "error"); }
}

/* ---- Products Admin ---- */
function renderProductsPanel(panel){
  panel.innerHTML = `
    <div class="admin-header">
      <h3>🛍️ Products (${products.length})</h3>
      <div style="display:flex;gap:8px;flex-wrap:wrap">
        <button class="btn green sm" onclick="openProductForm()">➕ Add Product</button>
      </div>
    </div>
    ${products.length ? products.map((p,i) => `
      <div class="product-admin-item">
        <div class="pai-info">
          <div class="pai-name">${p.emoji||""} ${p.name}</div>
          <div class="pai-meta">₹${p.price}${p.mrp ? ` (MRP ₹${p.mrp})` : ""} ${p.bestseller ? "• ⭐ Bestseller" : ""}</div>
        </div>
        <div class="pai-actions">
          <button class="icon-btn edit" onclick="openProductForm(${i})" title="Edit">✏️</button>
          <button class="icon-btn" onclick="deleteProduct(${i})" title="Delete">🗑️</button>
        </div>
      </div>`).join("") : '<div class="empty-state"><div class="ico">📦</div>कोई product नहीं है।</div>'}
    <div id="productFormArea"></div>`;
}

function openProductForm(index = -1){
  const p = index >= 0 ? products[index] : { name:"", hi:"", tag:"", price:0, mrp:0, emoji:"🫙", img:"", bestseller:false };
  
  let imgPreview = "";
  if (p.img) {
    const imgUrl = p.img.startsWith("http") || p.img.startsWith("data:") ? p.img : IMG_BASE + p.img;
    imgPreview = `<img src="${imgUrl}" style="max-height:100px;border-radius:8px;margin-top:10px;border:1px solid #ddd">`;
  }

  document.getElementById("productFormArea").innerHTML = `
    <div style="background:#fff8ea;padding:16px;border-radius:12px;margin-top:14px;border:2px solid var(--gold)">
      <h4 style="color:var(--green);margin-bottom:12px">${index>=0?'✏️ Edit':'➕ Add'} Product</h4>
      <form onsubmit="saveProduct(event, ${index})">
        <div class="form-group"><label>Name *</label><input name="name" required value="${p.name||''}"></div>
        <div class="form-group"><label>Hindi Name</label><input name="hi" value="${p.hi||''}"></div>
        <div class="form-group"><label>Description</label><input name="tag" value="${p.tag||''}"></div>
        <div class="form-row">
          <div class="form-group"><label>Price *</label><input type="number" name="price" required value="${p.price||''}"></div>
          <div class="form-group"><label>MRP</label><input type="number" name="mrp" value="${p.mrp||''}"></div>
        </div>
        <div class="form-row">
          <div class="form-group"><label>Emoji (Fallback)</label><input name="emoji" value="${p.emoji||'🫙'}" maxlength="4"></div>
          <div class="form-group">
            <label>Image Upload</label>
            <input type="file" accept="image/*" onchange="handleImageUpload(event)" style="padding:6px">
            <input type="hidden" name="img" id="imgBase64Input" value="${p.img||''}">
          </div>
        </div>
        <div id="imagePreview" style="margin-bottom:10px">${imgPreview}</div>
        <div class="form-group"><label><input type="checkbox" name="bestseller" ${p.bestseller?'checked':''}> ⭐ Bestseller</label></div>
        <div style="display:flex;gap:8px">
          <button type="submit" class="btn green sm">Save</button>
          <button type="button" class="btn ghost sm" onclick="document.getElementById('productFormArea').innerHTML=''">Cancel</button>
        </div>
      </form>
    </div>`;
}

function handleImageUpload(e) {
  const file = e.target.files[0];
  if (!file) return;
  
  const reader = new FileReader();
  reader.onload = function(event) {
    const img = new Image();
    img.onload = function() {
      const canvas = document.createElement('canvas');
      const MAX_WIDTH = 500;
      const scaleSize = MAX_WIDTH / img.width;
      canvas.width = MAX_WIDTH;
      canvas.height = img.height * scaleSize;
      const ctx = canvas.getContext('2d');
      ctx.drawImage(img, 0, 0, canvas.width, canvas.height);
      
      const base64String = canvas.toDataURL('image/jpeg', 0.7);
      
      document.getElementById('imgBase64Input').value = base64String;
      document.getElementById('imagePreview').innerHTML = `<img src="${base64String}" style="max-height:100px;border-radius:8px;margin-top:10px;border:1px solid #ddd">`;
    }
    img.src = event.target.result;
  }
  reader.readAsDataURL(file);
}

async function saveProduct(e, index){
  e.preventDefault();
  const fd = new FormData(e.target);
  const data = {
    name: fd.get("name").trim(),
    hi: fd.get("hi").trim(),
    tag: fd.get("tag").trim(),
    price: parseInt(fd.get("price")),
    mrp: parseInt(fd.get("mrp")) || null,
    emoji: fd.get("emoji").trim() || "🫙",
    img: fd.get("img").trim(),
    bestseller: fd.get("bestseller") === "on"
  };

  try {
    if (firebaseReady){
      if (index >= 0 && products[index].id){
        await db.ref('products/' + products[index].id).update(data);
      } else {
        await db.ref('products').push({ ...data, createdAt: firebase.database.ServerValue.TIMESTAMP });
      }
    }
    
    if (index >= 0) products[index] = { ...products[index], ...data };
    else products.push({ id:"local_"+Date.now(), ...data });
    
    localStorage.setItem("mindo_products_new", JSON.stringify(products));
    toast("✅ Saved", "success");
    renderProducts();
    renderAdminPanel();
  } catch(err){ toast("Save failed: " + err.message, "error"); }
}

async function deleteProduct(index){
  if (!confirm("Delete product '" + products[index].name + "'?")) return;
  try {
    if (firebaseReady && products[index].id && !products[index].id.startsWith("local_")){
      await db.ref('products/' + products[index].id).remove();
    }
    products.splice(index, 1);
    localStorage.setItem("mindo_products_new", JSON.stringify(products));
    toast("🗑️ Deleted");
    renderProducts();
    renderAdminPanel();
  } catch(err){ toast("Delete failed: " + err.message, "error"); }
}

/* ---- Payment Admin ---- */
function renderPaymentPanel(panel){
  panel.innerHTML = `
    <div class="admin-header"><h3>💳 Payment Settings</h3></div>
    <div style="background:#fff8ea;padding:20px;border-radius:14px;border:2px solid var(--gold)">
      <div class="form-group">
        <label>UPI ID</label>
        <input id="upiIdInput" value="${paymentSettings.upiId||''}" placeholder="e.g. 8383050500@ybl">
      </div>
      <div class="form-group">
        <label>QR Code Image</label>
        <input type="file" accept="image/*" id="qrFile" onchange="handleQrUpload(event)">
        ${paymentSettings.qrCode ? `<div style="margin-top:12px;text-align:center"><img src="${paymentSettings.qrCode}" style="max-width:180px;border-radius:12px;border:2px solid var(--gold)"></div>` : ""}
      </div>
      <button class="btn green" onclick="saveUpi()" style="width:100%">💾 Save UPI ID</button>
    </div>`;
}

async function handleQrUpload(e){
  const file = e.target.files[0];
  if (!file) return;
  if (file.size > 500 * 1024){ toast("Image too large (max 500KB)", "error"); return; }
  const reader = new FileReader();
  reader.onload = async (ev) => {
    try {
      const qrCode = ev.target.result;
      if (firebaseReady){
        await db.ref('settings/payment').update({ qrCode, updatedAt: firebase.database.ServerValue.TIMESTAMP });
      }
      paymentSettings.qrCode = qrCode;
      localStorage.setItem("mindo_payment", JSON.stringify(paymentSettings));
      toast("✅ QR saved", "success");
      renderAdminPanel();
    } catch(err){ toast("Upload failed: " + err.message, "error"); }
  };
  reader.readAsDataURL(file);
}

async function saveUpi(){
  const upiId = document.getElementById("upiIdInput").value.trim();
  try {
    if (firebaseReady){
      await db.ref('settings/payment').update({ upiId, updatedAt: firebase.database.ServerValue.TIMESTAMP });
    }
    paymentSettings.upiId = upiId;
    localStorage.setItem("mindo_payment", JSON.stringify(paymentSettings));
    toast("✅ UPI ID saved", "success");
  } catch(err){ toast("Save failed: " + err.message, "error"); }
}

function adminLogout(){
  auth.signOut().then(() => {
    closeModal("adminModal");
    toast("Logged out securely");
  });
}

/* ============================================================
   UTILS
   ============================================================ */
function closeModal(id){
  document.getElementById(id).classList.remove("active");
  document.body.style.overflow = "";
}

function toast(msg, type = ""){
  const t = document.getElementById("toast");
  t.textContent = msg;
  t.className = "toast " + type + " show";
  clearTimeout(t._timer);
  t._timer = setTimeout(() => t.classList.remove("show"), 3000);
}

document.querySelectorAll(".modal").forEach(m => {
  m.addEventListener("click", e => { if (e.target === m) closeModal(m.id); });
});

// Start
init();
</script>
</body>
</html>
