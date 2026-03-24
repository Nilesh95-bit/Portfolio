---
layout: null
---
<!DOCTYPE html>
<html lang="en"><head>
  <meta charset="utf-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1">
<title>Nilesh Malavia — Pharmaceutical Scientist</title>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,600;1,300;1,400&family=DM+Mono:wght@300;400;500&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet"/>
<style>
:root {
  --navy:#0d1b2a; --deep:#1a2e42; --mid:#2e4a63;
  --teal:#2a9d8f; --teal-light:#3dbfb0;
  --gold:#c9a84c; --gold-light:#e8c96a;
  --slate:#8ba3bc; --fog:#c8d8e8; --white:#ffffff;
  --serif:'Cormorant Garamond',Georgia,serif;
  --mono:'DM Mono',monospace; --sans:'DM Sans',sans-serif;
}
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
body{background:var(--navy);color:var(--fog);font-family:var(--sans);font-size:16px;line-height:1.7;overflow-x:hidden}
body::before{content:'';position:fixed;inset:0;background-image:radial-gradient(circle at 1px 1px,rgba(42,157,143,0.06) 1px,transparent 0);background-size:40px 40px;pointer-events:none;z-index:0}

/* NAV */
nav{position:fixed;top:0;left:0;right:0;z-index:100;display:flex;justify-content:space-between;align-items:center;padding:1.2rem 4rem;background:rgba(13,27,42,0.88);backdrop-filter:blur(14px);border-bottom:1px solid rgba(42,157,143,0.15)}
.nav-logo{font-family:var(--serif);font-size:1.2rem;font-weight:300;letter-spacing:.15em;color:var(--teal-light);text-decoration:none}
.nav-links{display:flex;gap:2.5rem;list-style:none}
.nav-links a{font-family:var(--mono);font-size:.72rem;letter-spacing:.12em;text-transform:uppercase;color:var(--slate);text-decoration:none;transition:color .2s}
.nav-links a:hover{color:var(--teal-light)}


.scroll-progress{position:fixed;top:0;left:0;height:3px;width:0;background:linear-gradient(90deg,var(--teal),var(--gold));z-index:150;box-shadow:0 0 12px rgba(61,191,176,.45)}

/* RECRUITER VALUE */
#value{background:linear-gradient(180deg,rgba(13,27,42,.45),rgba(26,46,66,.2))}
.value-grid{display:grid;grid-template-columns:repeat(4,minmax(0,1fr));gap:1px;background:rgba(139,163,188,.08);border:1px solid rgba(139,163,188,.08)}
.value-card{background:rgba(13,27,42,.78);padding:1.6rem;min-height:220px;position:relative;overflow:hidden}
.value-card::after{content:'';position:absolute;inset:auto -20% -35% auto;width:140px;height:140px;border-radius:50%;background:radial-gradient(circle,rgba(42,157,143,.12),transparent 68%);pointer-events:none}
.value-kicker{font-family:var(--mono);font-size:.62rem;letter-spacing:.14em;text-transform:uppercase;color:var(--teal);margin-bottom:.8rem}
.value-title{font-family:var(--serif);font-size:1.25rem;font-weight:300;color:var(--white);margin-bottom:.8rem}
.value-copy{font-size:.84rem;line-height:1.8;color:var(--fog)}
.value-metric{display:inline-block;margin-top:1rem;padding:.28rem .65rem;border:1px solid rgba(201,168,76,.25);background:rgba(201,168,76,.08);font-family:var(--mono);font-size:.58rem;letter-spacing:.08em;color:var(--gold-light);text-transform:uppercase}
.section-subtitle{max-width:760px;font-size:.95rem;line-height:1.85;color:var(--slate);margin:-2.2rem 0 2.2rem}

/* HERO */
#hero{position:relative;min-height:100vh;display:grid;grid-template-columns:1fr 1fr;align-items:center;padding:8rem 4rem 5rem;gap:4rem;overflow:hidden;z-index:1}
.hero-bg-circle{position:absolute;border-radius:50%;pointer-events:none}
.hero-bg-circle.c1{width:700px;height:700px;top:-200px;right:-150px;background:radial-gradient(circle,rgba(42,157,143,0.1) 0%,transparent 70%)}
.hero-bg-circle.c2{width:300px;height:300px;bottom:5%;left:30%;background:radial-gradient(circle,rgba(201,168,76,0.06) 0%,transparent 70%)}
.hero-left{}
.hero-eyebrow{font-family:var(--mono);font-size:.72rem;letter-spacing:.2em;text-transform:uppercase;color:var(--teal);margin-bottom:1.5rem;opacity:0;animation:fadeUp .8s .2s forwards}
.hero-name{font-family:var(--serif);font-size:clamp(3rem,6vw,5.5rem);font-weight:300;line-height:1.05;color:var(--white);letter-spacing:-.01em;margin-bottom:.5rem;opacity:0;animation:fadeUp .8s .35s forwards}
.hero-name em{font-style:italic;color:var(--teal-light)}
.hero-title{font-family:var(--serif);font-size:clamp(1rem,2vw,1.5rem);font-weight:300;font-style:italic;color:var(--slate);margin-bottom:2rem;opacity:0;animation:fadeUp .8s .5s forwards}
.hero-summary{font-size:.95rem;line-height:1.85;color:var(--fog);max-width:580px;margin-bottom:2.5rem;opacity:0;animation:fadeUp .8s .65s forwards}
.hero-tags{display:flex;flex-wrap:wrap;gap:.5rem;margin-bottom:2.5rem;opacity:0;animation:fadeUp .8s .8s forwards}
.tag{font-family:var(--mono);font-size:.65rem;letter-spacing:.08em;padding:.3rem .8rem;border:1px solid rgba(42,157,143,.35);border-radius:2px;color:var(--teal-light);background:rgba(42,157,143,.06)}
.hero-cta{display:flex;gap:1rem;flex-wrap:wrap;opacity:0;animation:fadeUp .8s .95s forwards}
.btn{font-family:var(--mono);font-size:.72rem;letter-spacing:.12em;text-transform:uppercase;padding:.85rem 2rem;text-decoration:none;border-radius:2px;transition:all .2s;cursor:pointer;border:none}
.btn-primary{background:var(--teal);color:var(--navy);font-weight:500}
.btn-primary:hover{background:var(--teal-light);transform:translateY(-1px)}
.btn-outline{border:1px solid rgba(200,216,232,.3);color:var(--fog);background:transparent}
.btn-outline:hover{border-color:var(--teal);color:var(--teal-light)}

/* HERO RIGHT — HPLC canvas panel */
.hero-right{opacity:0;animation:fadeUp .8s .6s forwards}
.analytical-panel{background:rgba(13,27,42,.8);border:1px solid rgba(42,157,143,.2);border-radius:4px;padding:1.5rem;position:relative}
.panel-label{font-family:var(--mono);font-size:.62rem;letter-spacing:.15em;text-transform:uppercase;color:var(--teal);margin-bottom:1rem;display:flex;justify-content:space-between;align-items:center}
.panel-dot{width:6px;height:6px;border-radius:50%;background:var(--teal);animation:blink 1.5s infinite}
#hplcCanvas{width:100%;height:180px;display:block}
.peak-labels{display:flex;justify-content:space-around;margin-top:.5rem}
.peak-label{font-family:var(--mono);font-size:.6rem;color:var(--slate);text-align:center}
.peak-label span{display:block;color:var(--teal-light);font-weight:500}

/* SECTIONS */
section{position:relative;z-index:1;padding:6rem 4rem}
.section-inner{max-width:1100px;margin:0 auto}
.section-label{font-family:var(--mono);font-size:.68rem;letter-spacing:.25em;text-transform:uppercase;color:var(--teal);margin-bottom:1rem}
.section-title{font-family:var(--serif);font-size:clamp(2rem,4vw,3rem);font-weight:300;color:var(--white);line-height:1.1;margin-bottom:3.5rem}

/* ABOUT */
#about{background:rgba(26,46,66,.4)}
.stats-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(140px,1fr));gap:2px;margin-bottom:4rem}
.stat-card{background:rgba(42,157,143,.06);border:1px solid rgba(42,157,143,.15);padding:1.8rem 1.2rem;text-align:center;transition:border-color .2s,background .2s}
.stat-card:hover{border-color:rgba(42,157,143,.4);background:rgba(42,157,143,.1)}
.stat-num{font-family:var(--serif);font-size:2.6rem;font-weight:300;color:var(--teal-light);line-height:1;margin-bottom:.4rem}
.stat-label{font-family:var(--mono);font-size:.6rem;letter-spacing:.12em;text-transform:uppercase;color:var(--slate)}
.about-cols{display:grid;grid-template-columns:1fr 1fr;gap:3rem;align-items:start}
.about-text{font-size:.95rem;line-height:1.9;color:var(--fog)}
.about-text p{margin-bottom:1.2rem}

/* DLS visualization */
.dls-container{background:rgba(13,27,42,.7);border:1px solid rgba(42,157,143,.2);border-radius:4px;padding:1.5rem;margin-top:2rem}
.dls-header{font-family:var(--mono);font-size:.62rem;letter-spacing:.15em;text-transform:uppercase;color:var(--teal);margin-bottom:1rem;display:flex;justify-content:space-between}
#dlsCanvas{width:100%;height:140px;display:block}
.dls-metrics{display:flex;gap:2rem;margin-top:.8rem}
.dls-metric{font-family:var(--mono);font-size:.65rem;color:var(--slate)}
.dls-metric span{color:var(--teal-light);display:block;font-size:.8rem}

/* LNP VISUAL */
.lnp-section{background:rgba(13,27,42,.5);border:1px solid rgba(42,157,143,.15);border-radius:4px;padding:2rem;margin:3rem 0;display:grid;grid-template-columns:auto 1fr;gap:3rem;align-items:center}
#lnpCanvas{width:220px;height:220px;flex-shrink:0}
.lnp-info h3{font-family:var(--serif);font-size:1.4rem;font-weight:300;color:var(--white);margin-bottom:1rem}
.lnp-legend{list-style:none;display:flex;flex-direction:column;gap:.6rem}
.lnp-legend li{display:flex;align-items:center;gap:.7rem;font-size:.82rem;color:var(--slate)}
.legend-dot{width:10px;height:10px;border-radius:50%;flex-shrink:0}

