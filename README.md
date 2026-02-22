# Bullom-website-Here is the complete HTML code:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>BULLOM – Sierra Leone's #1 Job & HR Platform</title>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@300;400;500;600;700&family=Playfair+Display:wght@700;800&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet" />
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css" />
  <style>
    :root {
      --primary: #0A2463;
      --primary-mid: #1A3A7E;
      --accent: #E63946;
      --gold: #F4A261;
      --teal: #06B6D4;
      --white: #ffffff;
      --off-white: #F7F8FC;
      --gray-100: #EFF1F7;
      --gray-200: #D8DCE9;
      --gray-400: #9BA3BF;
      --gray-600: #5A627A;
      --gray-800: #2D3247;
      --dark: #0B0F1E;
      --text: #1E2336;
      --text-light: #5A627A;
      --card-shadow: 0 4px 24px rgba(10,36,99,0.08);
      --card-hover: 0 12px 40px rgba(10,36,99,0.16);
      --radius: 12px;
      --radius-sm: 8px;
      --radius-lg: 20px;
      --transition: all 0.25s cubic-bezier(0.4, 0, 0.2, 1);
    }
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
    html { scroll-behavior: smooth; font-size: 16px; }
    body { font-family: 'DM Sans', sans-serif; color: var(--text); background: var(--white); line-height: 1.6; overflow-x: hidden; }
    a { text-decoration: none; color: inherit; }
    ul { list-style: none; }
    img { max-width: 100%; }
    button { cursor: pointer; border: none; outline: none; font-family: inherit; }
    .container { max-width: 1200px; margin: 0 auto; padding: 0 24px; }
    .section-tag { display: inline-flex; align-items: center; gap: 8px; background: rgba(10,36,99,0.07); color: var(--primary); padding: 6px 16px; border-radius: 100px; font-size: 12px; font-weight: 600; letter-spacing: 0.08em; text-transform: uppercase; margin-bottom: 16px; }
    .section-tag .dot { width: 6px; height: 6px; border-radius: 50%; background: var(--accent); }
    .section-title { font-family: 'Playfair Display', serif; font-size: clamp(28px, 4vw, 42px); font-weight: 800; color: var(--dark); line-height: 1.2; margin-bottom: 16px; }
    .section-subtitle { font-size: 17px; color: var(--text-light); max-width: 560px; line-height: 1.7; }
    .btn { display: inline-flex; align-items: center; gap: 8px; padding: 13px 28px; border-radius: var(--radius-sm); font-size: 15px; font-weight: 600; transition: var(--transition); white-space: nowrap; }
    .btn-primary { background: var(--primary); color: var(--white); }
    .btn-primary:hover { background: var(--primary-mid); transform: translateY(-2px); box-shadow: 0 8px 24px rgba(10,36,99,0.3); }
    .btn-outline { background: transparent; color: var(--primary); border: 2px solid var(--primary); }
    .btn-outline:hover { background: var(--primary); color: var(--white); transform: translateY(-2px); }
    .btn-accent { background: var(--accent); color: var(--white); }
    .btn-accent:hover { background: #c0303c; transform: translateY(-2px); box-shadow: 0 8px 24px rgba(230,57,70,0.35); }
    .badge { display: inline-block; padding: 3px 10px; border-radius: 100px; font-size: 11px; font-weight: 700; letter-spacing: 0.04em; }
    .badge-green { background: #D1FAE5; color: #065F46; }
    .badge-blue { background: #DBEAFE; color: #1E40AF; }
    .badge-orange { background: #FEF3C7; color: #92400E; }
    .badge-red { background: #FEE2E2; color: #991B1B; }

    /* ANNOUNCEMENT */
    .announcement-bar { background: var(--primary); color: var(--white); text-align: center; padding: 10px 24px; font-size: 13px; font-weight: 500; display: flex; align-items: center; justify-content: center; gap: 12px; position: relative; }
    .announcement-bar a { color: var(--gold); font-weight: 700; text-decoration: underline; }
    .announcement-bar .close-bar { position: absolute; right: 24px; background: none; color: rgba(255,255,255,0.6); font-size: 18px; line-height: 1; }

    /* NAVBAR */
    .navbar { position: sticky; top: 0; z-index: 1000; background: rgba(255,255,255,0.97); backdrop-filter: blur(16px); border-bottom: 1px solid var(--gray-100); transition: var(--transition); }
    .navbar.scrolled { box-shadow: 0 4px 24px rgba(10,36,99,0.1); }
    .nav-inner { display: flex; align-items: center; justify-content: space-between; height: 70px; gap: 32px; }
    .logo { display: flex; align-items: center; gap: 10px; font-family: 'Playfair Display', serif; font-size: 28px; font-weight: 800; }
    .logo-icon { width: 40px; height: 40px; background: var(--primary); border-radius: 10px; display: flex; align-items: center; justify-content: center; }
    .logo-icon span { color: var(--white); font-family: 'Playfair Display', serif; font-size: 20px; font-weigh
