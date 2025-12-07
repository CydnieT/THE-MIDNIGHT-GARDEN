# THE MIDNIGHT GARDEN — Site Build & Brand Documentation

---

## 1. Interactive Website Code (Complete One-File HTML Build)

The following is the final build of the interactive THE MIDNIGHT GARDEN website, suitable for deployment via GitHub Pages.  
Copy this file into `index.html` in your repository for direct deployment.

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width,initial-scale=1.0">
  <title>THE MIDNIGHT GARDEN</title>
  <style>
    /* Brand palette: Velvet Black, Garden Green, Petal Pink, Gold Foil */
    body {
      margin: 0;
      font-family: 'Montserrat', Arial, sans-serif;
      background: #1a1a1a;
      color: #f4f4f4;
    }
    header {
      background: linear-gradient(90deg, #103518 0%, #1a1a1a 100%);
      padding: 40px 0 20px;
      text-align: center;
    }
    header h1 {
      font-size: 3em;
      letter-spacing: 0.05em;
      font-family: 'Playfair Display', serif;
      color: #f4efdd;
      margin: 0;
      text-shadow: 0 2px 8px #0d120e, 0 0 6px #dbb95e;
    }
    header p {
      color: #b9848c;
      font-style: italic;
      font-size: 1.2em;
      letter-spacing: 0.05em;
      margin-top: 8px;
    }
    nav {
      margin: 25px 0;
      text-align: center;
    }
    nav button {
      background: #dbb95e;
      color: #1a1a1a;
      border: none;
      border-radius: 30px;
      padding: 14px 38px;
      margin: 0 10px;
      font-size: 1em;
      cursor: pointer;
      font-weight: bold;
      box-shadow: 0 2px 8px #dbb95e33;
      transition: background 0.2s;
    }
    nav button.active, nav button:hover {
      background: #103518;
      color: #dbb95e;
      outline: 2px solid #dbb95e;
    }
    .content {
      max-width: 820px;
      margin: 40px auto;
      background: #21242c;
      box-shadow: 0 0 16px #0a120833;
      border-radius: 18px;
      padding: 32px;
    }
    h2 {
      color: #dbb95e;
      font-family: 'Playfair Display', serif;
      font-size: 2em;
      margin-bottom: 24px;
    }
    ul {
      list-style: square inside;
      padding-left: 0;
      margin-bottom: 1.5em;
    }
    .product-list {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
      gap: 30px;
    }
    .product-card {
      background: #1a1a1a;
      padding: 18px;
      border-radius: 12px;
      box-shadow: 0 2px 10px #0a120870;
      border: 1.5px solid #103518;
      color: #dbb95e;
      text-align: center;
    }
    .calendar-table {
      width: 100%;
      border-collapse: collapse;
    }
    .calendar-table th, .calendar-table td {
      padding: 10px;
      border: 1px solid #dbb95e55;
      text-align: center;
      font-size: 1em;
    }
    .calendar-table th {
      background: #b9848c;
      color: #1a1a1a;
    }
    footer {
      background: #1a1a1a;
      text-align: center;
      padding: 24px 0;
      color: #b9848c;
      font-size: 1em;
    }
    @media (max-width:600px) {
      .content { padding: 10px; }
      header h1 { font-size: 2em; }
      nav button { padding: 10px 18px; font-size: 0.95em; }
      .product-list { grid-template-columns: 1fr; }
    }
  </style>
</head>
<body>
  <header>
    <h1>THE MIDNIGHT GARDEN</h1>
    <p>Luxury blooms, crafted at the witching hour</p>
    <nav>
      <button id="about-btn" class="active">About</button>
      <button id="products-btn">Products</button>
      <button id="calendar-btn">Drop Calendar</button>
      <button id="deploy-btn">Deployment</button>
    </nav>
  </header>
  <main>
    <section class="content" id="about">
      <h2>Brand Identity</h2>
      <p><strong>The Midnight Garden</strong> is a luxury brand inspired by the mystery and elegance found in twilight gardens. Our identity combines deep, romantic hues—velvet black, lush green, petal pink, and gold accents—to evoke a sophisticated, magical atmosphere.  
      <br><br>
      <em>Mission:</em> To provide unique, hand-crafted floral and botanical products for night owls, dreamers, and connoisseurs of beauty.  
      <br>
      <em>Values:</em> Botanical artistry, sustainability, enchantment, and inclusivity.</p>
    </section>
    <section class="content" id="products" style="display:none;">
      <h2>Product Line Breakdown</h2>
      <div class="product-list">
        <div class="product-card">
          <h3>Nocturne Bouquets</h3>
          <p>Opulent arrangements of rare midnight blooms. Exclusively available for evening deliveries.</p>
        </div>
        <div class="product-card">
          <h3>Enchanted Oils</h3>
          <p>Botanical-infused blends for aromatherapy and rituals. Sourced from moonlit gardens and enchanted herbs.</p>
        </div>
        <div class="product-card">
          <h3>Moonlit Candles</h3>
          <p>Hand-poured soy candles with garden scents for tranquil nights.</p>
        </div>
        <div class="product-card">
          <h3>Golden Petal Stationery</h3>
          <p>Letterpress cards and journals, adorned with garden gold foil and illustrations.</p>
        </div>
      </div>
    </section>
    <section class="content" id="calendar" style="display:none;">
      <h2>Drop Calendar</h2>
      <table class="calendar-table">
        <thead>
          <tr>
            <th>Date</th>
            <th>Collection</th>
            <th>Description</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>2025-02-02</td>
            <td>Winter Veil</td>
            <td>Limited-edition Nocturne Bouquets with icy accents</td>
          </tr>
          <tr>
            <td>2025-05-10</td>
            <td>Spring Equinox</td>
            <td>Fresh Moonlit Candles and Enchanted Oils launch</td>
          </tr>
          <tr>
            <td>2025-08-12</td>
            <td>Midsummer Dream</td>
            <td>Golden Petal Stationery + Summer Blossoms</td>
          </tr>
          <tr>
            <td>2025-10-31</td>
            <td>Twilight Ritual</td>
            <td>Special Halloween drop: Dark florals & mystical scents</td>
          </tr>
        </tbody>
      </table>
    </section>
    <section class="content" id="deploy" style="display:none;">
      <h2>Deployment Instructions (GitHub Pages)</h2>
      <ol>
        <li>
          <strong>Add Your Site File:</strong>  
          Save the website code above into a file named <code>index.html</code> at the root of your <code>MIDNIGHTGARDEN</code> repository.
        </li>
        <li>
          <strong>Enable GitHub Pages:</strong>  
          Go to your repository settings &gt; Pages.<br>
          Under <strong>Source</strong>, select your main branch (typically <code>main</code>) and <code>/root</code> directory.
        </li>
        <li>
          <strong>Save &amp; Visit:</strong>  
          After saving, GitHub Pages will deploy your site.<br>
          Your website will be live at: <br><code>https://CydnieT.github.io/MIDNIGHTGARDEN/</code>
        </li>
        <li>
          <strong>Updating Your Site:</strong>  
          Any change to <code>index.html</code> (via commit/push) will update your deployed website after a few moments.
        </li>
      </ol>
      <p>For contact info, custom domains, or advanced configuration, refer to the <a href="https://docs.github.com/en/pages/getting-started-with-github-pages">GitHub Pages documentation</a>.</p>
    </section>
  </main>
  <footer>
    &copy; 2025 THE MIDNIGHT GARDEN &mdash; Enchantment after dark.
  </footer>
  <script>
    // Button navigation
    const sections = ['about', 'products', 'calendar', 'deploy'];
    const buttons = sections.map(id => document.getElementById(id + '-btn'));
    const pages = sections.map(id => document.getElementById(id));
    buttons.forEach((btn, i) => {
      btn.addEventListener('click', () => {
        buttons.forEach(b => b.classList.remove('active'));
        btn.classList.add('active');
        pages.forEach((pg, j) => pg.style.display = (i === j) ? '' : 'none');
      });
    });
    // Initial section
    pages.forEach((pg, j) => pg.style.display = (j === 0) ? '' : 'none');
  </script>
</body>
</html>
```

---

## 2. Brand Identity Summary

- **Name:** THE MIDNIGHT GARDEN
- **Core Theme:** Nocturnal luxury, botanical beauty, enchanted twilight.
- **Palette:** Velvet Black, Garden Green, Petal Pink, Gold Foil.
- **Mission:** Hand-crafting extraordinary floral and botanical experiences for dreamers and night dwellers.
- **Values:** Artistic integrity, sustainability, magical storytelling, exclusivity.

---

## 3. Product Line Breakdown

- **Nocturne Bouquets:** Premium night-blooming floral arrangements, available for nighttime delivery.
- **Enchanted Oils:** Moonlit herbal aromatherapy blends for wellness and ritual.
- **Moonlit Candles:** Signature candles, inspired by midnight gardens.
- **Golden Petal Stationery:** Elegant letterpress and gold foil paper goods, celebrating botanical artistry.

---

## 4. Drop Calendar

| Date         | Collection          | Description                             |
|--------------|--------------------|-----------------------------------------|
| 2025-02-02   | Winter Veil        | Nocturne Bouquets with icy accents      |
| 2025-05-10   | Spring Equinox     | Moonlit Candles & Enchanted Oils        |
| 2025-08-12   | Midsummer Dream    | Golden Petal Stationery & Summer Florals|
| 2025-10-31   | Twilight Ritual    | Black Florals & Mystical Scents (Halloween)|

---

## 5. Deployment Instructions (GitHub Pages)

1. Save the HTML site build above as `index.html` at the root of your repository.
2. Go to the repository's GitHub settings &gt; Pages.
3. Select your main branch (`main`) and `/root` as the source.
4. Save; your site will update within minutes at  
   `https://CydnieT.github.io/MIDNIGHTGARDEN/`
5. For custom domain or extra features, consult the official [GitHub Pages docs](https://docs.github.com/en/pages/getting-started-with-github-pages).

---

_End of documentation. For brand updates, product expansion, or new drops, edit this file and redeploy!_
