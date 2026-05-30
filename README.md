# social
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fabio Alexandre — Redes Sociais</title>
    <link href="https://fonts.googleapis.com/css2?family=Syne:wght@400;600;800&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet">
    <style>
        *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

        :root {
            --bg: #0d0d0d;
            --surface: #161616;
            --border: rgba(255,255,255,0.08);
            --text: #f0ede8;
            --muted: #888;
            --accent: #c8f135;
        }

        body {
            background: var(--bg);
            color: var(--text);
            font-family: 'DM Sans', sans-serif;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            padding: 60px 20px;
        }

        .container {
            width: 100%;
            max-width: 480px;
        }

        /* hero */
        .hero {
            text-align: center;
            margin-bottom: 48px;
            animation: fadeUp 0.6s ease both;
        }

        .avatar-wrap {
            position: relative;
            display: inline-block;
            margin-bottom: 20px;
        }

        .avatar-wrap img {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            object-fit: cover;
            border: 2px solid var(--border);
            display: block;
        }

        .avatar-ring {
            position: absolute;
            inset: -6px;
            border-radius: 50%;
            border: 1.5px solid var(--accent);
            opacity: 0.6;
            animation: pulse 3s ease-in-out infinite;
        }

        @keyframes pulse {
            0%, 100% { transform: scale(1); opacity: 0.6; }
            50% { transform: scale(1.06); opacity: 0.2; }
        }

        .hero h1 {
            font-family: 'Syne', sans-serif;
            font-size: 28px;
            font-weight: 800;
            letter-spacing: -0.02em;
            margin-bottom: 8px;
        }

        .hero h1 span { color: var(--accent); }

        .hero p {
            font-size: 14px;
            color: var(--muted);
            line-height: 1.6;
            max-width: 320px;
            margin: 0 auto;
        }

        /* section title */
        .section-title {
            font-family: 'Syne', sans-serif;
            font-size: 11px;
            font-weight: 600;
            letter-spacing: 0.12em;
            text-transform: uppercase;
            color: var(--muted);
            margin-bottom: 14px;
        }

        /* social links */
        .links { display: flex; flex-direction: column; gap: 10px; margin-bottom: 40px; }

        .link-card {
            display: flex;
            align-items: center;
            gap: 16px;
            background: var(--surface);
            border: 1px solid var(--border);
            border-radius: 14px;
            padding: 14px 18px;
            text-decoration: none;
            color: var(--text);
            transition: border-color 0.2s, transform 0.15s, background 0.2s;
            animation: fadeUp 0.5s ease both;
        }

        .link-card:hover {
            border-color: rgba(200, 241, 53, 0.35);
            background: #1a1a1a;
            transform: translateY(-2px);
        }

        .link-card:active { transform: scale(0.98); }

        .link-icon {
            width: 40px;
            height: 40px;
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            flex-shrink: 0;
        }

        .link-icon img {
            width: 22px;
            height: 22px;
            object-fit: contain;
            filter: brightness(0) invert(1);
        }

        /* fallback SVG icons inline */
        .link-icon svg { width: 22px; height: 22px; }

        .ig-bg { background: linear-gradient(135deg, #833ab4, #fd1d1d, #fcb045); }
        .x-bg  { background: #1a1a1a; border: 1px solid rgba(255,255,255,0.15); }
        .tt-bg { background: #010101; border: 1px solid rgba(255,255,255,0.15); }
        .yt-bg { background: #ff0000; }

        .link-info { flex: 1; }
        .link-name {
            font-family: 'Syne', sans-serif;
            font-size: 15px;
            font-weight: 600;
            margin-bottom: 2px;
        }
        .link-desc { font-size: 12px; color: var(--muted); line-height: 1.4; }

        .link-arrow {
            color: var(--muted);
            font-size: 18px;
            transition: color 0.2s, transform 0.2s;
        }
        .link-card:hover .link-arrow { color: var(--accent); transform: translateX(3px); }

        /* stagger */
        .link-card:nth-child(1) { animation-delay: 0.15s; }
        .link-card:nth-child(2) { animation-delay: 0.25s; }
        .link-card:nth-child(3) { animation-delay: 0.35s; }
        .link-card:nth-child(4) { animation-delay: 0.45s; }

        @keyframes fadeUp {
            from { opacity: 0; transform: translateY(18px); }
            to   { opacity: 1; transform: translateY(0); }
        }

        footer {
            text-align: center;
            font-size: 12px;
            color: #444;
            padding-top: 12px;
            border-top: 1px solid var(--border);
        }
    </style>
</head>
<body>
<div class="container">

    <div class="hero">
        <div class="avatar-wrap">
            <img src="eu - Copia.jpg" alt="Foto de Fabio Alexandre">
            <div class="avatar-ring"></div>
        </div>
        <h1>Fabio <span>Alexandre</span></h1>
        <p>17 anos · futuro programador Python. Acompanha minha jornada nas redes!</p>
    </div>

    <p class="section-title">Minhas redes sociais</p>

    <div class="links">

        <a href="https://www.instagram.com/fabin0_0_0/" target="_blank" rel="noopener" class="link-card">
            <div class="link-icon ig-bg">
                <svg viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round">
                    <rect x="2" y="2" width="20" height="20" rx="5"/>
                    <circle cx="12" cy="12" r="4"/>
                    <circle cx="17.5" cy="6.5" r="0.5" fill="white" stroke="none"/>
                </svg>
            </div>
            <div class="link-info">
                <div class="link-name">Instagram</div>
                <div class="link-desc">@fabin0_0_0 — fotos e jornada como dev</div>
            </div>
            <span class="link-arrow">→</span>
        </a>

        <a href="https://x.com/itzfabin" target="_blank" rel="noopener" class="link-card">
            <div class="link-icon x-bg">
                <svg viewBox="0 0 24 24" fill="white">
                    <path d="M18.244 2.25h3.308l-7.227 8.26 8.502 11.24H16.17l-4.714-6.231-5.401 6.231H2.746l7.73-8.835L1.254 2.25H8.08l4.258 5.63 5.906-5.63zm-1.161 17.52h1.833L7.084 4.126H5.117z"/>
                </svg>
            </div>
            <div class="link-info">
                <div class="link-name">X (Twitter)</div>
                <div class="link-desc">@itzfabin — repostagens iradas</div>
            </div>
            <span class="link-arrow">→</span>
        </a>

        <a href="https://www.tiktok.com/@itz_fabin" target="_blank" rel="noopener" class="link-card">
            <div class="link-icon tt-bg">
                <svg viewBox="0 0 24 24" fill="white">
                    <path d="M19.59 6.69a4.83 4.83 0 0 1-3.77-4.25V2h-3.45v13.67a2.89 2.89 0 0 1-2.88 2.5 2.89 2.89 0 0 1-2.89-2.89 2.89 2.89 0 0 1 2.89-2.89c.28 0 .54.04.79.1V9.01a6.33 6.33 0 0 0-.79-.05 6.34 6.34 0 0 0-6.34 6.34 6.34 6.34 0 0 0 6.34 6.34 6.34 6.34 0 0 0 6.33-6.34V8.69a8.18 8.18 0 0 0 4.78 1.52V6.76a4.85 4.85 0 0 1-1.01-.07z"/>
                </svg>
            </div>
            <div class="link-info">
                <div class="link-name">TikTok</div>
                <div class="link-desc">@itz_fabin — vídeos e conteúdo</div>
            </div>
            <span class="link-arrow">→</span>
        </a>

        <a href="https://www.youtube.com/@fabioalexandre8342" target="_blank" rel="noopener" class="link-card">
            <div class="link-icon yt-bg">
                <svg viewBox="0 0 24 24" fill="white">
                    <path d="M23 7s-.3-1.9-1.1-2.7c-1.1-1.1-2.3-1.1-2.8-1.2C16.2 3 12 3 12 3s-4.2 0-7.1.1c-.6.1-1.8.1-2.8 1.2C1.3 5.1 1 7 1 7S.7 9.2.7 11.3v2c0 2.1.3 4.3.3 4.3s.3 1.9 1.1 2.7c1.1 1.1 2.5 1.1 3.1 1.1C7.2 21.6 12 21.6 12 21.6s4.2 0 7.1-.2c.6-.1 1.8-.1 2.8-1.2.8-.8 1.1-2.7 1.1-2.7s.3-2.1.3-4.3v-2C23.3 9.2 23 7 23 7zM9.7 15.5v-7.4l7.6 3.7-7.6 3.7z"/>
                </svg>
            </div>
            <div class="link-info">
                <div class="link-name">YouTube</div>
                <div class="link-desc">@fabioalexandre8342 — canal em crescimento</div>
            </div>
            <span class="link-arrow">→</span>
        </a>

    </div>

    <footer>feito por Fabio Alexandre · 2025</footer>

</div>
</body>
</html>
Página de links das minhas redes sociais — feita com HTML e CSS puro.