/* SKILLS */
#skills{background:transparent}
.skills-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(300px,1fr));gap:1.5px}
.skill-card{background:rgba(13,27,42,.6);border:1px solid rgba(139,163,188,.1);padding:2rem;transition:border-color .2s,transform .2s;position:relative;overflow:hidden}
.skill-card::before{content:'';position:absolute;top:0;left:0;width:3px;height:0;background:var(--teal);transition:height .3s}
.skill-card:hover::before{height:100%}
.skill-card:hover{border-color:rgba(42,157,143,.3);transform:translateY(-2px)}
.skill-card-title{font-family:var(--mono);font-size:.7rem;letter-spacing:.1em;text-transform:uppercase;color:var(--teal-light);margin-bottom:.8rem}
.skill-card-body{font-size:.86rem;line-height:1.75;color:var(--slate)}

/* EXPERIENCE */
#experience{background:rgba(26,46,66,.3)}
.exp-item{display:grid;grid-template-columns:200px 1fr;gap:3rem;padding:3rem 0;border-bottom:1px solid rgba(139,163,188,.1)}
.exp-item:last-child{border-bottom:none}
.exp-period{font-family:var(--mono);font-size:.7rem;letter-spacing:.08em;color:var(--teal);margin-bottom:.5rem}
.exp-org{font-family:var(--serif);font-size:1rem;font-style:italic;color:var(--slate);margin-bottom:.4rem}
.exp-loc{font-family:var(--mono);font-size:.62rem;color:rgba(139,163,188,.5)}
.exp-role{font-family:var(--serif);font-size:1.45rem;font-weight:300;color:var(--white);margin-bottom:1.2rem;line-height:1.2}
.exp-bullets{list-style:none}
.exp-bullets li{font-size:.88rem;line-height:1.75;color:var(--fog);padding:.4rem 0 .4rem 1.4rem;position:relative;border-bottom:1px solid rgba(139,163,188,.06)}
.exp-bullets li:last-child{border-bottom:none}
.exp-bullets li::before{content:'—';position:absolute;left:0;color:var(--teal);font-family:var(--mono);font-size:.75rem}
.exp-project-head{font-family:var(--mono);font-size:.65rem;letter-spacing:.12em;text-transform:uppercase;color:var(--gold);margin:1.5rem 0 .6rem}

/* STABILITY CHART */
.stability-panel{background:rgba(13,27,42,.7);border:1px solid rgba(42,157,143,.2);border-radius:4px;padding:1.5rem;margin:2rem 0}
.stability-header{font-family:var(--mono);font-size:.62rem;letter-spacing:.15em;text-transform:uppercase;color:var(--teal);margin-bottom:1rem;display:flex;justify-content:space-between;align-items:center}
#stabilityCanvas{width:100%;height:180px;display:block}
.stab-legend{display:flex;gap:1.5rem;margin-top:.8rem;flex-wrap:wrap}
.stab-legend-item{display:flex;align-items:center;gap:.5rem;font-family:var(--mono);font-size:.6rem;color:var(--slate)}
.stab-line{width:20px;height:2px}

/* PUBLICATIONS */
#publications{background:transparent}
.pub-grid{display:grid;grid-template-columns:1fr 1fr;gap:1.5px}
.pub-card{background:rgba(13,27,42,.7);border:1px solid rgba(139,163,188,.1);padding:1.8rem;transition:border-color .2s}
.pub-card:hover{border-color:rgba(42,157,143,.35)}
.pub-year{font-family:var(--mono);font-size:.62rem;letter-spacing:.1em;color:var(--teal);margin-bottom:.6rem}
.pub-title{font-family:var(--serif);font-size:1rem;font-style:italic;color:var(--white);line-height:1.45;margin-bottom:.6rem}
.pub-journal{font-size:.78rem;color:var(--slate)}
.pub-badge{display:inline-block;margin-top:.5rem;font-family:var(--mono);font-size:.58rem;letter-spacing:.06em;padding:.2rem .6rem;border-radius:2px;background:rgba(201,168,76,.1);border:1px solid rgba(201,168,76,.25);color:var(--gold-light)}
.patent-card{grid-column:1/-1;background:rgba(201,168,76,.04);border:1px solid rgba(201,168,76,.2);padding:1.8rem;display:flex;align-items:center;gap:2rem}
.patent-icon{font-family:var(--serif);font-size:3rem;color:var(--gold);opacity:.6;flex-shrink:0;font-style:italic}

/* PRESENTATIONS */
#presentations{background:rgba(26,46,66,.3)}
.pres-list{list-style:none}
.pres-item{display:grid;grid-template-columns:110px 1fr;gap:2rem;padding:1.4rem 0;border-bottom:1px solid rgba(139,163,188,.08);align-items:start}
.pres-item:last-child{border-bottom:none}
.pres-year{font-family:var(--mono);font-size:.68rem;color:var(--teal);padding-top:.2rem}
.pres-title{font-size:.9rem;color:var(--fog);line-height:1.6;margin-bottom:.3rem}
.pres-venue{font-family:var(--mono);font-size:.65rem;color:var(--slate)}
.pres-award{display:inline-block;margin-top:.4rem;font-family:var(--mono);font-size:.58rem;letter-spacing:.06em;padding:.2rem .6rem;background:rgba(201,168,76,.1);border:1px solid rgba(201,168,76,.22);color:var(--gold-light);border-radius:2px}

/* AWARDS */
#awards{background:transparent}
.awards-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(240px,1fr));gap:1px}
.award-card{background:rgba(13,27,42,.6);border:1px solid rgba(201,168,76,.12);padding:1.6rem 1.4rem;transition:border-color .2s,background .2s}
.award-card:hover{border-color:rgba(201,168,76,.35);background:rgba(201,168,76,.04)}
.award-year{font-family:var(--mono);font-size:.62rem;color:var(--gold);margin-bottom:.4rem}
.award-name{font-family:var(--serif);font-size:1rem;color:var(--white);line-height:1.3;margin-bottom:.3rem}
.award-org{font-size:.76rem;color:var(--slate)}

/* EDUCATION */
#education{background:rgba(26,46,66,.3)}
.edu-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(280px,1fr));gap:1.5px}
.edu-card{background:rgba(13,27,42,.6);border:1px solid rgba(139,163,188,.1);padding:2.5rem 2rem;position:relative;overflow:hidden}
.edu-card::after{content:attr(data-gpa);position:absolute;bottom:-.5rem;right:1rem;font-family:var(--serif);font-size:5rem;font-weight:300;color:rgba(42,157,143,.05);line-height:1;pointer-events:none}
.edu-degree{font-family:var(--serif);font-size:1.3rem;font-weight:300;color:var(--white);margin-bottom:.5rem}
.edu-school{font-family:var(--mono);font-size:.68rem;letter-spacing:.08em;color:var(--teal-light);margin-bottom:.3rem}
.edu-details{font-size:.8rem;color:var(--slate);margin-bottom:.8rem}
.edu-gpa{font-family:var(--mono);font-size:.68rem;color:var(--gold)}

/* CONTACT */
#contact{background:linear-gradient(135deg,rgba(26,46,66,.8) 0%,rgba(13,27,42,.95) 100%);text-align:center;padding:8rem 4rem}
.contact-email{font-family:var(--serif);font-size:clamp(1.5rem,4vw,2.8rem);font-weight:300;font-style:italic;color:var(--teal-light);text-decoration:none;display:block;margin:2rem 0;transition:color .2s}
.contact-email:hover{color:var(--white)}
.contact-links{display:flex;justify-content:center;gap:2rem;margin-top:2rem}
.contact-link{font-family:var(--mono);font-size:.7rem;letter-spacing:.12em;text-transform:uppercase;color:var(--slate);text-decoration:none;padding:.5rem 1.2rem;border:1px solid rgba(139,163,188,.2);border-radius:2px;transition:all .2s}
.contact-link:hover{color:var(--teal-light);border-color:var(--teal)}

/* FOOTER */
footer{background:rgba(13,27,42,.95);padding:2rem 4rem;display:flex;justify-content:space-between;align-items:center;border-top:1px solid rgba(42,157,143,.1);font-family:var(--mono);font-size:.62rem;color:rgba(139,163,188,.4);letter-spacing:.08em}

/* MOLECULE CANVAS (floating bg element) */
#moleculeCanvas{position:fixed;top:0;left:0;width:100%;height:100%;pointer-events:none;z-index:0;opacity:.35}

/* ANIMATIONS */
@keyframes fadeUp{from{opacity:0;transform:translateY(24px)}to{opacity:1;transform:translateY(0)}}
@keyframes blink{0%,100%{opacity:1}50%{opacity:.3}}
@keyframes spin{from{transform:rotate(0deg)}to{transform:rotate(360deg)}}
.reveal{opacity:0;transform:translateY(20px);transition:opacity .7s ease,transform .7s ease}
.reveal.visible{opacity:1;transform:none}

::-webkit-scrollbar{width:5px}
::-webkit-scrollbar-track{background:var(--navy)}
::-webkit-scrollbar-thumb{background:var(--mid);border-radius:3px}
::-webkit-scrollbar-thumb:hover{background:var(--teal)}



