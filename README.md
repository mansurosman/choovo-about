<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Choovo | About Us</title>
<style>
  body {
    margin: 0; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen,
    Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    background: #1b0e2f;
    color: white;
    line-height: 1.6;
    scroll-behavior: smooth;
  }
  h1,h2,h3,p { margin: 0 0 1rem 0; }
  a { color: #00f6ff; text-decoration: none; }
  a:hover { text-decoration: underline; }
  .container {
    max-width: 1100px;
    margin: auto;
    padding: 0 1rem;
  }
  #hero {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    padding: 4rem 1rem;
    position: relative;
    overflow: hidden;
  }
  #hero h1 {
    font-size: 2.5rem;
    font-weight: 800;
    max-width: 600px;
    margin-bottom: 1rem;
  }
  #hero p {
    color: #ffc98c;
    font-size: 1.25rem;
    max-width: 500px;
    margin-bottom: 2rem;
  }
  #hero .btn-group {
    display: flex;
    gap: 1rem;
    flex-wrap: wrap;
    justify-content: center;
  }
  button {
    font-weight: 700;
    padding: 0.75rem 1.5rem;
    border-radius: 6px;
    cursor: pointer;
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    user-select: none;
    border: none;
    transition: background-color 0.3s ease;
    font-size: 1rem;
  }
  button.primary {
    background: #ff5f56;
    color: white;
  }
  button.primary:hover {
    background: #ff7a71;
  }
  button.outline {
    border: 2px solid #00f6ff;
    color: #00f6ff;
    background: transparent;
  }
  button.outline:hover {
    background: rgba(0, 246, 255, 0.1);
  }
  .arrow-right {
    border: solid white;
    border-width: 0 2px 2px 0;
    display: inline-block;
    padding: 4px;
    transform: rotate(-45deg);
    margin-left: 8px;
  }
  section {
    padding: 4rem 1rem;
    max-width: 1100px;
    margin-left: auto;
    margin-right: auto;
  }
  h2 {
    font-size: 2rem;
    font-weight: 700;
    margin-bottom: 1rem;
  }
  h3 {
    font-size: 1.25rem;
    font-weight: 700;
    margin-bottom: 0.5rem;
  }
  p {
    color: #ffc98c;
  }
  #story {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px,1fr));
    gap: 2rem;
  }
  figure {
    background: rgba(34, 20, 56, 0.4);
    border-radius: 12px;
    padding: 1rem;
    box-shadow: 0 4px 15px rgba(0,0,0,0.3);
  }
  figure img {
    width: 100%;
    border-radius: 12px;
    margin-bottom: 0.75rem;
  }
  #values .grid {
    display: grid;
    grid-template-columns: repeat(auto-fit,minmax(260px,1fr));
    gap: 2rem;
  }
  #values .card {
    background: rgba(34, 20, 56, 0.6);
    border-radius: 16px;
    padding: 1.5rem;
    text-align: left;
    box-shadow: 0 4px 15px rgba(0,0,0,0.4);
    display: flex;
    flex-direction: column;
    height: 100%;
  }
  #values .icon {
    font-size: 2.5rem;
    margin-bottom: 0.75rem;
  }
  #how {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    gap: 2rem;
  }
  #how > div {
    flex: 1 1 320px;
  }
  #how ul {
    list-style: inside disc;
    color: #ffc98c;
    font-size: 1.1rem;
    margin-bottom: 2rem;
  }
  #how button {
    background: #00f6ff;
    color: #1b0e2f;
    padding: 0.75rem 1.5rem;
    font-weight: 700;
    border: none;
    border-radius: 8px;
    cursor: pointer;
    transition: background-color 0.3s ease;
  }
  #how button:hover {
    background: #00c0cc;
  }
  #how img {
    flex: 1 1 320px;
    max-width: 600px;
    width: 100%;
    border-radius: 24px;
    box-shadow: 0 8px 30px rgba(0,0,0,0.5);
  }
  #compare {
    background: #141025;
    color: white;
    text-align: center;
  }
  #compare table {
    width: 100%;
    border-collapse: collapse;
    margin-top: 1rem;
    font-size: 1rem;
  }
  #compare thead tr {
    background-color: #221438;
  }
  #compare th, #compare td {
    padding: 1rem;
    border: 1px solid #2a2142;
  }
  #compare tbody tr:hover {
    background-color: rgba(255, 255, 255, 0.05);
  }
  #dealers {
    text-align: center;
  }
  #dealers p {
    max-width: 600px;
    margin: 0 auto 2rem;
    color: #ffc98c;
  }
  #dealers img {
    max-width: 800px;
    width: 100%;
    border-radius: 24px;
    box-shadow: 0 8px 30px rgba(0,0,0,0.6);
  }
  #testimonials {
    background: #141025;
    text-align: center;
    color: #ffc98c;
  }
  #testimonials .grid {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 1.5rem;
  }
  #testimonials .card {
    background: rgba(34,20,56,0.6);
    border-radius: 12px;
    padding: 1.5rem;
    max-width: 300px;
    box-shadow: 0 4px 15px rgba(0,0,0,0.3);
    flex: 1 1 280px;
    display: flex;
    flex-direction: column;
  }
  #testimonials .card p {
    flex-grow: 1;
  }
  #testimonials .card span {
    margin-top: 1rem;
    font-weight: 700;
  }
  #cta {
    text-align: center;
    padding: 4rem 1rem;
  }
  #cta h2 {
    font-size: 2.5rem;
    font-weight: 900;
    margin-bottom: 2rem;
  }
  #cta button {
    background-color: #ff5f56;
    border: none;
    padding: 1rem 2rem;
    font-size: 1.25rem;
    color: white;
    font-weight: 900;
    border-radius: 8px;
    cursor: pointer;
    transition: background-color 0.3s ease;
  }
  #cta button:hover {
    background-color: #ff7a71;
  }
  footer {
    padding: 3rem 1rem;
    background: #1b0e2f;
    text-align: center;
    color: #ffc98c;
    font-size: 0.9rem;
  }
  @media (max-width: 768px) {
    #hero h1 {
      font-size: 1.9rem;
    }
    #hero p {
      font-size: 1rem;
    }
    #how {
      flex-direction: column;
    }
    #how img {
      max-width: 100%;
    }
    #testimonials .grid {
      flex-direction: column;
    }
  }
