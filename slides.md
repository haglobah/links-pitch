---
theme: default
title: Links—your links in one inbox
info: Demo day deck for links.humane.tools
colorSchema: light
transition: slide-left
fonts:
  sans: League Spartan
  mono: IBM Plex Mono
  weights: '400,500,600,700'
class: cover
layout: iframe
url: https://humane.tools/links
---

---
class: problems
clicks: 19
---

<!-- Clicks 1–3 reveal column one; 4 adds column two, 5–7 its items; 8 pans to column three; 9–15 build its first item (each tool, then its strikethrough, then the inbox), 16–17 its other items; 18 zooms out to all three; 19 zooms into column one for the demo, lighting the want being demoed. -->
<div class="pan">
  <div class="pan-track" :data-stage="$clicks >= 19 ? 4 : $clicks >= 18 ? 3 : $clicks >= 8 ? 2 : $clicks >= 4 ? 1 : 0">
    <div class="pan-col">
      <div class="col-head">
        <h3>Things I want to do</h3>
        <p class="demo-label">Demo</p>
      </div>
      <div v-click="1" class="problem">
        <span class="kicker !text-xl">1</span>
        <h1 class="!text-3xl">I want to read something</h1>
      </div>
      <div v-click="2" class="problem current">
        <span class="kicker !text-xl">2</span>
        <h1 class="!text-3xl">I want to share links during a conversation</h1>
      </div>
      <div v-click="3" class="problem">
        <span class="kicker !text-xl">3</span>
        <h1 class="!text-3xl">I want to read something, but later</h1>
      </div>
    </div>
    <div class="pan-col">
      <h3>Problems</h3>
      <div v-click="5" class="problem">
        <span class="kicker !text-xl">1</span>
        <h1 class="!text-3xl">Links live across all my messengers</h1>
      </div>
      <div v-click="6" class="problem">
        <span class="kicker !text-xl">2</span>
        <h1 class="!text-3xl">Finding links again I want to send to people is hard</h1>
      </div>
      <div v-click="7" class="problem">
        <span class="kicker !text-xl">3</span>
        <h1 class="!text-3xl">Saving links somewhere is (kinda) hard?</h1>
      </div>
    </div>
    <div class="pan-col">
      <h3>Solution shapes</h3>
      <div v-click="9" class="problem">
        <span class="kicker !text-xl">1</span>
        <h1 class="!text-3xl"><span class="strike" :class="{ struck: $clicks >= 10 }">Browser History</span><span v-click="11">, <span class="strike" :class="{ struck: $clicks >= 12 }">Bookmarks</span></span><span v-click="13">, <span class="strike" :class="{ struck: $clicks >= 14 }">Obsidian</span></span> <span v-click="15">→ One inbox</span></h1>
      </div>
      <div v-click="16" class="problem">
        <span class="kicker !text-xl">2</span>
        <h1 class="!text-3xl">Really good search and sorting over this inbox</h1>
      </div>
      <div v-click="17" class="problem">
        <span class="kicker !text-xl">3</span>
        <h1 class="!text-3xl">Capturing should be no more frictionful than closing a tab</h1>
      </div>
    </div>
  </div>
</div>

---

<div class="outro">
  <div class="card">
    <div class="card-text">
      <img src="/icon.svg" alt="" class="card-icon" />
      <h1>Links</h1>
      <p class="url">links.humane.tools</p>
      <img src="/qr-links.png" alt="QR code for links.humane.tools" class="qr-img" />
    </div>
    <div class="phone"><img src="/links-phone.png" alt="The Links inbox on a phone" /></div>
  </div>
  <div class="card">
    <div class="card-text">
      <img src="/ht-icon.svg" alt="" class="card-icon" />
      <h1>Humane Tools</h1>
      <p class="url">humane.tools</p>
      <img src="/qr-humane.png" alt="QR code for humane.tools" class="qr-img" />
    </div>
    <div class="phone"><img src="/humane-phone.png" alt="humane.tools on a phone" /></div>
  </div>
  <div class="maker">
    <img src="/beat.jpg" class="portrait" alt="Beat Hagenlocher" />
    <p class="url">beathagenlocher.com</p>
    <img src="/qr-beat.png" alt="QR code for beathagenlocher.com" class="qr-img" />
  </div>
</div>
