# 📅 [Kalendrirakendus Kalendar]

[![GitHub](https://img.shields.io/badge/GitHub-Tefix%2Fkaledar-blue?logo=github)](https://github.com/Tefix/kalendar)
[![Litsents](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Viimane kommit](https://img.shields.io/github/last-commit/Tefix/kalendar)](https://github.com/Tefix/kalendar/commits/)

**[Lühike projekti kirjeldus: interaktiivne kalendrirakendus sündmuste ja ajakavas haldamiseks]**

---

## 📑 Sisukord

- [Projekti kirjeldus](#-projekti-kirjeldus)
- [Mis oli realiseeritud](#-mis-oli-realiseeritud)
- [Kasutatavad tehnoloogiad](#-kasutatavad-tehnoloogiad)
- [Projekti struktuur](#-projekti-struktuur)
- [Käivitamise juhend](#-käivitamise-juhend)
- [Kasutamise näited](#-kasutamise-näited)
- [Peamised komponendid](#-peamised-komponendid)
- [Ülesannete loend](#-ülesannete-loend)
- [Märkused](#-märkused)
- [Kontaktid](#-kontaktid)

---

## 📝 Projekti kirjeldus

### Mis see on?

**Kalendar** on [kirjeldus: veebirakendustus kalendri haldamiseks, mis võimaldab kasutajatel luua sündmusi, määrata meeldetuletusi ja sünkroniseerida ajakava].

### Peamised funktsioonid

- ✅ [Funktsioon 1: sündmuste loomine ja redigeerimine]
- ✅ [Funktsioon 2: ajakavas vaatamine päevade, nädalate ja kuude kaupa]
- ✅ [Funktsioon 3: teatised ja meeldetuletused]
- ✅ [Funktsioon 4: andmete eksportimine erinevatesse vormingutesse]
- ✅ [Funktsioon 5: reageeriv disain mobiilsetele seadmetele]

> 📌 **Märkus**: Projekt arendatakse aktiivselt ja on staatuses [beta/alfa/tootmine].

---

## 🎯 Mis oli realiseeritud

### Versioon 1.0 (praegune)

1. **Kalendri kasutajaliides**
   - Kalendri ruudustiku visualiseerimine
   - Navigeerimine kuude ja aastate kaupa
   - Praeguse kuupäeva esiletõstmine

2. **Sündmuste haldamine**
   - Uute sündmuste loomine
   - Olemasolevate kirjete redigeerimine
   - Sündmuste kustutamine
   - Sündmuste kategoriseerimine tüüpide kaupa

3. **Andmete salvestamine**
   - Kohalik salvestusruum (LocalStorage)
   - Võimalus eksportida JSON-i
   - [Lisafunktsioon: sünkroniseerimine pilves]

4. **Kasutuskogemuse optimeerimine**
   - Reageeriv disain
   - Intuitiivne kasutajaliides
   - Klaviatuuri otseteed

---

## 🛠️ Kasutatavad tehnoloogiad

| Tehnoloogia | Kirjeldus | Versioon |
|:-----------|:---------|:------:|
| **HTML5** | Lehe struktuur | 5 |
| **CSS3** | Stiliseerimine ja paigutus | 3 |
| **JavaScript** | Rakenduse loogika | ES6+ |
| **[Raamistik]** | [Kasutamise kirjeldus] | [Versioon] |
| **LocalStorage API** | Andmete kohalik salvestamine | Native |

### Tehisarenduse ülevaade

```
Frontend: HTML5 + CSS3 + Vanilla JS
Salvestusruum: Brauseri LocalStorage / JSON
Juurutamine: GitHub Pages
Versioonihaldus: Git
```

---

## 📁 Projekti struktuur

```
kalendar/
├── index.html              # Rakenduse pealehekülg
├── css/
│   ├── style.css          # Põhilised stiilid
│   ├── responsive.css     # Mobiilsed stiilid
│   └── calendar.css       # Kalendri stiilid
├── js/
│   ├── main.js            # Peamine loogika
│   ├── calendar.js        # Kalendriga töötamise funktsioonid
│   ├── events.js          # Sündmuste haldamine
│   └── storage.js         # Salvestusruumiga töötamine
├── assets/
│   ├── images/            # Projekti pildid
│   ├── icons/             # Ikoonid
│   └── fonts/             # Veebikriftid
├── docs/
│   ├── API.md             # API dokumentatsioon
│   └── CONTRIBUTING.md    # Juhised kaasautorite jaoks
├── README.md              # See fail
└── LICENSE                # Projekti litsents
```

---

## 🚀 Käivitamise juhend

### Eeltingimused

- Kaasaegne veebibrauser (Chrome, Firefox, Safari, Edge)
- Tekstiredaktor koodi redigeerimiseks
- Git repositooriumi kloonimiseks

### Kohalik käivitamine

#### Viis 1: Repositooriumi kloonamine

```bash
# Kloonime repositooriumi
git clone https://github.com/Tefix/kalendar.git

# Läheme projekti kataloogi
cd kalendar

# Avame index.html brauseris
# Windowsil:
start index.html

# macOS-il:
open index.html

# Linuxil:
xdg-open index.html
```

#### Viis 2: Kohaliku serveri kasutamine

```bash
# Kui Teil on paigaldatud Python 3
python -m http.server 8000

# Või Python 2
python -m SimpleHTTPServer 8000

# Seejärel avage brauseris: http://localhost:8000
```

#### Viis 3: Live Server (VS Code)

1. Paigaldage VS Code laiendus "Live Server"
2. Avage `index.html`
3. Klõpsake alumisel paneelil "Go Live"

### Juurdepääs veebis

Rakendusele saab juurde pääseda aadressil: [Sisestage GitHub Pages URL]

> ⚠️ **Oluline**: Rakenduse korrektseks tööks peab JavaScript olema lubatud brauseris ja LocalStorage kasutamine lubatud.

---

## 💡 Kasutamise näited

### Näide 1: Sündmuse loomine

```javascript
// Loome uue sündmuse
const newEvent = {
  id: Date.now(),
  title: 'Kohtuminek tiimiga',
  date: '2026-04-15',
  time: '14:30',
  category: 'work',
  description: 'Uue projekti arutelu'
};

// Salvestame sündmuse
saveEvent(newEvent);
console.log('Sündmus edukalt loodud!');
```

### Näide 2: Sündmuste saamine päeva kohta

```javascript
// Saame kõik sündmused kindlale kuupäevale
const date = '2026-04-01';
const dayEvents = getEventsByDate(date);

// Väljastame sündmused
dayEvents.forEach(event => {
  console.log(`${event.time} - ${event.title}`);
});
```

### Näide 3: HTML struktuur

```html
<!-- Kalendri konteiner -->
<div id="calendar" class="calendar-container">
  <div class="calendar-header">
    <button class="prev-month">← Tagasi</button>
    <h2 id="current-month">Aprill 2026</h2>
    <button class="next-month">Edasi →</button>
  </div>
  
  <table class="calendar-table">
    <thead>
      <tr>
        <th>E</th>
        <th>T</th>
        <th>K</th>
        <th>N</th>
        <th>R</th>
        <th>L</th>
        <th>P</th>
      </tr>
    </thead>
    <tbody id="calendar-days">
      <!-- Kalendri päevad genereeritakse JS-ga -->
    </tbody>
  </table>
</div>
```

### Näide 4: CSS kasutamine

```css
/* Kalendri põhilised stiilid */
.calendar-container {
  max-width: 800px;
  margin: 20px auto;
  padding: 20px;
  border: 1px solid #ddd;
  border-radius: 8px;
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
}

.calendar-table {
  width: 100%;
  border-collapse: collapse;
  margin-top: 20px;
}

.calendar-table td {
  padding: 10px;
  border: 1px solid #eee;
  text-align: center;
  cursor: pointer;
  transition: background-color 0.3s;
}

.calendar-table td:hover {
  background-color: #f0f0f0;
}

.calendar-table td.today {
  background-color: #007bff;
  color: white;
  font-weight: bold;
}
```

> 💡 **Nõuanne**: Paremaks koodi mõistmiseks vaadake täielikke näiteid kaustas `examples/`.

---

## 📊 Peamised komponendid

| Komponent | Fail | Kirjeldus | Staatus |
|:----------|:-----|:---------|:------:|
| Kalender | `calendar.js` | Kuukavandi kuvamise loogika | ✅ Lõpetatud |
| Sündmused | `events.js` | Sündmuste haldamine (CRUD) | ✅ Lõpetatud |
| Salvestusruum | `storage.js` | Andmete salvestamine ja laadimine | ✅ Lõpetatud |
| Navigeerimine | `main.js` | Kuude vahel liikumine | ✅ Lõpetatud |
| Eksport | `export.js` | Andmete eksportimine JSON-i | 🔄 Arendamisel |
| Sünkroonimine | `sync.js` | Sünkroonimine pilves | ⏳ Kavandatud |

---

## ✅ Ülesannete loend

### Praegune sprint (Q2 2026)

- [x] Kalendri põhilised kasutajaliides
- [x] Sündmuste loomine
- [x] Sündmuste redigeerimine
- [x] Sündmuste kustutamine
- [ ] Filtreerimine kategooriate kaupa
- [ ] Sündmuste otsimine nime järgi
- [ ] Google Calendari integratsioon
- [ ] Mobiilirakendus (React Native)
- [ ] Tume teema
- [ ] Mitmekeelne tugi

### Tulevased versioonid

- [ ] API välisrakendustele
- [ ] Ühine kalender
- [ ] Videokonverentsi funktsioon
- [ ] Aja analüütika

---

## 📍 Märkused

### Teadaolevad piirangud

> ⚠️ **Tähelepanu**: LocalStoragel on suuruse piirang (~5-10 MB). Suuremate andmehulkade puhul soovitame kasutada serveripoolset lahendust.

### Jõudlus

```javascript
// Soovitatav sündmuste arv: kuni 1000
// Optimaalne arv sujuvaks tööks: kuni 500
// Aeglustumise korral kasutage lehitsemist
```

### Brauseri ühilduvus

| Brauser | Tugi | Märkused |
|:--------|:---------:|:-----------|
| Chrome | ✅ | Täielik tugi |
| Firefox | ✅ | Täielik tugi |
| Safari | ✅ | Täielik tugi |
| Edge | ✅ | Täielik tugi |
| IE 11 | ❌ | Kasutab vananenud API-d |

### Parimad praktikad

1. **Varundamine**: Eksportige andmed regulaarselt JSON-i
2. **Turvalisus**: Ärge saatke tundlikke andmeid tavalise HTTP-ga
3. **Kätus**: Rakendus salvestatakse brauseri poolt, puhastage kätust värskendamise korral
4. **Juurdepääsetavus**: Kasutage klaviatuuri navigeerimist (Tab, Enter, Delete)

### Jalused ja viited

Projekti inspireeriti[^1] veebirakendamise parimatest praktikatest[^2].

[^1]: Olemasolevate kalendrirakenduste uurimine
[^2]: Google Calendar, Apple Calendar, Notion Calendar

---

## 🐛 Silumine

### Levinud probleemid

**Probleem**: Sündmused ei salvestu pärast lehte uuesti laadimist
```
Lahendus: Kontrollige, kas LocalStorage on brauseris lubatud
Settings → Privacy → Cookies → Allow local storage
```

**Probleem**: Kalender kuvatakse valesti
```
Lahendus: Puhastage brauseri kätus (Ctrl+Shift+Delete)
Laadige leht uuesti (Ctrl+F5)
```

**Probleem**: JavaScript ei tööta
```
Lahendus: Avage DevTools (F12)
Kontrollige konsooli tõrgete suhtes (Console tab)
```

### Arendusmõõdu lubamine

```javascript
// Lisage brauseri konsooli
localStorage.setItem('DEBUG_MODE', 'true');
location.reload();
```

---

## 📚 Lisaressursid

- 📖 [Täielik dokumentatsioon](docs/README.md)
- 🤝 [Juhend kaasautorite jaoks](docs/CONTRIBUTING.md)
- 🐛 [Veajade jälitaja](https://github.com/Tefix/kalendar/issues)
- 📋 [Projekt (Roadmap)](https://github.com/Tefix/kalendar/projects)
- 💬 [Arutelud](https://github.com/Tefix/kalendar/discussions)

---

## 🔗 Kasulikud lingid

### Ametlik teave

- [GitHub repositoorium](https://github.com/Tefix/kalendar)
- [GitHub Pages](https://tefix.github.io/kalendar)
- [Probleemid](https://github.com/Tefix/kalendar/issues)

### Dokumentatsioon ja õpetused

- [MDN Web Docs - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
- [W3C HTML Specification](#)
