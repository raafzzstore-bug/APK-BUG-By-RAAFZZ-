# APK-BUG-By-RAAFZZ-
LIST BUG &amp; APK BUG
<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>RAAFZZ STORE</title>

<style>
:root{
  --bg:#06070c;
  --card:#10131c;
  --card2:#0c0f16;
  --border:#252a3a;
  --text:#f5f7ff;
  --muted:#929bb1;
  --purple:#765cff;
  --cyan:#00d9ff;
}

*{
  box-sizing:border-box;
  margin:0;
  padding:0;
}

html{
  scroll-behavior:smooth;
}

body{
  font-family:Arial,Helvetica,sans-serif;
  color:var(--text);
  background:
    radial-gradient(circle at 10% 0%,#21134b 0,transparent 30%),
    radial-gradient(circle at 90% 20%,#063e4c 0,transparent 25%),
    var(--bg);
  min-height:100vh;
}

a{
  text-decoration:none;
  color:inherit;
}

.container{
  width:min(1150px,92%);
  margin:auto;
}

/* NAVBAR */

header{
  position:sticky;
  top:0;
  z-index:100;
  background:rgba(6,7,12,.82);
  backdrop-filter:blur(18px);
  border-bottom:1px solid rgba(255,255,255,.07);
}

.navbar{
  height:70px;
  display:flex;
  justify-content:space-between;
  align-items:center;
}

.logo{
  font-size:21px;
  font-weight:900;
  letter-spacing:1px;
}

.logo span{
  color:var(--cyan);
}

.nav-links{
  display:flex;
  gap:25px;
  color:var(--muted);
  font-size:14px;
}

.nav-links a:hover{
  color:white;
}

/* HERO */

.hero{
  text-align:center;
  padding:80px 0 45px;
}

.badge{
  display:inline-block;
  padding:8px 14px;
  border-radius:50px;
  background:#15112b;
  border:1px solid #393061;
  color:#bcb0ff;
  font-size:12px;
  font-weight:bold;
}

.hero h1{
  font-size:clamp(42px,8vw,78px);
  line-height:.95;
  letter-spacing:-4px;
  margin:22px auto;
  max-width:850px;
}

.gradient{
  background:linear-gradient(
    90deg,
    #ffffff,
    #927eff,
    #00ddff
  );
  -webkit-background-clip:text;
  color:transparent;
}

.hero p{
  max-width:650px;
  margin:auto;
  color:var(--muted);
  line-height:1.7;
}

.hero-buttons{
  display:flex;
  justify-content:center;
  gap:12px;
  flex-wrap:wrap;
  margin-top:28px;
}

.btn{
  display:inline-flex;
  align-items:center;
  justify-content:center;
  padding:13px 18px;
  border-radius:12px;
  font-weight:bold;
  border:1px solid var(--border);
  transition:.2s;
}

.btn:hover{
  transform:translateY(-2px);
}

.primary{
  background:linear-gradient(135deg,var(--purple),#4b3ce4);
  border:0;
}

.secondary{
  background:#10131b;
}

/* SEARCH */

.section-title{
  margin:40px 0 18px;
}

.section-title h2{
  font-size:30px;
}

.section-title p{
  color:var(--muted);
  margin-top:5px;
  font-size:13px;
}

.tools{
  display:flex;
  gap:10px;
  margin-bottom:22px;
}

.search{
  flex:1;
  padding:15px;
  border-radius:12px;
  border:1px solid var(--border);
  background:#0d1017;
  color:white;
  outline:none;
}

.filter{
  padding:12px;
  border-radius:12px;
  border:1px solid var(--border);
  background:#0d1017;
  color:white;
}

/* PRODUCTS */

.products{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:18px;
}

.card{
  position:relative;
  overflow:hidden;
  padding:20px;
  border-radius:20px;
  border:1px solid var(--border);
  background:linear-gradient(
    180deg,
    var(--card),
    var(--card2)
  );
  box-shadow:0 15px 45px rgba(0,0,0,.25);
}

.card::before{
  content:"";
  position:absolute;
  width:150px;
  height:150px;
  left:-80px;
  top:-80px;
  background:var(--purple);
  filter:blur(70px);
  opacity:.15;
}

.tag{
  display:inline-block;
  padding:6px 9px;
  background:#191d2a;
  color:#aeb7d1;
  border-radius:7px;
  font-size:10px;
  font-weight:bold;
  margin-bottom:12px;
}

.card h3{
  font-size:22px;
  margin-bottom:8px;
}

.description{
  color:var(--muted);
  font-size:13px;
  line-height:1.5;
  min-height:40px;
}

.price-list{
  display:grid;
  gap:8px;
  margin:17px 0;
}

.price{
  display:flex;
  justify-content:space-between;
  align-items:center;
  padding:11px;
  border-radius:10px;
  background:#090c12;
  border:1px solid #202534;
  font-size:13px;
}

.price span{
  color:#7beaff;
  font-weight:bold;
}

.order{
  width:100%;
  background:linear-gradient(
    135deg,
    #00b9df,
    #665aff
  );
  border:0;
}

/* FEATURES */

.features{
  display:grid;
  grid-template-columns:repeat(4,1fr);
  gap:12px;
  margin-top:25px;
}

.feature{
  padding:18px;
  border-radius:15px;
  border:1px solid var(--border);
  background:#0d1017;
}

.feature h4{
  margin-bottom:7px;
}

.feature p{
  color:var(--muted);
  font-size:12px;
  line-height:1.5;
}

/* RECOMMENDATION */

.recommend{
  margin-top:20px;
  padding:20px;
  border:1px solid #2b3150;
  border-radius:18px;
  background:linear-gradient(
    100deg,
    #14172a,
    #0d111b
  );
  display:flex;
  justify-content:space-between;
  align-items:center;
  gap:15px;
}

.recommend p{
  color:var(--muted);
  font-size:12px;
  margin-top:5px;
}

/* EMPTY */

.empty{
  display:none;
  text-align:center;
  padding:30px;
  color:var(--muted);
  border:1px dashed var(--border);
  border-radius:15px;
}

/* FOOTER */

footer{
  margin-top:60px;
  border-top:1px solid var(--border);
  padding:30px 0;
  color:var(--muted);
  font-size:13px;
}

.footer{
  display:flex;
  justify-content:space-between;
  gap:15px;
  flex-wrap:wrap;
}

.note{
  margin-top:25px;
  text-align:center;
  color:#747d91;
  font-size:11px;
  line-height:1.6;
}

/* MOBILE */

@media(max-width:850px){

  .products{
    grid-template-columns:1fr 1fr;
  }

  .features{
    grid-template-columns:1fr 1fr;
  }

  .nav-links{
    display:none;
  }

}

@media(max-width:560px){

  .hero{
    padding-top:55px;
  }

  .hero h1{
    font-size:48px;
    letter-spacing:-2px;
  }

  .tools{
    flex-direction:column;
  }

  .products{
    grid-template-columns:1fr;
  }

  .features{
    grid-template-columns:1fr;
  }

  .recommend{
    flex-direction:column;
    align-items:flex-start;
  }

}
</style>
</head>

<body>

<!-- NAVBAR -->

<header>
  <div class="container navbar">

    <div class="logo">
      RAAFZZ<span> STORE</span>
    </div>

    <nav class="nav-links">
      <a href="#produk">Produk</a>
      <a href="#fitur">Fitur</a>
      <a href="#kontak">Kontak</a>
    </nav>

  </div>
</header>


<main class="container">

<!-- HERO -->

<section class="hero">

  <span class="badge">
    ⚡ DIGITAL TOOLS STORE
  </span>

  <h1>
    Temukan
    <span class="gradient">Tools</span>
    yang kamu butuhkan.
  </h1>

  <p>
    Selamat datang di RAAFZZ STORE.
    Jelajahi berbagai produk digital,
    pilih paket yang tersedia, dan hubungi
    admin untuk melakukan pemesanan.
  </p>

  <div class="hero-buttons">

    <a href="#produk" class="btn primary">
      🛒 Lihat Produk
    </a>

    <a
      href="https://t.me/raafzzstore"
      target="_blank"
      class="btn secondary"
    >
      ✈️ Telegram
    </a>

  </div>

</section>


<!-- PRODUK -->

<section id="produk">

  <div class="section-title">

    <h2>Produk</h2>

    <p>
      Pilih produk dan paket yang tersedia.
    </p>

  </div>


  <!-- SEARCH -->

  <div class="tools">

    <input
      id="search"
      class="search"
      type="search"
      placeholder="🔎 Cari produk atau paket..."
    >

    <select id="filter" class="filter">

      <option value="all">
        Semua Produk
      </option>

      <option value="blue">
        BLUE SHARK
      </option>

      <option value="just">
        JUSTKIDZ
      </option>

      <option value="mur">
        MURBUG FlyXcrasher
      </option>

    </select>

  </div>


  <div class="products" id="products">


    <!-- BLUE SHARK -->

    <article
      class="card product"
      data-type="blue"
      data-name="blue shark"
    >

      <span class="tag">
        🔥 POPULAR
      </span>

      <h3>
        BLUE SHARK
      </h3>

      <p class="description">
        Pilihan paket BLUE SHARK dengan
        berbagai durasi dan role.
      </p>


      <div class="price-list">

        <div class="price">
          <b>1K</b>
          <span>3 day</span>
        </div>

        <div class="price">
          <b>3K</b>
          <span>7 day</span>
        </div>

        <div class="price">
          <b>6K</b>
          <span>30 day</span>
        </div>

        <div class="price">
          <b>8K</b>
          <span>Permanent</span>
        </div>

        <div class="price">
          <b>RESELLER</b>
          <span>10K</span>
        </div>

        <div class="price">
          <b>VIP</b>
          <span>12K</span>
        </div>

        <div class="price">
          <b>ADMIN</b>
          <span>15K</span>
        </div>

        <div class="price">
          <b>PARTNER</b>
          <span>20K</span>
        </div>

        <div class="price">
          <b>MODERATOR</b>
          <span>25K</span>
        </div>

        <div class="price">
          <b>OWNER</b>
          <span>35K</span>
        </div>

      </div>


      <a
        href="#"
        class="btn order"
        onclick="order('BLUE SHARK');return false;"
      >
        💬 Pesan via WhatsApp
      </a>

    </article>



    <!-- JUSTKIDZ -->

    <article
      class="card product"
      data-type="just"
      data-name="justkidz"
    >

      <span class="tag">
        ✨ FEATURED
      </span>

      <h3>
        JUSTKIDZ
      </h3>

      <p class="description">
        Pilihan paket JUSTKIDZ dengan
        berbagai durasi dan role.
      </p>


      <div class="price-list">

        <div class="price">
          <b>1K</b>
          <span>3 day</span>
        </div>

        <div class="price">
          <b>3K</b>
          <span>7 day</span>
        </div>

        <div class="price">
          <b>6K</b>
          <span>30 day</span>
        </div>

        <div class="price">
          <b>8K</b>
          <span>Permanent</span>
        </div>

        <div class="price">
          <b>RESELLER</b>
          <span>10K</span>
        </div>

        <div class="price">
          <b>VIP</b>
          <span>12K</span>
        </div>

        <div class="price">
          <b>ADMIN</b>
          <span>15K</span>
        </div>

        <div class="price">
          <b>PARTNER</b>
          <span>20K</span>
        </div>

        <div class="price">
          <b>MODERATOR</b>
          <span>25K</span>
        </div>

        <div class="price">
          <b>OWNER</b>
          <span>35K</span>
        </div>

      </div>


      <a
        href="#"
        class="btn order"
        onclick="order('JUSTKIDZ');return false;"
      >
        💬 Pesan via WhatsApp
      </a>

    </article>



    <!-- MURBUG -->

    <article
      class="card product"
      data-type="mur"
      data-name="murbug flyxcrasher murbug"
    >

      <span class="tag">
        ⚡ SPECIAL
      </span>

      <h3>
        MURBUG FlyXcrasher
      </h3>

      <p class="description">
        Paket digital dengan pilihan
        permanent dan role khusus.
      </p>


      <div class="price-list">

        <div class="price">
          <b>4K</b>
          <span>Permanent</span>
        </div>

        <div class="price">
          <b>RESELLER</b>
          <span>8K</span>
        </div>

        <div class="price">
          <b>PARTNER</b>
          <span>15K</span>
        </div>

        <div class="price">
          <b>TK</b>
          <span>20K</span>
        </div>

        <div class="price">
          <b>OWNER</b>
          <span>30K</span>
        </div>

        <div class="price">
          <b>UPDATE</b>
          <span>FREE ALL UPDATE</span>
        </div>

      </div>


      <a
        href="#"
        class="btn order"
        onclick="order('MURBUG FlyXcrasher');return false;"
      >
        💬 Pesan via WhatsApp
      </a>

    </article>

  </div>


  <div id="empty" class="empty">
    Produk tidak ditemukan.
  </div>

</section>



<!-- FITUR -->

<section id="fitur">

  <div class="section-title">

    <h2>
      Fitur Store
    </h2>

    <p>
      Dibuat sederhana dan nyaman digunakan.
    </p>

  </div>


  <div class="features">

    <div class="feature">

      <h4>
        🔎 Pencarian
      </h4>

      <p>
        Cari produk atau paket
        dengan cepat.
      </p>

    </div>


    <div class="feature">

      <h4>
        ⭐ Rekomendasi
      </h4>

      <p>
        Produk unggulan ditampilkan
        dengan label khusus.
      </p>

    </div>


    <div class="feature">

      <h4>
        📱 Responsive
      </h4>

      <p>
        Tampilan menyesuaikan
        HP, tablet, dan desktop.
      </p>

    </div>


    <div class="feature">

      <h4>
        💬 Order Cepat
      </h4>

      <p>
        Pesanan langsung diarahkan
        ke WhatsApp admin.
      </p>

    </div>

  </div>



  <!-- CONTACT -->

  <div class="recommend" id="kontak">

    <div>

      <strong>
        Butuh bantuan memilih paket?
      </strong>

      <p>
        Hubungi admin RAAFZZ STORE.
      </p>

    </div>


    <a
      href="https://wa.me/6283116013787"
      target="_blank"
      class="btn primary"
    >
      Chat WhatsApp
    </a>

  </div>


  <div class="hero-buttons">

    <a
      href="https://t.me/raafzzstore"
      target="_blank"
      class="btn secondary"
    >
      ✈️ Telegram @raafzzstore
    </a>

  </div>


  <div class="note">
    Gunakan produk digital hanya untuk penggunaan
    yang sah dan tidak mengganggu perangkat atau
    akun pihak lain.
  </div>

</section>

</main>



<!-- FOOTER -->

<footer>

  <div class="container footer">

    <div>
      © 2026 RAAFZZ STORE
    </div>

    <div>
      WhatsApp: 6283116013787
      · Telegram: @raafzzstore
    </div>

  </div>

</footer>



<script>

const whatsappNumber = "6283116013787";


/* ORDER WHATSAPP */

function order(product){

  const message =
    "Halo RAAFZZ STORE, saya ingin memesan " +
    product +
    ". Mohon info paket dan cara pembayarannya.";

  const url =
    "https://wa.me/" +
    whatsappNumber +
    "?text=" +
    encodeURIComponent(message);

  window.open(url,"_blank");

}



/* SEARCH & FILTER */

const search =
  document.getElementById("search");

const filter =
  document.getElementById("filter");

const products =
  [...document.querySelectorAll(".product")];

const empty =
  document.getElementById("empty");


function renderProducts(){

  const keyword =
    search.value
      .toLowerCase()
      .trim();

  const selected =
    filter.value;

  let visible = 0;


  products.forEach(product => {

    const name =
      product.dataset.name
        .toLowerCase();

    const type =
      product.dataset.type;


    const matchesSearch =
      name.includes(keyword);

    const matchesFilter =
      selected === "all" ||
      selected === type;


    if(
      matchesSearch &&
      matchesFilter
    ){

      product.style.display =
        "block";

      visible++;

    }else{

      product.style.display =
        "none";

    }

  });


  empty.style.display =
    visible === 0
      ? "block"
      : "none";

}


search.addEventListener(
  "input",
  renderProducts
);

filter.addEventListener(
  "change",
  renderProducts
);

</script>

</body>
</html>
