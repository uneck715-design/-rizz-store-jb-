<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JB¹ TERBUKA BY RIZZ STORE - Jual Beli Akun Game</title>
    <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Rajdhani:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body { font-family: 'Rajdhani', sans-serif; background: #0a0a1a; min-height: 100vh; overflow-x: hidden; }
        .hero-section {
            position: relative; width: 100%; min-height: 100vh;
            background: linear-gradient(135deg, #0f0c29 0%, #302b63 50%, #24243e 100%);
            display: flex; flex-direction: column; align-items: center; justify-content: center;
            padding: 40px 20px;
        }
        .hero-section::before {
            content: ''; position: absolute; top: 0; left: 0; right: 0; bottom: 0;
            background: 
                radial-gradient(circle at 20% 50%, rgba(0, 240, 255, 0.15) 0%, transparent 50%),
                radial-gradient(circle at 80% 50%, rgba(255, 0, 255, 0.15) 0%, transparent 50%),
                radial-gradient(circle at 50% 50%, rgba(255, 107, 53, 0.1) 0%, transparent 50%);
            z-index: 1;
        }
        .particles { position: absolute; top: 0; left: 0; width: 100%; height: 100%; overflow: hidden; z-index: 2; pointer-events: none; }
        .particle { position: absolute; width: 4px; height: 4px; background: #00f0ff; border-radius: 50%; animation: float 6s infinite ease-in-out; box-shadow: 0 0 10px #00f0ff, 0 0 20px #00f0ff; }
        .particle:nth-child(1) { left: 10%; top: 20%; animation-delay: 0s; }
        .particle:nth-child(2) { left: 20%; top: 60%; animation-delay: 1s; background: #ff00ff; box-shadow: 0 0 10px #ff00ff; }
        .particle:nth-child(3) { left: 35%; top: 30%; animation-delay: 2s; }
        .particle:nth-child(4) { left: 50%; top: 70%; animation-delay: 0.5s; background: #ffff00; box-shadow: 0 0 10px #ffff00; }
        .particle:nth-child(5) { left: 65%; top: 25%; animation-delay: 1.5s; }
        .particle:nth-child(6) { left: 80%; top: 55%; animation-delay: 2.5s; background: #ff00ff; box-shadow: 0 0 10px #ff00ff; }
        .particle:nth-child(7) { left: 90%; top: 40%; animation-delay: 3s; }
        .particle:nth-child(8) { left: 45%; top: 15%; animation-delay: 1.8s; background: #00ff88; box-shadow: 0 0 10px #00ff88; }
        @keyframes float { 0%, 100% { transform: translateY(0) scale(1); opacity: 0.6; } 50% { transform: translateY(-30px) scale(1.2); opacity: 1; } }
        .content { position: relative; z-index: 3; text-align: center; width: 100%; max-width: 500px; }
        .logo-text {
            font-family: 'Orbitron', sans-serif; font-size: 48px; font-weight: 900;
            background: linear-gradient(135deg, #00f0ff, #ff00ff, #ff6b35);
            -webkit-background-clip: text; -webkit-text-fill-color: transparent;
            background-clip: text; text-transform: uppercase; letter-spacing: 5px;
            margin-bottom: 10px;
            animation: glow 3s infinite;
        }
        @keyframes glow { 0%, 100% { filter: drop-shadow(0 0 20px rgba(0,240,255,0.5)); } 50% { filter: drop-shadow(0 0 40px rgba(255,0,255,0.5)); } }
        .tagline { font-family: 'Orbitron', sans-serif; font-size: 13px; color: #00f0ff; text-transform: uppercase; letter-spacing: 4px; margin-bottom: 8px; text-shadow: 0 0 20px #00f0ff; animation: pulse 2s infinite; }
        @keyframes pulse { 0%, 100% { opacity: 0.7; } 50% { opacity: 1; } }
        .title { font-family: 'Orbitron', sans-serif; font-size: 28px; font-weight: 900; color: #ffffff; text-transform: uppercase; letter-spacing: 3px; margin-bottom: 5px; text-shadow: 0 0 20px #00f0ff, 0 0 40px #00f0ff, 0 0 80px #00f0ff; }
        .subtitle { font-size: 15px; color: #a0a0c0; margin-bottom: 30px; letter-spacing: 2px; }
        .buttons-container { display: flex; flex-direction: column; align-items: center; gap: 12px; width: 100%; margin-bottom: 20px; }
        .btn-channel {
            display: inline-flex; align-items: center; justify-content: center; gap: 12px;
            background: linear-gradient(135deg, #25D366 0%, #128C7E 100%); color: white;
            text-decoration: none; padding: 16px 35px; border-radius: 50px;
            font-family: 'Orbitron', sans-serif; font-size: 14px; font-weight: 700; text-transform: uppercase; letter-spacing: 2px;
            border: 2px solid rgba(255,255,255,0.2); box-shadow: 0 0 30px rgba(37,211,102,0.4), 0 10px 40px rgba(0,0,0,0.4);
            transition: all 0.3s ease; position: relative; overflow: hidden; width: 100%; max-width: 380px;
        }
        .btn-channel::before { content: ''; position: absolute; top: -50%; left: -50%; width: 200%; height: 200%; background: linear-gradient(45deg, transparent 40%, rgba(255,255,255,0.1) 50%, transparent 60%); animation: shine 3s infinite; }
        @keyframes shine { 0% { transform: translateX(-100%) rotate(45deg); } 100% { transform: translateX(100%) rotate(45deg); } }
        .btn-channel:hover { transform: translateY(-3px) scale(1.03); box-shadow: 0 0 50px rgba(37,211,102,0.6), 0 15px 50px rgba(0,0,0,0.5); }
        .btn-channel svg { width: 22px; height: 22px; fill: white; flex-shrink: 0; }
        .btn-group {
            display: inline-flex; align-items: center; justify-content: center; gap: 12px;
            background: linear-gradient(135deg, #ff6b35 0%, #ff006e 100%); color: white;
            text-decoration: none; padding: 16px 35px; border-radius: 50px;
            font-family: 'Orbitron', sans-serif; font-size: 14px; font-weight: 700; text-transform: uppercase; letter-spacing: 2px;
            border: 2px solid rgba(255,255,255,0.2); box-shadow: 0 0 30px rgba(255,107,53,0.4), 0 10px 40px rgba(0,0,0,0.4);
            transition: all 0.3s ease; position: relative; overflow: hidden; width: 100%; max-width: 380px;
        }
        .btn-group::before { content: ''; position: absolute; top: -50%; left: -50%; width: 200%; height: 200%; background: linear-gradient(45deg, transparent 40%, rgba(255,255,255,0.1) 50%, transparent 60%); animation: shine 3s infinite; }
        .btn-group:hover { transform: translateY(-3px) scale(1.03); box-shadow: 0 0 50px rgba(255,107,53,0.6), 0 15px 50px rgba(0,0,0,0.5); }
        .btn-group svg { width: 22px; height: 22px; fill: white; flex-shrink: 0; }
        .btn-contact {
            display: inline-flex; align-items: center; justify-content: center; gap: 10px;
            background: transparent; color: #00f0ff; text-decoration: none; padding: 12px 30px; border-radius: 50px;
            font-family: 'Rajdhani', sans-serif; font-size: 14px; font-weight: 700; letter-spacing: 2px;
            border: 2px solid #00f0ff; box-shadow: 0 0 20px rgba(0,240,255,0.2), inset 0 0 20px rgba(0,240,255,0.05);
            transition: all 0.3s ease; width: 100%; max-width: 380px;
        }
        .btn-contact:hover { background: rgba(0,240,255,0.1); transform: translateY(-2px); box-shadow: 0 0 40px rgba(0,240,255,0.4), inset 0 0 30px rgba(0,240,255,0.1); }
        .info-box { background: rgba(10,10,30,0.8); border: 1px solid rgba(0,240,255,0.3); border-radius: 20px; padding: 20px; margin-top: 15px; backdrop-filter: blur(10px); box-shadow: 0 0 40px rgba(0,240,255,0.1); }
        .info-title { font-family: 'Orbitron', sans-serif; font-size: 13px; color: #ff00ff; text-transform: uppercase; letter-spacing: 3px; margin-bottom: 12px; text-shadow: 0 0 15px #ff00ff; }
        .game-list { display: flex; flex-wrap: wrap; justify-content: center; gap: 8px; margin-bottom: 12px; }
        .game-tag { background: rgba(0,240,255,0.1); border: 1px solid rgba(0,240,255,0.4); color: #00f0ff; padding: 5px 14px; border-radius: 20px; font-size: 12px; font-weight: 600; letter-spacing: 1px; }
        .wa-number { font-family: 'Orbitron', sans-serif; font-size: 16px; color: #25D366; margin-top: 8px; text-shadow: 0 0 15px rgba(37,211,102,0.5); }
        .footer { margin-top: 15px; font-size: 11px; color: #555; letter-spacing: 2px; }
        .glitch { position: relative; }
        .glitch::before, .glitch::after { content: 'JB¹ TERBUKA'; position: absolute; top: 0; left: 0; width: 100%; height: 100%; }
        .glitch::before { color: #ff00ff; animation: glitch-1 2s infinite; clip-path: polygon(0 0, 100% 0, 100% 45%, 0 45%); }
        .glitch::after { color: #00f0ff; animation: glitch-2 2s infinite; clip-path: polygon(0 55%, 100% 55%, 100% 100%, 0 100%); }
        @keyframes glitch-1 { 0%, 100% { transform: translate(0); } 20% { transform: translate(-3px, 2px); } 40% { transform: translate(3px, -2px); } }
        @keyframes glitch-2 { 0%, 100% { transform: translate(0); } 20% { transform: translate(3px, -2px); } 40% { transform: translate(-3px, 2px); } }
        @media (max-width: 480px) {
            .logo-text { font-size: 36px; } .title { font-size: 22px; } .tagline { font-size: 10px; letter-spacing: 2px; }
            .btn-channel, .btn-group { padding: 14px 25px; font-size: 12px; } .btn-contact { padding: 10px 20px; font-size: 12px; }
            .hero-section { padding: 30px 15px; }
        }
    </style>
</head>
<body>
    <div class="hero-section">
        <div class="particles">
            <div class="particle"></div><div class="particle"></div><div class="particle"></div><div class="particle"></div>
            <div class="particle"></div><div class="particle"></div><div class="particle"></div><div class="particle"></div>
        </div>
        <div class="content">
            <div class="logo-text">RIZZ STORE X</div>
            <div class="tagline">⚡ Trusted Gaming Store ⚡</div>
            <h1 class="title glitch">JB¹ TERBUKA</h1>
            <p class="subtitle">BY RIZZ STORE</p>
            <div class="buttons-container">
                <a href="https://whatsapp.com/channel/0029Vb8G55F9Gv7WOQa1zy2O" class="btn-channel" target="_blank">
                    <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z"/></svg>
                    📢 Ikuti Saluran WhatsApp
                </a>
                <a href="https://chat.whatsapp.com/FOkUxtXBIDdASzqhkS0rZK" class="btn-group" target="_blank">
                    <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M16 11c1.66 0 2.99-1.34 2.99-3S17.66 5 16 5c-1.66 0-3 1.34-3 3s1.34 3 3 3zm-8 0c1.66 0 2.99-1.34 2.99-3S9.66 5 8 5C6.34 5 5 6.34 5 8s1.34 3 3 3zm0 2c-2.33 0-7 1.17-7 3.5V19h14v-2.5c0-2.33-4.67-3.5-7-3.5zm8 0c-.29 0-.62.02-.97.05 1.16.84 1.97 1.97 1.97 3.45V19h6v-2.5c0-2.33-4.67-3.5-7-3.5z"/></svg>
                    🔥 Masuk Grup JB¹ TERBUKA
                </a>
                <a href="https://wa.me/6289676044329" class="btn-contact" target="_blank">📱 Chat Admin Langsung</a>
            </div>
            <div class="info-box">
                <div class="info-title">🔥 Game yang Tersedia</div>
                <div class="game-list">
                    <span class="game-tag">Free Fire</span><span class="game-tag">Mobile Legends</span>
                    <span class="game-tag">PUBG Mobile</span><span class="game-tag">COD Mobile</span>
                    <span class="game-tag">Genshin Impact</span>
                </div>
                <div class="wa-number">📞 0896-7604-4329</div>
            </div>
            <div class="footer">© 2026 JB¹ TERBUKA BY RIZZ STORE | ALL RIGHTS RESERVED</div>
        </div>
    </div>
</body>
</html>