/* BIOPROCESS ANIMATION SECTION */
#bioprocess{background:rgba(13,27,42,.45)}
.process-grid{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:1.5rem}
.process-card{background:rgba(13,27,42,.72);border:1px solid rgba(42,157,143,.16);border-radius:6px;padding:1.4rem;position:relative;overflow:hidden;min-height:360px;box-shadow:0 10px 30px rgba(0,0,0,.12)}
.process-card::after{content:'';position:absolute;inset:auto 0 0 0;height:1px;background:linear-gradient(90deg,transparent,rgba(42,157,143,.35),transparent)}
.process-kicker{font-family:var(--mono);font-size:.62rem;letter-spacing:.14em;text-transform:uppercase;color:var(--teal);margin-bottom:.6rem}
.process-name{font-family:var(--serif);font-size:1.35rem;font-weight:300;color:var(--white);margin-bottom:.55rem}
.process-copy{font-size:.84rem;line-height:1.75;color:var(--slate);margin-bottom:1rem;max-width:34ch}
.process-stage{display:inline-flex;align-items:center;gap:.45rem;font-family:var(--mono);font-size:.6rem;letter-spacing:.08em;text-transform:uppercase;color:var(--gold-light);padding:.28rem .55rem;border:1px solid rgba(201,168,76,.22);background:rgba(201,168,76,.08);border-radius:999px;margin-bottom:1rem}
.process-viz{height:170px;border:1px solid rgba(139,163,188,.12);background:linear-gradient(180deg,rgba(26,46,66,.55),rgba(13,27,42,.85));border-radius:4px;position:relative;overflow:hidden}
.process-notes{list-style:none;margin-top:1rem;display:flex;flex-direction:column;gap:.5rem}
.process-notes li{font-size:.76rem;color:var(--fog);padding-left:1rem;position:relative}
.process-notes li::before{content:'';position:absolute;left:0;top:.54rem;width:5px;height:5px;border-radius:50%;background:var(--teal-light)}
.particle{position:absolute;border-radius:50%;opacity:.9;filter:drop-shadow(0 0 8px rgba(61,191,176,.16))}
.particle.protein{width:10px;height:10px;background:rgba(61,191,176,.92)}
.particle.impurity{width:7px;height:7px;background:rgba(255,155,155,.84)}
.particle.buffer{width:5px;height:5px;background:rgba(139,163,188,.72)}
.sep-column{position:absolute;left:50%;top:16px;transform:translateX(-50%);width:68px;height:138px;border-radius:34px;background:linear-gradient(180deg,rgba(232,201,106,.08),rgba(201,168,76,.18));border:1px solid rgba(201,168,76,.28);overflow:hidden}
.sep-resin{position:absolute;inset:16px 12px;border-radius:20px;background:repeating-linear-gradient(180deg,rgba(201,168,76,.2),rgba(201,168,76,.2) 6px,rgba(42,157,143,.12) 6px,rgba(42,157,143,.12) 12px)}
.sep-flow{position:absolute;left:50%;top:0;transform:translateX(-50%);width:2px;height:100%;background:linear-gradient(180deg,transparent,rgba(61,191,176,.8),transparent);animation:flowDown 1.8s linear infinite}
.sep-port{position:absolute;width:34px;height:10px;border-radius:10px;background:rgba(139,163,188,.18);border:1px solid rgba(139,163,188,.2);left:50%;transform:translateX(-50%)}
.sep-port.top{top:7px}.sep-port.bottom{bottom:7px}
.purify-chamber{position:absolute;left:18px;right:18px;top:26px;bottom:24px;border:1px solid rgba(61,191,176,.24);border-radius:10px;background:rgba(42,157,143,.05)}
.purify-layer{position:absolute;left:12px;right:12px;height:26px;border-radius:999px;background:linear-gradient(90deg,rgba(61,191,176,.18),rgba(201,168,76,.12));border:1px solid rgba(61,191,176,.15)}
.purify-layer.l1{top:18px}.purify-layer.l2{top:56px}.purify-layer.l3{top:94px}
.purify-arrow{position:absolute;left:16px;right:16px;top:50%;height:2px;background:linear-gradient(90deg,rgba(61,191,176,.1),rgba(61,191,176,.85),rgba(61,191,176,.1));animation:flowSide 1.6s linear infinite}
.tff-loop{position:absolute;inset:12px}
.tff-feed,.tff-retentate,.tff-permeate,.tff-membrane,.tff-pump{position:absolute;border:1px solid rgba(139,163,188,.2);background:rgba(26,46,66,.7);border-radius:6px}
.tff-feed{left:6px;top:52px;width:52px;height:62px}
.tff-retentate{right:6px;top:22px;width:58px;height:34px}
.tff-permeate{right:6px;bottom:18px;width:58px;height:34px}
.tff-membrane{left:74px;right:76px;top:42px;height:82px;border-radius:10px;background:linear-gradient(180deg,rgba(201,168,76,.08),rgba(61,191,176,.08));overflow:hidden}
.tff-pump{left:20px;bottom:18px;width:46px;height:24px;border-radius:999px}
.tff-path{position:absolute;background:rgba(139,163,188,.2)}
.tff-line1{left:56px;top:72px;width:22px;height:2px}.tff-line2{right:64px;top:38px;width:22px;height:2px}.tff-line3{right:64px;bottom:34px;width:22px;height:2px}
.tff-line4{left:42px;bottom:30px;width:2px;height:36px}.tff-line5{left:42px;top:64px;width:16px;height:2px}
.tff-stream{position:absolute;width:8px;height:8px;border-radius:50%;background:rgba(61,191,176,.9);box-shadow:0 0 0 4px rgba(61,191,176,.08)}
.tff-stream.impurity{background:rgba(255,155,155,.86)}
.tff-mesh{position:absolute;inset:8px;background:repeating-linear-gradient(90deg,rgba(201,168,76,.16),rgba(201,168,76,.16) 2px,transparent 2px,transparent 10px)}
.flow-label{position:absolute;font-family:var(--mono);font-size:.54rem;letter-spacing:.08em;text-transform:uppercase;color:var(--slate)}
.flow-label.feed{left:10px;top:32px}.flow-label.ret{right:8px;top:8px}.flow-label.perm{right:8px;bottom:58px}
@keyframes flowDown{0%{transform:translate(-50%,-35px)}100%{transform:translate(-50%,170px)}}
@keyframes flowSide{0%{transform:translateX(-18px)}100%{transform:translateX(18px)}}
@media(max-width:900px){.process-grid{grid-template-columns:1fr}.process-card{min-height:auto}}

@media(max-width:900px){
  #hero{grid-template-columns:1fr;padding:7rem 1.5rem 4rem}
  .hero-right{display:none}
  nav{padding:1rem 1.5rem}
  .nav-links{display:none}
  section{padding:4rem 1.5rem}
  .about-cols{grid-template-columns:1fr}
  .exp-item{grid-template-columns:1fr;gap:.5rem}
  .pub-grid{grid-template-columns:1fr}
  .pres-item{grid-template-columns:1fr;gap:.3rem}
  .lnp-section{grid-template-columns:1fr}
  .value-grid{grid-template-columns:1fr}
  footer{flex-direction:column;gap:.5rem;text-align:center}
}
</style>
</head>
<body>
<div class="scroll-progress" id="scrollProgress"></div>

<!-- floating molecule background canvas -->
<canvas id="moleculeCanvas"></canvas>

<nav>
  <a href="#hero" class="nav-logo">N. Malavia</a>
  <ul class="nav-links">
    <li><a href="#about">About</a></li>
    <li><a href="#skills">Skills</a></li>
    <li><a href="#experience">Experience</a></li>
    <li><a href="#publications">Publications</a></li>
    <li><a href="#presentations">Presentations</a></li>
    <li><a href="#awards">Awards</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</nav>

<!-- HERO -->
<section id="hero">
  <div class="hero-bg-circle c1"></div>
  <div class="hero-bg-circle c2"></div>
  <div class="hero-left">
    <p class="hero-eyebrow">Ph.D. Candidate · Pharmaceutics · University of Connecticut</p>
    <h1 class="hero-name">Nilesh<br><em>Malavia</em></h1>
    <p class="hero-title">Formulation Scientist — LNP, Injectable Drug Delivery & CMC</p>
    <p class="hero-summary">Translating bench-scale nanoparticle science into regulatory-ready drug products. Deep expertise in lipid nanoparticle manufacturing, oligonucleotide delivery systems, and long-term stability characterization. Defense: April 2026.</p>
    <div class="hero-tags">
      <span class="tag">Lipid Nanoparticles</span>
      <span class="tag">mRNA / Oligonucleotide Delivery</span>
      <span class="tag">Injectable Drug Products</span>
      <span class="tag">UPLC-CAD Analytics</span>
      <span class="tag">CMC Documentation</span>
      <span class="tag">TFF Manufacturing</span>
      <span class="tag">PBPK / IVIVC</span>
      <span class="tag">DoE / QbD</span>
    </div>
    <div class="hero-cta">
      <a href="#experience" class="btn btn-primary">View Experience</a>
      <a href="#contact" class="btn btn-outline">Get in Touch</a>
    </div>
  </div>

  <!-- HPLC CHROMATOGRAM PANEL -->
  <div class="hero-right">
    <div class="analytical-panel">
      <div class="panel-label">
        <span>UPLC-CAD Chromatogram — Lipid Analysis</span>
        <span class="panel-dot"></span>
      </div>
      <canvas id="hplcCanvas"></canvas>
      <div class="peak-labels">
        <div class="peak-label"><span>2.1 min</span>Lyso-PC-16</div>
        <div class="peak-label"><span>4.8 min</span>DSPG</div>
        <div class="peak-label"><span>7.2 min</span>HSPC</div>
        <div class="peak-label"><span>9.6 min</span>Cholesterol</div>
        <div class="peak-label"><span>12.4 min</span>DSPE-mPEG</div>
      </div>
    </div>
    <!-- DLS size distribution -->
    <div class="dls-container" style="margin-top:1.5rem">
      <div class="dls-header">
        <span>DLS Size Distribution — Liposomal NP</span>
        <span style="color:var(--teal-light)">Live scan</span>
      </div>
      <canvas id="dlsCanvas"></canvas>
      <div class="dls-metrics">
        <div class="dls-metric"><span id="dls-zave">127.3 nm</span>Z-average</div>
        <div class="dls-metric"><span id="dls-pdi">0.082</span>PDI</div>
        <div class="dls-metric"><span id="dls-zp">−32.4 mV</span>Zeta Potential</div>
      </div>
    </div>
  </div>
</section>

