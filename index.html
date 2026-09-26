"""
Pr Hubb | PR Consultancy Agency  —  premium edition
---------------------------------------------------
Single-file Flask application that serves the agency website.

Run:
    pip install flask
    python app.py                 ->  http://127.0.0.1:5000

Export a static index.html (deploy anywhere, no server needed):
    python app.py --build

BEFORE GOING LIVE
-----------------
Replace FORM_ENDPOINT below with your real endpoint:
  * Web3Forms  -> https://api.web3forms.com/submit   (also set WEB3FORMS_KEY)
  * Formspree  -> https://formspree.io/f/xxxxxxxx
Both are free and need no backend. The form posts via fetch() and shows a
success banner without reloading the page.
"""

import sys
from flask import Flask, render_template_string

app = Flask(__name__)

# ---------------------------------------------------------------------------
# FORM SETUP — swap these two values and the form is live
# ---------------------------------------------------------------------------

FORM_ENDPOINT = "https://api.web3forms.com/submit"   # e.g. https://api.web3forms.com/submit
WEB3FORMS_KEY = "96430f85-b5d0-4c6e-947f-aec55cb516b6"      # only needed for Web3Forms

# ---------------------------------------------------------------------------
# CONTENT — all copy lives here, so edits never touch markup
# ---------------------------------------------------------------------------

SITE = {
    "brand": "Pr Hubb",
    "brand_tagline": "PR Consultancy Agency",
    "title": "Pr Hubb | PR Consultancy Agency",
    "meta_description": (
        "Pr Hubb — strategic public relations and purposeful storytelling. "
        "Media relations, crisis management, reputation management and integrated marketing."
    ),
    "cta": "Let's build your visibility",
    "footer": "© Pr Hubb – PR Consultancy Agency. Communication with credibility and purpose.",
}

NAV = [
    {"label": "Services", "href": "#services"},
    {"label": "About us", "href": "#about"},
    {"label": "Our vision", "href": "#vision"},
    {"label": "Let's talk", "href": "#contact"},
]

HERO = {
    "eyebrow": "Strategic Public Relations",
    "headline_a": "Make your story matter.",
    "headline_b": "Build your reputation.",
    "subheadline": (
        "We help brands earn attention, build credibility and communicate with confidence "
        "through strategic public relations and purposeful storytelling."
    ),
    "support_label": "Communication with purpose",
    "support_text": (
        "From media relations to reputation management, we help your brand connect "
        "with the people who matter."
    ),
}

SERVICES_INTRO = {
    "headline_a": "Build influence.",
    "headline_b": "Protect your reputation.",
    "subtext": (
        "Thoughtful communication strategies that help your organisation stand out, "
        "earn trust and grow lasting relationships."
    ),
}

# Each icon is a 24x24 stroke glyph that reads at a glance.
ICONS = {
    "media": '<path d="M3 11l18-5v12L3 14v-3z"/><path d="M11.6 16.8a3 3 0 11-5.8-1.6"/>',
    "crisis": '<path d="M12 9v4"/><path d="M12 17h.01"/>'
              '<path d="M10.29 3.86L1.82 18a2 2 0 001.71 3h16.94a2 2 0 001.71-3L13.71 3.86a2 2 0 00-3.42 0z"/>',
    "reputation": '<path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/><path d="M9 12l2 2 4-4"/>',
    "research": '<circle cx="11" cy="11" r="8"/><path d="M21 21l-4.35-4.35"/><path d="M8 11h6"/><path d="M11 8v6"/>',
    "integrated": '<circle cx="18" cy="5" r="3"/><circle cx="6" cy="12" r="3"/><circle cx="18" cy="19" r="3"/>'
                  '<path d="M8.59 13.51l6.83 3.98"/><path d="M15.41 6.51L8.59 10.49"/>',
    "branding": '<path d="M12 2l2.9 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l7.1-1.01L12 2z"/>',
    "thought": '<path d="M9 18h6"/><path d="M10 22h4"/>'
               '<path d="M15.09 14c.18-.98.65-1.74 1.41-2.5A4.65 4.65 0 0018 8 6 6 0 006 8c0 1 .23 2.23 1.5 3.5.76.76 1.23 1.52 1.41 2.5"/>',
}

