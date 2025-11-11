<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Krishna — Profile Demo</title>
  <style>
    :root{
      --bg:#0b1020; --card:#0f1724; --muted:#9aa7c7;
    }
    *{box-sizing:border-box;font-family:Inter,ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,"Helvetica Neue",Arial;}
    body{margin:0; background:linear-gradient(180deg,#07102a 0%, #0b1020 100%); color:#e6eef8; display:flex; align-items:center; justify-content:center; min-height:100vh; padding:24px;}
    .card{width:920px; max-width:100%; background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01)); border-radius:16px; padding:28px; display:grid; grid-template-columns:120px 1fr; gap:20px; box-shadow: 0 10px 40px rgba(3,6,23,0.6);}
    .avatar{width:120px;height:120px;border-radius:12px;background:linear-gradient(135deg,#0ea5a0,#60a5fa); display:flex;align-items:center;justify-content:center;font-weight:700;font-size:26px; color:#021126;}
    .meta h1{margin:0;font-size:28px;}
    .meta p{color:var(--muted); margin:6px 0 12px;}
    .badges{display:flex; gap:8px; flex-wrap:wrap;}
    .btn{padding:8px 12px;border-radius:8px;background:#0ea5a0;color:#021126;text-decoration:none;font-weight:600;}
    .stats{display:flex; gap:12px; margin-top:12px;}
    .stat{background:rgba(255,255,255,0.02); padding:10px 12px;border-radius:10px; min-width:110px; text-align:center;}
    .muted{color:var(--muted); font-size:13px;}
    .typing{font-weight:700; color:#a5f3fc;}
    .controls{display:flex; gap:10px; align-items:center; margin-top:16px;}
  </style>
</head>
<body>
  <div class="card" role="region" aria-label="Profile card demo">
    <div>
      <div class="avatar" id="avatar">KR</div>
    </div>

    <div class="meta">
      <h1 id="name">Krishna <span class="muted">• Maker</span></h1>
      <p class="muted">I build small tools, bots and weird prototypes. Focus: JavaScript, UI, automation.</p>

      <div class="badges">
        <a href="#" class="btn" id="cta">Visit portfolio</a>
        <a href="#" class="btn" id="repo">View repos</a>
      </div>

      <div class="stats">
        <div class="stat">
          <div class="muted">Commits</div>
          <div id="commits" style="font-weight:800; font-size:18px;">0</div>
        </div>
        <div class="stat">
          <div class="muted">Projects</div>
          <div id="projects" style="font-weight:800; font-size:18px;">0</div>
        </div>
        <div class="stat">
          <div class="muted">Followers</div>
          <div id="followers" style="font-weight:800; font-size:18px;">0</div>
        </div>
      </div>

      <div class="controls">
        <div class="muted">Status:</div>
        <div class="typing" id="status">loading...</div>
      </div>
    </div>
  </div>

  <script src="script.js"></script>
</body>
</html>