<!-- ABOUT -->
<section id="about">
  <div class="section-inner">
    <p class="section-label reveal">Profile</p>
    <h2 class="section-title reveal">Building the science behind<br>tomorrow's medicines</h2>
    <div class="stats-grid reveal">
      <div class="stat-card"><div class="stat-num">4+</div><div class="stat-label">Years Research</div></div>
      <div class="stat-card"><div class="stat-num">8</div><div class="stat-label">Publications</div></div>
      <div class="stat-card"><div class="stat-num">1</div><div class="stat-label">U.S. Patent</div></div>
      <div class="stat-card"><div class="stat-num">9</div><div class="stat-label">Conferences</div></div>
      <div class="stat-card"><div class="stat-num">3.94</div><div class="stat-label">GPA / 4.0</div></div>
      <div class="stat-card"><div class="stat-num">10+</div><div class="stat-label">Awards</div></div>
    </div>
    <div class="about-cols reveal">
      <div>
        <div class="about-text">
          <p>I am a Ph.D. candidate in Pharmaceutics at the University of Connecticut, working at the intersection of lipid nanoparticle formulation science, analytical method development, and injectable drug product development. My research spans two major FDA-funded programs: continuous manufacturing and 18-month stability characterization of liposomal nanoparticle reference materials, and mechanistic investigation of long-acting injectable suspension depots.</p>
          <p>Prior to my doctorate, I worked as a Scientist at Cipla Ltd. advancing QbD-driven 505(b)(2) submissions, conducted nucleic acid delivery research at NIPER Mohali, and interned at AbbVie's sterile injectables group in summer 2025.</p>
        </div>
        <!-- LNP cross-section illustration -->
        <div class="lnp-section reveal">
          <canvas id="lnpCanvas" width="220" height="220"></canvas>
          <div class="lnp-info">
            <h3>Lipid Nanoparticle Architecture</h3>
            <ul class="lnp-legend">
              <li><span class="legend-dot" style="background:#3dbfb0"></span>Ionizable lipid core</li>
              <li><span class="legend-dot" style="background:#c9a84c"></span>Phospholipid bilayer (HSPC)</li>
              <li><span class="legend-dot" style="background:#8ba3bc"></span>Cholesterol stabilizer</li>
              <li><span class="legend-dot" style="background:#e8c96a"></span>PEG-lipid (DSPE-mPEG2000)</li>
              <li><span class="legend-dot" style="background:#ff9b9b"></span>Nucleic acid payload (mRNA/shRNA)</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="about-text">
        <p>My technical strengths center on nanoparticle manufacturing and characterization — from DLS, zeta potential, and UPLC-CAD analytics to TFF-based continuous manufacturing workflows. I have developed validated methods for simultaneous lipid component and degradation species quantification, enabling mechanistic identification of hydrolysis and oxidation pathways undetectable by DLS alone.</p>
        <p>I am actively seeking industry positions in formulation science, LNP/nucleic acid delivery, or drug product development, with particular interest in biotechs and innovative companies advancing mRNA therapeutics, gene delivery, or complex injectable platforms.</p>
      </div>
    </div>
  </div>
</section>


<!-- VALUE PROPOSITION -->
<section id="value">
  <div class="section-inner">
    <p class="section-label reveal">Why teams hire me</p>
    <h2 class="section-title reveal">A recruiter-friendly snapshot of my value</h2>
    <p class="section-subtitle reveal">I bridge formulation design, analytical depth, manufacturing execution, and translational thinking — the combination most hiring teams want for complex injectable, nanoparticle, and nucleic-acid drug product roles.</p>
    <div class="value-grid">
      <div class="value-card reveal">
        <div class="value-kicker">Formulation</div>
        <div class="value-title">Built for complex drug products</div>
        <div class="value-copy">Hands-on experience across lipid nanoparticles, liposomes, nucleic-acid delivery systems, long-acting injectables, sterile suspensions, and excipient-driven performance optimization.</div>
        <div class="value-metric">LNP + LAI + Sterile DP</div>
      </div>
      <div class="value-card reveal">
        <div class="value-kicker">Analytics</div>
        <div class="value-title">Strong analytical problem solver</div>
        <div class="value-copy">Comfortable moving from DLS and zeta potential to UPLC-CAD, LC-MS/MS, DSC, XRPD, FTIR, and orthogonal characterization to explain why a formulation succeeds or fails.</div>
        <div class="value-metric">Mechanism over guesswork</div>
      </div>
      <div class="value-card reveal">
        <div class="value-kicker">Manufacturing</div>
        <div class="value-title">Ready for process development</div>
        <div class="value-copy">Experience with continuous manufacturing workflows, TFF concentration and diafiltration, scale-aware formulation decisions, stability strategy, and GMP-aligned CMC documentation.</div>
        <div class="value-metric">From bench to CMC</div>
      </div>
      <div class="value-card reveal">
        <div class="value-kicker">Impact</div>
        <div class="value-title">Communicates science clearly</div>
        <div class="value-copy">Published, presented, patented, and collaborated across analytical, regulatory, and development teams — translating complex data into decisions that move programs forward.</div>
        <div class="value-metric">8 publications · 1 patent</div>
      </div>
    </div>
  </div>
</section>

<!-- SKILLS -->
<section id="skills">
  <div class="section-inner">
    <p class="section-label reveal">Technical expertise</p>
    <h2 class="section-title reveal">Core Competencies</h2>
    <div class="skills-grid">
      <div class="skill-card reveal"><div class="skill-card-title">Formulation & Process Development</div><div class="skill-card-body">LNP/liposome manufacturing, oligonucleotide & small molecule drug product development, sterile injectable formulation, excipient screening, suspension stabilization, wet media milling, nanoparticle scale-up and process parameter optimization</div></div>
      <div class="skill-card reveal"><div class="skill-card-title">Oligonucleotide & Nucleic Acid Delivery</div><div class="skill-card-body">shRNA/mRNA complexation and encapsulation, gel retardation assays, heparin displacement assays, DNase/serum stability assays, encapsulation efficiency, transfection potency — EGFP, MTT, apoptosis assays in MDA-MB-231 cells</div></div>
      <div class="skill-card reveal"><div class="skill-card-title">Continuous Manufacturing & TFF</div><div class="skill-card-body">Liposome formation, buffer exchange, concentration/diafiltration via tangential flow filtration as part of continuous nanoparticle manufacturing pipeline; EDC/NHS bioconjugation chemistry for surface modification</div></div>
      <div class="skill-card reveal"><div class="skill-card-title">Pre-formulation Characterization</div><div class="skill-card-body">DSC/TGA, XRPD, FTIR, SEM/TEM, DLS (Z-average, PDI), zeta potential — applied to define critical physicochemical properties and guide formulation strategy for injectable drug products</div></div>
      <div class="skill-card reveal"><div class="skill-card-title">Analytical Chemistry</div><div class="skill-card-body">UPLC-CAD method development & validation, HPLC/UPLC, LC-MS/MS, SEC-MALS; simultaneous lipid/degradation species quantification; mechanistic identification of hydrolysis and oxidation degradation pathways</div></div>
      <div class="skill-card reveal"><div class="skill-card-title">Stability & CMC</div><div class="skill-card-body">18-month ICH-aligned long-term stability studies, accelerated stability testing, lipid degradation pathway analysis, CMC documentation, GMP-compliant data packages, FDA BAA contract reporting</div></div>
      <div class="skill-card reveal"><div class="skill-card-title">PBPK / IVIVC Modeling</div><div class="skill-card-body">GastroPlus, Phoenix WinNonlin; mechanistic modeling linking formulation properties to systemic pharmacokinetics; in vitro–in vivo extrapolation supporting bioequivalence strategy and CMC documentation</div></div>
      <div class="skill-card reveal"><div class="skill-card-title">Regulatory & Quality</div><div class="skill-card-body">FDA 505(b)(2) submissions (Cipla), SOP authorship, deviation investigation & CAPA, risk assessment, cross-functional collaboration with analytical, regulatory, and manufacturing teams</div></div>
    </div>
  </div>
</section>



<!-- BIOPROCESS ANIMATION -->
<section id="bioprocess">
  <div class="section-inner">
    <p class="section-label reveal">Animated process science</p>
    <h2 class="section-title reveal">Protein separation, purification & TFF</h2>
    <div class="process-grid">
      <div class="process-card reveal">
        <div class="process-kicker">Step 01</div>
        <div class="process-name">Protein Separation</div>
        <div class="process-stage">Chromatographic capture</div>
        <p class="process-copy">A dynamic capture-column visualization showing product-rich protein bands progressing through the separation bed while smaller impurities pass differently through the system.</p>
        <div class="process-viz" id="sepViz">
          <div class="sep-port top"></div>
          <div class="sep-column">
            <div class="sep-resin"></div>
          </div>
          <div class="sep-port bottom"></div>
          <div class="sep-flow"></div>
        </div>
        <ul class="process-notes">
          <li>Animated feed loading into the resin bed</li>
          <li>Product and impurity species shown as distinct particles</li>
          <li>Designed to communicate selective separation visually</li>
        </ul>
      </div>

      <div class="process-card reveal">
        <div class="process-kicker">Step 02</div>
        <div class="process-name">Purification</div>
        <div class="process-stage">Multistage polishing</div>
        <p class="process-copy">A staged purification panel with progressively cleaner streams, illustrating enrichment across sequential polishing zones and improved product purity.</p>
        <div class="process-viz" id="purifyViz">
          <div class="purify-chamber">
            <div class="purify-layer l1"></div>
            <div class="purify-layer l2"></div>
            <div class="purify-layer l3"></div>
            <div class="purify-arrow"></div>
          </div>
        </div>
        <ul class="process-notes">
          <li>Three purification bands suggest stepwise cleanup</li>
          <li>Product particles emerge with fewer impurities downstream</li>
          <li>Subtle motion keeps the section visually alive without clutter</li>
        </ul>
      </div>

      <div class="process-card reveal">
        <div class="process-kicker">Step 03</div>
        <div class="process-name">Tangential Flow Filtration</div>
        <div class="process-stage">Concentration & diafiltration</div>
        <p class="process-copy">A recirculating TFF loop showing feed, retentate, and permeate paths with membrane-side particle motion to convey retention of larger species and solvent exchange.</p>
        <div class="process-viz" id="tffViz">
          <div class="tff-loop">
            <div class="flow-label feed">Feed</div>
            <div class="flow-label ret">Retentate</div>
            <div class="flow-label perm">Permeate</div>
            <div class="tff-feed"></div>
            <div class="tff-retentate"></div>
            <div class="tff-permeate"></div>
            <div class="tff-membrane"><div class="tff-mesh"></div></div>
            <div class="tff-pump"></div>
            <div class="tff-path tff-line1"></div>
            <div class="tff-path tff-line2"></div>
            <div class="tff-path tff-line3"></div>
            <div class="tff-path tff-line4"></div>
            <div class="tff-path tff-line5"></div>
          </div>
        </div>
        <ul class="process-notes">
          <li>Recirculation path emphasizes tangential membrane flow</li>
          <li>Permeate stream animated separately from retained product</li>
          <li>Useful visual cue for concentration and buffer exchange workflows</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<!-- EXPERIENCE -->