SERVICES = [
    {
        "icon": "media",
        "name": "Media Relations",
        "description": "Build meaningful media relationships, shape compelling stories and earn "
                       "visibility through strategic media engagement.",
    },
    {
        "icon": "crisis",
        "name": "Crisis Management",
        "description": "Navigate challenging moments with clear communication, timely response "
                       "and a considered plan.",
    },
    {
        "icon": "reputation",
        "name": "Reputation Management",
        "description": "Strengthen public trust and safeguard the credibility of your brand "
                       "and organisation.",
    },
    {
        "icon": "research",
        "name": "Market Research",
        "description": "Understand audiences, uncover insights and make informed "
                       "communication decisions.",
    },
    {
        "icon": "integrated",
        "name": "Integrated Marketing",
        "description": "Bring communication channels together for a consistent and memorable "
                       "brand experience.",
    },
    {
        "icon": "branding",
        "name": "Branding &amp; Strategic Positioning",
        "description": "Clarify what makes you different and position your brand to connect "
                       "with the right audience.",
    },
    {
        "icon": "thought",
        "name": "Thought Leadership",
        "description": "Develop authoritative voices and share ideas that inspire confidence "
                       "and shape conversations.",
    },
]

DIRECTION = {
    "headline": "Guided by purpose. Driven by trust.",
    "mission_label": "Our mission",
    "mission": "Build your brand awareness and visibility with credibility and authority.",
    "vision_label": "Our vision",
    "vision": (
        "To be a trusted leader in strategic communication, recognized for shaping "
        "narratives that inspire confidence and credibility."
    ),
}

ABOUT = {
    "headline_a": "Credibility is built.",
    "headline_b": "Not claimed.",
    "paragraphs": [
        "At Pr Hubb, we believe every brand has a story worth telling. Our work is centred on "
        "strategic communication that builds awareness, strengthens relationships and supports "
        "lasting credibility.",
        "We partner with organisations to communicate clearly, engage meaningfully and navigate "
        "the moments that shape public perception.",
    ],
    "promise_headline": "Visibility with substance.",
    "promise_body": (
        "We bring strategy, storytelling and relationship-building together to help your brand "
        "communicate with purpose and earn the confidence of its audiences."
    ),
}

CONTACT = {
    "headline": "Let's tell your story.",
    "subtext": (
        "Have a communication challenge or a brand you want to grow? Reach out to discuss "
        "how we can support your goals."
    ),
    "email": "info.prhubke@gmail.com",
    "phone": "+254 743 970 200",
    "phone_href": "+254743970200",
    "website": "www.prhubbke.co.ke",
    "address": "P.O. Box 50769-00100, Nairobi, Kenya",
    "button": "Send inquiry",
    "helper": "We usually reply within one business day.",
}

# ---------------------------------------------------------------------------
# TEMPLATE
# ---------------------------------------------------------------------------

