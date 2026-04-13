<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Centre of Corporate Studies | Training, E-Learning & Consulting — Nairobi, Kenya</title>
<link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:ital,wght@0,300;0,400;0,500;0,600;0,700;0,800;1,400&family=Playfair+Display:ital,wght@0,700;0,900;1,700&display=swap" rel="stylesheet">
<style>
:root {
  --ink: #0F1117;
  --ink2: #1A1D27;
  --ink3: #252836;
  --blue: #2563EB;
  --blue-dark: #1D4ED8;
  --blue-mid: #3B82F6;
  --blue-pale: #EFF6FF;
  --blue-dim: rgba(37,99,235,0.1);
  --teal: #0D9488;
  --amber: #F59E0B;
  --green: #10B981;
  --white: #FFFFFF;
  --slate: #F8FAFC;
  --slate2: #F1F5F9;
  --border: #E2E8F0;
  --text: #1E293B;
  --muted: #64748B;
  --muted2: #94A3B8;
  --serif: 'Playfair Display', Georgia, serif;
  --sans: 'Plus Jakarta Sans', sans-serif;
  --r: 8px;
  --r-lg: 16px;
  --r-xl: 24px;
}
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0;}
html{scroll-behavior:smooth;}
body{font-family:var(--sans);background:var(--white);color:var(--text);overflow-x:hidden;}
img{max-width:100%;display:block;}
a{text-decoration:none;color:inherit;}