<section id="experience">
  <div class="section-inner">
    <p class="section-label reveal">Career</p>
    <h2 class="section-title reveal">Research & Professional Experience</h2>

    <div class="exp-item reveal">
      <div class="exp-meta">
        <div class="exp-period">Aug 2021 — Present</div>
        <div class="exp-org">University of Connecticut</div>
        <div class="exp-loc">Storrs, CT</div>
      </div>
      <div>
        <div class="exp-role">Ph.D. Graduate Researcher<br>LNP Manufacturing, Process Development & Drug Delivery</div>
        <div class="exp-project-head">Project 1 — Continuous Manufacturing & LNP Stability</div>
        <ul class="exp-bullets">
          <li>Established long-term stability profiles for 7 liposomal nanoparticle formulations (50–200 nm) by executing 18-month ICH-aligned studies across 700+ time points, generating GMP-ready CQA data packages for an FDA BAA-funded program.</li>
          <li>Developed and validated a single UPLC-CAD method simultaneously quantifying 4 lipid components and 3 degradation species — enabling mechanistic identification of hydrolysis and oxidation pathways previously undetected by DLS.</li>
          <li>Prevented release of an out-of-spec batch by identifying PEG-concentration-dependent colloidal instability through orthogonal characterization (DLS, light microscopy, UPLC-CAD).</li>
          <li>Validated container closure compatibility across 2D bags and glass vials via accelerated stability studies up to 74 days at 4°C/25°C/37°C.</li>
        </ul>
        <div class="exp-project-head">Project 2 — LAI Suspension Injectable Depot</div>
        <ul class="exp-bullets">
          <li>Designed and characterized sterile suspension parenteral drug products to identify critical material attributes; performed pre-formulation and excipient compatibility studies.</li>
          <li>Developed novel in vitro drug release testing methods; built mechanistic IVIVC and PBPK models (GastroPlus, Phoenix WinNonlin) linking formulation properties to systemic PK.</li>
          <li>Invented dissolution adapter device — U.S. Patent No. 63/464,677, licensed to PION Inc.</li>
          <li>Published 4 first-author peer-reviewed articles; presented at 9 national and international conferences.</li>
        </ul>
        <!-- animated stability chart -->
        <div class="stability-panel">
          <div class="stability-header">
            <span>18-Month Long-Term Stability — Particle Size (Z-average, nm)</span>
            <span style="color:var(--teal-light)">4°C &amp; 25°C Storage</span>
          </div>
          <canvas id="stabilityCanvas"></canvas>
          <div class="stab-legend">
            <div class="stab-legend-item"><div class="stab-line" style="background:#3dbfb0"></div>LS100 0%PEG · 4°C</div>
            <div class="stab-legend-item"><div class="stab-line" style="background:#c9a84c"></div>LS100 2.5%PEG · 4°C</div>
            <div class="stab-legend-item"><div class="stab-line" style="background:rgba(61,191,176,.4);border-top:2px dashed #3dbfb0"></div>LS100 0%PEG · 25°C</div>
            <div class="stab-legend-item"><div class="stab-line" style="background:rgba(201,168,76,.4);border-top:2px dashed #c9a84c"></div>LS100 2.5%PEG · 25°C</div>
          </div>
        </div>
      </div>
    </div>

    <div class="exp-item reveal">
      <div class="exp-meta">
        <div class="exp-period">May — Aug 2025</div>
        <div class="exp-org">AbbVie</div>
        <div class="exp-loc">Irvine, CA</div>
      </div>
      <div>
        <div class="exp-role">Summer Intern<br>Drug Product Development (Injectables)</div>
        <ul class="exp-bullets">
          <li>Supported CMC characterization of PLGA microsphere long-acting sterile injectables using HPLC/HPSEC, FTIR, DSC/TGA, and laser diffraction; generated stability data packages informing formulation selection for a nonclinical program.</li>
          <li>Assessed E-beam sterilization impact on PLGA microsphere physicochemical properties; translated findings into actionable CMC strategy recommendations in a GMP-aligned environment.</li>
          <li>Collaborated cross-functionally with formulation, analytical, and regulatory teams to define release specifications and advance drug product characterization deliverables.</li>
        </ul>
      </div>
    </div>

    <div class="exp-item reveal">
      <div class="exp-meta">
        <div class="exp-period">Jul 2019 — Jul 2021</div>
        <div class="exp-org">Cipla Ltd.</div>
        <div class="exp-loc">India</div>
      </div>
      <div>
        <div class="exp-role">Scientist<br>Generic Drug Product Development & Regulatory</div>
        <ul class="exp-bullets">
          <li>Led QbD-driven formulation development of amorphous solid dispersions for US FDA 505(b)(2) submissions; applied risk-based approaches to define CQAs, CMAs, and CPPs.</li>
          <li>Authored CMC documentation, SOPs, and regulatory submission packages per GDP and cGMP; contributed to ANDA/505(b)(2) filings and FDA office action responses.</li>
          <li>Collaborated with manufacturing for scale-up and technology transfer; troubleshot deviations using CAPA and change control tools. Liaised with CRO/CDMO partners.</li>
        </ul>
      </div>
    </div>

    <div class="exp-item reveal">
      <div class="exp-meta">
        <div class="exp-period">Jul 2017 — Jul 2019</div>
        <div class="exp-org">NIPER Mohali</div>
        <div class="exp-loc">Punjab, India</div>
      </div>
      <div>
        <div class="exp-role">Graduate Research Assistant<br>Bioconjugate Nanoparticle Design & Nucleic Acid Delivery</div>
        <ul class="exp-bullets">
          <li>Designed histidine-lauric acid amphiphilic conjugate via EDC/NHS bioconjugation for LNP targeting moiety applications.</li>
          <li>Formulated dendrimer/surfactant NPs for combination docetaxel + SIRT1-silencing shRNA delivery; validated nucleic acid encapsulation by gel retardation, heparin displacement, and DNase stability assays.</li>
          <li>Conducted potency assays (EGFP transfection, MTT cytotoxicity, apoptosis) in MDA-MB-231 cells.</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<!-- PUBLICATIONS -->
<section id="publications">
  <div class="section-inner">
    <p class="section-label reveal">Research output</p>
    <h2 class="section-title reveal">Publications & Patent</h2>
    <div class="pub-grid">
      <div class="patent-card reveal">
        <div class="patent-icon">©</div>
        <div>
          <div class="pub-year">U.S. PATENT · FILED MAY 2024</div>
          <div class="pub-title">Dissolution Adapter — Method of Manufacture and Method of Use Thereof</div>
          <div class="pub-journal">No. 63/464,677 · Licensed & Commercialized by PION Inc.</div>
        </div>
      </div>
      <div class="pub-card reveal"><div class="pub-year">2026 · IN REVIEW</div><div class="pub-title">Mathematical modeling of drug release from long-acting suspensions</div><div class="pub-journal">Malavia N. et al. · Journal of Controlled Release</div></div>
      <div class="pub-card reveal"><div class="pub-year">2026 · IN REVIEW</div><div class="pub-title">Mechanistic Understanding of LAI Suspension Intramuscular Depot Formation: A Physicochemical Perspective</div><div class="pub-journal">Malavia N. et al. · Journal of Controlled Release</div></div>
      <div class="pub-card reveal"><div class="pub-year">2026 · ACCEPTED</div><div class="pub-title">Impact of macrophages on dissolution of prodrugs long-acting injectable suspensions</div><div class="pub-journal">Malavia N. et al. · International Journal of Pharmaceutics</div></div>
      <div class="pub-card reveal"><div class="pub-year">2026</div><div class="pub-title">Insights into development of long-acting injectable suspensions</div><div class="pub-journal">Malavia N. & Burgess D.J. · Journal of Controlled Release, 114721</div></div>
      <div class="pub-card reveal"><div class="pub-year">2026</div><div class="pub-title">Mechanistic Modeling of Intramuscular Administration of a Long-acting Injectable Accounting for Tissue Response at the Depot Site</div><div class="pub-journal">Silva D.A., … Malavia N. et al. · The AAPS Journal, 28(1), 1–15</div></div>
      <div class="pub-card reveal"><div class="pub-year">2025</div><div class="pub-title">Impact of agglomeration on in vitro performance of long-acting injectable suspensions</div><div class="pub-journal">Malavia N. et al. · International Journal of Pharmaceutics, 673, 125390</div></div>
      <div class="pub-card reveal"><div class="pub-year">2024</div><div class="pub-title">Novel dissolution methods for drug release testing of Long-Acting injectables</div><div class="pub-journal">Malavia N. et al. · International Journal of Pharmaceutics, 664, 124634</div></div>
      <div class="pub-card reveal"><div class="pub-year">2024</div><div class="pub-title">Development of mechanistic in vitro–in vivo extrapolation to support bioequivalence assessment of long-acting injectables</div><div class="pub-journal">Amaral D., … Malavia N. et al. · Pharmaceutics, 16(4), 552</div></div>
      <div class="pub-card reveal"><div class="pub-year">2021</div><div class="pub-title">Green surfactant-dendrimer aggreplexes: An ingenious way to launch dual attack on arch-enemy cancer</div><div class="pub-journal">Malavia N. et al. · Colloids and Surfaces B: Biointerfaces, 204, 111821</div></div>
    </div>
  </div>
</section>

<!-- PRESENTATIONS -->
<section id="presentations">
  <div class="section-inner">
    <p class="section-label reveal">Scientific dissemination</p>
    <h2 class="section-title reveal">Posters, Presentations & Invited Talks</h2>
    <ul class="pres-list">
      <li class="pres-item reveal"><div class="pres-year">Nov 2025</div><div><div class="pres-title">Impact of Polyethylene Glycol Polymer in the Development of Long-Acting Injectable Suspensions</div><div class="pres-venue">AAPS PharmSci 360 · San Antonio, TX</div></div></li>
      <li class="pres-item reveal"><div class="pres-year">Oct 2024</div><div><div class="pres-title">Impact of macrophages on the dissolution of long-acting injectable suspensions</div><div class="pres-venue">AAPS PharmSci 360 · Salt Lake City, UT</div><div class="pres-award">Selected for Special Poster Collection</div></div></li>
      <li class="pres-item reveal"><div class="pres-year">2024</div><div><div class="pres-title">Formulation Insights into Long-Acting Hormonal Contraceptives for Advancing Generic Development</div><div class="pres-venue">CRS Annual Meeting · Bologna, Italy</div><div class="pres-award">Top Poster Award</div></div></li>
      <li class="pres-item reveal"><div class="pres-year">2024</div><div><div class="pres-title">Formulation Insights into Long-Acting Injectable Suspensions for Advancing Product Development</div><div class="pres-venue">AAPS Northeast Regional Discussion Group · Mystic, CT</div><div class="pres-award">First Place Academic Research Award</div></div></li>
      <li class="pres-item reveal"><div class="pres-year">Oct 2023</div><div><div class="pres-title">Enabling Formulation Development of LAIs Through Understanding Critical Formulation Parameters</div><div class="pres-venue">AAPS PharmSci 360 · Orlando, FL</div></div></li>
      <li class="pres-item reveal"><div class="pres-year">Jul 2023</div><div><div class="pres-title">Fabrication of a Novel Adapter for in vitro Release Testing and IVIVC Development of Long-Acting Injectable Suspensions</div><div class="pres-venue">CRS Annual Meeting · Las Vegas, NV</div><div class="pres-award">Best Poster Award</div></div></li>
      <li class="pres-item reveal"><div class="pres-year">2023</div><div><div class="pres-title">Fabrication of a Novel Adapter for in vitro Release Testing and IVIVC Development</div><div class="pres-venue">AAPS Northeast Regional Discussion Group · Queens, NY</div></div></li>
      <li class="pres-item reveal"><div class="pres-year">Invited</div><div><div class="pres-title">Tumor Delivery of Plasmid DNA using pH-sensitive Liposomes</div><div class="pres-venue">All India Institute of Medical Sciences · Rishikesh, India</div><div class="pres-award">Invited Talk</div></div></li>
      <li class="pres-item reveal"><div class="pres-year">Invited</div><div><div class="pres-title">Tumor Delivery of Plasmid DNA using pH-sensitive Liposomes</div><div class="pres-venue">Bristol Myers Squibb Symposium at NIPER · India</div><div class="pres-award">Invited Talk</div></div></li>
    </ul>
  </div>
