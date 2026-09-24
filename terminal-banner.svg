<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Sharanya Shetty</title>
<link href="https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap" rel="stylesheet">
<style>
  * { box-sizing: border-box; margin: 0; padding: 0; }
  body {
    min-height: 100vh; background: #1b1b1b;
    display: flex; align-items: center; justify-content: center;
    overflow-x: hidden;
  }
  .wrap { overflow: hidden; flex: none; }
  .scene { transform-origin: top left; }
  .scene {
    position: relative; flex: none;
    width: 900px; height: 260px; overflow: hidden;
    background: linear-gradient(#79c0ff 0 120px, #8fcbff 120px);
  }
  .scene div { position: absolute; }

  /* sun + clouds */
  .sun { left: 790px; top: 24px; width: 44px; height: 44px; background: #ffe66d; box-shadow: inset 0 0 0 8px #fff3a3; }
  .cloud { background: #fff; width: 80px; height: 16px; animation: drift 45s linear infinite; }
  .cloud::before { content: ""; position: absolute; left: 16px; top: -16px; width: 48px; height: 16px; background: #fff; }
  .c1 { top: 30px; }
  .c2 { top: 80px; transform: scale(.8); animation-duration: 60s; animation-delay: -25s; }
  @keyframes drift { from { left: -120px; } to { left: 960px; } }

  /* ground */
  .grass { left: 0; top: 200px; width: 100%; height: 16px; background: #5da130; border-top: 4px solid #7bc043; }
  .dirt  { left: 0; top: 216px; width: 100%; height: 44px;
    background:
      linear-gradient(#6f4e35,#6f4e35) 30px 8px / 16px 16px no-repeat,
      linear-gradient(#6f4e35,#6f4e35) 260px 10px / 16px 16px no-repeat,
      linear-gradient(#6f4e35,#6f4e35) 510px 8px / 16px 16px no-repeat,
      linear-gradient(#6f4e35,#6f4e35) 770px 10px / 16px 16px no-repeat,
      linear-gradient(#7f7f7f,#7f7f7f) 80px 16px / 12px 12px no-repeat,
      linear-gradient(#7f7f7f,#7f7f7f) 580px 14px / 12px 12px no-repeat,
      #866043; }

  /* scrolling scenery */
  .tree { left: 0; top: 88px; width: 16px; height: 112px; animation: scroll 12s linear infinite; }
  .tree .trunk { left: 0; top: 64px; width: 16px; height: 48px; background: #6b4a2b; }
  .tree .leaves { left: -24px; top: 16px; width: 64px; height: 48px; background: #3f8f2e; }
  .tree .top { left: -8px; top: 0; width: 32px; height: 16px; background: #4fa83b; }
  .t2 { animation-delay: -6s; }
  .flower { left: 0; top: 176px; width: 12px; height: 24px; animation: scroll 8s linear infinite; }
  .flower .stem { left: 4px; top: 8px; width: 4px; height: 16px; background: #3f8f2e; }
  .flower .bloom { left: 0; top: 0; width: 12px; height: 8px; background: #e63946; }
  .f2 { animation-delay: -4s; } .f2 .bloom { background: #ffd166; }
  @keyframes scroll { from { transform: translateX(960px); } to { transform: translateX(-120px); } }

  /* the girl: origin (0,0) = center of head top */
  .girl { left: 150px; top: 72px; width: 0; height: 0; }
  .bob { animation: bob .6s ease-in-out infinite; }
  @keyframes bob { 50% { transform: translateY(-3px); } }
  .girl div { position: absolute; }

  .hairback { left: -20px; top: -2px; width: 40px; height: 70px; background: #3a2214;
    transform-origin: 50% 0; animation: sway 1.2s ease-in-out infinite; }
  @keyframes sway { 0%,100% { transform: rotate(2deg); } 50% { transform: rotate(-2deg); } }

  .arm, .leg { transform-origin: 50% 2px; animation: swing 1.2s ease-in-out infinite; }
  .arm { top: 36px; width: 16px; height: 44px; background: #f0bd97; }
  .arm .sleeve { left: 0; top: 0; width: 16px; height: 12px; background: #b56ee8; }
  .arm.back  { left: -32px; }
  .arm.front { left: 16px; animation-direction: reverse; }
  .leg { top: 80px; width: 16px; height: 48px; background: #f0bd97; transform-origin: 50% 0; }
  .leg .boot { left: 0; top: 36px; width: 16px; height: 12px; background: #5a3b7a; }
  .leg.l { left: -16px; animation-direction: reverse; }
  .leg.r { left: 0; }
  @keyframes swing { from { transform: rotate(28deg); } to { transform: rotate(-28deg); } }

  .shirt { left: -16px; top: 32px; width: 32px; height: 44px; background: #b56ee8; border-top: 4px solid #d29bf5; }
  .skirt { left: -20px; top: 68px; width: 40px; height: 22px; background: #ff8fc0; border-bottom: 6px solid #ff6fa8; }

  .head  { left: -16px; top: 0; width: 32px; height: 32px; background: #f7c9a6; }
  .head div { position: absolute; }
  .hair-t { left: 0; top: 0; width: 32px; height: 8px; background: #4b2e1a; }
  .hair-l { left: 0; top: 8px; width: 4px; height: 30px; background: #4b2e1a; }
  .hair-r { right: 0; top: 8px; width: 4px; height: 30px; background: #4b2e1a; }
  .fringe-l { left: 0; top: 8px; width: 8px; height: 4px; background: #4b2e1a; }
  .fringe-r { right: 0; top: 8px; width: 8px; height: 4px; background: #4b2e1a; }
  .bow { left: 22px; top: -6px; width: 14px; height: 10px; background: #ff4d94; }
  .bow::after { content: ""; position: absolute; left: 4px; top: 4px; width: 6px; height: 4px; background: #ffd1e6; }
  .lash { top: 14px; width: 8px; height: 2px; background: #2b1a10; }
  .eye  { top: 16px; width: 8px; height: 4px; background: #fff; }
  .eye::after { content: ""; position: absolute; top: 0; width: 4px; height: 4px; background: #8e44ad; }
  .eye.l::after { right: 0; } .eye.r::after { left: 0; }
  .blush { top: 22px; width: 4px; height: 2px; background: #ff9aa8; }
  .mouth { left: 12px; top: 26px; width: 8px; height: 2px; background: #c0575e; }
  .corner { top: 24px; width: 2px; height: 2px; background: #c0575e; }

  /* typed text */
  .text { left: 290px; top: 52px; font-family: 'Press Start 2P', 'Courier New', monospace; color: #fff; }
  .scene .text .line { position: relative; overflow: hidden; white-space: nowrap; width: 0; text-shadow: 3px 3px 0 #1b1b1b; }
  .l1 { font-size: 26px; line-height: 40px; animation: type1 7s steps(16) infinite; }
  .l2 { font-size: 13px; line-height: 30px; color: #ffe66d; animation: type2 7s steps(26) infinite; }
  @keyframes type1 { 0% { width: 0; } 45% { width: 16ch; } 92% { width: 16ch; } 100% { width: 0; } }
  @keyframes type2 { 0%, 15% { width: 0; } 60% { width: 26ch; } 92% { width: 26ch; } 100% { width: 0; } }
</style>
</head>
<body>
  <div class="wrap" id="wrap">
  <div class="scene" id="scene">
    <div class="sun"></div>
    <div class="cloud c1"></div>
    <div class="cloud c2"></div>

    <div class="grass"></div>
    <div class="dirt"></div>

    <div class="tree"><div class="trunk"></div><div class="leaves"></div><div class="top"></div></div>
    <div class="tree t2"><div class="trunk"></div><div class="leaves"></div><div class="top"></div></div>
    <div class="flower"><div class="stem"></div><div class="bloom"></div></div>
    <div class="flower f2"><div class="stem"></div><div class="bloom"></div></div>

    <div class="girl"><div class="bob" style="left:0;top:0">
      <div class="hairback"></div>
      <div class="arm back"><div class="sleeve"></div></div>
      <div class="leg l"><div class="boot"></div></div>
      <div class="leg r"><div class="boot"></div></div>
      <div class="shirt"></div>
      <div class="skirt"></div>
      <div class="head">
        <div class="hair-t"></div><div class="hair-l"></div><div class="hair-r"></div>
        <div class="fringe-l"></div><div class="fringe-r"></div>
        <div class="lash" style="left:4px"></div><div class="eye l" style="left:4px"></div>
        <div class="lash" style="left:20px"></div><div class="eye r" style="left:20px"></div>
        <div class="blush" style="left:4px"></div><div class="blush" style="left:24px"></div>
        <div class="corner" style="left:10px"></div><div class="mouth"></div><div class="corner" style="left:20px"></div>
        <div class="bow"></div>
      </div>
      <div class="arm front"><div class="sleeve"></div></div>
    </div></div>

    <div class="text">
      <div class="line l1">Hi, I'm Sharanya</div>
      <div class="line l2">backend * blockchain * DSA</div>
    </div>
  </div>
  </div>
<script>
  // scale the 900x260 scene to fit small screens (phones) without cutting the girl off
  function fit() {
    var s = Math.max(0.6, Math.min(1, window.innerWidth / 900));
    document.getElementById('scene').style.transform = 'scale(' + s + ')';
    var w = document.getElementById('wrap');
    w.style.width  = Math.min(window.innerWidth, 900 * s) + 'px';
    w.style.height = 260 * s + 'px';
  }
  fit(); window.addEventListener('resize', fit);
</script>
</body>
</html>
