# Data Source — Process Map

Interaktivna mapa procesa kreiranja **Data Source-a** za Virtual Shopping projekte u EyeSee-u.

Mapa prikazuje 5 glavnih koraka i 34 pod-koraka — od pripreme foldera, preko image sourcing-a, do finalnog popunjavanja KPI kolona.

🔗 **Live preview:** https://YOUR-USERNAME.github.io/REPO-NAME/

---

## Funkcionalnosti

- **Mapa-stil navigacija** — pinovi sa pulsirajućim tačkama, povezani isprekidanim linijama u brand bojama
- **Zoom & pan** — scroll mišem, drag, dugmad ili tastatura (`+`/`-`/`0`)
- **Detalji na klik** — klik na pin otvara sve pod-korake sa praktičnim savetima
- **Lične beleške** — polja za upis beleški po koraku i pod-koraku, sa auto-save u browser
- **Export/Import** — izvezi beleške kao Markdown (.md) ili JSON backup, uvezi na drugom uređaju
- **Tastaturne prečice** — `1-5` skok na korak, `Esc` zatvori, `Strelice` prebacivanje

---

## Pokretanje lokalno

Single-file HTML — nema build koraka, nema dependency-a.

```bash
# kloniraj repo
git clone https://github.com/YOUR-USERNAME/REPO-NAME.git
cd REPO-NAME

# otvori u browseru
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

Ili dupli-klik na `index.html` u file exploreru.

---

## Hosting na GitHub Pages

1. Push repo na GitHub
2. **Settings → Pages**
3. Source: **Deploy from a branch** → branch `main` → folder `/ (root)`
4. Sačekaj par minuta — sajt će biti dostupan na `https://YOUR-USERNAME.github.io/REPO-NAME/`

Pošto je sve u jednom HTML fajlu, ne treba nikakav build pipeline.

---

## Privatnost beleški

Beleške se čuvaju u **`localStorage`** browsera korisnika koji posećuje stranicu. Znači:

- Niko (uključujući autora repo-a) **ne vidi tvoje beleške**
- Beleške žive samo u tvom browseru, na tvom uređaju
- Brisanje cache-a / prelazak na drugi uređaj = beleške nestaju

**Preporuka:** Periodično koristi **Backup (.json)** ako želiš da prebacuješ beleške između uređaja ili da ih trajno arhiviraš.

---

## Tehnički

- Single-file `index.html` — sav HTML, CSS i JS u jednom fajlu
- Vanilla JS, bez frameworka
- Roboto font sa Google Fonts (jedini eksterni dependency)
- ~1400 linija koda, ~75 KB

---

## Struktura

```
.
├── index.html      # Cela aplikacija
├── README.md       # Ovaj fajl
└── LICENSE         # Licenca
```

---

## License

MIT — vidi [LICENSE](LICENSE).

Sadržaj se odnosi na interni EyeSee proces. Repo služi kao referenca za tim i ne predstavlja zvanični outputni dokument.

---

*Made for EyeSee · Virtual Shopping team · 2026*
