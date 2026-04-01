<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>The Good Vibes Studio – Head to Toe Beauty, Raipur</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,600;0,700;1,400;1,600&family=DM+Sans:wght@300;400;500;600&family=Great+Vibes&display=swap" rel="stylesheet">

<style>
/* ── TOKENS ───────────────────────────────────────── */
:root{
  --bg-main:#FDF0F7;
  --bg-alt:#F3EEFF;
  --bg-section:#FAE8F5;
  --bg-card:#FFFFFF;
  --bg-card2:#F9F0FF;
  --pink-deep:#C2185B;
  --pink:#E91E8C;
  --pink2:#F06292;
  --pink3:#F8BBD9;
  --pink4:#FDEEF6;
  --purple-deep:#4A148C;
  --purple:#7B1FA2;
  --purple2:#9C27B0;
  --purple3:#CE93D8;
  --purple4:#EDE7F6;
  --text-black:#1A0A2E;
  --text-dark:#2D1B4E;
  --text-mid:#4A2D6B;
  --text-muted:#7B5E9A;
  --gold:#A0720A;
  --gold2:#C89010;
  --gold3:#F5C842;
  --gold-light:#FFF8E1;
  --border:#E1BEF0;
  --border-pink:#F4B8D8;
}

*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
body{font-family:'DM Sans',sans-serif;background:var(--bg-main);color:var(--text-black);overflow-x:hidden;line-height:1.6}
img{display:block;width:100%}
a{text-decoration:none;color:inherit}
ul{list-style:none}
::-webkit-scrollbar{width:5px}
::-webkit-scrollbar-track{background:var(--bg-alt)}
::-webkit-scrollbar-thumb{background:var(--purple2);border-radius:10px}

/* NAV */
nav{
  position:fixed;top:0;left:0;right:0;z-index:500;
  padding:18px 60px;
  display:flex;align-items:center;justify-content:space-between;
  background:rgba(253,240,247,0.95);
  backdrop-filter:blur(20px);-webkit-backdrop-filter:blur(20px);
  border-bottom:1.5px solid var(--border-pink)
}
.nav-logo{
  font-family:'Great Vibes',cursive;font-size:32px;
  background:linear-gradient(135deg,var(--purple),var(--pink));
  -webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text
}
.nav-links{display:flex;gap:32px;align-items:center}
.nav-links a{
  font-size:12px;letter-spacing:1.5px;text-transform:uppercase;
  font-weight:600;color:var(--text-mid);
  transition:color .2s;position:relative;padding-bottom:4px
}
.nav-links a::after{
  content:'';position:absolute;bottom:0;left:50%;right:50%;
  height:2px;background:var(--gold2);border-radius:2px;
  transition:left .3s,right .3s
}
.nav-links a:hover{color:var(--purple)}
.nav-links a:hover::after{left:0;right:0}
.nav-book{
  background:linear-gradient(135deg,var(--purple),var(--pink));
  color:white!important;padding:10px 24px;border-radius:6px;
  font-size:12px!important;letter-spacing:1.5px!important;font-weight:700!important;
  box-shadow:0 4px 16px rgba(123,31,162,.25);
  transition:opacity .2s,transform .2s
}
.nav-book:hover{opacity:.9;transform:translateY(-1px)}
.nav-book::after{display:none!important}

