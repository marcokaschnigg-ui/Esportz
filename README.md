<!DOCTYPE html>
<html lang="de">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Meine gamer seite </title>
<Style>
#musicControl {
  position: fixed;
  bottom: 20px;
  right: 20px;

  display: flex;
  gap: 10px;
  align-items: center;

  background: rgba(0,0,0,0.6);
  padding: 10px 15px;
  border-radius: 10px;

  z-index: 1000;
}

#volume {
  width: 120px;
  accent-color: #00e5ff;
}

#musicBtn {
  background: transparent;
  border: 2px solid #00e5ff;
  color: #00e5ff;
  padding: 6px 12px;
  cursor: pointer;
}


section {
   padding: 100px 10%;
  background: rgba(0,0,0,0.6);
  text-align: center;
  color: white;
}


.card::before {
  content: "";
  position: absolute;
  inset: 0;
  background: rgba(0,0,0,0.35);   /* 🔥 mild dunkel */
  transition: 0.3s;
}
.cards {
  display: grid;
  grid-template-columns: repeat(auto-fit,minmax(200px,1fr)) ;
  gap: 10px;
}

.card {
  aspect-ratio: 16 / 9;
  border-radius: 12px;

  position: relative;
  overflow: hidden;

  display: flex;
  justify-content: center;
  align-items: center;

  font-size: 20px;
  font-weight: bold;
  color: white;

  background-size: cover;
  background-position: center;

  cursor: pointer;
}

.cs2 {
  background-image: url(cs2.png);
}

.valorant {
  background-image: url(valorant.png);
}

.fortnite {
  background-image: url(fortnite.png);
}
.card::before {
  content: "";
  position: absolute;
  inset: 0;
  background: rgba(0,0,0,0.35);
  transition: 0.3s;
}
.card:hover::before {
  background: rgba(0,0,0,0) ;
}

.cs2 {
  background-image: url(cs2.png);
  background-size: 100%;
  background-repeat: no-repeat;
}
/*AK hintergrund */
#ak-section {
  background-image: url(ak47.png);
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;

  position: relative;
}

.card span {
  position: relative;
  z-index: 2;

  text-shadow:
    0 0 5px #00e5ff,
    0 0 10px #00e5ff;
}
#ak-section::before {
  content: "";
  position: absolute;
  inset: 0;
  background: rgba(0,0,0,0.6);
}

#ak-section section {
  position: relative;
}


/*Hintergrund*/
.main {
min-height: 100vh;

background-image: url(test.png);
background-size: cover;
background-position: center;
background-repeat: no-repeat;
}

/*overlay*/
.overlay {
  min-height: 100vh;
  background: rgba(0,0,0,0.6);

  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

}

/* Willkommen Titel */
.titel {
  font-size: 60px;
  color: #00e5ff;
  text-transform: uppercase;

  text-shadow:
    1px 1px 0 #0088aa,
    2px 2px 0 #007799,
    3px 3px 0 #006688,
    4px 4px 0 #005577,
    0 0 15px #00e5ff;

  font-family: Arial, sans-serif;
}

.btn {
  margin-top: 25px;
  padding: 15px 40px;

  border: 2px solid #00e5ff;
  background: transparent;
  color: #00e5ff;

  font-size: 18px;
  cursor: pointer;
  border-radius: 6px;

  transition: 0.3s;
}

.btn:hover {
  background: #00e5ff;
  color: black;
  box-shadow: 0 0 20px #00e5ff;
}


nav {
  position: fixed;
  top: 0;
  width: 100%;
  height: 80px;

 background-image: url(nav.png.png);
 background-size: cover;
  background-position: center 23%;

  display: flex;
  justify-content: space-between;
  align-items: center;

  padding: 0 40px;
}
nav::before {
  content: "";
  position: absolute;
  inset: 0;
  background: rgba(0,0,0,0.5);
}

