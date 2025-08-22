# Sweden
Learn about sweden!


[24 Ngu Wey En SR2B.html](https://github.com/user-attachments/files/21927818/24.Ngu.Wey.En.SR2B.html)
<html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>发现瑞典 · 色彩缤纷的一页式介绍</title>
  <link href="https://fonts.googleapis.com/css2?family=Nunito:wght@400;700;900&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg1: #ff9a9e; --bg2: #fad0c4; --bg3: #fbc2eb; --bg4: #a18cd1; --bg5: #f6d365; --bg6: #fda085;
      --ink: #1f2937; --muted: #6b7280; --card: rgba(255,255,255,.82);
      --accent: #10b981; --accent2: #6366f1; --accent3: #f59e0b; --accent4: #ef4444; --accent5: #14b8a6;
    }
    *{box-sizing:border-box}
    html,body{margin:0}
    body{
      font-family: 'Nunito', system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, "PingFang SC","Noto Sans CJK SC","Microsoft Yahei", sans-serif;
      color: var(--ink);
      background: linear-gradient(135deg, var(--bg1), var(--bg2), var(--bg3), var(--bg4), var(--bg5), var(--bg6));
      background-size: 400% 400%;
      animation: moveBG 25s ease infinite;
      min-height: 100vh;
    }
    @keyframes moveBG{0%{background-position:0% 0%}50%{background-position:100% 100%}100%{background-position:0% 0%}}
    header{
      position: sticky; top: 0; z-index: 50;
      backdrop-filter: blur(10px);
      background: linear-gradient(90deg, rgba(255,255,255,.8), rgba(255,255,255,.6));
      box-shadow: 0 10px 30px rgba(0,0,0,.08);
    }
    .wrap{max-width:1100px;margin:0 auto;padding:16px}
    h1{margin:10px 0 6px;font-size: clamp(28px, 4vw, 46px);letter-spacing:1px}
    .sub{margin:0 0 14px;color:var(--muted)}
    .pillbar{display:flex;gap:10px;flex-wrap:wrap}
    .pill{
      user-select:none; cursor:pointer; border:2px solid transparent; color:#111; font-weight:800; letter-spacing:.5px;
      background:#fff; padding:10px 14px; border-radius:999px; box-shadow:0 6px 18px rgba(0,0,0,.08);
      transition: transform .15s ease, box-shadow .2s ease, color .2s ease, background .2s ease, border-color .2s ease;
    }
    .pill:hover{transform:translateY(-2px); box-shadow:0 10px 24px rgba(0,0,0,.12)}
    .pill.active{color:#fff; border-color: rgba(0,0,0,.08)}
    .pill[data-topic="geography"].active{background:var(--accent2)}
    .pill[data-topic="culture"].active{background:var(--accent)}
    .pill[data-topic="history"].active{background:var(--accent3)}
    .pill[data-topic="sights"].active{background:var(--accent4)}
    .pill[data-topic="food"].active{background:var(--accent5)}

    main{max-width:1100px;margin:20px auto 60px;padding:0 16px}
    .grid{display:grid;grid-template-columns:1.2fr .8fr;gap:20px}
    @media (max-width:960px){.grid{grid-template-columns:1fr;}}

    .card{
      background: var(--card);
      border-radius: 24px; overflow: clip; position:relative;
      box-shadow: 0 20px 50px rgba(0,0,0,.12);
      border:1px solid rgba(255,255,255,.6)
    }
    .card h2{font-size: clamp(22px, 3.4vw, 32px); margin:0;}
    .card .hdr{display:flex;align-items:center;justify-content:space-between;padding:18px 20px 10px}
    .tag{font-weight:900; font-size: 12px; letter-spacing:1px; padding:6px 10px; border-radius:999px; color:#fff}
    .tag.geo{background:var(--accent2)}
    .tag.cul{background:var(--accent)}
    .tag.his{background:var(--accent3)}
    .tag.sig{background:var(--accent4)}
    .tag.food{background:var(--accent5)}

    .content{padding:0 20px 18px; line-height:1.75}
    .content p{margin:.2rem 0 .6rem}
    .content ul{margin:.4rem 0 .2rem 1.1rem}
    .content li{margin:.2rem 0}
    .mut{color:var(--muted); font-size:14px}

    .hero{
      height: 320px; background:#ddd center/cover no-repeat; position:relative
    }
    .hero .cap{
      position:absolute; bottom:10px; right:10px; font-size:12px; background:rgba(0,0,0,.5); color:#fff; padding:6px 10px; border-radius:10px
    }

    .gallery{display:grid;grid-template-columns:repeat(2,1fr); gap:10px; padding:10px}
    .gallery img{width:100%;height:170px;object-fit:cover;border-radius:16px;display:block;transition:transform .3s ease;}
    .gallery img:hover{transform: scale(1.03)}

    .foot{
      margin: 20px auto 60px; max-width:1100px; padding: 0 16px; color:#111
    }
    .kbd{font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace; background:#111; color:#fff; padding:3px 8px; border-radius:8px}
  </style>
</head>
<body>
  <header>
    <div class="wrap">
      <h1>探索瑞典！</h1>
      <p class="sub">五彩缤纷 · 丰富多彩 · 认识瑞典！</p>
      <div class="pillbar" id="pillbar">
        <div class="pill active" data-topic="geography">地理 Geography</div>
        <div class="pill" data-topic="culture">文化 Culture</div>
        <div class="pill" data-topic="history">历史 History</div>
        <div class="pill" data-topic="sights">景点 Sights</div>
        <div class="pill" data-topic="food">美食 Food</div>
      </div>
    </div>
  </header>

  <main>
    <!-- LEFT: dynamic card -->
    <section class="grid">
      <article class="card" id="infoCard">
        <div class="hero" id="hero" style="background-image:url('https://upload.wikimedia.org/wikipedia/commons/0/0e/Stockhom_Gamla_Stan_Panorama.jpg')">
          
        </div>
        <div class="hdr">
          <h2 id="title">地理 Geography</h2>
          <span class="tag geo" id="tag">GEO</span>
        </div>
        <div class="content" id="content">
          <p><b>位置：</b>瑞典位于北欧斯堪的纳维亚半岛东部，首都<strong>斯德哥尔摩</strong>。</p>
          <ul>
            <li>全国人口约 <b>1,057 万</b>（2025 估），国土自南到北狭长，森林与湖泊众多。</li>
            <li><b>群岛之都：</b>斯德哥尔摩外海拥有 <b>3 万+</b> 岛屿、礁石与小岛。</li>
            <li><b>千湖之国：</b>瑞典有 <b>22,600</b> 个面积 ≥0.1 km² 的湖泊，8万+ 面积≥2英亩的湖泊。</li>
          </ul>
          <p class="mut">小趣闻：群岛中的 <span class="kbd">Ytterby</span> 小村为 4 种元素命名地（Y、Yb、Tb、Er）。</p>
        </div>
      </article>

      <!-- RIGHT: image gallery -->
      <aside class="card">
        <div class="hdr" style="padding-bottom:0">
          <h2>一眼爱上瑞典 · 图片墙</h2>
          <span class="tag sig">PHOTO</span>
        </div>
        <div class="gallery">
          <img src="https://upload.wikimedia.org/wikipedia/commons/0/0e/Stockhom_Gamla_Stan_Panorama.jpg" alt="斯德哥尔摩全景">
          <img src="https://www.swedishlapland.com/wp-content/uploads/resized/1b/5763_TLogart_1920x1080_1920x1080_6191c9f5645e9a8c1ea165816c662adb.jpg" alt="阿比斯库极光">
          <img src="https://cdn.britannica.com/81/254381-050-93642A37/Royal-Warship-Vasa-Vasamuseet-museum-Djurgarden-Stockholm-Sweden.jpg" alt="瓦萨战船">
          <img src="https://img.freepik.com/premium-photo/swedish-meatballs-cream-sauce-potatoes-lingonberry-sauce-swedish-cuisine-recipe_97840-4627.jpg" alt="瑞典肉丸 Köttbullar">
 <img src="https://cms.sweden.se/app/uploads/2021/05/cinnamon-buns-1-e1724337077140.jpg" alt="肉桂卷 kanelbullar">

        </div>
      </aside>
    </section>
  </main>

  <section class="foot">
    <p>💡 操作提示：点击顶部五个彩色小主题标签，可在左侧卡片中切换 <b>地理/文化/历史/景点/美食</b> 内容，标签会随主题切换而<b>动态变色</b>。</p>
  </section>

  <script>
    const topics = {
      geography: {
        title: '地理 Geography', tag: 'GEO', tagClass: 'geo',
        hero: "https://upload.wikimedia.org/wikipedia/commons/0/0e/Stockhom_Gamla_Stan_Panorama.jpg",
        html: `
          <p><b>位置：</b>瑞典位于北欧斯堪的纳维亚半岛东部，首都<strong>斯德哥尔摩</strong>。</p>
          <ul>
            <li>全国人口约 <b>1,057 万</b>（2025 估），国土自南到北狭长，森林与湖泊众多。</li>
            <li><b>群岛之都：</b>斯德哥尔摩外海拥有 <b>3 万+</b> 岛屿、礁石与小岛。</li>
            <li><b>千湖之国：</b>瑞典有 <b>22,600</b> 个面积 ≥0.1 km² 的湖泊，约 <b>97,500</b> 个面积 ≥2 英亩的湖泊。</li>
          </ul>
          <p class="mut">小趣闻：群岛中的 <span class="kbd">Ytterby</span> 小村为 4 种元素命名地（Y、Yb、Tb、Er）。</p>
        `
      },
      culture: {
        title: '文化 Culture', tag: 'CUL', tagClass: 'cul',
        hero: "https://cms.sweden.se/app/uploads/2021/05/cinnamon-buns-1-e1724337077140.jpg",
        html: `
          <p><b>Fika：</b>瑞典人最爱的“咖啡小憩”，配上肉桂卷、曲奇或三明治，讲究的是 <b>慢下来与社交</b>。</p>
          <ul>
            <li><b>Allemansrätten</b>（人人享有的自然通行权）：几乎可在全国自然界自由步行、骑行与露营，但要“<b>不打扰，不破坏</b>”。</li>
            <li>瑞典人热爱自然与平衡的生活方式，
              <span class="kbd">fika</span> 甚至常常写进公司的作息。</li>
          </ul>
          <p class="mut">每年 <b>10 月 4 日</b> 还有“肉桂卷日” 🥐。</p>
        `
      },
      history: {
        title: '历史 History', tag: 'HIS', tagClass: 'his',
        hero: "https://cdn.britannica.com/81/254381-050-93642A37/Royal-Warship-Vasa-Vasamuseet-museum-Djurgarden-Stockholm-Sweden.jpg",
        html: `
          <p><b>瓦萨号战船（Vasa）</b>：1628 年首航仅约 1.3 公里便因顶部过重倾覆沉没，1961 年整体打捞，现陈列于斯德哥尔摩 <b>瓦萨博物馆</b>。</p>
          <ul>
            <li>17 世纪瑞典是波罗的海强权，瓦萨象征着那个时代的雄心与教训。</li>
            <li>博物馆内可看到保存完好的船体雕刻与复原的船员故事。</li>
            <li>瓦萨号不仅是17世纪最强大的瑞典战舰——配备了 64 门铜炮、两层炮台与数百座华丽雕塑——更是在首航 1,300 米即因结构不稳沉没，却因保存完好成为今日世上保存最完好的17世纪船只。</li>

          </ul>
        `
      },
      sights: {
        title: '景点 Sights', tag: 'GO', tagClass: 'sig',
        hero: "https://www.swedishlapland.com/wp-content/uploads/resized/1b/5763_TLogart_1920x1080_1920x1080_6191c9f5645e9a8c1ea165816c662adb.jpg",
        html: `
          <p><b>阿比斯库 Abisko · 极光</b>：位于瑞典拉普兰，晴朗率高，是全球观赏 <b>极光</b> 的热门地点。</p>
          <ul>
            <li><b>极光天空站</b>（Aurora Sky Station）可乘坐缆椅上山观测。</li>
            <li><b>斯德哥尔摩群岛</b>：<b>3 万+</b> 岛屿的航海与徒步天堂，
              夏天可搭渡轮跳岛、冬季可体验海上滑冰。</li>
          </ul>
        `
      },
      food: {
        title: '美食 Food', tag: 'FOOD', tagClass: 'food',
        hero: "https://img.freepik.com/premium-photo/swedish-meatballs-cream-sauce-potatoes-lingonberry-sauce-swedish-cuisine-recipe_97840-4627.jpg",
        html: `
          <p><b>瑞典肉丸 Köttbullar</b>：经典吃法是<b>奶油酱</b> + <b>土豆泥</b> + <b>越橘酱</b>（lingonberry）。</p>
          <ul>
            <li><b>瑞典肉丸 Köttbullar</b>：鲜嫩多汁的肉丸浸润在浓郁奶油棕汁中，搭配绵滑土豆泥和清新微酸的蔓越莓酱，形成咸香、奶香与果酸的完美三重奏。</li>
            <li><b>肉桂卷 Kanelbullar</b>：与 <span class="kbd">fika</span> 绝佳搭档，10 月 4 日就是“肉桂卷日”。</li>
            <li>还有腌鲱鱼、三文鱼、脆饼等北欧风味等你探索！</li>
          </ul>
        `
      }
    };

    const pills = document.querySelectorAll('.pill');
    const infoCard = document.getElementById('infoCard');
    const titleEl = document.getElementById('title');
    const tagEl = document.getElementById('tag');
    const contentEl = document.getElementById('content');
    const heroEl = document.getElementById('hero');

    pills.forEach(p => p.addEventListener('click', () => {
      pills.forEach(x => x.classList.remove('active'));
      p.classList.add('active');
      const key = p.dataset.topic;
      const t = topics[key];
      heroEl.style.opacity = 0;
      infoCard.style.transform = 'translateY(-3px)';
      setTimeout(() => {
        titleEl.textContent = t.title;
        tagEl.textContent = t.tag;
        tagEl.className = 'tag ' + t.tagClass;
        contentEl.innerHTML = t.html;
        heroEl.style.backgroundImage = `url('${t.hero}')`;
        heroEl.style.opacity = 1;
        infoCard.style.transform = 'translateY(0)';
      }, 160);
    }));
  </script>
</body>
</html>