</style>
</head>
<body>

<section id="hero">
  <h1>We got tired of watching people get ripped off.</h1>
  <p>So we built Choovo — your logic-powered co-pilot.</p>
  <div class="btn-group">
    <button class="primary">Run a Reality Check <i class="arrow-right"></i></button>
    <button class="outline">Try Today’s Top 5</button>
  </div>
</section>

<section id="story" class="container">
  <figure>
    <h3>A great-looking car</h3>
    <p>Online ad looked perfect.</p>
  </figure>
  <figure>
    <h3>£1,800 later…</h3>
    <p>Hidden gearbox failure emerges.</p>
  </figure>
  <figure>
    <h3>There had to be a better way</h3>
    <p>Choovo's founding moment.</p>
  </figure>
</section>

<section id="values" class="container">
  <h2>What Choovo Stands For</h2>
  <p>Neutral by design. Built for safer roads and smarter money.</p>
  <div class="grid">
    <div class="card">
      <div class="icon">🛡️</div>
      <h3>Neutral by Design</h3>
      <p>We don't buy or sell cars. We just show the truth.</p>
    </div>
    <div class="card">
      <div class="icon">⚙️</div>
      <h3>Logic over Hype</h3>
      <p>Data science cuts through glossy ads & dealer games.</p>
    </div>
    <div class="card">
      <div class="icon">🚘</div>
      <h3>Safer Roads</h3>
      <p>Smart choices reduce breakdowns & accidents.</p>
    </div>
    <div class="card">
      <div class="icon">👥</div>
      <h3>Built for People</h3>
      <p>Buyers, honest sellers & good dealers win together.</p>
    </div>
    <div class="card">
      <div class="icon">💷</div>
      <h3>Smarter Money</h3>
      <p>Bank better deals, avoid costly repair traps.</p>
    </div>
  </div>
</section>

<section id="how" class="container">
  <h2>How Choovo Works</h2>
  <ul>
    <li><strong>Top 5 Scan:</strong> daily logic engine ranks safest, best-value cars.</li>
    <li><strong>Reality Checker:</strong> x-rays any listing for hidden MOT advisories & category damage.</li>
    <li><strong>Cost-to-Repair Radar:</strong> predicts future maintenance spend using aggregated warranty data.</li>
  </ul>
  <button>See the Logic in Action</button>
</section>

