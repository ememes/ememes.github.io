<!DOCTYPE html>
<html lang="tr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Ememes Destek</title>
  <meta name="description" content="Ememes uygulamaları için destek ve yardım sayfası. İletişim, sıkça sorulan sorular ve gizlilik politikası.">
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg: #f4f7fb;
      --text: #222;
      --primary: #3a7bd5;
      --secondary: #3a6073;
      --card-bg: #fff;
      --muted: #666;
      --radius: 16px;
    }
    * { box-sizing: border-box; margin: 0; padding: 0; }
    body {
      font-family: "Inter", sans-serif;
      background: var(--bg);
      color: var(--text);
      line-height: 1.6;
    }
    header {
      background: linear-gradient(135deg, var(--secondary), var(--primary));
      color: white;
      text-align: center;
      padding: 60px 20px 80px;
      position: relative;
      overflow: hidden;
    }
    header::after {
      content: "";
      position: absolute;
      width: 300px;
      height: 300px;
      background: rgba(255, 255, 255, 0.15);
      border-radius: 50%;
      top: -80px;
      right: -100px;
      filter: blur(60px);
    }
    header h1 {
      font-size: 2.2rem;
      font-weight: 700;
    }
    header p {
      margin-top: 10px;
      font-size: 1rem;
      color: rgba(255,255,255,0.9);
    }
    main {
      max-width: 900px;
      margin: -50px auto 60px;
      padding: 0 20px;
    }
    .card {
      background: var(--card-bg);
      border-radius: var(--radius);
      padding: 28px;
      margin-bottom: 24px;
      box-shadow: 0 8px 24px rgba(0,0,0,0.05);
      transition: transform 0.25s ease, box-shadow 0.25s ease;
    }
    .card:hover {
      transform: translateY(-3px);
      box-shadow: 0 12px 28px rgba(0,0,0,0.08);
    }
    h2 {
      font-size: 1.3rem;
      color: var(--primary);
      margin-bottom: 12px;
    }
    a.button {
      display: inline-block;
      background: var(--primary);
      color: white;
      padding: 10px 18px;
      border-radius: 10px;
      text-decoration: none;
      margin-top: 12px;
      font-weight: 600;
      transition: background 0.2s;
    }
    a.button:hover { background: #2f68b3; }
    .faq dt {
      font-weight: 600;
      margin-top: 14px;
    }
    .faq dd {
      color: var(--muted);
      margin-bottom: 10px;
      margin-left: 10px;
    }
    ul.contact-info {
      list-style: none;
      margin-top: 10px;
    }
    ul.contact-info li {
      margin-bottom: 8px;
      color: var(--muted);
    }
    footer {
      text-align: center;
      font-size: 0.9rem;
      color: var(--muted);
      padding: 30px 10px;
    }
    footer a {
      color: var(--primary);
      text-decoration: none;
      margin: 0 6px;
    }
    footer a:hover { text-decoration: underline; }
    @media (min-width: 700px) {
      header h1 { font-size: 2.6rem; }
      .card { padding: 36px; }
    }
  </style>
</head>
<body>
  <header>
    <h1>Ememes Destek</h1>
    <p>Herhangi bir sorun mu yaşıyorsunuz? Yardım etmek için buradayız.</p>
  </header>

  <main>
    <section class="card">
      <h2>📩 İletişim</h2>
      <p>Bize ulaşmak için aşağıdaki adresi kullanabilirsiniz:</p>
      <ul class="contact-info">
        <li><strong>E-posta:</strong> <a href="mailto:mertslvmert@gmail.com?subject=Ememes%20Destek">mertslvmert@gmail.com</a></li>
        <li><strong>Uygulama Adı:</strong> Ememes</li>
      </ul>
      <a href="mailto:mertslvmert@gmail.com?subject=Ememes%20Destek" class="button">E-posta Gönder</a>
    </section>

    <section class="card faq">
      <h2>💡 Sıkça Sorulan Sorular</h2>
      <dl>
        <dt>Uygulama açılmıyor, ne yapmalıyım?</dt>
        <dd>Uygulamayı kaldırıp yeniden yükleyin. Sorun devam ederse cihaz modelinizi ve iOS sürümünü belirterek bize yazın.</dd>

        <dt>Reklamlar veya satın alma görünmüyor.</dt>
        <dd>App Store hesabınızı ve hata ekran görüntüsünü gönderin, kısa sürede çözelim.</dd>

        <dt>Gizlilik politikası nerede?</dt>
        <dd><a href="/privacy.html">Gizlilik Politikası</a> sayfasında detayları bulabilirsiniz.</dd>
      </dl>
    </section>

    <section class="card">
      <h2>⚙️ Sorun Bildirirken</h2>
      <p>Hızlı çözüm için lütfen aşağıdaki bilgileri e-posta ile paylaşın:</p>
      <ul class="contact-info">
        <li>Cihaz modeli (ör. iPhone 12)</li>
        <li>iOS sürümü (ör. iOS 18.1)</li>
        <li>Ekran görüntüsü (varsa)</li>
        <li>Kısa sorun açıklaması</li>
      </ul>
    </section>
  </main>

  <footer>
    © <span id="year"></span> Ememes • 
    <a href="/privacy.html">Gizlilik Politikası</a> • 
    <a href="/terms.html">Kullanım Koşulları</a>
  </footer>

  <script>document.getElementById("year").textContent = new Date().getFullYear();</script>
</body>
</html>