</section>

<!-- AWARDS -->
<section id="awards">
  <div class="section-inner">
    <p class="section-label reveal">Recognition</p>
    <h2 class="section-title reveal">Awards & Fellowships</h2>
    <div class="awards-grid">
      <div class="award-card reveal"><div class="award-year">2025</div><div class="award-name">AAIPS Graduate Student Award</div></div>
      <div class="award-card reveal"><div class="award-year">2025</div><div class="award-name">IPEC Graduate Student Award</div></div>
      <div class="award-card reveal"><div class="award-year">2025</div><div class="award-name">Best Student Award</div><div class="award-org">Boehringer Ingelheim</div></div>
      <div class="award-card reveal"><div class="award-year">2025</div><div class="award-name">Dr. Edward A. Khairallah Fellowship</div><div class="award-org">University of Connecticut</div></div>
      <div class="award-card reveal"><div class="award-year">2025</div><div class="award-name">Doctoral Dissertation Fellowship</div><div class="award-org">University of Connecticut</div></div>
      <div class="award-card reveal"><div class="award-year">2025</div><div class="award-name">Gerald J. Jackson Graduate Student Fellowship</div><div class="award-org">University of Connecticut</div></div>
      <div class="award-card reveal"><div class="award-year">2024</div><div class="award-name">Top Research Poster Award</div><div class="award-org">Controlled Release Society · Bologna</div></div>
      <div class="award-card reveal"><div class="award-year">2024</div><div class="award-name">First Place Academic Research Award</div><div class="award-org">AAPS NERDG</div></div>
      <div class="award-card reveal"><div class="award-year">2023</div><div class="award-name">Best Research Poster Award</div><div class="award-org">Controlled Release Society · Las Vegas</div></div>
      <div class="award-card reveal"><div class="award-year">2021</div><div class="award-name">Predoctoral Fellowship</div><div class="award-org">University of Connecticut</div></div>
    </div>
  </div>
</section>

<!-- EDUCATION -->
<section id="education">
  <div class="section-inner">
    <p class="section-label reveal">Academic background</p>
    <h2 class="section-title reveal">Education</h2>
    <div class="edu-grid">
      <div class="edu-card reveal" data-gpa="3.94"><div class="edu-degree">Ph.D. in Pharmaceutics</div><div class="edu-school">University of Connecticut</div><div class="edu-details">Storrs, CT · Expected April 2026</div><div class="edu-gpa">GPA 3.94 / 4.0</div></div>
      <div class="edu-card reveal" data-gpa="3.90"><div class="edu-degree">M.S. in Pharmaceutical Sciences</div><div class="edu-school">NIPER Mohali</div><div class="edu-details">Punjab, India · June 2019</div><div class="edu-gpa">GPA 3.90 / 4.0</div></div>
      <div class="edu-card reveal" data-gpa="3.90"><div class="edu-degree">B.Pharm. in Pharmacy</div><div class="edu-school">Bombay College of Pharmacy</div><div class="edu-details">Mumbai, India · June 2017</div><div class="edu-gpa">GPA 3.90 / 4.0</div></div>
    </div>
  </div>
</section>

<!-- CONTACT -->
<section id="contact">
  <div class="section-inner">
    <p class="section-label" style="text-align:center">Get in touch</p>
    <h2 class="section-title" style="text-align:center;margin-bottom:0">Open to opportunities<br>in formulation science</h2>
    <a href="mailto:nilesh.malavia@uconn.edu" class="contact-email">nilesh.malavia@uconn.edu</a>
    <p style="font-family:var(--mono);font-size:.75rem;color:var(--slate);text-align:center;margin-bottom:1.5rem">+1 (959) 929-9274 · Willimantic, CT</p>
    <div class="contact-links">
      <a href="https://linkedin.com/in/nilesh-malviya" class="contact-link" target="_blank">LinkedIn</a>
      <a href="mailto:nilesh.malavia@uconn.edu" class="contact-link">Email</a>
    </div>
  </div>
</section>

<footer>
  <span>© 2026 Nilesh Malavia</span>
  <span>Ph.D. Candidate · Pharmaceutics · University of Connecticut</span>
  <span>Defense: April 2026</span>
</footer>

<script>
// ─────────────────────────────────────────────
// 1. FLOATING MOLECULE BACKGROUND
// ─────────────────────────────────────────────
(function(){
  const cvs = document.getElementById('moleculeCanvas');
  const ctx = cvs.getContext('2d');
  let W,H,nodes,frame=0;
  function resize(){
    W=cvs.width=window.innerWidth;
    H=cvs.height=window.innerHeight;
  }
  function initNodes(){
    nodes=[];
    const count=Math.floor(W*H/22000);
    for(let i=0;i<count;i++){
      nodes.push({
        x:Math.random()*W, y:Math.random()*H,
        vx:(Math.random()-.5)*0.18, vy:(Math.random()-.5)*0.18,
        r:Math.random()*2.5+1.5,
        type:Math.floor(Math.random()*4) // 0=C 1=N 2=O 3=P
      });
    }
  }
  const atomColors=['rgba(61,191,176,','rgba(139,163,188,','rgba(255,155,155,','rgba(201,168,76,'];
  const atomLabels=['C','N','O','P'];
  function draw(){
    ctx.clearRect(0,0,W,H);
    frame++;
    // bonds
    for(let i=0;i<nodes.length;i++){
      for(let j=i+1;j<nodes.length;j++){
        const dx=nodes[j].x-nodes[i].x, dy=nodes[j].y-nodes[i].y;
        const dist=Math.sqrt(dx*dx+dy*dy);
        if(dist<120){
          const alpha=(1-dist/120)*0.18;
          ctx.beginPath();
          ctx.moveTo(nodes[i].x,nodes[i].y);
          ctx.lineTo(nodes[j].x,nodes[j].y);
          ctx.strokeStyle=`rgba(42,157,143,${alpha})`;
          ctx.lineWidth=0.8;
          ctx.stroke();
        }
      }
    }
    // atoms
    nodes.forEach(n=>{
      n.x+=n.vx; n.y+=n.vy;
      if(n.x<-20)n.x=W+20; if(n.x>W+20)n.x=-20;
      if(n.y<-20)n.y=H+20; if(n.y>H+20)n.y=-20;
      ctx.beginPath();
      ctx.arc(n.x,n.y,n.r,0,Math.PI*2);
      ctx.fillStyle=atomColors[n.type]+'0.55)';
      ctx.fill();
      if(n.r>2.8){
        ctx.fillStyle=atomColors[n.type]+'0.7)';
        ctx.font=`${Math.floor(n.r*2.2)}px DM Mono,monospace`;
        ctx.textAlign='center';
        ctx.textBaseline='middle';
        ctx.fillText(atomLabels[n.type],n.x,n.y);
      }
    });
    requestAnimationFrame(draw);
  }
  resize(); initNodes(); draw();
  window.addEventListener('resize',()=>{resize();initNodes();});
})();

// ─────────────────────────────────────────────
// 2. HPLC CHROMATOGRAM
// ─────────────────────────────────────────────
(function(){
  const cvs=document.getElementById('hplcCanvas');
  if(!cvs)return;
  const ctx=cvs.getContext('2d');
  const peaks=[
    {t:0.14,h:0.38,w:0.025,col:'#ff9b9b',label:'Lyso-PC-16'},
    {t:0.32,h:0.62,w:0.03, col:'#8ba3bc',label:'DSPG'},
    {t:0.50,h:0.95,w:0.035,col:'#3dbfb0',label:'HSPC'},
    {t:0.65,h:0.75,w:0.04, col:'#c9a84c',label:'Cholesterol'},
    {t:0.85,h:0.55,w:0.03, col:'#e8c96a',label:'DSPE-mPEG'}
  ];
  let progress=0, done=false;
  function gaussian(x,mu,sigma){return Math.exp(-0.5*((x-mu)/sigma)**2)}
  function render(){
    const dpr=window.devicePixelRatio||1;
    const W=cvs.offsetWidth, H=cvs.offsetHeight;
    cvs.width=W*dpr; cvs.height=H*dpr;
    ctx.scale(dpr,dpr);
    ctx.clearRect(0,0,W,H);
    // grid
    ctx.strokeStyle='rgba(42,157,143,0.1)'; ctx.lineWidth=0.5;
    for(let i=0;i<=5;i++){
      const y=H-10-(i/5)*(H-20);
      ctx.beginPath();ctx.moveTo(40,y);ctx.lineTo(W-10,y);ctx.stroke();
    }
    // axes
    ctx.strokeStyle='rgba(139,163,188,0.4)'; ctx.lineWidth=1;
    ctx.beginPath();ctx.moveTo(40,10);ctx.lineTo(40,H-10);ctx.lineTo(W-10,H-10);ctx.stroke();
    ctx.fillStyle='rgba(139,163,188,0.5)';ctx.font='9px DM Mono,monospace';
    ctx.textAlign='center';
    ctx.fillText('0',40,H-2);ctx.fillText('5',40+(W-50)*0.33,H-2);
    ctx.fillText('10',40+(W-50)*0.66,H-2);ctx.fillText('15 min',W-10,H-2);
    // baseline
    const pts=500;
    const p=Math.min(progress,1);
    ctx.beginPath();
    let started=false;
    for(let i=0;i<pts*p;i++){
      const xr=i/pts;
      const xPx=40+xr*(W-50);
      let y=0;
      peaks.forEach(pk=>{ y+=pk.h*gaussian(xr,pk.t,pk.w); });
      // add baseline noise
      y+=Math.sin(i*0.4)*0.008+Math.random()*0.004;
      const yPx=H-10-y*(H-24);
      if(!started){ctx.moveTo(xPx,yPx);started=true;}
      else ctx.lineTo(xPx,yPx);
    }
    ctx.strokeStyle='rgba(61,191,176,0.85)';ctx.lineWidth=1.5;
    ctx.stroke();
    // filled peaks (only when full)
    if(p>=1){
      peaks.forEach(pk=>{
        ctx.beginPath();
        for(let i=0;i<=200;i++){
          const xr=(pk.t-pk.w*4)+i/200*(pk.w*8);
          const xPx=40+xr*(W-50);
          const pv=pk.h*gaussian(xr,pk.t,pk.w);
          const yPx=H-10-pv*(H-24);
          if(i===0)ctx.moveTo(xPx,H-10); else ctx.lineTo(xPx,yPx);
        }
        ctx.closePath();
        ctx.fillStyle=pk.col.replace('#','rgba(').length>7?pk.col+'33':hexAlpha(pk.col,0.15);
        ctx.fill();
      });
    }
    if(!done){ progress+=0.008; if(progress>=1)done=true; requestAnimationFrame(render); }
  }
  function hexAlpha(hex,a){
    const r=parseInt(hex.slice(1,3),16),g=parseInt(hex.slice(3,5),16),b=parseInt(hex.slice(5,7),16);
    return `rgba(${r},${g},${b},${a})`;
  }
  render();
})();

