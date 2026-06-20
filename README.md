<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>ONB Media | Cinematic Stories</title>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&display=swap" rel="stylesheet">

<style>
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
  font-family:'Inter',sans-serif;
}

body{
  background:#0a0a0f;
  color:#fff;
  overflow-x:hidden;
}

/* ===== INTRO ===== */
.intro{
  position:fixed;
  width:100%;
  height:100vh;
  background:black;
  display:flex;
  flex-direction:column;
  justify-content:center;
  align-items:center;
  z-index:9999;
  animation:fadeOut 1s ease forwards;
  animation-delay:3s;
}

.intro h1{
  font-size:55px;
  letter-spacing:6px;
  animation:zoom 2s ease;
}

.intro span{
  color:#ff2e63;
}

.intro p{
  color:#777;
  margin-top:10px;
}

@keyframes zoom{
  from{transform:scale(0.7);opacity:0;}
  to{transform:scale(1);opacity:1;}
}

@keyframes fadeOut{
  to{opacity:0;visibility:hidden;}
}

/* ===== HERO ===== */
.hero{
  height:100vh;
  display:flex;
  flex-direction:column;
  justify-content:center;
  align-items:center;
  text-align:center;
  background: radial-gradient(circle at top,#1a1a2e,#0a0a0f);
  padding:20px;
}

.hero h1{
  font-size:65px;
  font-weight:800;
}

.hero p{
  max-width:650px;
  margin-top:15px;
  color:#aaa;
  font-size:18px;
}

.glow{ color:#ff2e63; }

.btns{
  margin-top:30px;
  display:flex;
  flex-wrap:wrap;
  gap:12px;
  justify-content:center;
}

.btn{
  padding:12px 18px;
  border-radius:30px;
  border:1px solid #333;
  text-decoration:none;
  color:white;
  transition:0.3s;
}

.btn:hover{
  transform:scale(1.08);
  border-color:#ff2e63;
  box-shadow:0 0 20px #ff2e63;
}

/* ===== SECTION BASE ===== */
.section{
  padding:80px 20px;
}

.section h2{
  text-align:center;
  font-size:32px;
  margin-bottom:30px;
}

/* ===== FEATURED VIDEO ===== */
.video{
  max-width:900px;
  margin:auto;
  border-radius:18px;
  overflow:hidden;
  box-shadow:0 0 40px rgba(255,46,99,0.2);
}

.video iframe{
  width:100%;
  height:480px;
}

/* ===== ABOUT ===== */
.card{
  max-width:900px;
  margin:auto;
  background:#141422;
  padding:30px;
  border-radius:15px;
  color:#bbb;
  line-height:1.6;
}

/* ===== UPDATES (DYNAMIC AREA) ===== */
.updates-grid{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
  gap:20px;
  max-width:1100px;
  margin:auto;
}

.update-card{
  background:#141422;
  padding:20px;
  border-radius:15px;
  border:1px solid #222;
  transition:0.3s;
}

.update-card:hover{
  transform:translateY(-5px);
  border-color:#ff2e63;
}

.update-card h3{
  color:#ff2e63;
  margin-bottom:10px;
}

.update-card p{
  color:#aaa;
  font-size:14px;
}

/* ADD NEW UPDATE BOX */
.add-box{
  max-width:900px;
  margin:40px auto;
  background:#111;
  padding:20px;
  border-radius:15px;
  border:1px dashed #444;
}

.add-box input,
.add-box textarea{
  width:100%;
  margin-bottom:10px;
  padding:10px;
  background:#0a0a0f;
  border:1px solid #333;
  color:white;
  border-radius:8px;
}

.add-box button{
  padding:10px 20px;
  background:#ff2e63;
  border:none;
  color:white;
  border-radius:30px;
  cursor:pointer;
}

/* ===== FOOTER ===== */
footer{
  text-align:center;
  padding:40px;
  color:#777;
  border-top:1px solid #222;
}
</style>
</head>

<body>

<!-- INTRO -->
<div class="intro">
  <h1>ONB <span>MEDIA</span></h1>
  <p>Cinematic storytelling loading...</p>
</div>

<!-- HERO -->
<section class="hero">
  <h1>ONB <span class="glow">MEDIA</span></h1>
  <p>We create cinematic news, real voices, youth stories, and documentary-style digital media from Kenya to the world.</p>

  <div class="btns">
    <a class="btn" href="https://youtube.com/@atvkenya?si=pgx3uVAAm-wDMfHa">YouTube</a>
    <a class="btn" href="https://www.facebook.com/profile.php?id=61590682448775">Facebook</a>
    <a class="btn" href="https://www.instagram.com/observerx001?igsh=OGtmNTNjb2JqdGd1">Instagram</a>
    <a class="btn" href="https://www.tiktok.com/@onenarrativebrand?_r=1&_t=ZS-97MimsInQFb">TikTok</a>
    <a class="btn" href="https://wa.me/254117269158">WhatsApp</a>
  </div>
</section>

<!-- ABOUT -->
<section class="section">
  <h2>About ONB Media</h2>
  <div class="card">
    ONB Media is a modern cinematic media brand focused on storytelling, interviews, youth culture, and impactful visual journalism. We combine film-style production with real-world narratives.
  </div>
</section>

<!-- FEATURED VIDEO -->
<section class="section">
  <h2>Featured Story</h2>
  <div class="video">
    <iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ" allowfullscreen></iframe>
  </div>
</section>

<!-- UPDATES -->
<section class="section">
  <h2>Latest Updates</h2>

  <div class="updates-grid" id="updates">
    <div class="update-card">
      <h3>New Interview Drop</h3>
      <p>We just released a street interview series focusing on youth dreams and struggles.</p>
    </div>

    <div class="update-card">
      <h3>Behind The Scenes</h3>
      <p>Our latest production shows how ONB Media builds cinematic storytelling scenes.</p>
    </div>
  </div>

  <!-- ADD NEW UPDATE -->
  <div class="add-box">
    <h3 style="margin-bottom:10px;">Add New Update</h3>
    <input id="title" placeholder="Update title">
    <textarea id="desc" placeholder="Update description"></textarea>
    <button onclick="addUpdate()">Publish Update</button>
  </div>
</section>

<!-- FOOTER -->
<footer>
  © 2026 ONB Media • Cinematic Digital Journalism
</footer>

<script>
function addUpdate(){
  let title = document.getElementById("title").value;
  let desc = document.getElementById("desc").value;

  if(!title || !desc) return;

  let box = document.createElement("div");
  box.className = "update-card";
  box.innerHTML = "<h3>"+title+"</h3><p>"+desc+"</p>";

  document.getElementById("updates").prepend(box);

  document.getElementById("title").value = "";
  document.getElementById("desc").value = "";
}
</script>

</body>
</html> Onbmedia.com
Its a media owned by young souls where we cover what matters