<section id="compare" class="container" style="background:#141025; color:#fff;">
  <h2>Choovo vs. The Market</h2>
  <table style="width:100%; border-collapse: collapse; margin-top: 1rem; font-size:1rem;">
    <thead style="background:#221438;">
      <tr>
        <th style="padding:1rem; border:1px solid #2a2142;">Feature</th>
        <th style="padding:1rem; border:1px solid #2a2142;">HPI</th>
        <th style="padding:1rem; border:1px solid #2a2142;">Marketplace</th>
        <th style="padding:1rem; border:1px solid #2a2142;">Choovo</th>
      </tr>
    </thead>
    <tbody>
      <tr style="border-top:1px solid #2a2142;">
        <td style="padding:1rem;">Past-only history checks</td>
        <td style="padding:1rem; text-align:center;">✅</td>
        <td style="padding:1rem; text-align:center;">❌</td>
        <td style="padding:1rem; text-align:center;">✅ + future risk</td>
      </tr>
      <tr style="border-top:1px solid #2a2142;">
        <td style="padding:1rem;">Repair cost insight</td>
        <td style="padding:1rem; text-align:center;">❌</td>
        <td style="padding:1rem; text-align:center;">❌</td>
        <td style="padding:1rem; text-align:center;">✅</td>
      </tr>
      <tr style="border-top:1px solid #2a2142;">
        <td style="padding:1rem;">Neutral (no ads)</td>
        <td style="padding:1rem; text-align:center;">❌</td>
        <td style="padding:1rem; text-align:center;">❌</td>
        <td style="padding:1rem; text-align:center;">✅</td>
      </tr>
      <tr style="border-top:1px solid #2a2142;">
        <td style="padding:1rem;">Guided decision</td>
        <td style="padding:1rem; text-align:center;">❌</td>
        <td style="padding:1rem; text-align:center;">❌</td>
        <td style="padding:1rem; text-align:center;">✅</td>
      </tr>
    </tbody>
  </table>
</section>

<section id="dealers" class="container" style="text-align:center; padding: 4rem 1rem;">
  <h2>Good Dealers Thrive with Choovo</h2>
  <p style="max-width:600px; margin:auto; color:#ffc98c; margin-bottom:2rem;">
    Transparent cars sell faster and come back less. Our Trust-Score badge helps honest dealers stand out.
  </p>
</section>

<section id="testimonials" style="background:#141025; padding: 4rem 1rem; text-align:center; color:#ffc98c;">
  <h2>People We’ve Protected</h2>
  <div style="max-width:1100px; margin:auto; display:flex; flex-wrap:wrap; gap:1.5rem; justify-content:center;">
    <div style="background:rgba(34,20,56,0.6); border-radius:12px; padding:1.5rem; max-width:300px; box-shadow:0 4px 15px rgba(0,0,0,0.3); flex:1 1 280px; display:flex; flex-direction:column;">
      <p style="flex-grow:1;">“I saved £1,200 thanks to Choovo’s Top 5 scan.”</p>
      <span style="margin-top:1rem; font-weight:700;">— Aisha, Manchester</span>
    </div>
    <div style="background:rgba(34,20,56,0.6); border-radius:12px; padding:1.5rem; max-width:300px; box-shadow:0 4px 15px rgba(0,0,0,0.3); flex:1 1 280px; display:flex; flex-direction:column;">
      <p style="flex-grow:1;">“Reality Checker flagged hidden service gaps.”</p>
      <span style="margin-top:1rem; font-weight:700;">— Tom, Bristol</span>
    </div>
    <div style="background:rgba(34,20,56,0.6); border-radius:12px; padding:1.5rem; max-width:300px; box-shadow:0 4px 15px rgba(0,0,0,0.3); flex:1 1 280px; display:flex; flex-direction:column;">
      <p style="flex-grow:1;">“Better than HPI – full peace of mind.”</p>
      <span style="margin-top:1rem; font-weight:700;">— Jordan, Glasgow</span>
    </div>
  </div>
</section>

<section id="cta" style="text-align:center; padding:4rem 1rem;">
  <h2>Join the Logic Revolution</h2>
  <button style="background:#ff5f56; border:none; padding:1rem 2rem; font-size:1.25rem; color:white; font-weight:900; border-radius:8px; cursor:pointer; transition:background-color 0.3s ease;">
    Protect Your Purchase →
  </button>
</section>

<footer style="padding: 3rem 1rem; background: #1b0e2f; text-align: center; color: #ffc98c; font-size: 0.9rem;">
  © 2025 Choovo Ltd — Built in the UK for safer roads.
</footer>

</body>
</html>
# choovo-about