/* ─── TOPBAR ─── */
.topbar{background:var(--ink);padding:8px 2rem;display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;gap:8px;}
.topbar-left{display:flex;gap:1.5rem;align-items:center;flex-wrap:wrap;}
.topbar-item{font-size:12px;color:rgba(255,255,255,.65);display:flex;align-items:center;gap:5px;}
.topbar-item strong{color:#fff;}
.topbar-right{display:flex;gap:.75rem;align-items:center;}
.tb-btn{font-size:12px;color:rgba(255,255,255,.65);background:rgba(255,255,255,.08);border:1px solid rgba(255,255,255,.12);padding:5px 14px;border-radius:20px;cursor:pointer;transition:all .2s;}
.tb-btn:hover{color:#fff;border-color:rgba(255,255,255,.3);}
.tb-btn.primary{background:var(--blue);color:#fff;border-color:var(--blue);}
.tb-btn.primary:hover{background:var(--blue-dark);}

/* ─── NAV ─── */
nav{background:var(--white);border-bottom:1px solid var(--border);position:sticky;top:0;z-index:500;}
.nav-inner{max-width:1280px;margin:0 auto;padding:0 2rem;display:flex;align-items:center;justify-content:space-between;height:70px;gap:1.5rem;}
.nav-logo{display:flex;flex-direction:column;text-decoration:none;}
.logo-main{font-family:var(--serif);font-size:20px;font-weight:700;color:var(--ink);line-height:1.1;letter-spacing:-.3px;}
.logo-main span{color:var(--blue);}
.logo-sub{font-size:10px;font-weight:600;letter-spacing:.12em;text-transform:uppercase;color:var(--muted);margin-top:1px;}
.nav-links{display:flex;list-style:none;gap:0;}
.nav-links a{font-size:13px;font-weight:600;color:var(--muted);padding:0 1rem;height:70px;display:flex;align-items:center;transition:color .15s;border-bottom:2px solid transparent;margin-bottom:-1px;letter-spacing:.01em;}
.nav-links a:hover,.nav-links a.active{color:var(--blue);border-bottom-color:var(--blue);}
.nav-right{display:flex;gap:.75rem;align-items:center;flex-shrink:0;}
.btn-outline{background:transparent;color:var(--blue);border:1.5px solid var(--blue);padding:9px 20px;border-radius:var(--r);font-family:var(--sans);font-size:13px;font-weight:600;cursor:pointer;transition:all .2s;display:inline-block;}
.btn-outline:hover{background:var(--blue-pale);}
.btn-primary{background:var(--blue);color:#fff;border:none;padding:10px 22px;border-radius:var(--r);font-family:var(--sans);font-size:13px;font-weight:600;cursor:pointer;transition:all .2s;display:inline-block;}
.btn-primary:hover{background:var(--blue-dark);transform:translateY(-1px);}

/* ─── HERO ─── */
.hero{background:var(--ink);min-height:92vh;display:grid;grid-template-columns:1fr 1fr;align-items:center;position:relative;overflow:hidden;}
.hero-pattern{position:absolute;inset:0;background-image:radial-gradient(rgba(37,99,235,.15) 1px,transparent 1px);background-size:32px 32px;pointer-events:none;}
.hero-glow{position:absolute;top:-200px;right:-100px;width:700px;height:700px;background:radial-gradient(circle,rgba(37,99,235,.12) 0%,transparent 70%);pointer-events:none;}
.hero-left{padding:80px 3rem 80px 5rem;position:relative;z-index:2;}
.hero-badge{display:inline-flex;align-items:center;gap:8px;background:rgba(37,99,235,.15);border:1px solid rgba(37,99,235,.3);border-radius:20px;padding:6px 16px;margin-bottom:1.5rem;font-size:11px;font-weight:700;color:#93C5FD;letter-spacing:.1em;text-transform:uppercase;}
.badge-dot{width:6px;height:6px;background:#60A5FA;border-radius:50%;animation:blink 2s ease-in-out infinite;}
@keyframes blink{0%,100%{opacity:1;}50%{opacity:.2;}}
.hero h1{font-family:var(--serif);font-size:clamp(2.8rem,5vw,4.5rem);font-weight:900;color:#fff;line-height:1.08;margin-bottom:1.25rem;}
.hero h1 .accent{color:#60A5FA;font-style:italic;}
.hero h1 .dim{color:rgba(255,255,255,.35);}
.hero-sub{font-size:16px;color:rgba(255,255,255,.55);line-height:1.7;max-width:480px;margin-bottom:2rem;font-weight:300;}
.hero-actions{display:flex;gap:1rem;flex-wrap:wrap;margin-bottom:2.5rem;}
.btn-hero-primary{background:var(--blue);color:#fff;border:none;padding:15px 32px;border-radius:var(--r);font-family:var(--sans);font-size:15px;font-weight:700;cursor:pointer;transition:all .2s;display:inline-flex;align-items:center;gap:8px;}
.btn-hero-primary:hover{background:var(--blue-dark);transform:translateY(-2px);box-shadow:0 12px 40px rgba(37,99,235,.4);}
.btn-hero-ghost{background:transparent;color:#fff;border:1.5px solid rgba(255,255,255,.2);padding:14px 32px;border-radius:var(--r);font-family:var(--sans);font-size:15px;font-weight:500;cursor:pointer;transition:all .2s;display:inline-flex;align-items:center;gap:8px;}
.btn-hero-ghost:hover{border-color:rgba(255,255,255,.5);}
.hero-stats{display:flex;gap:2.5rem;flex-wrap:wrap;}
.hstat-num{font-family:var(--serif);font-size:2rem;font-weight:700;color:#60A5FA;line-height:1;}
.hstat-label{font-size:11px;color:rgba(255,255,255,.4);text-transform:uppercase;letter-spacing:.08em;margin-top:4px;font-weight:500;}
.hero-right{padding:80px 4rem 80px 2rem;position:relative;z-index:2;}

/* ─── SEARCH BAR ─── */
.search-hero{background:rgba(255,255,255,.06);border:1px solid rgba(255,255,255,.12);border-radius:var(--r-lg);padding:1.5rem;margin-bottom:1.25rem;}
.search-hero-title{font-size:13px;font-weight:700;color:rgba(255,255,255,.6);text-transform:uppercase;letter-spacing:.1em;margin-bottom:.75rem;}
.search-box{display:flex;background:rgba(255,255,255,.08);border:1px solid rgba(255,255,255,.12);border-radius:var(--r);overflow:hidden;transition:border-color .2s;}
.search-box:focus-within{border-color:var(--blue-mid);}
.search-input{flex:1;background:transparent;border:none;outline:none;padding:12px 16px;color:#fff;font-family:var(--sans);font-size:14px;}
.search-input::placeholder{color:rgba(255,255,255,.3);}
.search-cat{background:transparent;border:none;border-left:1px solid rgba(255,255,255,.1);color:rgba(255,255,255,.5);font-family:var(--sans);font-size:13px;padding:0 14px;cursor:pointer;outline:none;}
.search-cat option{background:var(--ink2);}
.btn-search{background:var(--blue);border:none;color:#fff;padding:0 20px;cursor:pointer;font-family:var(--sans);font-weight:600;font-size:14px;transition:background .2s;}
.btn-search:hover{background:var(--blue-dark);}
.search-tags{display:flex;flex-wrap:wrap;gap:6px;margin-top:.75rem;}
.stag{background:rgba(255,255,255,.06);border:1px solid rgba(255,255,255,.1);color:rgba(255,255,255,.5);padding:4px 12px;border-radius:20px;font-size:11px;font-weight:600;cursor:pointer;transition:all .2s;}
.stag:hover{border-color:var(--blue-mid);color:#93C5FD;background:rgba(37,99,235,.15);}

/* ─── MEMBERSHIP CARD (HERO) ─── */
.mem-card{background:linear-gradient(135deg,#1D4ED8 0%,#1e3a8a 100%);border-radius:var(--r-lg);padding:1.5rem;border:1px solid rgba(255,255,255,.1);}
.mem-card-label{font-size:10px;font-weight:700;letter-spacing:.15em;text-transform:uppercase;color:#93C5FD;margin-bottom:.5rem;}
.mem-card-title{font-family:var(--serif);font-size:1.5rem;font-weight:700;color:#fff;margin-bottom:.25rem;}
.mem-card-sub{font-size:13px;color:rgba(255,255,255,.55);margin-bottom:1rem;font-weight:300;}
.mem-price{display:flex;align-items:baseline;gap:6px;margin-bottom:1rem;}
.mem-amount{font-family:var(--serif);font-size:2.5rem;font-weight:700;color:#fff;line-height:1;}
.mem-period{font-size:13px;color:rgba(255,255,255,.5);}
.mem-old{font-size:14px;color:rgba(255,255,255,.3);text-decoration:line-through;}
.mem-features{display:flex;flex-direction:column;gap:7px;margin-bottom:1.25rem;}
.mem-feat{display:flex;align-items:center;gap:8px;font-size:13px;color:rgba(255,255,255,.75);}
.feat-check{width:16px;height:16px;border-radius:50%;background:rgba(96,165,250,.25);display:flex;align-items:center;justify-content:center;flex-shrink:0;font-size:9px;color:#93C5FD;}
.btn-mem{width:100%;background:#fff;color:var(--blue-dark);border:none;padding:12px;border-radius:var(--r);font-family:var(--sans);font-size:14px;font-weight:700;cursor:pointer;transition:all .2s;}
.btn-mem:hover{background:#EFF6FF;}

/* ─── SECTIONS ─── */
.section{padding:90px 0;}
.container{max-width:1280px;margin:0 auto;padding:0 2rem;}
.section-label{font-size:11px;font-weight:700;letter-spacing:.15em;text-transform:uppercase;color:var(--blue);margin-bottom:.5rem;}
.section-title{font-family:var(--serif);font-size:clamp(1.9rem,3.5vw,2.8rem);font-weight:700;color:var(--ink);line-height:1.15;margin-bottom:.75rem;}
.section-title .muted{color:var(--muted2);}
.section-sub{font-size:16px;color:var(--muted);line-height:1.7;max-width:560px;font-weight:300;}
.section-head-row{display:flex;align-items:flex-end;justify-content:space-between;margin-bottom:2.5rem;flex-wrap:wrap;gap:1rem;}

/* ─── TRUST BAR ─── */
.trust-bar{background:var(--slate2);border-top:1px solid var(--border);border-bottom:1px solid var(--border);padding:22px 0;}
.trust-items{display:flex;justify-content:space-around;align-items:center;flex-wrap:wrap;gap:1.5rem;}
.ti{display:flex;align-items:center;gap:10px;}
.ti-icon{font-size:22px;}
.ti-title{font-size:14px;font-weight:700;color:var(--ink);}
.ti-sub{font-size:12px;color:var(--muted);}

/* ─── COURSE CARDS ─── */
.courses-filters{display:flex;gap:.5rem;flex-wrap:wrap;margin-bottom:2rem;}
.filter-btn{background:var(--white);border:1.5px solid var(--border);color:var(--muted);padding:7px 18px;border-radius:20px;font-family:var(--sans);font-size:13px;font-weight:600;cursor:pointer;transition:all .2s;}
.filter-btn:hover,.filter-btn.active{background:var(--blue);color:#fff;border-color:var(--blue);}
.courses-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:1.5rem;}
.course-card{background:var(--white);border:1.5px solid var(--border);border-radius:var(--r-lg);overflow:hidden;transition:all .25s;cursor:pointer;}
.course-card:hover{border-color:var(--blue);box-shadow:0 12px 40px rgba(37,99,235,.12);transform:translateY(-3px);}
.course-thumb{height:160px;background:var(--ink2);display:flex;align-items:center;justify-content:center;font-size:3.5rem;position:relative;}
.course-cat-badge{position:absolute;top:12px;left:12px;background:rgba(37,99,235,.9);color:#fff;font-size:10px;font-weight:700;padding:3px 10px;border-radius:4px;letter-spacing:.05em;text-transform:uppercase;}
.course-format{position:absolute;top:12px;right:12px;font-size:10px;font-weight:700;padding:3px 10px;border-radius:4px;text-transform:uppercase;letter-spacing:.05em;}
.course-format.online{background:rgba(16,185,129,.9);color:#fff;}
.course-format.live{background:rgba(245,158,11,.9);color:#fff;}
.course-format.hybrid{background:rgba(13,148,136,.9);color:#fff;}
.course-body{padding:1.25rem;}
.course-rating{display:flex;align-items:center;gap:5px;margin-bottom:.5rem;}
.stars{color:#F59E0B;font-size:12px;letter-spacing:1px;}
.rating-num{font-size:12px;font-weight:600;color:var(--muted);}
.course-title{font-size:15px;font-weight:700;color:var(--ink);margin-bottom:.4rem;line-height:1.35;}
.course-desc{font-size:12px;color:var(--muted);line-height:1.55;margin-bottom:.85rem;}
.course-meta{display:flex;gap:1rem;flex-wrap:wrap;margin-bottom:.85rem;}
.course-meta-item{font-size:11px;color:var(--muted);display:flex;align-items:center;gap:4px;font-weight:500;}
.course-footer{display:flex;align-items:center;justify-content:space-between;padding-top:.85rem;border-top:1px solid var(--border);}
.course-price{font-family:var(--serif);font-size:1.3rem;font-weight:700;color:var(--ink);}
.course-price-old{font-size:12px;color:var(--muted2);text-decoration:line-through;margin-left:4px;}
.btn-enrol{background:var(--blue-pale);color:var(--blue-dark);border:none;padding:7px 16px;border-radius:var(--r);font-family:var(--sans);font-size:12px;font-weight:700;cursor:pointer;transition:all .2s;}
.btn-enrol:hover{background:var(--blue);color:#fff;}

/* ─── CALENDAR / UPCOMING ─── */
.calendar-section{background:var(--ink);}
.calendar-section .section-title{color:#fff;}
.calendar-section .section-sub{color:rgba(255,255,255,.5);}
.calendar-section .section-label{color:#60A5FA;}
.cal-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:1rem;margin-top:2.5rem;}
.cal-card{background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.08);border-radius:var(--r-lg);padding:1.5rem;transition:all .2s;}
.cal-card:hover{background:rgba(37,99,235,.1);border-color:rgba(37,99,235,.3);transform:translateY(-2px);}
.cal-date-block{display:flex;align-items:center;gap:12px;margin-bottom:1rem;}
.cal-day{font-family:var(--serif);font-size:2.2rem;font-weight:700;color:#60A5FA;line-height:1;}
.cal-month-year{font-size:11px;color:rgba(255,255,255,.4);text-transform:uppercase;letter-spacing:.08em;font-weight:600;}
.cal-duration{font-size:10px;color:#93C5FD;background:rgba(37,99,235,.2);padding:3px 8px;border-radius:3px;font-weight:700;margin-top:3px;display:inline-block;}
.cal-title{font-size:15px;font-weight:700;color:#fff;margin-bottom:.4rem;line-height:1.3;}
.cal-meta{font-size:12px;color:rgba(255,255,255,.4);margin-bottom:1rem;}
.cal-footer{display:flex;align-items:center;justify-content:space-between;padding-top:.85rem;border-top:1px solid rgba(255,255,255,.07);}
.cal-seats{font-size:11px;color:#93C5FD;font-weight:600;}
.btn-cal{background:var(--blue);color:#fff;border:none;padding:8px 18px;border-radius:var(--r);font-family:var(--sans);font-size:12px;font-weight:700;cursor:pointer;transition:all .2s;}
.btn-cal:hover{background:var(--blue-dark);}

/* ─── MEMBERSHIPS ─── */
.plans-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:1.5rem;margin-top:2.5rem;}
.plan-card{background:var(--white);border:1.5px solid var(--border);border-radius:var(--r-xl);padding:2rem;transition:all .2s;position:relative;}
.plan-card.featured{border-color:var(--blue);border-width:2px;}
.plan-badge{position:absolute;top:-14px;left:50%;transform:translateX(-50%);background:var(--blue);color:#fff;font-size:11px;font-weight:700;padding:4px 16px;border-radius:20px;letter-spacing:.06em;text-transform:uppercase;white-space:nowrap;}
.plan-icon{font-size:2rem;margin-bottom:.75rem;display:block;}
.plan-name{font-size:13px;font-weight:700;text-transform:uppercase;letter-spacing:.1em;color:var(--muted);margin-bottom:.25rem;}
.plan-price{display:flex;align-items:baseline;gap:6px;margin:1rem 0 .25rem;}
.plan-amount{font-family:var(--serif);font-size:2.5rem;font-weight:700;color:var(--ink);line-height:1;}
.plan-period{font-size:13px;color:var(--muted);}
.plan-desc{font-size:13px;color:var(--muted);margin-bottom:1.5rem;line-height:1.55;}
.plan-features{display:flex;flex-direction:column;gap:8px;margin-bottom:1.75rem;}
.plan-feat{display:flex;align-items:center;gap:8px;font-size:13px;color:var(--text);}
.plan-feat-icon{color:var(--green);font-size:14px;flex-shrink:0;width:16px;}
.btn-plan{width:100%;padding:13px;border-radius:var(--r);font-family:var(--sans);font-size:14px;font-weight:700;cursor:pointer;transition:all .2s;}
.btn-plan.primary{background:var(--blue);color:#fff;border:none;}
.btn-plan.primary:hover{background:var(--blue-dark);}
.btn-plan.outline{background:transparent;color:var(--blue);border:1.5px solid var(--blue);}
.btn-plan.outline:hover{background:var(--blue-pale);}

/* ─── CATEGORIES ─── */
.cat-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:1rem;margin-top:2rem;}
.cat-card{background:var(--white);border:1.5px solid var(--border);border-radius:var(--r-lg);padding:1.5rem 1.25rem;text-align:center;cursor:pointer;transition:all .2s;text-decoration:none;display:block;}
.cat-card:hover{border-color:var(--blue);background:var(--blue-pale);transform:translateY(-2px);}
.cat-card:hover .cat-count{color:var(--blue);}
.cat-icon{font-size:2rem;margin-bottom:.75rem;display:block;}
.cat-name{font-size:14px;font-weight:700;color:var(--ink);margin-bottom:3px;}
.cat-count{font-size:12px;color:var(--muted);transition:color .2s;}

/* ─── E-LEARNING DASHBOARD PREVIEW ─── */
.dash-preview{background:var(--slate);border-radius:var(--r-xl);border:1.5px solid var(--border);overflow:hidden;margin-top:2.5rem;}
.dash-header{background:var(--ink);padding:1rem 1.5rem;display:flex;align-items:center;gap:1rem;}
.dash-dots{display:flex;gap:5px;}
.dash-dot{width:10px;height:10px;border-radius:50%;}
.dash-title{font-size:13px;color:rgba(255,255,255,.5);font-weight:500;}
.dash-inner{display:grid;grid-template-columns:220px 1fr;min-height:400px;}
.dash-sidebar{background:var(--ink2);padding:1.25rem;border-right:1px solid rgba(255,255,255,.06);}
.dash-nav-item{display:flex;align-items:center;gap:10px;padding:8px 10px;border-radius:var(--r);cursor:pointer;margin-bottom:4px;transition:all .2s;font-size:13px;color:rgba(255,255,255,.5);font-weight:500;}
.dash-nav-item.active{background:rgba(37,99,235,.2);color:#93C5FD;}
.dash-nav-item:hover{background:rgba(255,255,255,.05);color:rgba(255,255,255,.8);}
.dash-nav-icon{font-size:15px;width:20px;text-align:center;}
.dash-main{padding:1.5rem;overflow:auto;}
.dash-welcome{font-size:16px;font-weight:700;color:var(--ink);margin-bottom:4px;}
.dash-sub{font-size:13px;color:var(--muted);margin-bottom:1.5rem;}
.dash-stats{display:grid;grid-template-columns:repeat(3,1fr);gap:.75rem;margin-bottom:1.5rem;}
.dash-stat{background:var(--white);border:1px solid var(--border);border-radius:var(--r);padding:.85rem;}
.dash-stat-num{font-size:1.4rem;font-weight:700;color:var(--ink);font-family:var(--serif);}
.dash-stat-label{font-size:11px;color:var(--muted);margin-top:2px;}
.dash-courses-label{font-size:12px;font-weight:700;color:var(--ink);margin-bottom:.75rem;text-transform:uppercase;letter-spacing:.06em;}
.dash-course-item{background:var(--white);border:1px solid var(--border);border-radius:var(--r);padding:.75rem 1rem;display:flex;align-items:center;gap:1rem;margin-bottom:.5rem;}
.dci-icon{font-size:1.25rem;width:36px;height:36px;background:var(--blue-pale);border-radius:var(--r);display:flex;align-items:center;justify-content:center;flex-shrink:0;}
.dci-name{font-size:13px;font-weight:600;color:var(--ink);flex:1;}
.dci-progress{font-size:11px;color:var(--muted);}
.progress-bar{height:4px;background:var(--border);border-radius:2px;margin-top:4px;width:140px;}
.progress-fill{height:100%;border-radius:2px;background:var(--blue);}
.dash-cert-item{background:var(--white);border:1px solid var(--border);border-radius:var(--r);padding:.75rem 1rem;display:flex;align-items:center;justify-content:space-between;margin-bottom:.5rem;}
.cert-name{font-size:13px;font-weight:600;color:var(--ink);}
.cert-date{font-size:11px;color:var(--muted);}
.btn-cert{background:var(--blue-pale);color:var(--blue-dark);border:none;padding:5px 12px;border-radius:var(--r);font-size:11px;font-weight:700;cursor:pointer;}

/* ─── TESTIMONIALS ─── */
.testi-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:1.5rem;margin-top:2.5rem;}
.testi-card{background:var(--white);border:1.5px solid var(--border);border-radius:var(--r-lg);padding:1.75rem;transition:all .2s;}
.testi-card:hover{border-color:rgba(37,99,235,.3);box-shadow:0 8px 30px rgba(37,99,235,.08);transform:translateY(-2px);}
.testi-stars{color:#F59E0B;font-size:14px;letter-spacing:2px;margin-bottom:.85rem;}
.testi-text{font-family:var(--serif);font-size:15px;font-style:italic;color:var(--text);line-height:1.7;margin-bottom:1.25rem;}
.testi-footer{display:flex;align-items:center;gap:.75rem;padding-top:1rem;border-top:1px solid var(--border);}
.testi-av{width:38px;height:38px;border-radius:50%;background:var(--blue-pale);display:flex;align-items:center;justify-content:center;font-size:13px;font-weight:700;color:var(--blue-dark);flex-shrink:0;}
.testi-name{font-size:13px;font-weight:700;color:var(--ink);}
.testi-role{font-size:11px;color:var(--muted);margin-top:1px;}
.testi-sector{margin-left:auto;font-size:10px;text-transform:uppercase;letter-spacing:.08em;color:var(--blue);background:var(--blue-pale);padding:3px 8px;border-radius:3px;font-weight:700;}

/* ─── STATS BANNER ─── */
.stats-banner{background:var(--blue);padding:60px 0;}
.stats-inner{display:grid;grid-template-columns:repeat(4,1fr);gap:2rem;text-align:center;}
.stat-big{font-family:var(--serif);font-size:3rem;font-weight:700;color:#fff;letter-spacing:-.02em;}
.stat-label{font-size:12px;font-weight:600;color:rgba(255,255,255,.6);text-transform:uppercase;letter-spacing:.08em;margin-top:4px;}

/* ─── CORPORATE ─── */
.corp-inner{display:grid;grid-template-columns:1fr 1fr;gap:5rem;align-items:center;}
.corp-form{background:var(--slate);border:1.5px solid var(--border);border-radius:var(--r-xl);padding:2.5rem;}
.form-title{font-family:var(--serif);font-size:1.5rem;font-weight:700;color:var(--ink);margin-bottom:.25rem;}
.form-sub{font-size:13px;color:var(--muted);margin-bottom:1.5rem;}
.fg{margin-bottom:1.1rem;}
.fl{display:block;font-size:11px;font-weight:700;color:var(--muted);letter-spacing:.06em;text-transform:uppercase;margin-bottom:6px;}
.fi,.fs,.ft{width:100%;background:var(--white);border:1.5px solid var(--border);border-radius:var(--r);padding:11px 14px;color:var(--text);font-family:var(--sans);font-size:14px;outline:none;transition:border-color .2s;}
.fi:focus,.fs:focus,.ft:focus{border-color:var(--blue);}
.fs option{background:var(--white);}
.ft{min-height:90px;resize:vertical;}
.fg-2{display:grid;grid-template-columns:1fr 1fr;gap:.85rem;}
.corp-perks{margin-top:2rem;display:flex;flex-direction:column;gap:1.25rem;}
.corp-perk{display:flex;gap:.85rem;align-items:flex-start;}
.cp-icon{width:36px;height:36px;flex-shrink:0;background:var(--blue-pale);border-radius:var(--r);display:flex;align-items:center;justify-content:center;font-size:17px;}
.cp-title{font-size:14px;font-weight:700;color:var(--ink);margin-bottom:2px;}
.cp-body{font-size:13px;color:var(--muted);line-height:1.55;}

/* ─── CONSULTING ─── */
.cons-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:1rem;margin-top:2rem;}
.cons-card{background:var(--white);border:1.5px solid var(--border);border-radius:var(--r-lg);padding:1.5rem;transition:all .2s;cursor:pointer;}
.cons-card:hover{border-color:var(--blue);transform:translateY(-2px);}
.cons-icon{font-size:1.75rem;margin-bottom:.75rem;display:block;}
.cons-title{font-size:15px;font-weight:700;color:var(--ink);margin-bottom:.4rem;}
.cons-body{font-size:13px;color:var(--muted);line-height:1.55;}
.cons-link{font-size:12px;color:var(--blue);font-weight:600;margin-top:.75rem;display:inline-block;}

/* ─── FOOTER ─── */
footer{background:var(--ink);padding:60px 0 28px;}
.footer-grid{display:grid;grid-template-columns:2fr 1fr 1fr 1fr;gap:3rem;margin-bottom:3rem;}
.footer-brand p{font-size:13px;color:rgba(255,255,255,.35);line-height:1.7;margin-top:.85rem;max-width:280px;font-weight:300;}
.footer-col-title{font-size:11px;font-weight:700;letter-spacing:.12em;text-transform:uppercase;color:#60A5FA;margin-bottom:1rem;}
.footer-links{list-style:none;display:flex;flex-direction:column;gap:9px;}
.footer-links a{font-size:13px;color:rgba(255,255,255,.35);transition:color .2s;}
.footer-links a:hover{color:#60A5FA;}
.footer-bottom{border-top:1px solid rgba(255,255,255,.07);padding-top:1.5rem;display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;gap:1rem;}
.footer-copy{font-size:12px;color:rgba(255,255,255,.2);}
.footer-socials{display:flex;gap:8px;}
.social-btn{width:32px;height:32px;border:1px solid rgba(255,255,255,.1);border-radius:var(--r);display:flex;align-items:center;justify-content:center;font-size:13px;color:rgba(255,255,255,.35);transition:all .2s;text-decoration:none;}
.social-btn:hover{border-color:#60A5FA;color:#60A5FA;}

/* ─── WHATSAPP ─── */
.wa-float{position:fixed;bottom:2rem;right:2rem;z-index:900;width:56px;height:56px;background:#25D366;border-radius:50%;display:flex;align-items:center;justify-content:center;box-shadow:0 4px 20px rgba(37,211,102,.4);cursor:pointer;text-decoration:none;transition:all .2s;animation:wa-pulse 3s ease-in-out infinite;}
@keyframes wa-pulse{0%,100%{box-shadow:0 4px 20px rgba(37,211,102,.4);}50%{box-shadow:0 4px 36px rgba(37,211,102,.65);}}
.wa-float:hover{transform:scale(1.1);}
.wa-float svg{width:28px;height:28px;fill:#fff;}

/* ─── ANIMATIONS ─── */
.fade-up{opacity:0;transform:translateY(28px);transition:opacity .7s ease,transform .7s ease;}
.fade-up.visible{opacity:1;transform:translateY(0);}
.s1{transition-delay:.1s;}.s2{transition-delay:.2s;}.s3{transition-delay:.3s;}.s4{transition-delay:.4s;}

/* ─── RESPONSIVE ─── */
@media(max-width:1100px){
  .hero{grid-template-columns:1fr;}
  .hero-right{display:none;}
  .hero-left{padding:80px 2rem;}
  .footer-grid{grid-template-columns:1fr 1fr;gap:2rem;}
  .corp-inner{grid-template-columns:1fr;}
}
@media(max-width:900px){
  .courses-grid,.testi-grid,.plans-grid{grid-template-columns:1fr 1fr;}
  .cat-grid{grid-template-columns:repeat(2,1fr);}
  .cal-grid{grid-template-columns:1fr;}
  .stats-inner{grid-template-columns:repeat(2,1fr);}
  .cons-grid{grid-template-columns:1fr 1fr;}
  .nav-links{display:none;}
  .dash-inner{grid-template-columns:1fr;}
  .dash-sidebar{display:none;}
}
@media(max-width:600px){
  .courses-grid,.testi-grid,.plans-grid,.cons-grid{grid-template-columns:1fr;}
  .cat-grid{grid-template-columns:1fr 1fr;}
  .stats-inner{grid-template-columns:1fr 1fr;}
  .footer-grid{grid-template-columns:1fr;}
  .fg-2{grid-template-columns:1fr;}
}
</style>
</head>
<body>

<!-- WA FLOAT -->
<a class="wa-float" href="https://wa.me/254722223084?text=Hello%20CCS%2C%20I%27m%20interested%20in%20your%20training%20programs.%20Can%20you%20help?" target="_blank">
  <svg viewBox="0 0 24 24"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347z"/><path d="M12 0C5.373 0 0 5.373 0 12c0 2.126.556 4.121 1.528 5.847L0 24l6.335-1.652A11.954 11.954 0 0012 24c6.627 0 12-5.373 12-12S18.627 0 12 0zm0 21.818a9.818 9.818 0 01-5.013-1.378l-.36-.214-3.732.978.994-3.636-.235-.374A9.818 9.818 0 1112 21.818z"/></svg>
</a>

<!-- TOPBAR -->
<div class="topbar">
  <div class="topbar-left">
    <div class="topbar-item">📞 <strong>+254 722 223 084</strong></div>
    <div class="topbar-item">✉️ <strong>info@corporate.co.ke</strong></div>
    <div class="topbar-item">📍 Repen Complex, Nairobi</div>
  </div>
  <div class="topbar-right">
    <button class="tb-btn" onclick="showModal('login')">Log In</button>
    <button class="tb-btn primary" onclick="showModal('signup')">Start Learning Free</button>
  </div>
</div>

<!-- NAV -->
<nav>
  <div class="nav-inner">
    <a href="#" class="nav-logo">
      <div class="logo-main">Centre of <span>Corporate</span> Studies</div>
      <div class="logo-sub">Training · E-Learning · Consulting · Kenya</div>
    </a>
    <ul class="nav-links">
      <li><a href="#courses" class="active">Courses</a></li>
      <li><a href="#calendar">Live Training</a></li>
      <li><a href="#membership">Membership</a></li>
      <li><a href="#consulting">Consulting</a></li>
      <li><a href="#corporate">Corporate</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
    <div class="nav-right">
      <a href="#membership" class="btn-outline">View Plans</a>
      <a href="#courses" class="btn-primary">Browse Courses</a>
    </div>
  </div>
</nav>

<!-- HERO -->
<section class="hero">
  <div class="hero-pattern"></div>
  <div class="hero-glow"></div>
  <div class="hero-left">
    <div class="hero-badge"><div class="badge-dot"></div> Kenya's Premier Corporate Learning Platform</div>
    <h1>Learn Today.<br><span class="accent">Lead</span> Tomorrow.<br><span class="dim">Anywhere.</span></h1>
    <p class="hero-sub">Professional training, certified e-learning courses, and expert consulting — all in one platform. Study online at your pace or attend live sessions in Nairobi.</p>
    <div class="hero-actions">
      <a href="#courses" class="btn-hero-primary">🎓 Browse All Courses</a>
      <a href="#membership" class="btn-hero-ghost">💎 View Membership Plans</a>
    </div>
    <div class="hero-stats">
      <div><div class="hstat-num">500+</div><div class="hstat-label">Organisations trained</div></div>
      <div><div class="hstat-num">50+</div><div class="hstat-label">Online courses</div></div>
      <div><div class="hstat-num">20yr</div><div class="hstat-label">Industry experience</div></div>
      <div><div class="hstat-num">CPD</div><div class="hstat-label">Accredited certificates</div></div>
    </div>
  </div>
  <div class="hero-right">
    <!-- Search & Course Finder -->
    <div class="search-hero">
      <div class="search-hero-title">🔍 Find Your Course</div>
      <div class="search-box">
        <input class="search-input" type="text" placeholder="e.g. Leadership, Finance, HR Management..." id="heroSearch">
        <select class="search-cat" id="heroCategory">
          <option value="">All Topics</option>
          <option>Leadership</option><option>Finance</option><option>HR</option>
          <option>Project Management</option><option>Sales & Marketing</option>
          <option>Procurement</option><option>Customer Service</option><option>Strategy</option>
        </select>
        <button class="btn-search" onclick="searchCourses()">Search</button>
      </div>
      <div class="search-tags">
        <span class="stag" onclick="quickSearch('Leadership')">Leadership</span>
        <span class="stag" onclick="quickSearch('Finance')">Finance</span>
        <span class="stag" onclick="quickSearch('HR')">HR</span>
        <span class="stag" onclick="quickSearch('Project Management')">Project Mgmt</span>
        <span class="stag" onclick="quickSearch('Procurement')">Procurement</span>
        <span class="stag" onclick="quickSearch('Online')">Online Only</span>
      </div>
    </div>
    <!-- Membership Card -->
    <div class="mem-card">
      <div class="mem-card-label">💎 CCS Prime Membership</div>
      <div class="mem-card-title">Unlimited Learning Access</div>
      <div class="mem-card-sub">All online courses + recordings + certificates for one annual fee</div>
      <div class="mem-price">
        <div class="mem-amount">KES 15,000</div>
        <div class="mem-period">/year</div>
        <div class="mem-old">KES 45,000</div>
      </div>
      <div class="mem-features">
        <div class="mem-feat"><div class="feat-check">✓</div>Unlimited access to 50+ courses</div>
        <div class="mem-feat"><div class="feat-check">✓</div>CPD-accredited certificates</div>
        <div class="mem-feat"><div class="feat-check">✓</div>Live session recordings</div>
        <div class="mem-feat"><div class="feat-check">✓</div>Learner dashboard & progress tracking</div>
      </div>
      <button class="btn-mem" onclick="enrollMembership()">Get Prime Access — KES 15,000/yr</button>
    </div>
  </div>
</section>

<!-- TRUST BAR -->
<div class="trust-bar">
  <div class="container">
    <div class="trust-items">
      <div class="ti"><div class="ti-icon">🎓</div><div><div class="ti-title">CPD Accredited</div><div class="ti-sub">Internationally recognised certificates</div></div></div>
      <div class="ti"><div class="ti-icon">💻</div><div><div class="ti-title">Learn Anywhere</div><div class="ti-sub">Online · Virtual · In-person</div></div></div>
      <div class="ti"><div class="ti-icon">📱</div><div><div class="ti-title">M-Pesa Accepted</div><div class="ti-sub">Instant enrolment after payment</div></div></div>
      <div class="ti"><div class="ti-icon">🏆</div><div><div class="ti-title">20 Years Experience</div><div class="ti-sub">Kenya's trusted training partner</div></div></div>
      <div class="ti"><div class="ti-icon">🔄</div><div><div class="ti-title">Self-Paced</div><div class="ti-sub">Study at your own speed</div></div></div>
    </div>
  </div>
</div>

<!-- COURSE CATEGORIES -->
<section class="section" style="background:var(--slate2);padding-bottom:0;">
  <div class="container">
    <div class="fade-up">
      <div class="section-label">Browse by topic</div>
      <h2 class="section-title">Learn What <span class="muted">Matters Most</span></h2>
    </div>
    <div class="cat-grid fade-up">
      <a href="#courses" class="cat-card"><span class="cat-icon">🏆</span><div class="cat-name">Leadership & Management</div><div class="cat-count">12 courses</div></a>
      <a href="#courses" class="cat-card"><span class="cat-icon">💰</span><div class="cat-name">Finance & Accounting</div><div class="cat-count">8 courses</div></a>
      <a href="#courses" class="cat-card"><span class="cat-icon">👥</span><div class="cat-name">Human Resources</div><div class="cat-count">9 courses</div></a>
      <a href="#courses" class="cat-card"><span class="cat-icon">📊</span><div class="cat-name">Strategic Planning</div><div class="cat-count">6 courses</div></a>
      <a href="#courses" class="cat-card"><span class="cat-icon">📈</span><div class="cat-name">Sales & Marketing</div><div class="cat-count">7 courses</div></a>
      <a href="#courses" class="cat-card"><span class="cat-icon">📋</span><div class="cat-name">Procurement & Contracts</div><div class="cat-count">5 courses</div></a>
      <a href="#courses" class="cat-card"><span class="cat-icon">🗂️</span><div class="cat-name">Project Management</div><div class="cat-count">8 courses</div></a>
      <a href="#courses" class="cat-card"><span class="cat-icon">⭐</span><div class="cat-name">Customer Service</div><div class="cat-count">6 courses</div></a>
    </div>
  </div>
</section>

<!-- COURSES -->
<section class="section" id="courses" style="background:var(--slate2);">
  <div class="container">
    <div class="section-head-row fade-up">
      <div>
        <div class="section-label">Online & in-person</div>
        <h2 class="section-title">Featured <span class="muted">Courses</span></h2>
        <p class="section-sub">Self-paced online courses, live virtual cohorts, and in-house training — all CPD accredited.</p>
      </div>
      <a href="#courses" class="btn-outline" style="flex-shrink:0;">View All 50+ Courses →</a>
    </div>
    <div class="courses-filters fade-up">
      <button class="filter-btn active" onclick="filterCourses(this,'all')">All Courses</button>
      <button class="filter-btn" onclick="filterCourses(this,'online')">Online Only</button>
      <button class="filter-btn" onclick="filterCourses(this,'live')">Live Training</button>
      <button class="filter-btn" onclick="filterCourses(this,'leadership')">Leadership</button>
      <button class="filter-btn" onclick="filterCourses(this,'finance')">Finance</button>
      <button class="filter-btn" onclick="filterCourses(this,'hr')">HR</button>
      <button class="filter-btn" onclick="filterCourses(this,'project')">Project Mgmt</button>
    </div>
    <div class="courses-grid" id="coursesGrid">
      <!-- Rendered by JS -->
    </div>
  </div>
</section>

<!-- E-LEARNING DASHBOARD PREVIEW -->
<section class="section" style="background:var(--white);">
  <div class="container">
    <div class="section-head-row fade-up">
      <div>
        <div class="section-label">Your learning hub</div>
        <h2 class="section-title">A Dashboard Built <span class="muted">for Learners</span></h2>
        <p class="section-sub">Track your progress, download certificates, access course recordings, and manage your learning journey — all in one place.</p>
      </div>
      <button class="btn-primary" onclick="showModal('signup')">Create Free Account →</button>
    </div>
    <div class="dash-preview fade-up">
      <div class="dash-header">
        <div class="dash-dots">
          <div class="dash-dot" style="background:#FF5F57;"></div>
          <div class="dash-dot" style="background:#FEBC2E;"></div>
          <div class="dash-dot" style="background:#28C840;"></div>
        </div>
        <div class="dash-title">CCS Learning Portal — My Dashboard</div>
      </div>
      <div class="dash-inner">
        <div class="dash-sidebar">
          <div style="font-size:12px;font-weight:700;color:rgba(255,255,255,.3);letter-spacing:.1em;text-transform:uppercase;margin-bottom:1rem;padding:0 10px;">Menu</div>
          <div class="dash-nav-item active"><span class="dash-nav-icon">🏠</span>Dashboard</div>
          <div class="dash-nav-item"><span class="dash-nav-icon">📚</span>My Courses</div>
          <div class="dash-nav-item"><span class="dash-nav-icon">🎓</span>Certificates</div>
          <div class="dash-nav-item"><span class="dash-nav-icon">📅</span>Upcoming Sessions</div>
          <div class="dash-nav-item"><span class="dash-nav-icon">📝</span>Assignments</div>
          <div class="dash-nav-item"><span class="dash-nav-icon">💬</span>Discussion Forum</div>
          <div class="dash-nav-item"><span class="dash-nav-icon">⚙️</span>Settings</div>
        </div>
        <div class="dash-main">
          <div class="dash-welcome">Good morning, Janet 👋</div>
          <div class="dash-sub">You have 2 courses in progress and 1 certificate ready to download.</div>
          <div class="dash-stats">
            <div class="dash-stat"><div class="dash-stat-num">4</div><div class="dash-stat-label">Courses enrolled</div></div>
            <div class="dash-stat"><div class="dash-stat-num">2</div><div class="dash-stat-label">Certificates earned</div></div>
            <div class="dash-stat"><div class="dash-stat-num">67%</div><div class="dash-stat-label">Avg. completion</div></div>
          </div>
          <div class="dash-courses-label">Continue Learning</div>
          <div class="dash-course-item"><div class="dci-icon">🏆</div><div style="flex:1;"><div class="dci-name">Strategic Leadership for Managers</div><div class="dci-progress">67% complete</div><div class="progress-bar"><div class="progress-fill" style="width:67%"></div></div></div></div>
          <div class="dash-course-item"><div class="dci-icon">💰</div><div style="flex:1;"><div class="dci-name">Finance for Non-Finance Managers</div><div class="dci-progress">34% complete</div><div class="progress-bar"><div class="progress-fill" style="width:34%"></div></div></div></div>
          <div class="dash-courses-label" style="margin-top:1.25rem;">Your Certificates</div>
          <div class="dash-cert-item"><div><div class="cert-name">HR Management — Fundamentals</div><div class="cert-date">Issued: March 2026 · CPD Accredited</div></div><button class="btn-cert">⬇ Download</button></div>
          <div class="dash-cert-item"><div><div class="cert-name">Customer Service Excellence</div><div class="cert-date">Issued: Jan 2026 · CPD Accredited</div></div><button class="btn-cert">⬇ Download</button></div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- LIVE TRAINING CALENDAR -->
<section class="calendar-section section" id="calendar">
  <div class="container">
    <div class="section-head-row fade-up">
      <div>
        <div class="section-label">Upcoming sessions</div>
        <h2 class="section-title" style="color:#fff;">Live Training <span style="color:rgba(255,255,255,.3);">Calendar</span></h2>
        <p class="section-sub">Attend in Nairobi or join virtually via Zoom. Book early — sessions fill fast.</p>
      </div>
      <button class="btn-primary" style="flex-shrink:0;">View Full Calendar →</button>
    </div>
    <div class="cal-grid fade-up">
      <div class="cal-card">
        <div class="cal-date-block"><div><div class="cal-day">22</div><div class="cal-month-year">April 2026</div><div class="cal-duration">3 Days</div></div></div>
        <div class="cal-title">Strategic Leadership for Senior Managers</div>
        <div class="cal-meta">📍 Nairobi CBD · Also Virtual · Group discounts available</div>
        <div class="cal-footer"><span class="cal-seats">⚡ 6 seats remaining</span><button class="btn-cal" onclick="bookSession('Strategic Leadership Apr 22')">Book Now</button></div>
      </div>
      <div class="cal-card">
        <div class="cal-date-block"><div><div class="cal-day">5</div><div class="cal-month-year">May 2026</div><div class="cal-duration">2 Days</div></div></div>
        <div class="cal-title">Financial Management for Non-Finance Professionals</div>
        <div class="cal-meta">📍 Westlands, Nairobi · CPD Accredited</div>
        <div class="cal-footer"><span class="cal-seats">⚡ 9 seats remaining</span><button class="btn-cal" onclick="bookSession('Financial Management May 5')">Book Now</button></div>
      </div>
      <div class="cal-card">
        <div class="cal-date-block"><div><div class="cal-day">19</div><div class="cal-month-year">May 2026</div><div class="cal-duration">3 Days</div></div></div>
        <div class="cal-title">HR Management & Labour Law Compliance</div>
        <div class="cal-meta">📍 Nairobi CBD · Virtual option available</div>
        <div class="cal-footer"><span class="cal-seats">⚡ 7 seats remaining</span><button class="btn-cal" onclick="bookSession('HR Management May 19')">Book Now</button></div>
      </div>
      <div class="cal-card">
        <div class="cal-date-block"><div><div class="cal-day">3</div><div class="cal-month-year">June 2026</div><div class="cal-duration">2 Days</div></div></div>
        <div class="cal-title">Project Management — PMP Aligned</div>
        <div class="cal-meta">🌐 Virtual Only — Zoom · Recordings provided</div>
        <div class="cal-footer"><span class="cal-seats">⚡ 14 seats remaining</span><button class="btn-cal" onclick="bookSession('Project Management June 3')">Book Now</button></div>
      </div>
      <div class="cal-card">
        <div class="cal-date-block"><div><div class="cal-day">17</div><div class="cal-month-year">June 2026</div><div class="cal-duration">1 Day</div></div></div>
        <div class="cal-title">Customer Service Excellence Masterclass</div>
        <div class="cal-meta">📍 Nairobi CBD · Limited to 20 participants</div>
        <div class="cal-footer"><span class="cal-seats">⚡ 5 seats remaining</span><button class="btn-cal" onclick="bookSession('Customer Service June 17')">Book Now</button></div>
      </div>
      <div class="cal-card">
        <div class="cal-date-block"><div><div class="cal-day">30</div><div class="cal-month-year">June 2026</div><div class="cal-duration">3 Days</div></div></div>
        <div class="cal-title">Procurement & Contract Management</div>
        <div class="cal-meta">📍 Nairobi · Also Virtual · Government & NGO rates</div>
        <div class="cal-footer"><span class="cal-seats">⚡ 10 seats remaining</span><button class="btn-cal" onclick="bookSession('Procurement June 30')">Book Now</button></div>
      </div>
    </div>
    <div style="text-align:center;margin-top:2rem;" class="fade-up">
      <a href="https://wa.me/254722223084?text=I%27d%20like%20to%20book%20a%20training%20session.%20Can%20you%20send%20the%20full%202026%20calendar?" target="_blank" class="btn-primary" style="display:inline-flex;align-items:center;gap:8px;">💬 Request Inhouse Training for Your Team</a>
    </div>
  </div>
</section>

<!-- MEMBERSHIP PLANS -->
<section class="section" id="membership">
  <div class="container">
    <div class="fade-up" style="text-align:center;max-width:600px;margin:0 auto;">
      <div class="section-label">Flexible access</div>
      <h2 class="section-title">Choose Your <span class="muted">Learning Plan</span></h2>
      <p class="section-sub" style="margin:0 auto;">From a single course to unlimited annual access — we have a plan for every professional and every team.</p>
    </div>
    <div class="plans-grid fade-up">
      <div class="plan-card">
        <span class="plan-icon">📖</span>
        <div class="plan-name">Starter</div>
        <div class="plan-price"><div class="plan-amount">KES 3,500</div><div class="plan-period">per course</div></div>
        <div class="plan-desc">Perfect for individuals looking to upskill in one specific area. Buy any single online course and study at your own pace.</div>
        <div class="plan-features">
          <div class="plan-feat"><span class="plan-feat-icon">✓</span>1 online course (lifetime access)</div>
          <div class="plan-feat"><span class="plan-feat-icon">✓</span>CPD certificate on completion</div>
          <div class="plan-feat"><span class="plan-feat-icon">✓</span>Course recordings & materials</div>
          <div class="plan-feat"><span class="plan-feat-icon">✓</span>Mobile & desktop access</div>
        </div>
        <button class="btn-plan outline" onclick="enrolPlan('Starter')">Browse Courses</button>
      </div>
      <div class="plan-card featured">
        <div class="plan-badge">Most Popular</div>
        <span class="plan-icon">💎</span>
        <div class="plan-name" style="color:var(--blue);">CCS Prime</div>
        <div class="plan-price"><div class="plan-amount">KES 15,000</div><div class="plan-period">/year</div></div>
        <div class="plan-desc">Unlimited access to all 50+ online courses for 12 months. The most cost-effective way to build multiple professional skills.</div>
        <div class="plan-features">
          <div class="plan-feat"><span class="plan-feat-icon" style="color:var(--blue);">✓</span>Unlimited access to all 50+ courses</div>
          <div class="plan-feat"><span class="plan-feat-icon" style="color:var(--blue);">✓</span>New courses added monthly</div>
          <div class="plan-feat"><span class="plan-feat-icon" style="color:var(--blue);">✓</span>All CPD certificates included</div>
          <div class="plan-feat"><span class="plan-feat-icon" style="color:var(--blue);">✓</span>Live session recordings</div>
          <div class="plan-feat"><span class="plan-feat-icon" style="color:var(--blue);">✓</span>Priority support & WhatsApp access</div>
          <div class="plan-feat"><span class="plan-feat-icon" style="color:var(--blue);">✓</span>10% off all live training sessions</div>
        </div>
        <button class="btn-plan primary" onclick="enrolPlan('Prime')">Get Prime — KES 15,000/yr</button>
      </div>
      <div class="plan-card">
        <span class="plan-icon">🏢</span>
        <div class="plan-name">Corporate Teams</div>
        <div class="plan-price"><div class="plan-amount">KES 80,000</div><div class="plan-period">/20 users/yr</div></div>
        <div class="plan-desc">Empower your entire team with a shared corporate licence. Assign courses, track progress, and pull completion reports for HR.</div>
        <div class="plan-features">
          <div class="plan-feat"><span class="plan-feat-icon">✓</span>20 user seats (expandable)</div>
          <div class="plan-feat"><span class="plan-feat-icon">✓</span>Admin dashboard & reporting</div>
          <div class="plan-feat"><span class="plan-feat-icon">✓</span>Course assignment & tracking</div>
          <div class="plan-feat"><span class="plan-feat-icon">✓</span>Custom learning paths</div>
          <div class="plan-feat"><span class="plan-feat-icon">✓</span>Dedicated account manager</div>
          <div class="plan-feat"><span class="plan-feat-icon">✓</span>LPO & invoicing accepted</div>
        </div>
        <button class="btn-plan outline" onclick="enrolPlan('Corporate')">Request a Demo</button>
      </div>
    </div>
  </div>
</section>

<!-- STATS -->
<div class="stats-banner">
  <div class="container">
    <div class="stats-inner fade-up">
      <div><div class="stat-big">500+</div><div class="stat-label">Organisations trained</div></div>
      <div><div class="stat-big">50+</div><div class="stat-label">Online courses</div></div>
      <div><div class="stat-big">10,000+</div><div class="stat-label">Professionals trained</div></div>
      <div><div class="stat-big">98%</div><div class="stat-label">Client satisfaction</div></div>
    </div>
  </div>
</div>

<!-- TESTIMONIALS -->
<section class="section" style="background:var(--slate2);">
  <div class="container">
    <div class="fade-up" style="text-align:center;max-width:580px;margin:0 auto;">
      <div class="section-label">What professionals say</div>
      <h2 class="section-title">Trusted by <span class="muted">Kenya's Top Organisations</span></h2>
    </div>
    <div class="testi-grid fade-up">
      <div class="testi-card">
        <div class="testi-stars">★★★★★</div>
        <div class="testi-text">"CCS delivered an in-house HR training for our team that was practical, contextual, and measurable. The facilitator understood our banking environment deeply. We've already booked our second session."</div>
        <div class="testi-footer"><div class="testi-av">HK</div><div><div class="testi-name">Head of HR</div><div class="testi-role">Leading Commercial Bank, Nairobi</div></div><div class="testi-sector">Banking</div></div>
      </div>
      <div class="testi-card">
        <div class="testi-stars">★★★★★</div>
        <div class="testi-text">"The online leadership course was excellent — I completed it over 3 weeks while working full-time. The certificate is now on my CV and it's already opened doors. CCS is genuinely world-class."</div>
        <div class="testi-footer"><div class="testi-av">PM</div><div><div class="testi-name">Programme Manager</div><div class="testi-role">UNDP Kenya, Nairobi</div></div><div class="testi-sector">NGO / UN</div></div>
      </div>
      <div class="testi-card">
        <div class="testi-stars">★★★★★</div>
        <div class="testi-text">"We enrolled 15 procurement officers in the online procurement course. The team completed it at their own pace, the content was current and Kenya-specific, and the certificates were accepted by our board."</div>
        <div class="testi-footer"><div class="testi-av">GW</div><div><div class="testi-name">Procurement Director</div><div class="testi-role">County Government of Nairobi</div></div><div class="testi-sector">Government</div></div>
      </div>
    </div>
  </div>
</section>

<!-- CORPORATE TRAINING -->
<section class="section" id="corporate" style="background:var(--white);">
  <div class="container">
    <div class="corp-inner">
      <div class="fade-up">
        <div class="section-label">For organisations</div>
        <h2 class="section-title">Corporate &amp; Inhouse <span class="muted">Training</span></h2>
        <p class="section-sub">We design and deliver training programmes customised to your organisation's needs, industry, and goals — at your premises or virtually.</p>
        <div class="corp-perks">
          <div class="corp-perk"><div class="cp-icon">🎯</div><div><div class="cp-title">100% customised to your industry</div><div class="cp-body">No generic slide decks. Every programme is built around your sector, your team, and your specific challenges.</div></div></div>
          <div class="corp-perk"><div class="cp-icon">📊</div><div><div class="cp-title">Pre and post-training assessment</div><div class="cp-body">We measure learning outcomes so you can demonstrate ROI to leadership and your board.</div></div></div>
          <div class="corp-perk"><div class="cp-icon">📋</div><div><div class="cp-title">LPO and invoicing supported</div><div class="cp-body">Formal procurement process welcome. We work with government, NGOs, and corporates on LPO terms.</div></div></div>
          <div class="corp-perk"><div class="cp-icon">🌍</div><div><div class="cp-title">Delivery anywhere in East Africa</div><div class="cp-body">Our facilitators travel. We have delivered inhouse training in Kenya, Uganda, Tanzania, Rwanda, and Ethiopia.</div></div></div>
        </div>
      </div>
      <div class="corp-form fade-up">
        <div class="form-title">Request a Training Proposal</div>
        <div class="form-sub">We respond within 24 hours with a tailored proposal and pricing.</div>
        <div class="fg-2">
          <div class="fg"><label class="fl">First Name</label><input class="fi" type="text" placeholder="Jane"></div>
          <div class="fg"><label class="fl">Last Name</label><input class="fi" type="text" placeholder="Mwangi"></div>
        </div>
        <div class="fg"><label class="fl">Work Email</label><input class="fi" type="email" placeholder="jane@yourcompany.com"></div>
        <div class="fg"><label class="fl">Phone / WhatsApp</label><input class="fi" type="tel" placeholder="+254 7XX XXX XXX"></div>
        <div class="fg"><label class="fl">Organisation</label><input class="fi" type="text" placeholder="Company or institution name"></div>
        <div class="fg-2">
          <div class="fg"><label class="fl">Training Area</label>
            <select class="fs">
              <option>Leadership & Management</option><option>Finance & Accounting</option>
              <option>HR Management</option><option>Strategic Planning</option>
              <option>Sales & Marketing</option><option>Procurement</option>
              <option>Project Management</option><option>Customer Service</option>
              <option>Team Building</option><option>Custom programme</option>
            </select>
          </div>
          <div class="fg"><label class="fl">Number of Staff</label>
            <select class="fs">
              <option>5–15 staff</option><option>16–30 staff</option>
              <option>31–60 staff</option><option>60+ staff</option>
            </select>
          </div>
        </div>
        <div class="fg"><label class="fl">Message / Details</label><textarea class="ft" placeholder="Tell us your training goals, preferred dates, or any specific requirements..."></textarea></div>
        <button class="btn-primary" style="width:100%;padding:14px;font-size:15px;" onclick="submitCorp()">📤 Request Training Proposal</button>
        <div style="display:flex;align-items:center;gap:.75rem;margin-top:1rem;">
          <div style="flex:1;height:1px;background:var(--border);"></div>
          <div style="font-size:11px;color:var(--muted2);">or</div>
          <div style="flex:1;height:1px;background:var(--border);"></div>
        </div>
        <a href="https://wa.me/254722223084?text=Hello%20CCS%2C%20I%27d%20like%20to%20discuss%20inhouse%20training%20for%20my%20organisation." target="_blank" style="display:flex;align-items:center;justify-content:center;gap:8px;background:#25D366;color:#fff;padding:13px;border-radius:var(--r);font-family:var(--sans);font-size:14px;font-weight:700;margin-top:.75rem;transition:background .2s;" onmouseover="this.style.background='#1fb855'" onmouseout="this.style.background='#25D366'">💬 WhatsApp Us for Fastest Response</a>
      </div>
    </div>
  </div>
</section>

<!-- CONSULTING -->
<section class="section" id="consulting" style="background:var(--slate2);">
  <div class="container">
    <div class="section-head-row fade-up">
      <div>
        <div class="section-label">Advisory services</div>
        <h2 class="section-title">Consulting &amp; <span class="muted">Advisory</span></h2>
        <p class="section-sub">Beyond training — we embed with your organisation to solve complex strategic, governance, and operational challenges.</p>
      </div>
      <a href="#contact" class="btn-outline">Request a Consultation →</a>
    </div>
    <div class="cons-grid fade-up">
      <div class="cons-card"><span class="cons-icon">📊</span><div class="cons-title">Monitoring & Evaluation</div><div class="cons-body">M&E framework design, data collection systems, and impact reporting for NGOs, government, and development projects.</div><div class="cons-link">Learn more →</div></div>
      <div class="cons-card"><span class="cons-icon">🏛️</span><div class="cons-title">Corporate Governance</div><div class="cons-body">Board effectiveness, governance frameworks, and leadership advisory for organisations seeking stronger accountability structures.</div><div class="cons-link">Learn more →</div></div>
      <div class="cons-card"><span class="cons-icon">🏗️</span><div class="cons-title">Business Architecture</div><div class="cons-body">Operating model design, business process optimisation, and organisational restructuring to improve performance and agility.</div><div class="cons-link">Learn more →</div></div>
      <div class="cons-card"><span class="cons-icon">💹</span><div class="cons-title">Financial Services Consulting</div><div class="cons-body">Strategy, risk management, and regulatory compliance advisory for banks, SACCOs, MFIs, and fintech companies.</div><div class="cons-link">Learn more →</div></div>
      <div class="cons-card"><span class="cons-icon">🌾</span><div class="cons-title">Agribusiness Consulting</div><div class="cons-body">Value chain analysis, market linkage strategies, and agricultural enterprise development for smallholders and agri-businesses.</div><div class="cons-link">Learn more →</div></div>
      <div class="cons-card"><span class="cons-icon">🔀</span><div class="cons-title">Mergers & Acquisitions</div><div class="cons-body">Due diligence, integration planning, and post-merger organisational alignment across East Africa's corporate landscape.</div><div class="cons-link">Learn more →</div></div>
    </div>
  </div>
</section>

<!-- CONTACT -->
<section class="section" style="background:var(--ink);" id="contact">
  <div class="container">
    <div style="display:grid;grid-template-columns:1fr 1fr;gap:4rem;align-items:start;" class="fade-up">
      <div>
        <div class="section-label" style="color:#60A5FA;">Get in touch</div>
        <h2 class="section-title" style="color:#fff;font-family:var(--serif);">Ready to <span style="color:#60A5FA;">Start?</span></h2>
        <p style="font-size:15px;color:rgba(255,255,255,.5);line-height:1.7;font-weight:300;margin-bottom:2rem;">Call us, WhatsApp us, or fill in the form. We respond within 24 hours with a personalised plan.</p>
        <div style="display:flex;flex-direction:column;gap:1.25rem;">
          <div style="display:flex;gap:1rem;align-items:flex-start;">
            <div style="width:40px;height:40px;background:rgba(37,99,235,.2);border-radius:var(--r);display:flex;align-items:center;justify-content:center;font-size:18px;flex-shrink:0;">📞</div>
            <div><div style="font-size:11px;text-transform:uppercase;letter-spacing:.08em;color:rgba(255,255,255,.35);margin-bottom:3px;">Call us</div><div style="font-size:15px;color:#fff;font-weight:600;">+254 722 223 084<br>+254 020 200 4965</div></div>
          </div>
          <div style="display:flex;gap:1rem;align-items:flex-start;">
            <div style="width:40px;height:40px;background:rgba(37,99,235,.2);border-radius:var(--r);display:flex;align-items:center;justify-content:center;font-size:18px;flex-shrink:0;">✉️</div>
            <div><div style="font-size:11px;text-transform:uppercase;letter-spacing:.08em;color:rgba(255,255,255,.35);margin-bottom:3px;">Email</div><div style="font-size:15px;color:#fff;font-weight:600;">info@corporate.co.ke</div></div>
          </div>
          <div style="display:flex;gap:1rem;align-items:flex-start;">
            <div style="width:40px;height:40px;background:rgba(37,99,235,.2);border-radius:var(--r);display:flex;align-items:center;justify-content:center;font-size:18px;flex-shrink:0;">📍</div>
            <div><div style="font-size:11px;text-transform:uppercase;letter-spacing:.08em;color:rgba(255,255,255,.35);margin-bottom:3px;">Office</div><div style="font-size:15px;color:#fff;font-weight:600;">Repen Complex, 2nd Floor, Suite 206<br>P.O. Box 26615 – 00100, Nairobi</div></div>
          </div>
        </div>
        <a href="https://wa.me/254722223084?text=Hello%20CCS%2C%20I%27d%20like%20to%20enquire%20about%20your%20services." target="_blank" style="display:inline-flex;align-items:center;gap:8px;background:#25D366;color:#fff;padding:14px 28px;border-radius:var(--r);font-family:var(--sans);font-size:15px;font-weight:700;margin-top:2rem;transition:background .2s;">💬 WhatsApp Us Now</a>
      </div>
      <div style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.09);border-radius:var(--r-xl);padding:2rem;">
        <div class="form-title" style="color:#fff;font-family:var(--serif);">Send an Enquiry</div>
        <div class="form-sub" style="color:rgba(255,255,255,.4);margin-bottom:1.25rem;">We'll get back to you within 24 hours.</div>
        <div class="fg-2">
          <div class="fg"><label class="fl" style="color:rgba(255,255,255,.4);">Name</label><input class="fi" style="background:rgba(255,255,255,.06);border-color:rgba(255,255,255,.1);color:#fff;" type="text" placeholder="Your name"></div>
          <div class="fg"><label class="fl" style="color:rgba(255,255,255,.4);">Phone</label><input class="fi" style="background:rgba(255,255,255,.06);border-color:rgba(255,255,255,.1);color:#fff;" type="tel" placeholder="+254 7XX XXX XXX"></div>
        </div>
        <div class="fg"><label class="fl" style="color:rgba(255,255,255,.4);">Email</label><input class="fi" style="background:rgba(255,255,255,.06);border-color:rgba(255,255,255,.1);color:#fff;" type="email" placeholder="your@email.com"></div>
        <div class="fg"><label class="fl" style="color:rgba(255,255,255,.4);">I'm interested in</label>
          <select class="fs" style="background:rgba(255,255,255,.06);border-color:rgba(255,255,255,.1);color:rgba(255,255,255,.7);">
            <option>Online course enrolment</option><option>CCS Prime Membership</option><option>Corporate team licence</option>
            <option>Inhouse training programme</option><option>Consulting services</option><option>Live training booking</option>
          </select>
        </div>
        <div class="fg"><label class="fl" style="color:rgba(255,255,255,.4);">Message</label><textarea class="ft" style="background:rgba(255,255,255,.06);border-color:rgba(255,255,255,.1);color:#fff;" placeholder="Tell us how we can help..."></textarea></div>
        <button class="btn-primary" style="width:100%;padding:14px;font-size:15px;" onclick="submitContact()">Send Enquiry →</button>
      </div>
    </div>
  </div>
</section>

<!-- FOOTER -->
<footer>
  <div class="container">
    <div class="footer-grid">
      <div>
        <div class="nav-logo" style="margin-bottom:.5rem;">
          <div class="logo-main" style="font-size:18px;">Centre of <span>Corporate</span> Studies</div>
        </div>
        <div class="footer-brand">Kenya's premier professional training and e-learning platform. CPD-accredited courses, live sessions, and expert consulting — all in one place.</div>
        <div style="margin-top:1.25rem;display:flex;gap:.75rem;flex-wrap:wrap;">
          <a href="https://wa.me/254722223084" target="_blank" style="background:#25D366;color:#fff;font-size:12px;font-weight:700;padding:7px 14px;border-radius:var(--r);text-decoration:none;">WhatsApp</a>
          <a href="tel:+254722223084" style="background:rgba(255,255,255,.08);color:rgba(255,255,255,.6);font-size:12px;font-weight:700;padding:7px 14px;border-radius:var(--r);text-decoration:none;">Call Us</a>
        </div>
      </div>
      <div>
        <div class="footer-col-title">E-Learning</div>
        <ul class="footer-links">
          <li><a href="#courses">All Online Courses</a></li>
          <li><a href="#membership">CCS Prime Membership</a></li>
          <li><a href="#membership">Corporate Licence</a></li>
          <li><a href="#calendar">Live Training Calendar</a></li>
          <li><a href="#">Certificate Verification</a></li>
        </ul>
      </div>
      <div>
        <div class="footer-col-title">Training Areas</div>
        <ul class="footer-links">
          <li><a href="#">Leadership & Management</a></li>
          <li><a href="#">Finance & Accounting</a></li>
          <li><a href="#">HR Management</a></li>
          <li><a href="#">Project Management</a></li>
          <li><a href="#">Sales & Marketing</a></li>
          <li><a href="#">Procurement & Contracts</a></li>
        </ul>
      </div>
      <div>
        <div class="footer-col-title">Company</div>
        <ul class="footer-links">
          <li><a href="#">About CCS</a></li>
          <li><a href="#">Our Trainers</a></li>
          <li><a href="#consulting">Consulting Services</a></li>
          <li><a href="#corporate">Inhouse Training</a></li>
          <li><a href="#">Blog & Resources</a></li>
          <li><a href="#contact">Contact Us</a></li>
        </ul>
        <div style="margin-top:1.25rem;">
          <div class="footer-col-title">Follow us</div>
          <div class="footer-socials">
            <a href="#" class="social-btn" title="LinkedIn">in</a>
            <a href="#" class="social-btn" title="Twitter">𝕏</a>
            <a href="#" class="social-btn" title="Facebook">f</a>
            <a href="#" class="social-btn" title="YouTube">▶</a>
          </div>
        </div>
      </div>
    </div>
    <div class="footer-bottom">
      <div class="footer-copy">© 2026 Centre of Corporate Studies. All rights reserved. · corporate.co.ke</div>
      <div style="display:flex;gap:8px;flex-wrap:wrap;">
        <span style="background:rgba(255,255,255,.06);border:1px solid rgba(255,255,255,.1);color:rgba(255,255,255,.35);font-size:11px;font-weight:700;padding:4px 10px;border-radius:4px;">M-Pesa</span>
        <span style="background:rgba(255,255,255,.06);border:1px solid rgba(255,255,255,.1);color:rgba(255,255,255,.35);font-size:11px;font-weight:700;padding:4px 10px;border-radius:4px;">Visa</span>
        <span style="background:rgba(255,255,255,.06);border:1px solid rgba(255,255,255,.1);color:rgba(255,255,255,.35);font-size:11px;font-weight:700;padding:4px 10px;border-radius:4px;">Mastercard</span>
        <span style="background:rgba(255,255,255,.06);border:1px solid rgba(255,255,255,.1);color:rgba(255,255,255,.35);font-size:11px;font-weight:700;padding:4px 10px;border-radius:4px;">PayPal</span>
      </div>
    </div>
  </div>
</footer>

<!-- MODAL -->
<div id="modalOverlay" style="display:none;position:fixed;inset:0;background:rgba(0,0,0,.6);backdrop-filter:blur(8px);z-index:1000;align-items:center;justify-content:center;padding:2rem;">
  <div id="modalBox" style="background:var(--white);border-radius:var(--r-xl);max-width:480px;width:100%;padding:2.5rem;position:relative;">
    <button onclick="closeModal()" style="position:absolute;top:1rem;right:1rem;background:var(--slate2);border:none;width:32px;height:32px;border-radius:50%;cursor:pointer;font-size:16px;display:flex;align-items:center;justify-content:center;">✕</button>
    <div id="modalContent"></div>
  </div>
</div>

<script>
const courses = [
  {id:1,icon:'🏆',cat:'leadership',format:'online',title:'Strategic Leadership for Managers',desc:'Master leadership frameworks, decision-making, and team motivation. Ideal for mid-to-senior managers.',rating:'4.9',reviews:124,duration:'8 hrs',modules:12,price:'KES 5,500',oldPrice:'KES 9,000',badge:'Bestseller'},
  {id:2,icon:'💰',cat:'finance',format:'online',title:'Financial Management for Non-Finance Professionals',desc:'Understand financial statements, budgeting, and cost management without an accounting background.',rating:'4.8',reviews:89,duration:'6 hrs',modules:9,price:'KES 4,500',oldPrice:'KES 7,500',badge:'Popular'},
  {id:3,icon:'👥',cat:'hr',format:'online',title:'Human Resource Management — Complete Course',desc:'Recruitment, performance management, HR strategy, labour law compliance, and talent development.',rating:'4.9',reviews:156,duration:'10 hrs',modules:14,price:'KES 6,000',oldPrice:'KES 10,000',badge:'Bestseller'},
  {id:4,icon:'📊',cat:'leadership',format:'live',title:'Strategic Planning & Execution Masterclass',desc:'Build and implement a winning organisational strategy using proven frameworks and real-world case studies.',rating:'4.7',reviews:43,duration:'3 Days',modules:null,price:'KES 28,000',oldPrice:'KES 35,000',badge:'Live'},
  {id:5,icon:'📋',cat:'project',format:'online',title:'Project Management Fundamentals (PMP-Aligned)',desc:'Plan, execute, monitor, and close projects using internationally recognised project management standards.',rating:'4.8',reviews:98,duration:'8 hrs',modules:11,price:'KES 5,000',oldPrice:'KES 8,500',badge:''},
  {id:6,icon:'📈',cat:'sales',format:'online',title:'Modern Sales & Marketing for Business Growth',desc:'Customer acquisition, digital marketing, brand positioning, and revenue growth strategies for East African markets.',rating:'4.7',reviews:67,duration:'7 hrs',modules:10,price:'KES 4,800',oldPrice:'KES 8,000',badge:'New'},
  {id:7,icon:'⭐',cat:'hr',format:'live',title:'Customer Service Excellence Workshop',desc:'Practical techniques for service delivery, complaint handling, and customer retention. Highly interactive.',rating:'4.9',reviews:212,duration:'1 Day',modules:null,price:'KES 15,000',oldPrice:'KES 20,000',badge:'Bestseller'},
  {id:8,icon:'🤝',cat:'leadership',format:'hybrid',title:'Team Building & High-Performance Culture',desc:'Build cohesive, high-performing teams through communication frameworks, trust building, and collaborative problem-solving.',rating:'4.8',reviews:78,duration:'2 Days / 5 hrs online',modules:8,price:'KES 8,500',oldPrice:'KES 12,000',badge:''},
  {id:9,icon:'📦',cat:'procurement',format:'online',title:'Procurement & Contract Management',desc:'End-to-end procurement processes, contract drafting, negotiation, and vendor management best practices.',rating:'4.7',reviews:55,duration:'6 hrs',modules:9,price:'KES 5,200',oldPrice:'KES 8,500',badge:''},
];

let activeFilter = 'all';

function renderCourses(filter){
  const grid = document.getElementById('coursesGrid');
  const filtered = filter==='all' ? courses : courses.filter(c => c.cat===filter || c.format===filter);
  grid.innerHTML = filtered.map(c=>`
    <div class="course-card">
      <div class="course-thumb" style="background:${c.format==='online'?'#1e3a8a':c.format==='live'?'#1a3a2a':'#2a1a3a'};">
        <div style="font-size:3.5rem;">${c.icon}</div>
        <div class="course-cat-badge">${c.cat.charAt(0).toUpperCase()+c.cat.slice(1)}</div>
        <div class="course-format ${c.format}">${c.format==='online'?'Self-Paced':c.format==='live'?'Live Session':'Hybrid'}</div>
      </div>
      <div class="course-body">
        <div class="course-rating">
          <div class="stars">★★★★★</div>
          <div class="rating-num">${c.rating} (${c.reviews} reviews)</div>
          ${c.badge?`<span style="margin-left:auto;font-size:10px;background:var(--blue-pale);color:var(--blue-dark);padding:2px 8px;border-radius:3px;font-weight:700;">${c.badge}</span>`:''}
        </div>
        <div class="course-title">${c.title}</div>
        <div class="course-desc">${c.desc}</div>
        <div class="course-meta">
          <span class="course-meta-item">⏱ ${c.duration}</span>
          ${c.modules?`<span class="course-meta-item">📚 ${c.modules} modules</span>`:''}
          <span class="course-meta-item">🎓 CPD Certificate</span>
        </div>
        <div class="course-footer">
          <div><span class="course-price">${c.price}</span><span class="course-price-old">${c.oldPrice}</span></div>
          <button class="btn-enrol" onclick="enrollCourse('${c.title}','${c.price}')">Enrol Now →</button>
        </div>
      </div>
    </div>
  `).join('');
}

function filterCourses(btn, filter){
  document.querySelectorAll('.filter-btn').forEach(b=>b.classList.remove('active'));
  btn.classList.add('active');
  activeFilter = filter;
  renderCourses(filter);
}

function searchCourses(){
  const q = document.getElementById('heroSearch').value.toLowerCase();
  const cat = document.getElementById('heroCategory').value.toLowerCase();
  const filtered = courses.filter(c=>
    (!q || c.title.toLowerCase().includes(q) || c.desc.toLowerCase().includes(q) || c.cat.includes(q)) &&
    (!cat || c.cat.includes(cat) || c.title.toLowerCase().includes(cat))
  );
  document.getElementById('courses').scrollIntoView({behavior:'smooth'});
  setTimeout(()=>{
    const grid = document.getElementById('coursesGrid');
    grid.innerHTML = filtered.length ? filtered.map(c=>`
      <div class="course-card">
        <div class="course-thumb" style="background:#1e3a8a;"><div style="font-size:3.5rem;">${c.icon}</div>
          <div class="course-cat-badge">${c.cat}</div>
          <div class="course-format ${c.format}">${c.format}</div>
        </div>
        <div class="course-body">
          <div class="course-rating"><div class="stars">★★★★★</div><div class="rating-num">${c.rating} (${c.reviews})</div></div>
          <div class="course-title">${c.title}</div>
          <div class="course-desc">${c.desc}</div>
          <div class="course-footer"><div><span class="course-price">${c.price}</span><span class="course-price-old">${c.oldPrice}</span></div><button class="btn-enrol" onclick="enrollCourse('${c.title}','${c.price}')">Enrol →</button></div>
        </div>
      </div>`).join('') :
      '<div style="grid-column:1/-1;text-align:center;padding:3rem;color:var(--muted);font-size:15px;">No courses found. <a href="#contact" style="color:var(--blue);font-weight:600;">Contact us</a> — we may be able to build it for you.</div>';
  },400);
}

function quickSearch(term){
  document.getElementById('heroSearch').value = term;
  searchCourses();
}

function enrollCourse(title, price){
  showModal('enrol', title, price);
}

function enrollMembership(){ showModal('membership'); }
function enrolPlan(plan){ showModal(plan==='Prime'?'membership':plan==='Corporate'?'corporate-plan':'starter'); }
function bookSession(session){ showModal('book', session); }
function submitCorp(){ alert('Thank you! Our training team will contact you within 24 hours with a tailored proposal.\n\nFor faster response, WhatsApp us on +254 722 223 084.'); }
function submitContact(){ alert('Enquiry received! We will respond within 24 hours.\n\nFor faster response, WhatsApp us on +254 722 223 084.'); }

function showModal(type, arg1, arg2){
  const overlay = document.getElementById('modalOverlay');
  const content = document.getElementById('modalContent');
  overlay.style.display = 'flex';
  if(type==='login'){
    content.innerHTML = `<div style="font-family:var(--serif);font-size:1.6rem;font-weight:700;color:var(--ink);margin-bottom:.25rem;">Welcome Back</div>
      <div style="font-size:13px;color:var(--muted);margin-bottom:1.5rem;">Log in to your CCS learning dashboard</div>
      <div class="fg"><label class="fl">Email</label><input class="fi" type="email" placeholder="your@email.com"></div>
      <div class="fg"><label class="fl">Password</label><input class="fi" type="password" placeholder="••••••••"></div>
      <button class="btn-primary" style="width:100%;padding:13px;font-size:14px;margin-top:.5rem;" onclick="alert('Login functionality — connect to your backend/LMS')">Log In to Dashboard</button>
      <div style="text-align:center;margin-top:1rem;font-size:13px;color:var(--muted);">No account? <a href="#" onclick="showModal('signup')" style="color:var(--blue);font-weight:600;">Sign up free</a></div>`;
  } else if(type==='signup'){
    content.innerHTML = `<div style="font-family:var(--serif);font-size:1.6rem;font-weight:700;color:var(--ink);margin-bottom:.25rem;">Start Learning Today</div>
      <div style="font-size:13px;color:var(--muted);margin-bottom:1.5rem;">Create your free CCS account</div>
      <div style="display:grid;grid-template-columns:1fr 1fr;gap:.75rem;">
        <div class="fg"><label class="fl">First Name</label><input class="fi" type="text" placeholder="Jane"></div>
        <div class="fg"><label class="fl">Last Name</label><input class="fi" type="text" placeholder="Mwangi"></div>
      </div>
      <div class="fg"><label class="fl">Email</label><input class="fi" type="email" placeholder="your@email.com"></div>
      <div class="fg"><label class="fl">Phone / WhatsApp</label><input class="fi" type="tel" placeholder="+254 7XX XXX XXX"></div>
      <div class="fg"><label class="fl">Password</label><input class="fi" type="password" placeholder="Create a password"></div>
      <button class="btn-primary" style="width:100%;padding:13px;font-size:14px;margin-top:.5rem;" onclick="alert('Account created! Connect this to your LMS backend.')">Create My Account</button>
      <div style="text-align:center;margin-top:1rem;font-size:13px;color:var(--muted);">Already have an account? <a href="#" onclick="showModal('login')" style="color:var(--blue);font-weight:600;">Log in</a></div>`;
  } else if(type==='enrol'){
    content.innerHTML = `<div style="font-family:var(--serif);font-size:1.4rem;font-weight:700;color:var(--ink);margin-bottom:.25rem;">Enrol Now</div>
      <div style="font-size:13px;color:var(--muted);margin-bottom:1.25rem;">${arg1}</div>
      <div style="background:var(--blue-pale);border-radius:var(--r);padding:1rem;margin-bottom:1.25rem;display:flex;justify-content:space-between;align-items:center;">
        <div style="font-size:14px;font-weight:600;color:var(--ink);">Course fee</div>
        <div style="font-family:var(--serif);font-size:1.5rem;font-weight:700;color:var(--blue);">${arg2}</div>
      </div>
      <div class="fg"><label class="fl">Your Name</label><input class="fi" type="text" placeholder="Full name"></div>
      <div class="fg"><label class="fl">Email</label><input class="fi" type="email" placeholder="your@email.com"></div>
      <div class="fg"><label class="fl">Phone / WhatsApp</label><input class="fi" type="tel" placeholder="+254 7XX XXX XXX"></div>
      <div class="fg"><label class="fl">Payment Method</label>
        <select class="fs"><option>M-Pesa</option><option>Visa / Mastercard</option><option>PayPal</option><option>Bank Transfer</option></select>
      </div>
      <button class="btn-primary" style="width:100%;padding:13px;font-size:14px;" onclick="alert('Enrolment submitted! You will receive payment instructions via email and WhatsApp within minutes.')">Confirm Enrolment & Pay</button>
      <div style="font-size:11px;color:var(--muted);text-align:center;margin-top:.75rem;">You get instant access after payment confirmation.</div>`;
  } else if(type==='membership'){
    content.innerHTML = `<div style="font-family:var(--serif);font-size:1.4rem;font-weight:700;color:var(--ink);margin-bottom:.25rem;">Get CCS Prime Membership</div>
      <div style="font-size:13px;color:var(--muted);margin-bottom:1.25rem;">Unlimited access to all 50+ courses for one year</div>
      <div style="background:var(--blue);border-radius:var(--r);padding:1rem;margin-bottom:1.25rem;text-align:center;">
        <div style="font-family:var(--serif);font-size:2.5rem;font-weight:700;color:#fff;line-height:1;">KES 15,000</div>
        <div style="font-size:13px;color:rgba(255,255,255,.7);margin-top:4px;">per year — save over KES 30,000 vs buying individually</div>
      </div>
      <div class="fg"><label class="fl">Your Name</label><input class="fi" type="text" placeholder="Full name"></div>
      <div class="fg"><label class="fl">Email</label><input class="fi" type="email" placeholder="your@email.com"></div>
      <div class="fg"><label class="fl">Phone / WhatsApp</label><input class="fi" type="tel" placeholder="+254 7XX XXX XXX"></div>
      <div class="fg"><label class="fl">Payment Method</label>
        <select class="fs"><option>M-Pesa</option><option>Visa / Mastercard</option><option>PayPal</option><option>Bank Transfer / LPO</option></select>
      </div>
      <button class="btn-primary" style="width:100%;padding:13px;font-size:14px;" onclick="alert('Prime Membership requested! Payment instructions will be sent to your email and WhatsApp within minutes.')">Get Prime Access — KES 15,000/yr</button>`;
  } else if(type==='book'){
    content.innerHTML = `<div style="font-family:var(--serif);font-size:1.4rem;font-weight:700;color:var(--ink);margin-bottom:.25rem;">Book Your Seat</div>
      <div style="font-size:13px;color:var(--muted);margin-bottom:1.25rem;">${arg1}</div>
      <div class="fg"><label class="fl">Full Name</label><input class="fi" type="text" placeholder="Your name"></div>
      <div class="fg"><label class="fl">Email</label><input class="fi" type="email" placeholder="your@email.com"></div>
      <div class="fg"><label class="fl">Phone / WhatsApp</label><input class="fi" type="tel" placeholder="+254 7XX XXX XXX"></div>
      <div class="fg"><label class="fl">Organisation</label><input class="fi" type="text" placeholder="Company or institution"></div>
      <div class="fg"><label class="fl">Attendance Mode</label><select class="fs"><option>In-person (Nairobi)</option><option>Virtual (Zoom)</option></select></div>
      <button class="btn-primary" style="width:100%;padding:13px;font-size:14px;" onclick="alert('Booking confirmed! We will send payment details and joining instructions to your email and WhatsApp.')">Confirm Booking</button>`;
  }
}

function closeModal(){
  document.getElementById('modalOverlay').style.display='none';
}
document.getElementById('modalOverlay').addEventListener('click', function(e){
  if(e.target===this) closeModal();
});

const obs = new IntersectionObserver(entries=>{
  entries.forEach(e=>{ if(e.isIntersecting) e.target.classList.add('visible'); });
},{threshold:0.08});
document.querySelectorAll('.fade-up').forEach(el=>obs.observe(el));

renderCourses('all');
</script>
</body>
</html>