TEMPLATE = r"""<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>{{ site.title }}</title>
<meta name="description" content="{{ site.meta_description }}">
<meta name="theme-color" content="#0A1024">

<script src="https://cdn.tailwindcss.com"></script>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Sora:wght@400;500;600;700&family=Inter:wght@400;500;600&display=swap" rel="stylesheet">

<script>
  tailwind.config = {
    theme: {
      extend: {
        colors: {
          midnight: { 950:'#060B1A', 900:'#0A1024', 800:'#111A33', 700:'#1B2745' },
          slate2:   { 500:'#64748B', 400:'#94A3B8', 300:'#CBD5E1' },
          emerald2: { 400:'#34D399', 500:'#10B981', 600:'#059669' },
          bone:     '#F7F8FA',
        },
        fontFamily: {
          display: ['Sora', 'system-ui', 'sans-serif'],
          sans: ['Inter', 'system-ui', 'sans-serif'],
        },
      },
    },
  };
</script>

<style>
  html { scroll-behavior: smooth; }
  body { font-family:'Inter', system-ui, sans-serif; color:#111A33; background:#fff; }
  .font-display { font-family:'Sora', system-ui, sans-serif; letter-spacing:-0.025em; }
  ::selection { background:#10B981; color:#fff; }

  a:focus-visible, button:focus-visible, input:focus-visible, textarea:focus-visible {
    outline:2px solid #10B981; outline-offset:3px; border-radius:2px;
  }

  /* ---------- glassmorphic nav ---------- */
  #nav {
    background: rgba(255,255,255,.62);
    backdrop-filter: blur(14px) saturate(180%);
    -webkit-backdrop-filter: blur(14px) saturate(180%);
    border-bottom: 1px solid rgba(17,26,51,.06);
    transition: background .4s ease, box-shadow .4s ease, border-color .4s ease;
  }
  #nav.scrolled {
    background: rgba(255,255,255,.82);
    box-shadow: 0 8px 32px -12px rgba(10,16,36,.16);
    border-bottom-color: rgba(17,26,51,.09);
  }

  /* ---------- accent glow ---------- */
  .glow { position:absolute; border-radius:9999px; filter:blur(90px); pointer-events:none; }
  .glow-a { width:520px; height:520px; background:rgba(16,185,129,.16); top:-140px; right:-120px; }
  .glow-b { width:420px; height:420px; background:rgba(27,39,69,.10);  top:180px;  left:-180px; }

  /* ---------- buttons ---------- */
  .btn {
    display:inline-flex; align-items:center; justify-content:center; gap:.5rem;
    font-weight:500; border-radius:9999px;
    transition: transform .3s cubic-bezier(.22,1,.36,1), box-shadow .3s ease, background-color .3s ease, color .3s ease, border-color .3s ease;
  }
  .btn-primary { background:#0A1024; color:#fff; box-shadow:0 8px 20px -10px rgba(10,16,36,.7); }
  .btn-primary:hover { transform:translateY(-2px); background:#111A33; box-shadow:0 16px 30px -12px rgba(10,16,36,.6); }
  .btn-accent { background:#10B981; color:#04231A; box-shadow:0 8px 24px -10px rgba(16,185,129,.8); }
  .btn-accent:hover { transform:translateY(-2px); background:#34D399; box-shadow:0 18px 34px -12px rgba(16,185,129,.7); }
  .btn-ghost { background:rgba(255,255,255,.08); color:#fff; border:1px solid rgba(255,255,255,.22); }
  .btn-ghost:hover { transform:translateY(-2px); background:rgba(255,255,255,.14); }
  .btn-outline { color:#0A1024; border:1px solid rgba(10,16,36,.15); }
  .btn-outline:hover { transform:translateY(-2px); border-color:rgba(10,16,36,.4); }
  .btn .arrow { transition: transform .3s ease; }
  .btn:hover .arrow { transform: translateX(3px); }

  /* ---------- cards ---------- */
  .card {
    position:relative; background:#fff; border:1px solid rgba(17,26,51,.08); border-radius:18px;
    transition: transform .4s cubic-bezier(.22,1,.36,1), box-shadow .4s ease, border-color .4s ease;
  }
  .card-hover::before {
    content:''; position:absolute; inset:0; border-radius:18px; opacity:0;
    background: linear-gradient(160deg, rgba(16,185,129,.07), transparent 55%);
    transition: opacity .4s ease; pointer-events:none;
  }
  .card-hover:hover { transform:translateY(-6px); box-shadow:0 24px 44px -24px rgba(10,16,36,.35); border-color:rgba(16,185,129,.35); }
  .card-hover:hover::before { opacity:1; }
  .card-icon {
    width:52px; height:52px; border-radius:14px; display:grid; place-items:center;
    background:#F1F5F9; color:#1B2745;
    transition: background .4s ease, color .4s ease, transform .4s cubic-bezier(.22,1,.36,1);
  }
  .card-hover:hover .card-icon { background:#0A1024; color:#34D399; transform:scale(1.06) rotate(-3deg); }

  /* ---------- dividers ---------- */
  .divider { height:1px; background:linear-gradient(90deg, transparent, rgba(17,26,51,.14), transparent); }
  .divider-dot { display:grid; place-items:center; }
  .divider-dot span { display:block; width:6px; height:6px; border-radius:9999px; background:#10B981; box-shadow:0 0 0 6px rgba(16,185,129,.12); }

  /* ---------- reveal ---------- */
  .reveal { opacity:0; transform:translateY(22px); transition:opacity .8s ease, transform .8s cubic-bezier(.22,1,.36,1); }
  .reveal.in { opacity:1; transform:none; }

  @keyframes riseIn { from{opacity:0; transform:translateY(20px);} to{opacity:1; transform:none;} }
  .hero-rise > * { animation: riseIn .9s cubic-bezier(.22,1,.36,1) both; }
  .hero-rise > *:nth-child(1){animation-delay:.05s}
  .hero-rise > *:nth-child(2){animation-delay:.18s}
  .hero-rise > *:nth-child(3){animation-delay:.31s}
  .hero-rise > *:nth-child(4){animation-delay:.44s}

  /* ---------- nav underline ---------- */
  .nav-link { position:relative; }
  .nav-link::after {
    content:''; position:absolute; left:0; bottom:-5px; width:0; height:2px;
    background:#10B981; border-radius:2px; transition:width .3s ease;
  }
  .nav-link:hover::after { width:100%; }

  /* ---------- form fields ---------- */
  .field {
    width:100%; background:rgba(255,255,255,.05); color:#fff;
    border:1px solid rgba(255,255,255,.16); border-radius:12px;
    padding:.85rem 1rem; font-size:16px;
    transition: border-color .3s ease, background .3s ease, box-shadow .3s ease;
  }
  .field::placeholder { color:rgba(255,255,255,.34); }
  .field:focus {
    outline:none; border-color:#10B981; background:rgba(255,255,255,.08);
    box-shadow:0 0 0 4px rgba(16,185,129,.14);
  }

  /* ---------- toast ---------- */
  #toast {
    position:fixed; left:50%; bottom:1.5rem; transform:translate(-50%, 150%);
    z-index:80; width:calc(100% - 2rem); max-width:26rem;
    transition: transform .55s cubic-bezier(.22,1,.36,1), opacity .4s ease;
    opacity:0;
  }
  #toast.show { transform:translate(-50%, 0); opacity:1; }

  @media (prefers-reduced-motion: reduce) {
    html { scroll-behavior:auto; }
    *, *::before, *::after { animation:none !important; transition:none !important; }
    .reveal { opacity:1 !important; transform:none !important; }
  }
</style>
</head>

<body class="antialiased">

<!-- ======================= NAV ======================= -->
<header id="nav" class="fixed top-0 inset-x-0 z-50">
  <div class="max-w-7xl mx-auto px-5 sm:px-6 lg:px-10">
    <div class="flex items-center justify-between h-[72px]">
      <a href="#top" class="flex items-baseline gap-2.5">
        <span class="font-display text-[1.35rem] font-bold text-midnight-900">{{ site.brand }}</span>
        <span class="hidden sm:inline text-[11px] font-medium text-slate2-500">{{ site.brand_tagline }}</span>
      </a>

      <nav class="hidden md:flex items-center gap-9 text-[15px] font-medium text-midnight-800/85">
        {% for item in nav %}<a href="{{ item.href }}" class="nav-link">{{ item.label }}</a>{% endfor %}
      </nav>

      <a href="#contact" class="btn btn-primary hidden md:inline-flex text-[14px] px-5 py-2.5">
        {{ site.cta }} <span class="arrow" aria-hidden="true">&rarr;</span>
      </a>

      <button id="menuBtn" class="md:hidden p-2 -mr-2 text-midnight-900" aria-label="Open menu" aria-expanded="false" aria-controls="mobileMenu">
        <svg id="iconOpen" class="w-6 h-6" fill="none" stroke="currentColor" stroke-width="1.75" viewBox="0 0 24 24"><path stroke-linecap="round" d="M4 7h16M4 12h16M4 17h16"/></svg>
        <svg id="iconClose" class="w-6 h-6 hidden" fill="none" stroke="currentColor" stroke-width="1.75" viewBox="0 0 24 24"><path stroke-linecap="round" d="M6 18L18 6M6 6l12 12"/></svg>
      </button>
    </div>
  </div>

  <div id="mobileMenu" class="md:hidden hidden border-t border-midnight-900/10 bg-white/95 backdrop-blur-xl">
    <nav class="flex flex-col px-5 py-4 gap-1 text-[16px]">
      {% for item in nav %}<a href="{{ item.href }}" class="py-3 border-b border-midnight-900/5">{{ item.label }}</a>{% endfor %}
      <a href="#contact" class="btn btn-primary mt-4 w-full px-5 py-3.5 text-[15px]">
        {{ site.cta }} <span class="arrow" aria-hidden="true">&rarr;</span>
      </a>
    </nav>
  </div>
</header>

<!-- ======================= HERO ======================= -->
<section id="top" class="relative overflow-hidden pt-32 pb-20 md:pt-44 md:pb-28 px-5 sm:px-6 lg:px-10 bg-white">
  <div class="glow glow-a"></div>
  <div class="glow glow-b"></div>

  <div class="relative max-w-7xl mx-auto">
    <div class="hero-rise max-w-3xl">
      <p class="inline-flex items-center gap-2 text-[13px] font-medium text-emerald2-600 bg-emerald2-500/10 border border-emerald2-500/20 rounded-full px-3.5 py-1.5">
        <span class="w-1.5 h-1.5 rounded-full bg-emerald2-500"></span>{{ hero.eyebrow }}
      </p>
      <h1 class="font-display mt-7 text-[2.5rem] leading-[1.06] sm:text-6xl md:text-[4.4rem] md:leading-[1.03] font-bold text-midnight-900">
        {{ hero.headline_a }}<br class="hidden sm:block"> {{ hero.headline_b }}
      </h1>
      <p class="mt-7 text-[17px] md:text-xl text-slate2-500 max-w-xl leading-relaxed">{{ hero.subheadline }}</p>
      <div class="mt-10 flex flex-col sm:flex-row sm:items-center gap-4">
        <a href="#contact" class="btn btn-accent px-7 py-3.5 text-[15px] w-full sm:w-auto">
          {{ site.cta }} <span class="arrow" aria-hidden="true">&rarr;</span>
        </a>
        <a href="#services" class="btn btn-outline px-7 py-3.5 text-[15px] w-full sm:w-auto">
          See what we do
        </a>
      </div>
    </div>

    <div class="mt-20 md:mt-24">
      <div class="divider"></div>
      <div class="grid md:grid-cols-[220px_1fr] gap-5 md:gap-12 pt-8">
        <p class="text-[13px] font-medium text-emerald2-600">{{ hero.support_label }}</p>
        <p class="text-[17px] md:text-lg text-slate2-500 leading-relaxed max-w-2xl">{{ hero.support_text }}</p>
      </div>
    </div>
  </div>
</section>

<!-- ======================= SERVICES ======================= -->
<section id="services" class="px-5 sm:px-6 lg:px-10 py-20 md:py-28 bg-bone border-y border-midnight-900/[0.06]">
  <div class="max-w-7xl mx-auto">
    <div class="reveal grid md:grid-cols-[1fr_1.05fr] gap-8 md:gap-16 mb-14 md:mb-16">
      <h2 class="font-display text-[2rem] sm:text-4xl md:text-[2.9rem] leading-[1.12] font-bold text-midnight-900">
        {{ services_intro.headline_a }}<br>{{ services_intro.headline_b }}
      </h2>
      <p class="text-[17px] md:text-lg text-slate2-500 leading-relaxed self-end max-w-xl">{{ services_intro.subtext }}</p>
    </div>

    <div class="reveal grid sm:grid-cols-2 lg:grid-cols-3 gap-5 md:gap-6">
      {% for s in services %}
      <article class="card card-hover p-7 md:p-8">
        <div class="card-icon">
          <svg class="w-6 h-6" fill="none" stroke="currentColor" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24" aria-hidden="true">{{ icons[s.icon]|safe }}</svg>
        </div>
        <h3 class="font-display mt-6 text-[1.2rem] font-semibold text-midnight-900 leading-snug">{{ s.name|safe }}</h3>
        <p class="mt-3 text-[15px] leading-relaxed text-slate2-500">{{ s.description }}</p>
      </article>
      {% endfor %}

      <!-- closing tile balances the 7-item grid -->
      <article class="card p-7 md:p-8 bg-midnight-900 border-midnight-900 flex flex-col justify-between">
        <div>
          <h3 class="font-display text-[1.2rem] font-semibold text-white leading-snug">Not sure where to start?</h3>
          <p class="mt-3 text-[15px] leading-relaxed text-slate2-400">Tell us what you're working on and we'll suggest the right mix.</p>
        </div>
        <a href="#contact" class="btn btn-ghost mt-7 px-5 py-3 text-[14px] self-start">
          Talk to us <span class="arrow" aria-hidden="true">&rarr;</span>
        </a>
      </article>
    </div>
  </div>
</section>

<!-- ======================= MISSION & VISION ======================= -->
<section id="vision" class="px-5 sm:px-6 lg:px-10 pt-20 md:pt-28 pb-14 md:pb-20 bg-white">
  <div class="max-w-7xl mx-auto reveal">
    <h2 class="font-display text-[2rem] sm:text-4xl md:text-5xl font-bold text-midnight-900 max-w-2xl leading-[1.12] mb-12 md:mb-16">
      {{ direction.headline }}
    </h2>

    <div class="grid md:grid-cols-2 gap-5 md:gap-6">
      <div class="card card-hover p-8 md:p-10 bg-midnight-900 border-midnight-900">
        <p class="text-[13px] font-medium text-emerald2-400">{{ direction.mission_label }}</p>
        <p class="font-display mt-5 text-[1.5rem] md:text-[1.9rem] leading-snug font-semibold text-white">{{ direction.mission }}</p>
      </div>
      <div class="card card-hover p-8 md:p-10">
        <p class="text-[13px] font-medium text-emerald2-600">{{ direction.vision_label }}</p>
        <p class="font-display mt-5 text-[1.5rem] md:text-[1.9rem] leading-snug font-semibold text-midnight-900">{{ direction.vision }}</p>
      </div>
    </div>
  </div>
</section>

<!-- elegant break between vision and about -->
<div class="px-5 sm:px-6 lg:px-10 bg-white">
  <div class="max-w-7xl mx-auto divider-dot"><span></span></div>
</div>

<!-- ======================= ABOUT ======================= -->
<section id="about" class="px-5 sm:px-6 lg:px-10 pt-14 md:pt-20 pb-20 md:pb-28 bg-white">
  <div class="max-w-7xl mx-auto reveal">
    <div class="grid md:grid-cols-[0.85fr_1.15fr] gap-10 md:gap-20">
      <h2 class="font-display text-[2rem] sm:text-4xl md:text-5xl font-bold text-midnight-900 leading-[1.12]">
        {{ about.headline_a }}<br>{{ about.headline_b }}
      </h2>

      <div class="max-w-2xl">
        <div class="space-y-5 text-[17px] leading-[1.75] text-slate2-500">
          {% for para in about.paragraphs %}<p>{{ para }}</p>{% endfor %}
        </div>

        <div class="card card-hover mt-10 p-7 md:p-8 bg-bone">
          <h3 class="font-display text-[1.25rem] font-semibold text-midnight-900">{{ about.promise_headline }}</h3>
          <p class="mt-3 text-[16px] leading-relaxed text-slate2-500">{{ about.promise_body }}</p>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ======================= CONTACT ======================= -->
<section id="contact" class="relative overflow-hidden px-5 sm:px-6 lg:px-10 py-20 md:py-28 bg-midnight-900 text-white">
  <div class="glow" style="width:480px;height:480px;background:rgba(16,185,129,.14);bottom:-160px;left:-120px;"></div>

  <div class="relative max-w-7xl mx-auto">
    <div class="grid lg:grid-cols-[1fr_1.1fr] gap-12 lg:gap-20">

      <!-- left: heading + direct gateways -->
      <div>
        <h2 class="font-display text-[2rem] sm:text-4xl md:text-5xl font-bold leading-[1.12] mb-5">{{ contact.headline }}</h2>
        <p class="text-[17px] text-slate2-400 leading-relaxed max-w-md mb-10">{{ contact.subtext }}</p>

        <!-- tap to call / tap to email -->
        <div class="grid sm:grid-cols-2 gap-4 mb-10">
          <a href="tel:{{ contact.phone_href }}" class="card card-hover p-5 bg-white/[0.06] border-white/[0.14] flex items-center gap-4">
            <span class="w-11 h-11 rounded-xl grid place-items-center bg-emerald2-500/15 text-emerald2-400 shrink-0">
              <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="1.7" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><path d="M22 16.92v3a2 2 0 01-2.18 2 19.79 19.79 0 01-8.63-3.07 19.5 19.5 0 01-6-6A19.79 19.79 0 012.12 4.18 2 2 0 014.11 2h3a2 2 0 012 1.72c.13.96.36 1.9.7 2.81a2 2 0 01-.45 2.11L8.09 9.91a16 16 0 006 6l1.27-1.27a2 2 0 012.11-.45c.9.34 1.85.57 2.81.7A2 2 0 0122 16.92z"/></svg>
            </span>
            <span class="min-w-0">
              <span class="block text-[12px] text-slate2-400">Call us</span>
              <span class="block text-[15px] font-medium">{{ contact.phone }}</span>
            </span>
          </a>

          <a href="mailto:{{ contact.email }}" class="card card-hover p-5 bg-white/[0.06] border-white/[0.14] flex items-center gap-4">
            <span class="w-11 h-11 rounded-xl grid place-items-center bg-emerald2-500/15 text-emerald2-400 shrink-0">
              <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="1.7" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><rect x="2" y="4" width="20" height="16" rx="2"/><path d="M22 6l-10 7L2 6"/></svg>
            </span>
            <span class="min-w-0">
              <span class="block text-[12px] text-slate2-400">Email us</span>
              <span class="block text-[15px] font-medium truncate">{{ contact.email }}</span>
            </span>
          </a>
        </div>

        <dl class="space-y-4 text-[15px] border-t border-white/10 pt-8">
          <div class="flex gap-4">
            <dt class="text-slate2-400 w-24 shrink-0">Website</dt>
            <dd>{{ contact.website }}</dd>
          </div>
          <div class="flex gap-4">
            <dt class="text-slate2-400 w-24 shrink-0">Address</dt>
            <dd>{{ contact.address }}</dd>
          </div>
        </dl>
      </div>

      <!-- right: working form -->
      <div class="card p-6 sm:p-8 md:p-9 bg-white/[0.05] border-white/[0.14]">
        <form id="inquiryForm" action="{{ form_endpoint }}" method="POST" class="space-y-5">
          <!-- Web3Forms access key. Formspree users can delete this line. -->
          <input type="hidden" name="access_key" value="{{ web3forms_key }}">
          <input type="hidden" name="subject" value="New inquiry from the Pr Hubb website">
          <!-- honeypot: bots fill this in, people never see it -->
          <input type="checkbox" name="botcheck" style="display:none" tabindex="-1" aria-hidden="true">

          <div>
            <label for="name" class="block text-[13px] text-slate2-400 mb-2">Your name</label>
            <input class="field" type="text" id="name" name="name" required autocomplete="name" placeholder="Jane Wanjiru">
          </div>
          <div>
            <label for="email" class="block text-[13px] text-slate2-400 mb-2">Email address</label>
            <input class="field" type="email" id="email" name="email" required autocomplete="email" placeholder="jane@company.com">
          </div>
          <div>
            <label for="message" class="block text-[13px] text-slate2-400 mb-2">How can we help?</label>
            <textarea class="field resize-none" id="message" name="message" rows="5" required
              placeholder="Tell us a little about your brand and what you're working on."></textarea>
          </div>

          <div class="pt-1">
            <button id="submitBtn" type="submit" class="btn btn-accent w-full sm:w-auto px-7 py-3.5 text-[15px]">
              <span id="btnLabel">{{ contact.button }}</span>
              <span class="arrow" aria-hidden="true">&rarr;</span>
            </button>
            <p class="mt-4 text-[13px] text-slate2-400">{{ contact.helper }}</p>
          </div>
        </form>
      </div>
    </div>
  </div>
</section>

<!-- ======================= FOOTER ======================= -->
<footer class="px-5 sm:px-6 lg:px-10 py-9 bg-midnight-950 text-slate2-400">
  <div class="max-w-7xl mx-auto flex flex-col sm:flex-row items-center justify-between gap-3 text-[13px] text-center sm:text-left">
    <p>{{ site.footer }}</p>
    <p class="text-slate2-500">Nairobi, Kenya</p>
  </div>
</footer>

<!-- ======================= TOAST ======================= -->
<div id="toast" role="status" aria-live="polite">
  <div class="flex items-center gap-3.5 bg-white rounded-2xl pl-5 pr-6 py-4 shadow-[0_24px_60px_-20px_rgba(10,16,36,.55)] border border-midnight-900/[0.07]">
    <span id="toastIcon" class="w-9 h-9 rounded-full grid place-items-center bg-emerald2-500/10 text-emerald2-600 shrink-0">
      <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><path d="M20 6L9 17l-5-5"/></svg>
    </span>
    <p id="toastText" class="text-[15px] font-medium text-midnight-900">Message sent! We will get back to you shortly.</p>
  </div>
</div>

<script>
(function () {
  'use strict';

  /* ---------- glassmorphic nav state ---------- */
  var nav = document.getElementById('nav');
  var onScroll = function () { nav.classList.toggle('scrolled', window.scrollY > 12); };
  window.addEventListener('scroll', onScroll, { passive: true });
  onScroll();

  /* ---------- mobile menu ---------- */
  var menuBtn = document.getElementById('menuBtn');
  var mobileMenu = document.getElementById('mobileMenu');
  var iconOpen = document.getElementById('iconOpen');
  var iconClose = document.getElementById('iconClose');

  function closeMenu() {
    mobileMenu.classList.add('hidden');
    iconOpen.classList.remove('hidden');
    iconClose.classList.add('hidden');
    menuBtn.setAttribute('aria-expanded', 'false');
  }

  menuBtn.addEventListener('click', function () {
    var willOpen = mobileMenu.classList.contains('hidden');
    mobileMenu.classList.toggle('hidden', !willOpen);
    iconOpen.classList.toggle('hidden', willOpen);
    iconClose.classList.toggle('hidden', !willOpen);
    menuBtn.setAttribute('aria-expanded', willOpen ? 'true' : 'false');
  });

  mobileMenu.querySelectorAll('a').forEach(function (link) {
    link.addEventListener('click', closeMenu);
  });

  /* ---------- smooth scroll, offset for the fixed nav ---------- */
  var reduceMotion = window.matchMedia('(prefers-reduced-motion: reduce)').matches;
  document.querySelectorAll('a[href^="#"]').forEach(function (link) {
    link.addEventListener('click', function (e) {
      var id = link.getAttribute('href');
      if (id === '#') return;
      var target = document.querySelector(id);
      if (!target) return;
      e.preventDefault();
      closeMenu();
      var top = target.getBoundingClientRect().top + window.scrollY - 72;
      window.scrollTo({ top: top, behavior: reduceMotion ? 'auto' : 'smooth' });
      history.replaceState(null, '', id);
    });
  });

  /* ---------- one gentle reveal per section ---------- */
  if ('IntersectionObserver' in window && !reduceMotion) {
    var io = new IntersectionObserver(function (entries) {
      entries.forEach(function (entry) {
        if (entry.isIntersecting) { entry.target.classList.add('in'); io.unobserve(entry.target); }
      });
    }, { threshold: 0.1, rootMargin: '0px 0px -60px 0px' });
    document.querySelectorAll('.reveal').forEach(function (el) { io.observe(el); });
  } else {
    document.querySelectorAll('.reveal').forEach(function (el) { el.classList.add('in'); });
  }

  /* ---------- toast banner ---------- */
  var toast = document.getElementById('toast');
  var toastText = document.getElementById('toastText');
  var toastIcon = document.getElementById('toastIcon');
  var toastTimer;

  function showToast(message, ok) {
    toastText.textContent = message;
    toastIcon.className = ok
      ? 'w-9 h-9 rounded-full grid place-items-center bg-emerald2-500/10 text-emerald2-600 shrink-0'
      : 'w-9 h-9 rounded-full grid place-items-center bg-amber-500/10 text-amber-600 shrink-0';
    toast.classList.add('show');
    clearTimeout(toastTimer);
    toastTimer = setTimeout(function () { toast.classList.remove('show'); }, 5200);
  }

  /* ---------- form submit, no page reload ---------- */
  var form = document.getElementById('inquiryForm');
  var submitBtn = document.getElementById('submitBtn');
  var btnLabel = document.getElementById('btnLabel');
  var originalLabel = btnLabel.textContent;

  form.addEventListener('submit', function (e) {
    e.preventDefault();
    if (!form.reportValidity()) return;

    var endpoint = form.getAttribute('action');

    /* Endpoint not configured yet: fall back to the visitor's email client
       so no inquiry is lost while the site is being set up. */
    if (!endpoint || endpoint.indexOf('YOUR_FORM_ENDPOINT') === 0) {
      var name = document.getElementById('name').value.trim();
      var email = document.getElementById('email').value.trim();
      var message = document.getElementById('message').value.trim();
      var subject = encodeURIComponent('New inquiry from ' + name);
      var body = encodeURIComponent('Name: ' + name + '\nEmail: ' + email + '\n\nMessage:\n' + message);
      showToast('Opening your email app to send this inquiry.', true);
      window.location.href = 'mailto:{{ contact.email }}?subject=' + subject + '&body=' + body;
      return;
    }

    submitBtn.disabled = true;
    submitBtn.style.opacity = '.72';
    btnLabel.textContent = 'Sending';

    fetch(endpoint, {
      method: 'POST',
      body: new FormData(form),
      headers: { 'Accept': 'application/json' }
    })
      .then(function (res) {
        if (!res.ok) throw new Error('Request failed');
        showToast('Message sent! We will get back to you shortly.', true);
        form.reset();
      })
      .catch(function () {
        showToast('That did not send. Please email us at {{ contact.email }}.', false);
      })
      .then(function () {
        submitBtn.disabled = false;
        submitBtn.style.opacity = '';
        btnLabel.textContent = originalLabel;
      });
  });
})();
</script>

</body>
</html>
"""

CONTEXT = dict(
    site=SITE,
    nav=NAV,
    hero=HERO,
    services_intro=SERVICES_INTRO,
    services=SERVICES,
    icons=ICONS,
    direction=DIRECTION,
    about=ABOUT,
    contact=CONTACT,
    form_endpoint=FORM_ENDPOINT,
    web3forms_key=WEB3FORMS_KEY,
)

# ---------------------------------------------------------------------------
# ROUTES / BUILD
# ---------------------------------------------------------------------------


@app.route("/")
def home():
    return render_template_string(TEMPLATE, **CONTEXT)


def build(path="index.html"):
    with app.app_context():
        html = render_template_string(TEMPLATE, **CONTEXT)
    with open(path, "w", encoding="utf-8") as f:
        f.write(html)
    print(f"Wrote {path} ({len(html):,} bytes)")


if __name__ == "__main__":
    if "--build" in sys.argv:
        build()
    else:
        app.run(debug=True, port=5000)