/* HERO */
.hero{position:relative;min-height:100vh;display:flex;align-items:center;justify-content:center;overflow:hidden}
.hero-bg{position:absolute;inset:0;z-index:0}
.hero-bg img{width:100%;height:100%;object-fit:cover;filter:brightness(0.36) saturate(1.3)}
.hero-bg-overlay{
  position:absolute;inset:0;
  background:
    radial-gradient(ellipse 70% 60% at 80% 30%,rgba(156,39,176,.6) 0%,transparent 60%),
    radial-gradient(ellipse 60% 50% at 15% 75%,rgba(233,30,140,.5) 0%,transparent 55%),
    linear-gradient(180deg,rgba(74,20,140,.45) 0%,rgba(194,24,91,.3) 100%)
}
.hero-inner{
  position:relative;z-index:2;
  text-align:center;padding:140px 40px 90px;
  max-width:980px;margin:auto
}
.hero-eyebrow{
  display:inline-flex;align-items:center;gap:12px;
  border:1px solid rgba(245,200,66,.6);border-radius:4px;
  padding:8px 22px;margin-bottom:40px;
  font-size:11px;letter-spacing:3px;text-transform:uppercase;
  color:var(--gold3);background:rgba(180,134,11,.15)
}
.hero-title{
  font-family:'Playfair Display',serif;
  font-size:clamp(48px,8vw,92px);
  line-height:1.04;font-weight:700;color:#FFF;margin-bottom:12px;
  text-shadow:0 2px 24px rgba(0,0,0,.25)
}
.hero-title .hl{
  font-style:italic;
  background:linear-gradient(135deg,var(--gold3),#FFD580);
  -webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text
}
.hero-title .script{
  font-family:'Great Vibes',cursive;font-size:1.05em;
  background:linear-gradient(135deg,#FFD580,var(--pink3));
  -webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text;
  display:block
}
.hero-sub{font-size:16px;font-weight:300;color:rgba(255,255,255,.9);letter-spacing:.5px;margin:28px auto;max-width:600px;line-height:1.9}
.hero-btns{display:flex;gap:16px;justify-content:center;flex-wrap:wrap;margin-top:44px}
.btn-primary{
  background:linear-gradient(135deg,var(--purple),var(--pink));
  color:white;padding:16px 40px;border-radius:6px;
  font-size:13px;letter-spacing:2px;text-transform:uppercase;font-weight:700;
  box-shadow:0 8px 30px rgba(123,31,162,.45);transition:transform .2s,box-shadow .2s
}
.btn-primary:hover{transform:translateY(-3px);box-shadow:0 14px 40px rgba(233,30,140,.5)}
.btn-gold{
  border:2px solid var(--gold3);color:var(--gold3);
  padding:16px 40px;border-radius:6px;
  font-size:13px;letter-spacing:2px;text-transform:uppercase;font-weight:700;
  background:rgba(180,134,11,.15);transition:background .2s,transform .2s
}
.btn-gold:hover{background:rgba(212,160,23,.25);transform:translateY(-3px)}
.hero-stats{
  display:flex;gap:60px;justify-content:center;flex-wrap:wrap;
  margin-top:70px;padding-top:40px;border-top:1px solid rgba(255,255,255,.2)
}
.stat span{
  display:block;font-family:'Playfair Display',serif;font-size:44px;font-weight:700;
  background:linear-gradient(135deg,var(--gold3),#FFD580);
  -webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text
}
.stat p{font-size:11px;letter-spacing:2.5px;text-transform:uppercase;color:rgba(255,255,255,.65);margin-top:6px}

/* MARQUEE */
.marquee-wrap{background:linear-gradient(135deg,var(--purple),#AB47BC,var(--pink));padding:14px 0;overflow:hidden;white-space:nowrap}
.marquee-track{display:inline-flex;animation:marquee 24s linear infinite}
.marquee-track span{font-size:12px;letter-spacing:3.5px;text-transform:uppercase;color:white;font-weight:600;padding:0 32px}
.marquee-track .sep{color:rgba(255,255,255,.4);font-size:8px}
@keyframes marquee{from{transform:translateX(0)}to{transform:translateX(-50%)}}

/* SECTION COMMON */
section{position:relative;padding:100px 60px}
.sec-tag{
  display:inline-flex;align-items:center;gap:10px;
  font-size:11px;letter-spacing:3px;text-transform:uppercase;
  color:var(--pink-deep);font-weight:700;margin-bottom:16px
}
.sec-tag::before{content:'';display:block;width:24px;height:2px;background:var(--gold2);border-radius:2px}
.sec-title{font-family:'Playfair Display',serif;font-size:clamp(34px,4vw,54px);font-weight:700;line-height:1.15;color:var(--text-black)}
.sec-title em{
  font-style:italic;
  background:linear-gradient(135deg,var(--purple),var(--pink));
  -webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text
}
.sec-line{width:60px;height:3px;background:linear-gradient(90deg,var(--gold),var(--gold3));margin:22px 0;border-radius:3px}
.sec-line.c{margin-left:auto;margin-right:auto}
.sec-desc{font-size:15px;font-weight:400;line-height:1.9;color:var(--text-mid);max-width:520px}

/* ABOUT */
.about{
  background:
    radial-gradient(ellipse 60% 60% at 0% 50%,rgba(206,147,216,.3) 0%,transparent 55%),
    var(--bg-alt)
}
.about-grid{display:grid;grid-template-columns:1fr 1fr;gap:80px;align-items:center;max-width:1200px;margin:auto}
.about-img-wrap{position:relative}
.about-frame{
  aspect-ratio:3/4;border-radius:2px 56px 2px 56px;overflow:hidden;
  border:3px solid var(--border);box-shadow:0 30px 80px rgba(123,31,162,.18)
}
.about-frame img{width:100%;height:100%;object-fit:cover}
.about-float{
  position:absolute;bottom:-24px;right:-24px;
  background:white;border-radius:14px;padding:22px 28px;
  border:2px solid var(--border-pink);text-align:center;
  box-shadow:0 16px 40px rgba(156,39,176,.15)
}
.about-float .num{
  font-family:'Playfair Display',serif;font-size:40px;font-weight:700;
  background:linear-gradient(135deg,var(--gold),var(--gold2));
  -webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text
}
.about-float .lbl{font-size:11px;letter-spacing:2px;text-transform:uppercase;color:var(--text-muted)}
.about-accent{position:absolute;top:-24px;left:-24px;width:100px;height:100px;border:2px solid var(--border);border-radius:50%}
.about-content .pills{display:flex;flex-wrap:wrap;gap:8px;margin-top:28px}
.pill{border:1px solid var(--border);border-radius:4px;padding:7px 16px;font-size:11px;letter-spacing:1.5px;text-transform:uppercase;color:var(--purple);background:var(--purple4);font-weight:600}

/* IMAGE BANNER */
.img-banner{width:100%;height:320px;overflow:hidden;position:relative}
.img-banner img{width:100%;height:100%;object-fit:cover}
.img-banner-overlay{position:absolute;inset:0;background:linear-gradient(135deg,rgba(123,31,162,.6),rgba(194,24,91,.45))}
.img-banner-text{position:absolute;inset:0;display:flex;align-items:center;justify-content:center;flex-direction:column;gap:12px;text-align:center;padding:40px}
.img-banner-text h3{font-family:'Playfair Display',serif;font-size:38px;font-weight:700;color:white;text-shadow:0 2px 20px rgba(0,0,0,.25)}
.img-banner-text p{font-size:15px;color:rgba(255,255,255,.85);font-weight:300}

/* SERVICES */
.services-section{
  background:
    radial-gradient(ellipse 70% 50% at 100% 50%,rgba(248,187,217,.4) 0%,transparent 60%),
    var(--bg-main)
}
.services-intro{max-width:1200px;margin:0 auto 64px;display:flex;justify-content:space-between;align-items:flex-end;flex-wrap:wrap;gap:20px}
.svc-categories{max-width:1200px;margin:auto;display:grid;grid-template-columns:repeat(3,1fr);gap:24px}
.svc-cat-card{background:var(--bg-card);border:1.5px solid var(--border);border-radius:16px;overflow:hidden;transition:border-color .3s,transform .3s,box-shadow .3s}
.svc-cat-card:hover{border-color:var(--pink2);transform:translateY(-6px);box-shadow:0 20px 50px rgba(233,30,140,.12)}
.svc-cat-img{height:160px;overflow:hidden;position:relative}
.svc-cat-img img{width:100%;height:100%;object-fit:cover;transition:transform .5s}
.svc-cat-card:hover .svc-cat-img img{transform:scale(1.07)}
.svc-cat-img-overlay{position:absolute;inset:0;background:linear-gradient(to bottom,transparent 30%,rgba(74,20,140,.55) 100%)}
.svc-cat-header{padding:20px 24px 16px;border-bottom:1px solid var(--border);display:flex;align-items:center;gap:12px}
.svc-cat-icon{font-size:24px}
.svc-cat-header h3{font-family:'Playfair Display',serif;font-size:19px;font-weight:700;color:var(--text-black)}
.svc-cat-header p{font-size:12px;color:var(--text-muted);margin-top:2px}
.svc-cat-body{padding:18px 24px 22px}
.svc-item{display:flex;justify-content:space-between;align-items:center;padding:8px 0;border-bottom:1px solid rgba(225,190,240,.4)}
.svc-item:last-child{border:none}
.svc-item-name{font-size:13.5px;color:var(--text-dark);display:flex;align-items:center;gap:8px}
.svc-item-name::before{content:'';display:block;width:5px;height:5px;border-radius:50%;background:linear-gradient(135deg,var(--purple),var(--pink));flex-shrink:0}
.svc-price-tag{font-size:12px;color:var(--gold);font-weight:700;letter-spacing:.5px;white-space:nowrap}

/* BRIDAL */
.bridal{
  background:
    radial-gradient(ellipse 70% 60% at 90% 40%,rgba(206,147,216,.35) 0%,transparent 60%),
    radial-gradient(ellipse 50% 50% at 10% 70%,rgba(248,187,217,.4) 0%,transparent 55%),
    var(--bg-alt)
}
.bridal-inner{max-width:1200px;margin:auto}
.bridal-top{display:grid;grid-template-columns:1fr 1fr;gap:80px;align-items:center;margin-bottom:64px}
.bridal-img{aspect-ratio:4/3;border-radius:2px 56px 2px 56px;overflow:hidden;border:3px solid var(--border-pink);position:relative;box-shadow:0 30px 80px rgba(233,30,140,.18)}
.bridal-img img{width:100%;height:100%;object-fit:cover}
.pkg-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:24px}
.pkg-card{background:var(--bg-card);border:1.5px solid var(--border);border-radius:16px;padding:34px 26px;transition:transform .3s,border-color .3s,box-shadow .3s}
.pkg-card:hover{transform:translateY(-6px);border-color:var(--pink2);box-shadow:0 20px 50px rgba(233,30,140,.12)}
.pkg-card.best{border-color:var(--pink2);background:linear-gradient(160deg,var(--purple4),var(--pink4));position:relative}
.pkg-badge{
  position:absolute;top:-13px;left:50%;transform:translateX(-50%);
  background:linear-gradient(135deg,var(--purple),var(--pink));
  color:white;font-size:10px;letter-spacing:2px;text-transform:uppercase;
  padding:5px 18px;border-radius:4px;font-weight:700;white-space:nowrap
}
.pkg-card h3{font-family:'Playfair Display',serif;font-size:24px;font-weight:700;color:var(--text-black);margin-bottom:6px}
.pkg-subtitle{font-size:12px;color:var(--gold);font-weight:600;letter-spacing:1px;text-transform:uppercase;margin-bottom:20px}
.pkg-features{margin-bottom:28px}
.pkg-features li{font-size:13.5px;color:var(--text-dark);padding:8px 0;border-bottom:1px solid var(--border);display:flex;gap:10px;align-items:center}
.pkg-features li:last-child{border:none}
.pkg-features li::before{content:'✦';color:var(--pink);font-size:9px;flex-shrink:0}
.pkg-cta{
  display:block;text-align:center;
  background:linear-gradient(135deg,#25D366,#128C7E);
  color:white;padding:13px 20px;border-radius:8px;
  font-size:12px;letter-spacing:1.5px;text-transform:uppercase;font-weight:700;
  box-shadow:0 4px 16px rgba(37,211,102,.3);transition:opacity .2s,transform .2s
}
.pkg-cta:hover{opacity:.9;transform:translateY(-2px)}

/* GALLERY */
.gallery{
  background:
    radial-gradient(ellipse 60% 60% at 100% 0%,rgba(248,187,217,.35) 0%,transparent 55%),
    var(--bg-section)
}
.gallery-header{display:flex;justify-content:space-between;align-items:flex-end;max-width:1200px;margin:0 auto 48px;flex-wrap:wrap;gap:20px}
.gallery-grid{display:grid;grid-template-columns:repeat(4,1fr);grid-template-rows:auto auto;gap:16px;max-width:1200px;margin:auto}
.g-item{position:relative;overflow:hidden;border-radius:14px;border:2px solid var(--border-pink);cursor:pointer}
.g-item-1{grid-column:span 2;grid-row:span 2}
.g-item img{width:100%;height:100%;object-fit:cover;min-height:200px;transition:transform .6s}
.g-item-1 img{min-height:420px}
.g-item:hover img{transform:scale(1.07)}
.g-overlay{position:absolute;inset:0;background:linear-gradient(to top,rgba(74,20,140,.8) 0%,transparent 60%);display:flex;align-items:flex-end;padding:20px;opacity:0;transition:opacity .3s}
.g-item:hover .g-overlay{opacity:1}
.g-overlay span{font-size:13px;letter-spacing:2px;text-transform:uppercase;color:white;font-weight:600}

/* GALLERY FILTERS */
.gallery-filters{display:flex;flex-wrap:wrap;gap:10px;max-width:1200px;margin:0 auto 40px;justify-content:center}
.g-filter{
  padding:9px 20px;border-radius:6px;font-size:11px;letter-spacing:1.5px;text-transform:uppercase;
  font-weight:700;cursor:pointer;border:1.5px solid var(--border);
  background:transparent;color:var(--text-mid);transition:all .25s;font-family:'DM Sans',sans-serif
}
.g-filter:hover,.g-filter.active{
  background:linear-gradient(135deg,var(--purple),var(--pink));
  color:white;border-color:transparent;
  box-shadow:0 4px 16px rgba(123,31,162,.3)
}
.g-item{transition:opacity .35s,transform .35s}
.g-item.hidden{opacity:0;pointer-events:none;transform:scale(0.92);display:none}
.g-cat-label{
  position:absolute;top:12px;left:12px;z-index:2;
  background:rgba(74,20,140,.82);backdrop-filter:blur(6px);
  color:white;font-size:10px;letter-spacing:2px;text-transform:uppercase;
  padding:5px 12px;border-radius:4px;font-weight:700;
  border:1px solid rgba(255,255,255,.25)
}

/* TESTIMONIALS */
.testimonials{
  background:
    radial-gradient(ellipse 60% 60% at 0% 50%,rgba(206,147,216,.25) 0%,transparent 55%),
    var(--bg-alt)
}
.testi-header{text-align:center;margin-bottom:60px}
.testi-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:24px;max-width:1200px;margin:auto}
.testi-card{background:var(--bg-card);border:1.5px solid var(--border);border-radius:16px;padding:32px 28px;transition:border-color .3s,box-shadow .3s}
.testi-card:hover{border-color:var(--pink2);box-shadow:0 16px 40px rgba(233,30,140,.1)}
.stars{color:var(--gold2);font-size:18px;letter-spacing:2px;margin-bottom:16px}
.testi-card p{font-size:14px;color:var(--text-mid);line-height:1.8;font-weight:300;margin-bottom:24px;font-style:italic}
.testi-author{display:flex;align-items:center;gap:14px}
.testi-avatar{width:48px;height:48px;border-radius:50%;overflow:hidden;border:2px solid var(--border-pink);flex-shrink:0}
.testi-name{font-size:14px;font-weight:700;color:var(--text-black)}
.testi-role{font-size:12px;color:var(--text-muted);margin-top:2px}

/* PROCESS */
.process{
  background:
    radial-gradient(ellipse 70% 60% at 50% 100%,rgba(248,187,217,.4) 0%,transparent 60%),
    var(--bg-main)
}
.process-inner{max-width:1200px;margin:auto}
.process-img{width:100%;height:280px;border-radius:16px;overflow:hidden;margin:48px 0;position:relative;border:2px solid var(--border-pink)}
.process-img img{width:100%;height:100%;object-fit:cover}
.process-img::after{content:'';position:absolute;inset:0;background:linear-gradient(135deg,rgba(123,31,162,.25),rgba(194,24,91,.15))}
.steps{display:grid;grid-template-columns:repeat(4,1fr);gap:32px;max-width:1200px;margin:0 auto;position:relative}
.steps::before{content:'';position:absolute;top:44px;left:12.5%;right:12.5%;height:2px;background:linear-gradient(90deg,var(--purple),var(--pink));z-index:0;border-radius:2px}
.step{text-align:center;position:relative;z-index:1}
.step-num{font-size:11px;letter-spacing:3px;color:var(--text-muted);text-transform:uppercase;margin-bottom:8px;font-weight:600}
.step-icon{width:52px;height:52px;border-radius:50%;background:linear-gradient(135deg,var(--purple),var(--pink));display:flex;align-items:center;justify-content:center;font-size:22px;margin:0 auto 20px;box-shadow:0 8px 24px rgba(123,31,162,.3)}
.step h4{font-size:16px;font-weight:700;color:var(--text-black);margin-bottom:10px}
.step p{font-size:13.5px;color:var(--text-mid);line-height:1.7}

/* CONTACT */
.contact{
  background:
    radial-gradient(ellipse 60% 60% at 100% 50%,rgba(248,187,217,.35) 0%,transparent 55%),
    var(--bg-alt)
}
.contact-inner{display:grid;grid-template-columns:1fr 1fr;gap:72px;max-width:1200px;margin:auto;align-items:start}
.contact-img{width:100%;height:200px;border-radius:12px;overflow:hidden;margin-bottom:32px;border:2px solid var(--border-pink)}
.contact-img img{width:100%;height:100%;object-fit:cover}
.info-item{display:flex;gap:18px;padding:20px 0;border-bottom:1px solid var(--border)}
.info-icon{width:42px;height:42px;border-radius:10px;background:var(--purple4);border:1px solid var(--border);display:flex;align-items:center;justify-content:center;font-size:18px;flex-shrink:0}
.info-label{font-size:11px;letter-spacing:2px;text-transform:uppercase;color:var(--text-muted);margin-bottom:5px;font-weight:600}
.info-val{font-size:14.5px;color:var(--text-dark);line-height:1.6}
.book-card{background:var(--bg-card);border:2px solid var(--border-pink);border-radius:20px;padding:44px 36px;text-align:center;box-shadow:0 20px 60px rgba(233,30,140,.1)}
.book-card h3{font-family:'Playfair Display',serif;font-size:28px;font-weight:700;color:var(--text-black);margin-bottom:16px}
.book-card p{font-size:14px;color:var(--text-mid);line-height:1.8;font-weight:400;margin-bottom:32px}
.wa-btn{
  display:inline-flex;align-items:center;gap:10px;justify-content:center;
  background:linear-gradient(135deg,#25D366,#128C7E);
  color:white;padding:16px 36px;border-radius:8px;width:100%;
  font-size:14px;letter-spacing:1.5px;text-transform:uppercase;font-weight:700;
  box-shadow:0 8px 24px rgba(37,211,102,.3);transition:transform .2s,box-shadow .2s
}
.wa-btn:hover{transform:translateY(-3px);box-shadow:0 14px 36px rgba(37,211,102,.4)}
.social-row{display:flex;gap:12px;margin-top:20px}
.social-btn{flex:1;padding:12px 16px;border-radius:8px;border:1.5px solid var(--border);color:var(--text-mid);font-size:12px;letter-spacing:1px;text-transform:uppercase;text-align:center;transition:background .2s,border-color .2s;font-weight:600}
.social-btn:hover{background:var(--purple4);border-color:var(--purple3)}
.offer-box{margin-top:28px;padding:20px;background:linear-gradient(135deg,var(--gold-light),rgba(245,200,66,.1));border-radius:10px;border:1.5px dashed var(--gold2)}
.offer-label{font-size:11px;letter-spacing:2.5px;text-transform:uppercase;color:var(--gold);margin-bottom:8px;font-weight:700}
.offer-box p{font-size:13.5px;color:var(--text-dark);margin:0}

/* FOOTER */
footer{background:linear-gradient(135deg,var(--purple-deep),#6A0080,var(--pink-deep));padding:64px 60px 36px;text-align:center}
.footer-logo{font-family:'Great Vibes',cursive;font-size:38px;background:linear-gradient(135deg,var(--gold3),#FFD580);-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text;margin-bottom:8px}
.footer-tagline{font-size:11px;letter-spacing:3px;text-transform:uppercase;color:rgba(255,255,255,.6);margin-bottom:36px}
.footer-links{display:flex;gap:32px;justify-content:center;flex-wrap:wrap;margin-bottom:36px}
.footer-links a{font-size:12px;letter-spacing:1.5px;text-transform:uppercase;color:rgba(255,255,255,.6);transition:color .2s;font-weight:500}
.footer-links a:hover{color:var(--gold3)}
.footer-divider{height:1px;background:rgba(255,255,255,.15);margin-bottom:28px}
.footer-copy{font-size:12px;color:rgba(255,255,255,.5)}

/* WA FLOAT */
.wa-float{position:fixed;bottom:32px;right:32px;z-index:400;width:58px;height:58px;border-radius:50%;background:linear-gradient(135deg,#25D366,#128C7E);display:flex;align-items:center;justify-content:center;font-size:26px;box-shadow:0 8px 28px rgba(37,211,102,.5);transition:transform .2s}
.wa-float:hover{transform:scale(1.12)}
.wa-tooltip{position:absolute;right:70px;background:var(--text-black);color:white;font-size:12px;letter-spacing:1px;padding:8px 14px;border-radius:6px;white-space:nowrap;opacity:0;pointer-events:none;transition:opacity .2s}
.wa-float:hover .wa-tooltip{opacity:1}

.fade-up{opacity:0;transform:translateY(30px);transition:opacity .6s,transform .6s}
.fade-up.visible{opacity:1;transform:translateY(0)}

@media(max-width:1024px){.svc-categories{grid-template-columns:repeat(2,1fr)}.pkg-grid{grid-template-columns:1fr 1fr}}
@media(max-width:768px){
  nav{padding:14px 20px}.nav-links{display:none}
  section{padding:72px 22px}
  .about-grid,.bridal-top,.contact-inner{grid-template-columns:1fr;gap:44px}
  .svc-categories,.pkg-grid{grid-template-columns:1fr}
  .gallery-grid{grid-template-columns:repeat(2,1fr)}.g-item-1{grid-column:span 2}
  .testi-grid{grid-template-columns:1fr}
  .steps{grid-template-columns:1fr 1fr;gap:24px}.steps::before{display:none}
  .hero-stats{gap:28px}
  footer{padding:48px 22px 24px}
}
</style>
</head>
<body>

<!-- NAV -->
<nav id="mainNav">
  <div class="nav-logo">The Good Vibes Studio</div>
  <div class="nav-links">
    <a href="#about">About</a>
    <a href="#services">Services</a>
    <a href="#bridal">Bridal</a>
    <a href="#gallery">Gallery</a>
    <a href="#reviews">Reviews</a>
    <a href="#contact" class="nav-book">Book Now</a>
  </div>
</nav>

<!-- HERO -->
<section class="hero" id="home">
  <div class="hero-bg">
    <img src="https://images.unsplash.com/photo-1522335789203-aabd1fc54bc9?w=1600&q=85" alt="Salon">
    <div class="hero-bg-overlay"></div>
  </div>
  <div class="hero-inner">
    <div class="hero-eyebrow"><span>✦</span> Raipur's Premium Beauty Studio <span>✦</span></div>
    <h1 class="hero-title">
      Head to Toe
      <span class="script">Beauty & Beyond</span>
    </h1>
    <p class="hero-sub">Hair · Skin · Nails · Makeup · Body · Mehendi · Bridal — every service you need under one roof. Crafted with care, delivered with luxury.</p>
    <div class="hero-btns">
      <a href="#services" class="btn-primary">Explore All Services</a>
      <a href="https://wa.me/918085306764" class="btn-gold">WhatsApp Us</a>
    </div>
    <div class="hero-stats">
      <div class="stat"><span>6+</span><p>Years Experience</p></div>
      <div class="stat"><span>500+</span><p>Happy Brides</p></div>
      <div class="stat"><span>15+</span><p>Services Offered</p></div>
      <div class="stat"><span>4.9★</span><p>Client Rating</p></div>
    </div>
  </div>
</section>

<!-- MARQUEE -->
<div class="marquee-wrap">
  <div class="marquee-track">
    <span>Hair Services</span><span class="sep">✦</span><span>Bridal Makeup</span><span class="sep">✦</span><span>Facials & Skincare</span><span class="sep">✦</span><span>Nail Art & Design</span><span class="sep">✦</span><span>Mehendi</span><span class="sep">✦</span><span>Body Treatments</span><span class="sep">✦</span><span>Waxing & Threading</span><span class="sep">✦</span><span>Pre-Bridal Packages</span><span class="sep">✦</span><span>Home Service Available</span><span class="sep">✦</span>
    <span>Hair Services</span><span class="sep">✦</span><span>Bridal Makeup</span><span class="sep">✦</span><span>Facials & Skincare</span><span class="sep">✦</span><span>Nail Art & Design</span><span class="sep">✦</span><span>Mehendi</span><span class="sep">✦</span><span>Body Treatments</span><span class="sep">✦</span><span>Waxing & Threading</span><span class="sep">✦</span><span>Pre-Bridal Packages</span><span class="sep">✦</span><span>Home Service Available</span><span class="sep">✦</span>
  </div>
</div>

<!-- ABOUT -->
<section class="about" id="about">
  <div class="about-grid">
    <div class="about-img-wrap fade-up">
      <div class="about-accent"></div>
      <div class="about-frame">
        <img src="IMG_20260327_204057.jpg" alt="Khushi - Makeup Artist">
      </div>
      <div class="about-float"><div class="num">6+</div><div class="lbl">Years of Art</div></div>
    </div>
    <div class="about-content fade-up">
      <div class="sec-tag">About the Artist</div>
      <h2 class="sec-title">Hello, I'm <em>Khushi</em></h2>
      <div class="sec-line"></div>
      <p class="sec-desc">A certified makeup artist, nail technician &amp; beauty specialist based in Raipur. I believe beauty is a form of self-expression — my art enhances your natural glow and makes you feel extraordinary on your most special days.</p>
      <p class="sec-desc" style="margin-top:16px">From intimate home sessions to grand bridal transformations, every client receives a personalised luxury experience — tailored just for you.</p>
      <div class="pills">
        <span class="pill">Makeup Artist</span><span class="pill">Nail Artist</span><span class="pill">Bridal Specialist</span><span class="pill">Home Service</span><span class="pill">Mehendi Expert</span><span class="pill">Hair Specialist</span>
      </div>
    </div>
  </div>
</section>

<!-- BANNER: Hair -->
<div class="img-banner">
  <img src="IMG-20260327-WA0005.jpg" alt="Hair Services Banner">
  <div class="img-banner-overlay"></div>
  <div class="img-banner-text">
    <h3>Complete Hair Care</h3>
    <p>From everyday cuts to luxury bridal hairstyles — we do it all</p>
  </div>
</div>

<!-- SERVICES -->
<section class="services-section" id="services">
  <div class="services-intro">
    <div>
      <div class="sec-tag">What We Offer</div>
      <h2 class="sec-title">Complete <em>Head to Toe</em><br>Services</h2>
      <div class="sec-line"></div>
    </div>
    <p class="sec-desc" style="text-align:right;max-width:340px">From haircut to pedicure — every beauty need covered under one premium roof.</p>
  </div>
  <div class="svc-categories">

    <!-- HAIR -->
    <div class="svc-cat-card fade-up">
      <div class="svc-cat-img"><img src="IMG-20260327-WA0004.jpg" alt="Hair"><div class="svc-cat-img-overlay"></div></div>
      <div class="svc-cat-header"><div class="svc-cat-icon">💇‍♀️</div><div><h3>Hair Services</h3><p>Cut, colour, spa & styling</p></div></div>
      <div class="svc-cat-body">
        <div style="font-size:11px;letter-spacing:2px;text-transform:uppercase;color:var(--purple);font-weight:700;padding:6px 0 4px">Hair Cut</div>
        <div class="svc-item"><span class="svc-item-name">Level Cut</span><span class="svc-price-tag">₹150</span></div>
        <div class="svc-item"><span class="svc-item-name">U Cut</span><span class="svc-price-tag">₹150</span></div>
        <div class="svc-item"><span class="svc-item-name">V Cut</span><span class="svc-price-tag">₹150</span></div>
        <div class="svc-item"><span class="svc-item-name">Layer Cut</span><span class="svc-price-tag">₹300</span></div>
        <div class="svc-item"><span class="svc-item-name">Step Cut</span><span class="svc-price-tag">₹350</span></div>
        <div class="svc-item"><span class="svc-item-name">Trimming</span><span class="svc-price-tag">₹200</span></div>
        <div style="font-size:11px;letter-spacing:2px;text-transform:uppercase;color:var(--purple);font-weight:700;padding:6px 0 4px;margin-top:8px;border-top:1px solid var(--border)">Hair Colour</div>
        <div class="svc-item"><span class="svc-item-name">Root Touch-Up</span><span class="svc-price-tag">₹350</span></div>
        <div class="svc-item"><span class="svc-item-name">Full Hair Color</span><span class="svc-price-tag">₹1,000</span></div>
        <div class="svc-item"><span class="svc-item-name">Highlights (per strip)</span><span class="svc-price-tag">₹200</span></div>
        <div class="svc-item"><span class="svc-item-name">Global Highlights</span><span class="svc-price-tag">₹3,000</span></div>
        <div style="font-size:11px;letter-spacing:2px;text-transform:uppercase;color:var(--purple);font-weight:700;padding:6px 0 4px;margin-top:8px;border-top:1px solid var(--border)">Hair Treatment</div>
        <div class="svc-item"><span class="svc-item-name">Hair Smoothening</span><span class="svc-price-tag">₹3,000</span></div>
        <div class="svc-item"><span class="svc-item-name">Hair Keratin</span><span class="svc-price-tag">₹2,500</span></div>
        <div class="svc-item"><span class="svc-item-name">Kerasmooth</span><span class="svc-price-tag">₹4,500</span></div>
        <div class="svc-item"><span class="svc-item-name">Botox Treatment</span><span class="svc-price-tag">₹3,500</span></div>
        <div class="svc-item"><span class="svc-item-name">Nanoplastia Treatment</span><span class="svc-price-tag">₹4,500</span></div>
        <div class="svc-item"><span class="svc-item-name">Bond Repair Treatment</span><span class="svc-price-tag">₹2,000</span></div>
        <div class="svc-item"><span class="svc-item-name">Dandruff Treatment</span><span class="svc-price-tag">₹700</span></div>
        <div class="svc-item"><span class="svc-item-name">Split End Treatment</span><span class="svc-price-tag">₹500</span></div>
        <div class="svc-item"><span class="svc-item-name">Permanent Hair Spa</span><span class="svc-price-tag">₹1,500</span></div>
        <div class="svc-item"><span class="svc-item-name">Damage Hair Treatment</span><span class="svc-price-tag">₹1,500</span></div>
      </div>
    </div>

    <!-- FACE & SKIN -->
    <div class="svc-cat-card fade-up">
      <div class="svc-cat-img"><img src="https://images.unsplash.com/photo-1616394584738-fc6e612e71b9?w=700&q=80" alt="Skincare"><div class="svc-cat-img-overlay"></div></div>
      <div class="svc-cat-header"><div class="svc-cat-icon">✨</div><div><h3>Face & Skin</h3><p>Glow treatments & facials</p></div></div>
      <div class="svc-cat-body">
        <div style="font-size:11px;letter-spacing:2px;text-transform:uppercase;color:var(--purple);font-weight:700;padding:6px 0 4px">Face Cleanup</div>
        <div class="svc-item"><span class="svc-item-name">Fruit Cleanup</span><span class="svc-price-tag">₹300</span></div>
        <div class="svc-item"><span class="svc-item-name">Papaya Cleanup</span><span class="svc-price-tag">₹300</span></div>
        <div class="svc-item"><span class="svc-item-name">D-Tan Cleanup</span><span class="svc-price-tag">₹350</span></div>
        <div class="svc-item"><span class="svc-item-name">Coffee Cleanup</span><span class="svc-price-tag">₹300</span></div>
        <div class="svc-item"><span class="svc-item-name">O3+ Cleanup</span><span class="svc-price-tag">₹500</span></div>
        <div class="svc-item"><span class="svc-item-name">Lotus Cleanup</span><span class="svc-price-tag">₹350</span></div>
        <div class="svc-item"><span class="svc-item-name">Vitamin C Cleanup</span><span class="svc-price-tag">₹300</span></div>
        <div style="font-size:11px;letter-spacing:2px;text-transform:uppercase;color:var(--purple);font-weight:700;padding:6px 0 4px;margin-top:8px;border-top:1px solid var(--border)">D-Tan & Bleach</div>
        <div class="svc-item"><span class="svc-item-name">Face D-Tan</span><span class="svc-price-tag">₹150</span></div>
        <div class="svc-item"><span class="svc-item-name">Face Bleach</span><span class="svc-price-tag">₹150</span></div>
        <div class="svc-item"><span class="svc-item-name">Full Body D-Tan</span><span class="svc-price-tag">₹700</span></div>
        <div class="svc-item"><span class="svc-item-name">Full Body Bleach</span><span class="svc-price-tag">₹700</span></div>
        <div style="font-size:11px;letter-spacing:2px;text-transform:uppercase;color:var(--purple);font-weight:700;padding:6px 0 4px;margin-top:8px;border-top:1px solid var(--border)">Facial</div>
        <div class="svc-item"><span class="svc-item-name">Gold Facial</span><span class="svc-price-tag">₹500</span></div>
        <div class="svc-item"><span class="svc-item-name">Papaya Facial</span><span class="svc-price-tag">₹550</span></div>
        <div class="svc-item"><span class="svc-item-name">Vitamin C Facial</span><span class="svc-price-tag">₹550</span></div>
        <div class="svc-item"><span class="svc-item-name">D-Tan Facial</span><span class="svc-price-tag">₹600</span></div>
        <div class="svc-item"><span class="svc-item-name">Pearl Facial</span><span class="svc-price-tag">₹700</span></div>
        <div class="svc-item"><span class="svc-item-name">Coffee Facial</span><span class="svc-price-tag">₹600</span></div>
        <div class="svc-item"><span class="svc-item-name">Lotus Facial</span><span class="svc-price-tag">₹800</span></div>
        <div class="svc-item"><span class="svc-item-name">O3+ Whitening Facial</span><span class="svc-price-tag">₹850</span></div>
        <div class="svc-item"><span class="svc-item-name">O3+ Bridal Facial</span><span class="svc-price-tag">₹1,500</span></div>
        <div class="svc-item"><span class="svc-item-name">O3+ Vitamin C Facial</span><span class="svc-price-tag">₹1,350</span></div>
        <div class="svc-item"><span class="svc-item-name">Melanin Control Facial</span><span class="svc-price-tag">₹2,000</span></div>
        <div class="svc-item"><span class="svc-item-name">Insta-Fair Facial</span><span class="svc-price-tag">₹2,000</span></div>
      </div>
    </div>

    <!-- MAKEUP -->
    <div class="svc-cat-card fade-up">
      <div class="svc-cat-img"><img src="Screenshot_2026-04-01-18-02-52-98_1c337646f29875672b5a61192b9010f9.jpg" alt="Makeup"><div class="svc-cat-img-overlay"></div></div>
      <div class="svc-cat-header"><div class="svc-cat-icon">💄</div><div><h3>Makeup</h3><p>HD, Airbrush & Bridal looks</p></div></div>
      <div class="svc-cat-body">
        <div style="font-size:11px;letter-spacing:2px;text-transform:uppercase;color:var(--purple);font-weight:700;padding:6px 0 4px">Makeup with Hairstyle</div>
        <div class="svc-item"><span class="svc-item-name">Simple Makeup + Hairstyle</span><span class="svc-price-tag">₹1,200</span></div>
        <div class="svc-item"><span class="svc-item-name">Party Makeup + Hairstyle</span><span class="svc-price-tag">₹1,500</span></div>
        <div class="svc-item"><span class="svc-item-name">Engagement Makeup + Hairstyle</span><span class="svc-price-tag">₹4,500</span></div>
        <div class="svc-item"><span class="svc-item-name">Sangeet Makeup + Hairstyle</span><span class="svc-price-tag">₹5,000</span></div>
        <div class="svc-item"><span class="svc-item-name">Mehendi Makeup + Hairstyle</span><span class="svc-price-tag">₹3,500</span></div>
        <div class="svc-item"><span class="svc-item-name">Haldi Makeup + Hairstyle</span><span class="svc-price-tag">₹3,500</span></div>
        <div class="svc-item"><span class="svc-item-name">Bridal Makeup + Hairstyle</span><span class="svc-price-tag">₹5,000</span></div>
        <div class="svc-item"><span class="svc-item-name">Reception Makeup + Hairstyle</span><span class="svc-price-tag">₹5,000</span></div>
      </div>
    </div>

    <!-- NAILS -->
    <div class="svc-cat-card fade-up">
      <div class="svc-cat-img"><img src="https://images.unsplash.com/photo-1604654894610-df63bc536371?w=700&q=80" alt="Nails"><div class="svc-cat-img-overlay"></div></div>
      <div class="svc-cat-header"><div class="svc-cat-icon">💅</div><div><h3>Nail Care & Art</h3><p>Manicure, pedicure & art</p></div></div>
      <div class="svc-cat-body">
        <div style="font-size:11px;letter-spacing:2px;text-transform:uppercase;color:var(--purple);font-weight:700;padding:6px 0 4px">Manicure & Pedicure</div>
        <div class="svc-item"><span class="svc-item-name">Manicure + Pedicure</span><span class="svc-price-tag">₹500</span></div>
        <div class="svc-item"><span class="svc-item-name">Crystal Manicure + Pedicure</span><span class="svc-price-tag">₹650</span></div>
        <div class="svc-item"><span class="svc-item-name">O3+ Manicure + Pedicure</span><span class="svc-price-tag">₹800</span></div>
        <div class="svc-item"><span class="svc-item-name">Raga Manicure + Pedicure</span><span class="svc-price-tag">₹700</span></div>
        <div style="font-size:11px;letter-spacing:2px;text-transform:uppercase;color:var(--purple);font-weight:700;padding:6px 0 4px;margin-top:8px;border-top:1px solid var(--border)">Massage & Body Care</div>
        <div class="svc-item"><span class="svc-item-name">Full Body Oil Massage</span><span class="svc-price-tag">₹699</span></div>
        <div class="svc-item"><span class="svc-item-name">Full Body Polishing</span><span class="svc-price-tag">₹1,500</span></div>
        <div class="svc-item"><span class="svc-item-name">Full Body Scrubbing</span><span class="svc-price-tag">₹800</span></div>
      </div>
    </div>

    <!-- WAXING & BODY -->
    <div class="svc-cat-card fade-up">
      <div class="svc-cat-img"><img src="https://images.unsplash.com/photo-1570172619644-dfd03ed5d881?w=700&q=80" alt="Body Care"><div class="svc-cat-img-overlay"></div></div>
      <div class="svc-cat-header"><div class="svc-cat-icon">🌸</div><div><h3>Waxing & Body Care</h3><p>Rica, full body & de-tan</p></div></div>
      <div class="svc-cat-body">
        <div style="font-size:11px;letter-spacing:2px;text-transform:uppercase;color:var(--purple);font-weight:700;padding:6px 0 4px">Normal Wax</div>
        <div class="svc-item"><span class="svc-item-name">Full Hand Wax</span><span class="svc-price-tag">₹100</span></div>
        <div class="svc-item"><span class="svc-item-name">Half Leg Wax</span><span class="svc-price-tag">₹100</span></div>
        <div class="svc-item"><span class="svc-item-name">Full Leg Wax</span><span class="svc-price-tag">₹250</span></div>
        <div class="svc-item"><span class="svc-item-name">Tummy Wax</span><span class="svc-price-tag">₹100</span></div>
        <div class="svc-item"><span class="svc-item-name">Back Wax</span><span class="svc-price-tag">₹150</span></div>
        <div class="svc-item"><span class="svc-item-name">Underarm Wax</span><span class="svc-price-tag">₹50</span></div>
        <div class="svc-item"><span class="svc-item-name">Full Body Wax</span><span class="svc-price-tag">₹650</span></div>
        <div style="font-size:11px;letter-spacing:2px;text-transform:uppercase;color:var(--purple);font-weight:700;padding:6px 0 4px;margin-top:8px;border-top:1px solid var(--border)">Dark Chocolate Wax</div>
        <div class="svc-item"><span class="svc-item-name">Full Hand Wax</span><span class="svc-price-tag">₹120</span></div>
        <div class="svc-item"><span class="svc-item-name">Half Leg Wax</span><span class="svc-price-tag">₹120</span></div>
        <div class="svc-item"><span class="svc-item-name">Full Leg Wax</span><span class="svc-price-tag">₹280</span></div>
        <div class="svc-item"><span class="svc-item-name">Tummy Wax</span><span class="svc-price-tag">₹150</span></div>
        <div class="svc-item"><span class="svc-item-name">Back Wax</span><span class="svc-price-tag">₹250</span></div>
        <div class="svc-item"><span class="svc-item-name">Full Body Wax</span><span class="svc-price-tag">₹750</span></div>
        <div style="font-size:11px;letter-spacing:2px;text-transform:uppercase;color:var(--purple);font-weight:700;padding:6px 0 4px;margin-top:8px;border-top:1px solid var(--border)">White Chocolate Wax</div>
        <div class="svc-item"><span class="svc-item-name">Full Hand Wax</span><span class="svc-price-tag">₹150</span></div>
        <div class="svc-item"><span class="svc-item-name">Half Leg Wax</span><span class="svc-price-tag">₹150</span></div>
        <div class="svc-item"><span class="svc-item-name">Full Leg Wax</span><span class="svc-price-tag">₹300</span></div>
        <div class="svc-item"><span class="svc-item-name">Underarm Wax</span><span class="svc-price-tag">₹50</span></div>
        <div class="svc-item"><span class="svc-item-name">Tummy Wax</span><span class="svc-price-tag">₹120</span></div>
        <div class="svc-item"><span class="svc-item-name">Back Wax</span><span class="svc-price-tag">₹150</span></div>
        <div class="svc-item"><span class="svc-item-name">Full Body Wax</span><span class="svc-price-tag">₹800</span></div>
        <div style="font-size:11px;letter-spacing:2px;text-transform:uppercase;color:var(--purple);font-weight:700;padding:6px 0 4px;margin-top:8px;border-top:1px solid var(--border)">Oil Wax</div>
        <div class="svc-item"><span class="svc-item-name">Full Hand Wax</span><span class="svc-price-tag">₹200</span></div>
        <div class="svc-item"><span class="svc-item-name">Half Leg Wax</span><span class="svc-price-tag">₹200</span></div>
        <div class="svc-item"><span class="svc-item-name">Full Leg Wax</span><span class="svc-price-tag">₹400</span></div>
        <div class="svc-item"><span class="svc-item-name">Underarm Wax</span><span class="svc-price-tag">₹50</span></div>
        <div class="svc-item"><span class="svc-item-name">Tummy Wax</span><span class="svc-price-tag">₹150</span></div>
        <div class="svc-item"><span class="svc-item-name">Back Wax</span><span class="svc-price-tag">₹200</span></div>
        <div class="svc-item"><span class="svc-item-name">Full Body Wax</span><span class="svc-price-tag">₹1000</span></div>
      </div>
    </div>

    <!-- HOME SERVICE -->
    <div class="svc-cat-card fade-up" style="border-color:var(--pink2);background:linear-gradient(160deg,var(--purple4),var(--pink4))">
      <div class="svc-cat-img"><img src="https://images.unsplash.com/photo-1498843053639-170ff2122f35?w=700&q=80" alt="Home Service"><div class="svc-cat-img-overlay"></div></div>
      <div class="svc-cat-header" style="background:linear-gradient(135deg,var(--purple4),var(--pink4))"><div class="svc-cat-icon">🏡</div><div><h3>Home Salon Service</h3><p>All services at your doorstep</p></div></div>
      <div class="svc-cat-body">
        <div class="svc-item"><span class="svc-item-name">Bridal / Pre-Bridal at Home</span><span class="svc-price-tag">Available</span></div>
        <div class="svc-item"><span class="svc-item-name">Makeup at Home</span><span class="svc-price-tag">+₹300 travel</span></div>
        <div class="svc-item"><span class="svc-item-name">Facial & Cleanup at Home</span><span class="svc-price-tag">Available</span></div>
        <div class="svc-item"><span class="svc-item-name">Waxing at Home</span><span class="svc-price-tag">Available</span></div>
        <div class="svc-item"><span class="svc-item-name">Hair Services at Home</span><span class="svc-price-tag">Available</span></div>
        <div class="svc-item"><span class="svc-item-name">Mehendi at Home / Venue</span><span class="svc-price-tag">Available</span></div>
        <div class="svc-item"><span class="svc-item-name">Nail Art at Home</span><span class="svc-price-tag">Available</span></div>
        <div class="svc-item"><span class="svc-item-name">Manicure & Pedicure at Home</span><span class="svc-price-tag">Available</span></div>
        <div style="margin-top:20px;padding:14px;background:var(--pink4);border-radius:8px;border:1px solid var(--border-pink)">
          <p style="font-size:12.5px;color:var(--pink-deep);text-align:center;font-weight:700">💬 WhatsApp to book home service</p>
        </div>
      </div>
    </div>

  </div>
</section>

<!-- BANNER: Bridal -->
<div class="img-banner">
  <img src="IMG-20260327-WA0041.jpg" alt="Bridal">
  <div class="img-banner-overlay"></div>
  <div class="img-banner-text">
    <h3>Bridal Beauty at Its Finest</h3>
    <p>Because your wedding day deserves nothing less than perfection</p>
  </div>
</div>

<!-- BRIDAL -->
<section class="bridal" id="bridal">
  <div class="bridal-inner">
    <div class="bridal-top">
      <div class="fade-up">
        <div class="sec-tag">Bridal Experience</div>
        <h2 class="sec-title">Your Dream <em>Bridal Look</em><br>Awaits</h2>
        <div class="sec-line"></div>
        <p class="sec-desc">Your wedding day deserves perfection. We curate a complete bridal beauty experience — from pre-bridal treatments to the final look on your big day. From head to toe, every detail is taken care of.</p>
        <a href="https://wa.me/918085306764" class="wa-btn" style="display:inline-flex;width:auto;margin-top:36px;padding:14px 32px">💬 Check Bridal Availability</a>
      </div>
      <div class="bridal-img fade-up">
        <img src="Screenshot_2026-04-01-17-48-30-64_1c337646f29875672b5a61192b9010f9.jpg" alt="Bridal Makeup">
      </div>
    </div>
    <div class="pkg-grid">
      <div class="pkg-card fade-up">
        <h3>Silver Bridal</h3><div class="pkg-subtitle">✦ Essential Package</div>
        <ul class="pkg-features">
          <li>HD Bridal Makeup</li><li>Bridal Hairstyle</li><li>Eyebrow Threading & Shaping</li>
          <li>Full Body Waxing</li><li>D-Tan Facial + Cleanup</li><li>Mehendi (Hands & Feet)</li><li>Basic Nail Color</li>
        </ul>
        <a href="https://wa.me/918085306764" class="pkg-cta">💬 Enquire Now</a>
      </div>
      <div class="pkg-card best fade-up">
        <span class="pkg-badge">Most Popular</span>
        <h3>Gold Bridal</h3><div class="pkg-subtitle">✦ Premium Package</div>
        <ul class="pkg-features">
          <li>Airbrush HD Makeup</li><li>Elaborate Bridal Hair</li><li>3 Pre-Bridal Facial Sessions</li>
          <li>Bridal Nail Art (Hands & Feet)</li><li>Gold Facial + Cleanup</li><li>Mehendi Day Full Look</li>
          <li>Full Body Waxing + De-Tan</li><li>Body Scrub + Polishing</li><li>Saree Draping Included</li>
        </ul>
        <a href="https://wa.me/918085306764" class="pkg-cta">💬 Book This Package</a>
      </div>
      <div class="pkg-card fade-up">
        <h3>Diamond Bridal</h3><div class="pkg-subtitle">✦ Luxury Package</div>
        <ul class="pkg-features">
          <li>All Gold Package Inclusions</li><li>5 Pre-Bridal Treatment Sessions</li><li>Full Family Makeup (4 persons)</li>
          <li>Diamond Facial Series</li><li>Engagement Look Included</li><li>Reception Makeup</li>
          <li>Rajasthani Bridal Mehendi</li><li>Luxury Spa Manicure & Pedicure</li><li>Home / Venue Service Option</li>
        </ul>
        <a href="https://wa.me/918085306764" class="pkg-cta">💬 Enquire Now</a>
      </div>
    </div>
  </div>
</section>

<!-- BANNER: Beauty Ritual -->
<div class="img-banner">
  <img src="Screenshot_2026-04-01-18-03-21-97_1c337646f29875672b5a61192b9010f9.jpg" alt="Beauty">
  <div class="img-banner-overlay"></div>
  <div class="img-banner-text">
    <h3>Beauty is a Ritual</h3>
    <p>Every visit is a luxury escape — see the transformations we create</p>
  </div>
</div>

<!-- GALLERY -->
<section class="gallery" id="gallery">
  <div class="gallery-header">
    <div>
      <div class="sec-tag">Portfolio</div>
      <h2 class="sec-title">A Glimpse of <em>Our Work</em></h2>
      <div class="sec-line"></div>
    </div>
    <a href="https://www.instagram.com/_the_good_vibes123" class="btn-primary" style="height:fit-content">Follow on Instagram ↗</a>
  </div>

  <!-- FILTER TABS -->
  <div class="gallery-filters">
    <button class="g-filter active" data-filter="all">✨ All Work</button>
    <button class="g-filter" data-filter="bridal">👰🏻 Bridal</button>
    <button class="g-filter" data-filter="engagement">💍 Engagement</button>
    <button class="g-filter" data-filter="sangeet">🎶 Sangeet</button>
    <button class="g-filter" data-filter="party-makeup">💄 Party Makeup</button>
    <button class="g-filter" data-filter="hair-style">🌺 Hair Style</button>
    <button class="g-filter" data-filter="hair-art">✂️ Hair Art</button>
    <button class="g-filter" data-filter="hair-treatment">💆🏻 Hair Treatment</button>
    <button class="g-filter" data-filter="hair-cut">✂ Hair Cut</button>
  </div>

  <div class="gallery-grid" id="galleryGrid">

    <!-- HAIR STYLE — half-up braided curls (Image 1) -->
    <div class="g-item g-item-1 fade-up" data-cat="hair-style">
      <div class="g-cat-label">Hair Style</div>
      <img src="Screenshot_2026-04-01-18-03-21-97_1c337646f29875672b5a61192b9010f9.jpg" alt="Hair Style">
      <div class="g-overlay"><span>Party Hair Style</span></div>
    </div>

    <!-- PARTY MAKEUP — makeup done (Image 2) -->
    <div class="g-item fade-up" data-cat="party-makeup">
      <div class="g-cat-label">Party Makeup</div>
      <img src="Screenshot_2026-04-01-18-02-52-98_1c337646f29875672b5a61192b9010f9.jpg" alt="Party Makeup">
      <div class="g-overlay"><span>Party Makeup</span></div>
    </div>

    <!-- BRIDAL — woman in black (Image 3) -->
    <div class="g-item fade-up" data-cat="bridal">
      <div class="g-cat-label">Bridal Look</div>
      <img src="Screenshot_2026-04-01-17-48-30-64_1c337646f29875672b5a61192b9010f9.jpg" alt="Bridal Look">
      <div class="g-overlay"><span>Bridal Look</span></div>
    </div>

    <!-- ENGAGEMENT LOOK — red outfit updo (Image 4) -->
    <div class="g-item fade-up" data-cat="engagement">
      <div class="g-cat-label">Engagement</div>
      <img src="Screenshot_2026-03-27-20-42-29-23_6012fa4d4ddec268fc5c7112cbb265e7.jpg" alt="Engagement Look">
      <div class="g-overlay"><span>Engagement Look</span></div>
    </div>

    <!-- BRIDAL — white lehenga (Image 5) -->
    <div class="g-item fade-up" data-cat="bridal">
      <div class="g-cat-label">Bridal</div>
      <img src="IMG_20260327_204057.jpg" alt="Bridal">
      <div class="g-overlay"><span>Bridal</span></div>
    </div>

    <!-- HAIR ART — braid with maang tikka (Image 6) -->
    <div class="g-item fade-up" data-cat="hair-art">
      <div class="g-cat-label">Hair Art</div>
      <img src="IMG_20260327_204014.jpg" alt="Hair Art">
      <div class="g-overlay"><span>Hair Art</span></div>
    </div>

    <!-- HAIR ART — stylist doing hair (Image 7) -->
    <div class="g-item fade-up" data-cat="hair-art">
      <div class="g-cat-label">Hair Art</div>
      <img src="IMG-20260327-WA0038.jpg" alt="Hair Art">
      <div class="g-overlay"><span>Hair Art</span></div>
    </div>

    <!-- SANGEET LOOK — red lehenga (Image 8) -->
    <div class="g-item fade-up" data-cat="sangeet">
      <div class="g-cat-label">Sangeet</div>
      <img src="IMG-20260327-WA0045.jpg" alt="Sangeet Look">
      <div class="g-overlay"><span>Sangeet Look</span></div>
    </div>

    <!-- BRIDAL LEHENGA — pink lehenga (Image 9) -->
    <div class="g-item fade-up" data-cat="bridal">
      <div class="g-cat-label">Bridal Lehenga</div>
      <img src="IMG-20260327-WA0041.jpg" alt="Bridal Lehenga">
      <div class="g-overlay"><span>Bridal Lehenga</span></div>
    </div>

    <!-- HAIR TREATMENT — straight silk hair (Image 10) -->
    <div class="g-item fade-up" data-cat="hair-treatment">
      <div class="g-cat-label">Hair Treatment</div>
      <img src="IMG-20260327-WA0005.jpg" alt="Hair Treatment">
      <div class="g-overlay"><span>Hair Treatment</span></div>
    </div>

    <!-- HAIR CUT — wavy styled hair -->
    <div class="g-item fade-up" data-cat="hair-cut">
      <div class="g-cat-label">Hair Cut</div>
      <img src="IMG-20260327-WA0004.jpg" alt="Hair Cut">
      <div class="g-overlay"><span>Hair Cut</span></div>
    </div>

    <!-- ENGAGEMENT SIDE PROFILE — red dress updo ponytail -->
    <div class="g-item fade-up" data-cat="engagement">
      <div class="g-cat-label">Engagement</div>
      <img src="Screenshot_2026-03-27-20-39-39-84_6012fa4d4ddec268fc5c7112cbb265e7.jpg" alt="Engagement Side Look">
      <div class="g-overlay"><span>Engagement Look</span></div>
    </div>

    <!-- PARTY MAKEUP — elegant teal outfit full face -->
    <div class="g-item fade-up" data-cat="party-makeup">
      <div class="g-cat-label">Party Makeup</div>
      <img src="Screenshot_2026-03-27-20-39-13-71_6012fa4d4ddec268fc5c7112cbb265e7.jpg" alt="Party Makeup Teal">
      <div class="g-overlay"><span>Party Makeup</span></div>
    </div>

  </div>
</section>

<!-- TESTIMONIALS -->
<section class="testimonials" id="reviews">
  <div class="testi-header fade-up">
    <div class="sec-tag" style="justify-content:center;padding-left:0">Client Love</div>
    <h2 class="sec-title" style="text-align:center">What Our <em>Clients Say</em></h2>
    <div class="sec-line c"></div>
    <p class="sec-desc" style="text-align:center;margin:12px auto 0">Hundreds of happy clients — here are a few of their stories.</p>
  </div>
  <div class="testi-grid">
    <div class="testi-card fade-up">
      <div class="stars">★★★★★</div>
      <p>"Khushi made me feel like an absolute queen on my wedding day. The makeup lasted the entire ceremony. Everyone kept asking who did my look!"</p>
      <div class="testi-author"><div class="testi-avatar"><img src="https://images.unsplash.com/photo-1438761681033-6461ffad8d80?w=100&q=80" alt=""></div><div><div class="testi-name">Priya Sharma</div><div class="testi-role">Bride · December 2025</div></div></div>
    </div>
    <div class="testi-card fade-up">
      <div class="stars">★★★★★</div>
      <p>"I've been getting facials and waxing done here for a year. The results are always immaculate and the vibe is so warm and professional. Highly recommend!"</p>
      <div class="testi-author"><div class="testi-avatar"><img src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?w=100&q=80" alt=""></div><div><div class="testi-name">Anjali Kapoor</div><div class="testi-role">Regular Client</div></div></div>
    </div>
    <div class="testi-card fade-up">
      <div class="stars">★★★★★</div>
      <p>"The home salon service is a game-changer. Got my engagement makeup done at home and looked absolutely stunning. Very punctual and uses only premium products."</p>
      <div class="testi-author"><div class="testi-avatar"><img src="https://images.unsplash.com/photo-1534528741775-53994a69daeb?w=100&q=80" alt=""></div><div><div class="testi-name">Riya Mehta</div><div class="testi-role">Home Service Client</div></div></div>
    </div>
  </div>
</section>

<!-- PROCESS -->
<section class="process">
  <div class="process-inner">
    <div style="text-align:center">
      <div class="sec-tag" style="justify-content:center;padding-left:0">Our Process</div>
      <h2 class="sec-title" style="text-align:center">Booking is <em>Effortless</em></h2>
      <div class="sec-line c"></div>
    </div>
    <div class="process-img fade-up">
      <img src="IMG-20260327-WA0038.jpg" alt="Beauty Studio">
    </div>
    <div class="steps">
      <div class="step fade-up"><div class="step-num">Step 01</div><div class="step-icon">💬</div><h4>WhatsApp Us</h4><p>Send us a message with your event date and desired service.</p></div>
      <div class="step fade-up"><div class="step-num">Step 02</div><div class="step-icon">📅</div><h4>Pick a Slot</h4><p>We confirm availability and lock in your appointment.</p></div>
      <div class="step fade-up"><div class="step-num">Step 03</div><div class="step-icon">🌸</div><h4>Trial Session</h4><p>Optional pre-event trial to ensure your look is perfect.</p></div>
      <div class="step fade-up"><div class="step-num">Step 04</div><div class="step-icon">✨</div><h4>Look Stunning</h4><p>Arrive and leave radiant — ready to conquer the world.</p></div>
    </div>
  </div>
</section>

<!-- CONTACT -->
<section class="contact" id="contact">
  <div class="contact-inner">
    <div class="fade-up">
      <div class="sec-tag">Find Us</div>
      <h2 class="sec-title">Visit or <em>Call Us</em></h2>
      <div class="sec-line"></div>
      <div class="contact-img"><img src="IMG_20260327_204014.jpg" alt="Our Studio"></div>
      <div>
        <div class="info-item"><div class="info-icon">📍</div><div><div class="info-label">Studio Address</div><div class="info-val">Badwani Complex, 1st Floor, Near Amit Furniture,<br>Street No.3, Fafadi Naka, Raipur</div></div></div>
        <div class="info-item"><div class="info-icon">📞</div><div><div class="info-label">Phone / WhatsApp</div><div class="info-val"><a href="tel:+918085306764" style="color:var(--purple)">+91 80853 06764</a></div></div></div>
        <div class="info-item"><div class="info-icon">⏰</div><div><div class="info-label">Working Hours</div><div class="info-val">Mon – Sat: 9:00 AM – 8:00 PM<br>Sunday: By Appointment Only</div></div></div>
        <div class="info-item" style="border:none"><div class="info-icon">📸</div><div><div class="info-label">Instagram</div><div class="info-val"><a href="https://www.instagram.com/_the_good_vibes123" style="color:var(--pink-deep)">@_the_good_vibes123</a></div></div></div>
      </div>
      <div style="margin-top:28px;border-radius:14px;overflow:hidden;border:2px solid var(--border-pink)">
        <iframe src="https://maps.google.com/maps?q=Fafadi+Naka+Raipur&t=&z=14&ie=UTF8&iwloc=&output=embed" width="100%" height="220" style="border:0;display:block" allowfullscreen loading="lazy"></iframe>
      </div>
    </div>
    <div class="book-card fade-up">
      <div style="font-size:52px;margin-bottom:20px">💅</div>
      <h3>Ready to Glow?</h3>
      <p>Whether it's your wedding day, a special party, or just some everyday self-care — we're here for you. Book via WhatsApp for instant confirmation.</p>
      <a href="https://wa.me/918085306764?text=Hi%20Khushi!%20I%20would%20like%20to%20book%20an%20appointment%20at%20The%20Good%20Vibes%20Studio." class="wa-btn">💬 Book on WhatsApp</a>
      <div class="social-row">
        <a href="https://www.instagram.com/_the_good_vibes123" class="social-btn">📸 Instagram</a>
        <a href="https://wa.me/918085306764" class="social-btn">💬 WhatsApp</a>
      </div>
      <div class="offer-box">
        <div class="offer-label">🌟 Current Offer</div>
        <p>Bridal bookings open! Ask about exclusive pre-bridal packages and combo deals. Mention <strong style="color:var(--gold)">"GOOD VIBES"</strong> for a special discount.</p>
      </div>
    </div>
  </div>
</section>

<!-- FOOTER -->
<footer>
  <div class="footer-logo">The Good Vibes Studio</div>
  <div class="footer-tagline">Luxury Beauty · Raipur · Est. 2016</div>
  <div class="footer-links">
    <a href="#about">About</a><a href="#services">Services</a><a href="#bridal">Bridal</a>
    <a href="#gallery">Gallery</a><a href="#reviews">Reviews</a><a href="#contact">Contact</a>
  </div>
  <div class="footer-divider"></div>
  <div class="footer-copy">© 2026 The Good Vibes Studio by Khushi Makhija · All rights reserved</div>
</footer>

<!-- WA FLOAT -->
<a class="wa-float" href="https://wa.me/918085306764?text=Hi%20Khushi!%20I%27d%20like%20to%20book%20an%20appointment." target="_blank">
  <span class="wa-tooltip">Book Appointment</span>💬
</a>

<script>
const obs = new IntersectionObserver((entries) => {
  entries.forEach(e => { if(e.isIntersecting){ e.target.classList.add('visible'); obs.unobserve(e.target); } });
}, { threshold: 0.1 });
document.querySelectorAll('.fade-up').forEach(el => obs.observe(el));
window.addEventListener('scroll', () => {
  document.getElementById('mainNav').style.padding = window.scrollY > 60 ? '12px 60px' : '18px 60px';
});

// Gallery filter
document.querySelectorAll('.g-filter').forEach(btn => {
  btn.addEventListener('click', () => {
    document.querySelectorAll('.g-filter').forEach(b => b.classList.remove('active'));
    btn.classList.add('active');
    const filter = btn.dataset.filter;
    document.querySelectorAll('.g-item').forEach(item => {
      if(filter === 'all' || item.dataset.cat === filter){
        item.classList.remove('hidden');
      } else {
        item.classList.add('hidden');
      }
    });
    // Re-assign g-item-1 (large slot) to first visible item
    const visible = document.querySelectorAll('.g-item:not(.hidden)');
    document.querySelectorAll('.g-item').forEach(i => i.classList.remove('g-item-1'));
    if(visible.length > 0) visible[0].classList.add('g-item-1');
  });
});
</script>
</body>
</html>