nav * {
  position: relative;
}
nav h2 {
  font-size: 26px;
  font-weight: bold;
  text-transform: uppercase;
  letter-spacing: 4px;

  color: #00e5ff;

  text-shadow:
    1px 1px 0 #0088aa,
    2px 2px 0 #007799,
    3px 3px 0 #006688,
    0 0 10px #00e5ff,
    0 0 25px #00e5ff,
    0 0 50px #00e5ff;

  animation: esportsGlow 2s infinite alternate;

  position: relative;
  z-index: 2;
}
@keyframes esportsGlow {
  from {
    text-shadow:
      0 0 10px #00e5ff,
      0 0 20px #00e5ff;
  }

  to {
    text-shadow:
      0 0 20px #00e5ff,
      0 0 40px #00e5ff;
  }
}







.menu a {
  color: white;
  text-decoration: none;
  margin-right: 70px;
}

.menu a:hover {
  color: #00e5ff;
}

nav {
  position: fixed;
  top: -70px;          /* 🔥 Start versteckt */
  left: 0;

  width: 100%;
  height: 80px;

  background-image: url("nav.png");
  background-size: cover;
  background-position: center 23%;

  display: flex;
  justify-content: space-between;
  align-items: center;

  padding: 0 40px;
  z-index: 100;

  transition: top 0.4s ease;   /* Animation */
}

/* Maus irgendwo → Navbar kommt runter */
body:hover nav {
  top: 0;
}

/* Dunkles Overlay */
nav::before {
  content: "";
  position: absolute;
  inset: 0;

  background: rgba(0,0,0,0.6);
  transition: background 0.4s ease;

  z-index: -1;
}

/* Hover = Overlay geht auf */
nav:hover::before {
  background: rgba(0,0,0,0);
}

/* Text über Overlay */
nav * {
  position: relative;
  z-index: 2;
}

/* GamerHub / Esports Titel */
nav h2 {
  font-size: 26px;
  font-weight: bold;
  text-transform: uppercase;
  letter-spacing: 4px;

  color: #00e5ff;

  text-shadow:
    1px 1px 0 #0088aa,
    2px 2px 0 #007799,
    3px 3px 0 #006688,
    0 0 10px #00e5ff,
    0 0 25px #00e5ff,
    0 0 50px #00e5ff;

  animation: esportsGlow 2s infinite alternate;
}

/* Glow Animation */
@keyframes esportsGlow {
  from {
    text-shadow:
      0 0 10px #00e5ff,
      0 0 20px #00e5ff;
  }

  to {
    text-shadow:
      0 0 20px #00e5ff,
      0 0 40px #00e5ff;
  }
}

</Style>

<head>

 <body>

  <nav>
    <h2>Esports</h2>
    <div class="menu">
    <a href="#home">Home</a>
    <a href="#games">Games</a>
    <a href="#kontakt">Kontakt</a>
  </div>
  </nav>

<div class="main" id="home" >
  <div class=" overlay">
 
 <button class="btn">Start</button>



</div>

 



</div>

<div id="ak-section">

<section id="games">
  <h2>Unsere Games</h2>
<div class="cards">
  <div class="card cs2"><span>CS2</span></div>
  <div class="card valorant"><span>Valorant</span></div>
  <div class="card fortnite"><span>Fortnite</span></div>
</div>
  
  </div>
</section>

<section id="kontakt">
  <h2>Kontakt</h2>
  <p>Email: gamer@email.de</p>
</section>

</div>

<div id="musicControl">
  <button id="musicBtn">▶ Musik starten</button>
  <input type="range" id="volume" min="0" max="100" value="50">
</div>

<audio id="bgMusic" loop preload="auto">
  <source src="music.mp3.mp3" type="audio/mpeg">
</audio>

<script>
const btn = document.getElementById("musicBtn");
const music = document.getElementById("bgMusic");
const volume = document.getElementById("volume");

music.volume = 0.5;

btn.addEventListener("click", () => {
  if (music.paused) {
    music.play();
    btn.textContent = "⏸ Musik stoppen";
  } else {
    music.pause();
    btn.textContent = "▶ Musik starten";
  }
});

volume.addEventListener("input", function() {
  music.volume = this.value / 100;
});
</script>



</body>

</html>
