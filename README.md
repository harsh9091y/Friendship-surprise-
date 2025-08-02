# Friendship-surprise-
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Surprise for Tanu 💛</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    html, body { height: 100%; font-family: 'Segoe UI', sans-serif; }
    .page {
      display: none;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      height: 100vh;
      text-align: center;
      padding: 2rem;
    }
    .active { display: flex; }
    h1 { font-size: 2.5rem; color: #fff; }
    p {
      color: #fff;
      font-size: 1.2rem;
      max-width: 600px;
    }
    .btn {
      padding: 10px 20px;
      font-size: 1rem;
      margin-top: 20px;
      background-color: #fff;
      color: #333;
      border: none;
      border-radius: 8px;
      cursor: pointer;
    }
    .heart {
      font-size: 3rem;
      animation: beat 1s infinite alternate;
    }
    @keyframes beat {
      from { transform: scale(1); }
      to { transform: scale(1.2); }
    }
    .fireworks {
      position: fixed;
      top: 0;
      left: 0;
      width: 100vw;
      height: 100vh;
      pointer-events: none;
      background: url('https://media.giphy.com/media/3oEjI6SIIHBdRxXI40/giphy.gif') center center no-repeat;
      background-size: cover;
      z-index: 999;
    }
    body.page2 { background: linear-gradient(to right, #fbc2eb, #a6c1ee); }
    body.page3 { background: linear-gradient(to right, #fdfbfb, #ebedee); color: #333; }
    body.page4 { background-color: black; }
  </style>
</head>
<body class="page1">
  <audio autoplay loop>
    <source src="https://dl.sndup.net/86dt/Yeh%20Dosti%20Hum%20Nahi%20Todenge.mp3" type="audio/mpeg">
  </audio>

  <div id="page1" class="page active">
    <h1>Challenge for you, Tanu (Bhutni 😁)</h1>
    <p>Ready to unlock your Friendship Day Surprise? Click below if you dare 😎</p>
    <button class="btn" onclick="goToPage(2)">I'm Ready! 🔓</button>
  </div>

  <div id="page2" class="page">
    <div class="heart">💛💛💛</div>
    <h1>Happy Friendship Day Bhutni! 🥹💫</h1>
    <p>Tera smile sabse badi taqat hai... yeh sirf ek beginning hai 😉</p>
    <button class="btn" onclick="goToPage(3)">Next 💌</button>
  </div>

  <div id="page3" class="page">
    <h1>Letter from Your Bhaylu 😁💗</h1>
    <p>
      Hpy friendship day bhutni 💕💫... itne din se bole ja rhi thi frndship day aarha h 😂🤣... samj to na aari likhu ke 😂😞...
      m bhot lucky hu jo tu meri dost ha na.. na bestie 😂... Teri vjh se bhut kuch meri jivan bhut aanad myi hoyo h 🥹...
      kafi baar mero mood krb rhto to tu minute me ek dum shi kar dya ha bhutni jo ha jadu kardya ha 😂...
      tne hasti dekh mera muh p bhi smile aaja h khud hi jyada kuch to karno bhi na pde 😂🥹...
      bhut kuch sikho bhi h tera si mne life me for example bakwas 🤣😂...
      tu bhot aachi ha yaar sach me 😊 meri bhayli ko ha 😹...
      aur faltu ki overthinking si mood krb mat kra kr khush rha kar jo hoga dekha jayega smji 🤡...
      logo ki baato se mt dimg krb kiya kr pgl... bhawan kre apni dosti nue hi bni rve hmesha 🥹🧿...
      bas aur to ke hi bolu khush rha kr.... suthri to wase bhi ha par hasti Hui jyada suthri laga ha ek no. 😉 biftiful 😂😂🤣...
      bas bas baki chiz to wase bhi bol dugo 😂 nhi to bero na kitni bdi hojave go yo 😂...
    </p>
    <button class="btn" onclick="goToPage(4)">Final Boom! 🎆</button>
  </div>

  <div id="page4" class="page">
    <div class="fireworks"></div>
    <h1 style="color: yellow">🎉 Happy Friendship Day, Bhutni! 🎉</h1>
    <p style="color: white">Dosti ka patakha phoot chuka hai! 😁💥</p>
  </div>

  <script>
    function goToPage(pageNumber) {
      document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
      document.body.className = 'page' + pageNumber;
      document.getElementById('page' + pageNumber).classList.add('active');
    }
  </script>
</body>
</html>
