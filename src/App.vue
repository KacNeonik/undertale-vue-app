<template>
  <div class="container">
      <header class="dialogue-box intro-box">
          <div style="text-align: center;">
              <img src="/logo.png" alt="UNDERTALE Logo" class="logo-img">
          </div>
          <p>Dawno, dawno temu, dwie rasy rządziły Ziemią: <br><span class="highlight">LUDZIE</span> i <span class="highlight">POTWORY</span>.</p>
          <p>Pewnego dnia wybuchła wojna między nimi. Po długiej bitwie ludzie odnieśli zwycięstwo i zapieczętowali potwory pod ziemią za pomocą magicznego zaklęcia.</p>
      </header>

      <main>
          <section class="dialogue-box">
              <h2>W czym tkwi sekret?</h2>
              <p>Undertale to niezależna gra RPG stworzona przez Toby'ego Foxa w 2015 roku. To, co odróżnia ją od innych gier z tego gatunku, to fakt, że <span class="yellow-text">nie musisz nikogo zabijać</span>.</p>
              <p>Każdy konflikt można rozwiązać pokojowo poprzez rozmowę, komplementy, a nawet flirt. Twój wybór (Pacyfista, Neutralny, Ludobójca) drastycznie zmienia zakończenie gry i stosunek postaci do Ciebie.</p>
          </section>

          <section class="dialogue-box">
              <h2>Kluczowe Postacie</h2>
              <div class="characters-grid">
                  <div class="character">
                      <img src="/toriel.png" alt="Grafika przedstawiająca Toriel" class="character-img">
                      <h3>Toriel</h3>
                      <p>Opiekuńcza strażniczka Ruin. Uczy gracza podstawowych mechanik gry i piecze pyszne ciasto toffi-cynamonowe.</p>
                  </div>
                  <div class="character">
                      <img src="/sans.png" alt="Grafika przedstawiająca Sansa" class="character-img">
                      <h3>Sans</h3>
                      <p>Leniwy szkielet, który uwielbia rzucać suchymi żartami. Mimo swojego wyglądu, jest jedną z najbardziej tajemniczych postaci.</p>
                  </div>
                  <div class="character">
                      <img src="/papyrus.png" alt="Grafika przedstawiająca Papyrusa" class="character-img">
                      <h3>Papyrus</h3>
                      <p>Wysoki, głośny szkielet z wielkim marzeniem o dołączeniu do Królewskiej Gwardii. Kocha spaghetti.</p>
                  </div>
              </div>
          </section>

          <div class="action-buttons">
              <details class="action-item">
                  <summary class="button"><img src="/FIght.png" alt="PRZYCISK FIGHT" class="btn-img"></summary>
                  <div class="info-box">
                      <p>* Atakujesz cel. Ciosy bezpowrotnie zwiększają Twoje LV.</p>
                  </div>
              </details>

              <details class="action-item">
                  <summary class="button"><img src="/Act.png" alt="PRZYCISK ACT" class="btn-img"></summary>
                  <div class="info-box">
                      <p>* Różne interakcje (np. rozmowa). Klucz do pacyfizmu.</p>
                  </div>
              </details>

              <details class="action-item">
                  <summary class="button"><img src="/Item.png" alt="PRZYCISK ITEM" class="btn-img"></summary>
                  <div class="info-box">
                      <p>* Używasz przedmiotów z ekwipunku, aby odzyskać utracone HP.</p>
                  </div>
              </details>

              <details class="action-item">
                  <summary class="button"><img src="/mercy.png" alt="PRZYCISK MERCY" class="btn-img"></summary>
                  <div class="info-box">
                      <p class="yellow-text">* Oszczędzasz potwora, kończąc walkę pokojowo.</p>
                  </div>
              </details>
          </div>
      </main>

      <footer>
          <p>Wiedza o tym że znalazłeś tę stronę</p>
          <p class="red-text">NAPEŁNIA CIĘ DETERMINACJĄ.</p>
      </footer>
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap');


* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    background-color: #000000;
    color: #FFFFFF;
    font-family: 'Press Start 2P', cursive;
    line-height: 1.8;
    font-size: 14px;
    padding: 20px;
}

.container {
    max-width: 800px;
    margin: 0 auto;
}

.dialogue-box {
    border: 5px solid #FFFFFF;
    background-color: #000000;
    padding: 30px;
    margin-bottom: 30px;
    border-radius: 4px;
}

.logo-img {
    max-width: 100%;
    width: 400px;
    height: auto;
    margin-bottom: 25px;
    image-rendering: pixelated;
}

h2 {
    font-size: 18px;
    margin-bottom: 20px;
}

h3 {
    font-size: 16px;
    margin-bottom: 10px;
    color: #FFFF00;
}

p {
    margin-bottom: 20px;
}

.highlight {
    color: #A0A0A0;
}

.yellow-text {
    color: #FFFF00;
}

.red-text {
    color: #FF0000;
    text-align: center;
    font-size: 18px;
    margin-top: 10px;
}

.characters-grid {
    display: grid;
    grid-template-columns: 1fr;
    gap: 20px;
}

@media (min-width: 600px) {
    .characters-grid {
        grid-template-columns: 1fr 1fr 1fr;
    }
}

.character {
    border: 2px dashed #FFFFFF;
    padding: 15px;
    text-align: center;
}

.character-img {
    max-width: 100px;
    height: auto;
    margin-bottom: 15px;
    image-rendering: pixelated;
}

.action-buttons {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    flex-wrap: wrap;
    margin-bottom: 40px;
}

.action-item {
    width: 22%;
}

.button {
    text-align: center;
    border: none;
    padding: 0;
    list-style: none;
}

.button::-webkit-details-marker {
    display: none; 
}

.btn-img {
    max-width: 100%; 
    height: auto;     
    image-rendering: pixelated; 
    cursor: pointer;   
    transition: transform 0.2s;
}

.btn-img:hover {
    transform: scale(1.05); 
}

.info-box {
    border: 2px dashed #FFFFFF;
    padding: 10px;
    margin-top: 15px;
    font-size: 10px;
    line-height: 1.5;
    background-color: #000000;
    text-align: left;
}

.info-box p {
    margin-bottom: 0; 
}

footer {
    text-align: center;
    margin-top: 50px;
    padding-bottom: 30px;
}
</style>