// ─────────────────────────────────────────────
// 3. DLS SIZE DISTRIBUTION
// ─────────────────────────────────────────────
(function(){
  const cvs=document.getElementById('dlsCanvas');
  if(!cvs)return;
  const ctx=cvs.getContext('2d');
  let t=0;
  function gaussian(x,mu,sigma){return Math.exp(-0.5*((x-mu)/sigma)**2)}
  function render(){
    const dpr=window.devicePixelRatio||1;
    const W=cvs.offsetWidth,H=cvs.offsetHeight;
    cvs.width=W*dpr;cvs.height=H*dpr;
    ctx.scale(dpr,dpr);
    ctx.clearRect(0,0,W,H);
    t+=0.018;
    // fluctuating mean/width (simulates live DLS scan noise)
    const mu=127+Math.sin(t)*3;
    const sig=18+Math.cos(t*0.7)*2;
    const pts=200;
    const xMin=40,xMax=280;
    // fill
    ctx.beginPath();
    ctx.moveTo(30+(0/pts)*(W-40),H-10);
    for(let i=0;i<=pts;i++){
      const sz=xMin+i/pts*(xMax-xMin);
      const v=gaussian(sz,mu,sig)+Math.random()*0.01;
      const xPx=30+i/pts*(W-40);
      const yPx=H-10-v*(H-20)*0.92;
      if(i===0)ctx.moveTo(xPx,H-10);
      ctx.lineTo(xPx,yPx);
    }
    ctx.closePath();
    ctx.fillStyle='rgba(42,157,143,0.12)';ctx.fill();
    // line
    ctx.beginPath();
    for(let i=0;i<=pts;i++){
      const sz=xMin+i/pts*(xMax-xMin);
      const v=gaussian(sz,mu,sig)+Math.random()*0.008;
      const xPx=30+i/pts*(W-40);
      const yPx=H-10-v*(H-20)*0.92;
      if(i===0)ctx.moveTo(xPx,yPx);
      else ctx.lineTo(xPx,yPx);
    }
    ctx.strokeStyle='rgba(61,191,176,0.85)';ctx.lineWidth=1.5;ctx.stroke();
    // x-axis labels
    ctx.fillStyle='rgba(139,163,188,0.5)';ctx.font='8px DM Mono,monospace';ctx.textAlign='center';
    [50,100,150,200,250].forEach(sz=>{
      const xPx=30+(sz-xMin)/(xMax-xMin)*(W-40);
      ctx.fillText(sz+'nm',xPx,H-1);
    });
    // live readout
    document.getElementById('dls-zave').textContent=(mu).toFixed(1)+' nm';
    requestAnimationFrame(render);
  }
  render();
})();

// ─────────────────────────────────────────────
// 4. LNP CROSS-SECTION (animated)
// ─────────────────────────────────────────────
(function(){
  const cvs=document.getElementById('lnpCanvas');
  if(!cvs)return;
  const ctx=cvs.getContext('2d');
  const W=220,H=220,cx=110,cy=110;
  let t=0;
  function draw(){
    ctx.clearRect(0,0,W,H);
    t+=0.012;
    const r=78;
    // outer PEG corona — animated wisps
    for(let i=0;i<16;i++){
      const angle=(i/16)*Math.PI*2+t*0.3;
      const len=12+Math.sin(t*1.5+i)*4;
      const bx=cx+Math.cos(angle)*(r+4);
      const by=cy+Math.sin(angle)*(r+4);
      const ex=cx+Math.cos(angle)*(r+4+len);
      const ey=cy+Math.sin(angle)*(r+4+len);
      ctx.beginPath();ctx.moveTo(bx,by);ctx.lineTo(ex,ey);
      ctx.strokeStyle='rgba(232,201,106,0.55)';ctx.lineWidth=2;
      ctx.lineCap='round';ctx.stroke();
    }
    // phospholipid bilayer outer
    const gOuter=ctx.createRadialGradient(cx,cy,r-8,cx,cy,r+4);
    gOuter.addColorStop(0,'rgba(201,168,76,0.15)');
    gOuter.addColorStop(0.5,'rgba(201,168,76,0.55)');
    gOuter.addColorStop(1,'rgba(201,168,76,0.1)');
    ctx.beginPath();ctx.arc(cx,cy,r,0,Math.PI*2);
    ctx.fillStyle=gOuter;ctx.fill();
    ctx.strokeStyle='rgba(201,168,76,0.7)';ctx.lineWidth=1;ctx.stroke();
    // phospholipid bilayer inner
    const rInner=r-12;
    ctx.beginPath();ctx.arc(cx,cy,rInner,0,Math.PI*2);
    ctx.strokeStyle='rgba(201,168,76,0.35)';ctx.lineWidth=1;ctx.stroke();
    // cholesterol molecules (small lines)
    for(let i=0;i<12;i++){
      const angle=(i/12)*Math.PI*2+Math.sin(t+i)*0.08;
      const ri=rInner+2,ro=r-3;
      ctx.beginPath();
      ctx.moveTo(cx+Math.cos(angle)*ri,cy+Math.sin(angle)*ri);
      ctx.lineTo(cx+Math.cos(angle)*ro,cy+Math.sin(angle)*ro);
      ctx.strokeStyle='rgba(139,163,188,0.45)';ctx.lineWidth=1.5;ctx.stroke();
    }
    // ionizable lipid core
    const gCore=ctx.createRadialGradient(cx-10,cy-10,5,cx,cy,rInner-4);
    gCore.addColorStop(0,'rgba(61,191,176,0.45)');
    gCore.addColorStop(1,'rgba(42,157,143,0.2)');
    ctx.beginPath();ctx.arc(cx,cy,rInner-4,0,Math.PI*2);
    ctx.fillStyle=gCore;ctx.fill();
    // mRNA payload (wavy line inside)
    ctx.beginPath();
    for(let i=0;i<=60;i++){
      const px=cx-30+i;
      const py=cy+Math.sin((i*0.25)+t*1.5)*12+Math.sin((i*0.5)+t)*5;
      if(i===0)ctx.moveTo(px,py);else ctx.lineTo(px,py);
    }
    ctx.strokeStyle='rgba(255,155,155,0.85)';ctx.lineWidth=2;
    ctx.lineCap='round';ctx.stroke();
    // second strand
    ctx.beginPath();
    for(let i=0;i<=50;i++){
      const px=cx-22+i;
      const py=cy-10+Math.sin((i*0.28)+t*1.2+1)*8;
      if(i===0)ctx.moveTo(px,py);else ctx.lineTo(px,py);
    }
    ctx.strokeStyle='rgba(255,155,155,0.5)';ctx.lineWidth=1.5;ctx.stroke();
    requestAnimationFrame(draw);
  }
  draw();
})();

