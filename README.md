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
