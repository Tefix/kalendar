# 📅 ProjectLibre — Kalendri ja Diagrammide

> Õppeprojekt: veebileht, mis selgitab ProjectLibre põhifunktsioone — kalendri loomine, tööaegade muutmine ja diagrammide kasutamine.

---

## 📖 Sisukord

- [Projekti kirjeldus](#-projekti-kirjeldus)
- [Failide struktuur](#-failide-struktuur)
- [Tehtud tööd](#-tehtud-tööd)
- [Lehtede ülevaade](#-lehtede-ülevaade)
- [Kasutatud tehnoloogiad](#-kasutatud-tehnoloogiad)
- [GitHub Issues ja Kanban](#-github-issues-ja-kanban)
- [Commit-sõnumite näited](#-commit-sõnumite-näited)
- [Ekraanipildid](#-ekraanipildid)
- [Autor](#-autor)

---

## 📌 Projekti kirjeldus

See projekt on **õppeotstarbeline veebileht**, mis tutvustab ProjectLibre tarkvara kasutamist.  
Leht on loodud HTML ja CSS abil ning sisaldab samm-sammulisi juhendeid koos ekraanipiltidega.

> [!NOTE]
> ProjectLibre on **tasuta ja avatud lähtekoodiga** MS Projecti alternatiiv, mida on alla laetud üle 8,2 miljoni korra.

> [!IMPORTANT]
> Iga haru (`branch`) sisaldab oma `README.md` faili, mis kirjeldab selle haru muutusi.

---

## 📁 Failide struktuur

```
projektilibre-kalender/
├── index.html          # Kalendri loomine ProjectLibres
├── diagramm.html       # Diagrammide loomine ProjectLibres
├── style.css           # Ühine stiilileht kõigile lehtedele
└── README.md           # See fail
```

> [!WARNING]
> Fail `valem.html` on **kustutatud** — selle sisu asendati `index.html` failis ProjectLibre juhendiga.

---

## ✅ Tehtud tööd

### Task list — kõik ülesanded

- [x] `#7` — Kustuta fail `valem.html`
- [x] `#5` — Uuenda `index.html`, lisa juhised uue kalendri loomiseks ProjectLibre's
- [x] `#6` — Uuenda diagrammide lehekülg ProjectLibre põhjal
- [x] `#10` — Uue kalendri loomine veebilehel
- [x] `#11` — Teksti genereerimine Claude-ga
- [x] `#13` — Uus CSS-stiil
- [x] `#9` — Muuta navigatsioonimenüüd
- [x] `#8` — ProjectLibre ekraanipildid teha
- [ ] `#4` — 30.03 *(töös)*
- [ ] `#12` — Pildid on ise tehtud *(backlogis)*

---

## 📄 Lehtede ülevaade

### 1. `index.html` — Kalendri loomine

Lehel selgitatakse **7 sammus**, kuidas luua uus kalender ProjectLibres:

| Samm | Teema | Kirjeldus |
|------|-------|-----------|
| 01 | Mis on kalender? | Kalendritüübid — projekti, ülesande, ressursi kalender |
| 02 | Ava Calendar | `File → Calendar` — avab kalendrite halduse |
| 03 | Uus kalender | `New…` → sisesta nimi → koopia Standard-ist |
| 04 | Muuda tööpäevi | Kliki päeval → Working / Non-default / Non-working |
| 05 | Mittetööpäevad | Riiklikud pühad punaseks — projektile ignoreeritakse |
| 06 | Options | Tunde/päev, tunde/nädal — **kohustuslik seadistada!** |
| 07 | Ressursile | `Resource Information → Base Calendar` |

### 2. `diagramm.html` — Diagrammide loomine

Lehel kirjeldatakse kõiki ProjectLibre diagrammitüüpe:

| Diagramm | Asukoht | Kirjeldus |
|----------|---------|-----------|
| **Gantt Chart** | Vaikimisi vaade | Ajariba ülesannetega |
| **Network Diagram** | View → Network Diagram | Sõltuvuste karpdiagramm |
| **WBS** | View → WBS | Tööjaotusstruktuuri puu |
| **Resource Histogram** | View → Histogram | Ressursikoormus tulpdiagrammina |
| **Task Usage** | View → Task Usage | Ülesanded vs töötunnid |

---

## 🛠 Kasutatud tehnoloogiad

- **HTML5** — lehe struktuur ja sisu
- **CSS3** — kujundus, animatsioonid, CSS muutujad
- **Google Fonts** — Syne (pealkirjad) + Lora (tekst)
- **JavaScript** — scroll-animatsioonid (Intersection Observer)
- **ProjectLibre** — ekraanipiltide allikas[^1]
- **GitHub Pages** — lehe avaldamine

---

## 📋 GitHub Issues ja Kanban

Projekt kasutab **GitHub Projects Kanban-tahvlit** ülesannete haldamiseks.

### Veerud

| Veerg | Tähendus |
|-------|----------|
| **Backlog** | Planeeritud, alustamata |
| **Ready** | Valmis alustamiseks |
| **In progress** | Aktiivselt töös |
| **In review** | Ülevaatamisel |
| **Vaatamiseks** | Valmis / kontrollimiseks |

### Issues ja nende seos commitidega

Commit-sõnumites kasuta märksõnu, et issue **automaatselt sulgeda**:

```
git commit -m "Kustuta valem.html - Closes #7"
git commit -m "Lisa ProjectLibre kalendri juhend - Fixes #5"
git commit -m "Uuenda diagramm.html - Closes #6"
git commit -m "Muuda navigatsioonimenüüd - Closes #9"
```

> [!TIP]
> Märksõnad `Closes`, `Fixes`, `Resolves` + `#number` sulgevad issue automaatselt pärast `merge`'i peaharusse.

---

## 💾 Commit-sõnumite näited

```bash
# Hea commit-sõnum — kirjeldav ja seotud issue-ga
git commit -m "Lisa HTML struktuur - Closes #10"
git commit -m "Lisa CSS stiilid ja animatsioonid - Closes #13"
git commit -m "Uuenda index.html ProjectLibre kalendri juhendiga - Fixes #5"
git commit -m "Kustuta valem.html projektist - Closes #7"
git commit -m "Muuta navigatsioonimenüüd, eemalda valem.html link - Closes #9"

# Halb commit-sõnum — ebainformatiivne
git commit -m "update"
git commit -m "fix stuff"
```

---

## 🖼 Ekraanipildid

🖼️ Ekraanipildid
📆 Kalendri loomine

<img width="595" height="123" alt="pilt" src="https://github.com/user-attachments/assets/5729a5e4-a590-496b-a5d0-8228ba8abf21" />

Kalender
🧮 Custom Fields

<img width="595" height="123" alt="pilt" src="https://github.com/user-attachments/assets/5c25aa99-116d-4a9f-9744-322eca7f8b0b" />

Fields
📊 Diagrammid

<img width="570" height="123" alt="pilt" src="https://github.com/user-attachments/assets/02e4bdd2-df27-448d-86e7-7e235828d5e2" />


Diagrammid

---

## 👤 Autor

| Väli | Info |
|------|------|
| **Nimi** | Roman Zaitsev |
| **Grupp** | TARpv24 |
| **Projekt** | ProjectLibre õppeleht |
| **Aasta** | 2026 |

---

[^1]: ProjectLibre on avatud lähtekoodiga tarkvara, saadaval aadressil [projectlibre.com](https://www.projectlibre.com) ja [SourceForge](https://sourceforge.net/projects/projectlibre/). Ekraanipildid on tehtud õppeotstarbel.

---

*Loodud õppeotstarbel · TARpv24 · 2026*