// ─────────────────────────────────────────────
// 5. STABILITY CURVE CHART
// ─────────────────────────────────────────────
(function(){
  const cvs=document.getElementById('stabilityCanvas');
  if(!cvs)return;
  const ctx=cvs.getContext('2d');
  // time points (days): 0,30,60,90,180,270,365,548,700
  const timePoints=[0,30,60,90,180,270,365,548,700];
  const series=[
    {label:'LS100 0%PEG 4°C',  col:'#3dbfb0',dash:false,data:[100,101,100.5,101,102,101.5,101,102,102.5]},
    {label:'LS100 2.5%PEG 4°C',col:'#c9a84c',dash:false,data:[110,111,110.5,112,111,112,113,112,113]},
    {label:'LS100 0%PEG 25°C', col:'#3dbfb0',dash:true, data:[100,101.5,103,104,106,107,108,109,111]},
    {label:'LS100 2.5%PEG 25°C',col:'#c9a84c',dash:true,data:[110,112,115,118,135,160,210,280,380]},
  ];
  let progress=0,done=false;
  function render(){
    const dpr=window.devicePixelRatio||1;
    const W=cvs.offsetWidth,H=cvs.offsetHeight;
    cvs.width=W*dpr;cvs.height=H*dpr;
    ctx.scale(dpr,dpr);
    ctx.clearRect(0,0,W,H);
    const pad={l:48,r:20,t:10,b:28};
    const pw=W-pad.l-pad.r,ph=H-pad.t-pad.b;
    const maxT=700,minY=90,maxY=420;
    function tx(t){return pad.l+t/maxT*pw}
    function ty(y){return pad.t+ph-(y-minY)/(maxY-minY)*ph}
    // grid
    ctx.strokeStyle='rgba(42,157,143,0.1)';ctx.lineWidth=0.5;
    [100,150,200,250,300,350,400].forEach(y=>{
      ctx.beginPath();ctx.moveTo(pad.l,ty(y));ctx.lineTo(W-pad.r,ty(y));ctx.stroke();
      ctx.fillStyle='rgba(139,163,188,0.45)';ctx.font='8px DM Mono,monospace';
      ctx.textAlign='right';ctx.fillText(y,pad.l-4,ty(y)+3);
    });
    [0,180,365,548,700].forEach(t=>{
      ctx.beginPath();ctx.moveTo(tx(t),pad.t);ctx.lineTo(tx(t),H-pad.b);ctx.stroke();
      ctx.fillStyle='rgba(139,163,188,0.45)';ctx.font='8px DM Mono,monospace';
      ctx.textAlign='center';ctx.fillText(t+'d',tx(t),H-pad.b+10);
    });
    // axes
    ctx.strokeStyle='rgba(139,163,188,0.3)';ctx.lineWidth=1;
    ctx.beginPath();ctx.moveTo(pad.l,pad.t);ctx.lineTo(pad.l,H-pad.b);ctx.lineTo(W-pad.r,H-pad.b);ctx.stroke();
    // y-axis label
    ctx.save();ctx.translate(12,H/2);ctx.rotate(-Math.PI/2);
    ctx.fillStyle='rgba(139,163,188,0.6)';ctx.font='8px DM Mono,monospace';ctx.textAlign='center';
    ctx.fillText('Z-average (nm)',0,0);ctx.restore();
    // series
    const p=Math.min(progress,1);
    series.forEach(s=>{
      const pts=Math.floor(p*(timePoints.length-1));
      if(pts<1)return;
      ctx.beginPath();
      ctx.setLineDash(s.dash?[6,4]:[]);
      for(let i=0;i<=pts;i++){
        const xp=tx(timePoints[i]),yp=ty(s.data[i]);
        if(i===0)ctx.moveTo(xp,yp);else ctx.lineTo(xp,yp);
      }
      // partial last segment
      if(pts<timePoints.length-1){
        const frac=(p*(timePoints.length-1))-pts;
        const x1=tx(timePoints[pts]),y1=ty(s.data[pts]);
        const x2=tx(timePoints[pts+1]),y2=ty(s.data[pts+1]);
        ctx.lineTo(x1+(x2-x1)*frac,y1+(y2-y1)*frac);
      }
      ctx.strokeStyle=s.col;ctx.lineWidth=2;ctx.stroke();
      ctx.setLineDash([]);
      // data points
      for(let i=0;i<=pts;i++){
        ctx.beginPath();ctx.arc(tx(timePoints[i]),ty(s.data[i]),3,0,Math.PI*2);
        ctx.fillStyle=s.col;ctx.fill();
      }
    });
    // aggregation annotation
    if(p>0.7){
      const ax=tx(450),ay=ty(220);
      ctx.fillStyle='rgba(255,155,155,0.8)';ctx.font='9px DM Mono,monospace';ctx.textAlign='left';
      ctx.fillText('↑ Aggregation onset',ax,ay);
    }
    if(!done){progress+=0.006;if(progress>=1)done=true;requestAnimationFrame(render);}
  }
  // trigger when visible
  const obs=new IntersectionObserver(([e])=>{if(e.isIntersecting){render();obs.disconnect();}},{threshold:.3});
  obs.observe(cvs);
})();

// ─────────────────────────────────────────────
// 6. BIOPROCESS PARTICLE ANIMATIONS
// ─────────────────────────────────────────────
(function(){
  function spawnParticle(parent, cls, x, y){
    const el=document.createElement('span');
    el.className=`particle ${cls}`;
    el.style.left=`${x}px`;
    el.style.top=`${y}px`;
    parent.appendChild(el);
    return el;
  }

  // Protein separation column
  const sep=document.getElementById('sepViz');
  if(sep){
    const proteins=[], impurities=[];
    for(let i=0;i<8;i++) proteins.push(spawnParticle(sep,'protein',76+Math.random()*40,10-Math.random()*140));
    for(let i=0;i<6;i++) impurities.push(spawnParticle(sep,'impurity',90+Math.random()*24,8-Math.random()*140));
    let tick=0;
    const animateSep=()=>{
      tick+=0.016;
      proteins.forEach((p,i)=>{
        let y=parseFloat(p.style.top);
        y+=0.95+Math.sin(tick+i)*0.08;
        let x=104+Math.sin(tick*1.5+i)*10;
        if(y>152){ y=-12-Math.random()*80; x=94+Math.random()*22; }
        p.style.top=`${y}px`; p.style.left=`${x}px`;
      });
      impurities.forEach((p,i)=>{
        let y=parseFloat(p.style.top);
        y+=1.3+Math.cos(tick*1.3+i)*0.12;
        let x=(i%2===0?84:122)+Math.sin(tick*2+i)*18;
        if(y>162){ y=-18-Math.random()*60; x=88+Math.random()*30; }
        p.style.top=`${y}px`; p.style.left=`${x}px`;
      });
      requestAnimationFrame(animateSep);
    };
    animateSep();
  }

  // Purification chamber
  const pur=document.getElementById('purifyViz');
  if(pur){
    const clean=[], dirty=[];
    for(let i=0;i<11;i++) dirty.push(spawnParticle(pur, i<6?'impurity':'protein', 4-Math.random()*90, 46+Math.random()*70));
    for(let i=0;i<6;i++) clean.push(spawnParticle(pur,'protein', 4-Math.random()*120, 48+Math.random()*60));
    let t=0;
    const animatePur=()=>{
      t+=0.018;
      dirty.forEach((p,i)=>{
        let x=parseFloat(p.style.left), y=parseFloat(p.style.top);
        x+=0.85 + (p.classList.contains('impurity')?0.35:0.15);
        y += Math.sin(t*2+i)*0.28;
        if(x>260){ x=-10-Math.random()*70; y=44+Math.random()*76; }
        if(p.classList.contains('impurity') && x>170) p.style.opacity='0.18';
        else p.style.opacity='0.88';
        p.style.left=`${x}px`; p.style.top=`${y}px`;
      });
      clean.forEach((p,i)=>{
        let x=parseFloat(p.style.left), y=parseFloat(p.style.top);
        x+=1.05; y += Math.cos(t*1.8+i)*0.22;
        if(x>260){ x=-30-Math.random()*90; y=52+Math.random()*50; }
        p.style.left=`${x}px`; p.style.top=`${y}px`;
      });
      requestAnimationFrame(animatePur);
    };
    animatePur();
  }

  // TFF loop
  const tff=document.getElementById('tffViz');
  if(tff){
    const loop=[];
    const perm=[];
    const loopPath=[
      [30,84],[52,84],[74,84],[98,84],[122,84],[146,84],[170,84],[194,60],[224,39],[247,39],
      [215,39],[190,39],[165,39],[140,39],[114,39],[88,39],[56,39],[42,39],[42,58],[42,86],[42,112],[42,128],[42,142],[42,110],[42,84],[28,84]
    ];
    const permPath=[[150,84],[170,84],[190,84],[210,96],[230,110],[248,126]];
    function makeStream(cls, path, arr){
      for(let i=0;i<4;i++){
        const el=document.createElement('span');
        el.className=`tff-stream ${cls||''}`.trim();
        el.dataset.offset=String((i/path.length)*path.length);
        tff.appendChild(el); arr.push({el,path});
      }
    }
    makeStream('', loopPath, loop);
    makeStream('impurity', permPath, perm);
    let frame=0;
    const move=(obj, speed)=>{
      const path=obj.path; let idx=(parseFloat(obj.el.dataset.offset)+frame*speed)%path.length; const i0=Math.floor(idx), i1=(i0+1)%path.length; const frac=idx-i0;
      const [x0,y0]=path[i0], [x1,y1]=path[i1];
      obj.el.style.left=`${x0+(x1-x0)*frac}px`;
      obj.el.style.top=`${y0+(y1-y0)*frac}px`;
    };
    const animateTff=()=>{
      frame+=0.03;
      loop.forEach(o=>move(o,0.18));
      perm.forEach(o=>move(o,0.12));
      requestAnimationFrame(animateTff);
    };
    animateTff();
  }
})();

// ─────────────────────────────────────────────
// 7. SCROLL REVEAL
// ─────────────────────────────────────────────
const obs=new IntersectionObserver((entries)=>{
  entries.forEach((e,i)=>{
    if(e.isIntersecting){
      setTimeout(()=>e.target.classList.add('visible'),i*70);
      obs.unobserve(e.target);
    }
  });
},{threshold:.08});
document.querySelectorAll('.reveal').forEach(el=>obs.observe(el));

// ─────────────────────────────────────────────
// 8. SCROLL PROGRESS + STAT COUNTUP
// ─────────────────────────────────────────────
(function(){
  const bar=document.getElementById('scrollProgress');
  function updateBar(){
    const h=document.documentElement;
    const total=h.scrollHeight-window.innerHeight;
    const pct=total>0?(window.scrollY/total)*100:0;
    bar.style.width=Math.max(0,Math.min(100,pct))+'%';
  }
  updateBar();
  window.addEventListener('scroll',updateBar,{passive:true});

  const stats=[...document.querySelectorAll('.stat-num')];
  const originals=stats.map(el=>el.textContent.trim());
  stats.forEach(el=>{el.dataset.target=el.textContent.trim(); if(/^[0-9.]+\+?$/.test(el.textContent.trim())) el.textContent='0';});
  const obs=new IntersectionObserver((entries)=>{
    entries.forEach(entry=>{
      if(!entry.isIntersecting) return;
      const el=entry.target;
      const target=el.dataset.target||el.textContent.trim();
      if(el.dataset.done==='1') return;
      el.dataset.done='1';
      if(!/^[0-9.]+\+?$/.test(target)) { el.textContent=target; return; }
      const plus=target.endsWith('+');
      const raw=parseFloat(target.replace('+',''));
      const decimals=(target.includes('.') && raw<10)?2:0;
      const start=performance.now();
      const dur=1200;
      function step(now){
        const p=Math.min(1,(now-start)/dur);
        const ease=1-Math.pow(1-p,3);
        const val=raw*ease;
        el.textContent=val.toFixed(decimals)+(plus && p===1?'+':'');
        if(p<1) requestAnimationFrame(step);
      }
      requestAnimationFrame(step);
    });
  },{threshold:.45});
  stats.forEach(el=>obs.observe(el));
})();

</script>
</body>
</html>
