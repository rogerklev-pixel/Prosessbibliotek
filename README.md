[README.md](https://github.com/user-attachments/files/27374784/README.md)
# Prosessbibliotek – Oppsettsinstruksjoner

## Filer i pakken
| Fil | Beskrivelse |
|---|---|
| `index.html` | Den offentlige siden – kun lesing, del denne lenken med teamet |
| `admin.html` | Administratorsiden – kun du bruker denne |
| `processes.json` | Dataene – alle prosessbeskrivelsene lagres her |

---

## Steg 1 – Endre admin-passord

Åpne `admin.html` i en teksteditor og finn linjen:

```js
const ADMIN_PASSWORD = 'prosess2024';
```

Bytt ut `prosess2024` med et passord du velger selv.

---

## Steg 2 – Legg ut på GitHub Pages (gratis)

### Første gang
1. Gå til [github.com](https://github.com) og logg inn (eller opprett en konto)
2. Klikk **New repository**
3. Gi repositoryet et navn, f.eks. `prosessbibliotek`
4. Sett det til **Public** (kreves for gratis GitHub Pages)
5. Klikk **Create repository**
6. Last opp alle tre filene (`index.html`, `admin.html`, `processes.json`)
7. Gå til **Settings → Pages**
8. Under *Source*, velg **Deploy from a branch** → branch: `main`, mappe: `/ (root)`
9. Klikk **Save**

Etter noen minutter er siden tilgjengelig på:
`https://[ditt-brukernavn].github.io/prosessbibliotek/`

### Del disse lenkene
- **Teamet ditt:** `https://[brukernavn].github.io/prosessbibliotek/`
- **Deg selv (admin):** `https://[brukernavn].github.io/prosessbibliotek/admin.html`

---

## Steg 3 – Slik legger du til nye prosesser

1. Gå til `admin.html`-lenken din
2. Logg inn med passordet
3. Klikk **Ny prosess**, fyll ut skjemaet, klikk **Lagre**
4. En fil kalt `processes.json` lastes automatisk ned til datamaskinen din
5. Gå til GitHub-repositoryet ditt
6. Klikk på `processes.json` → klikk på blyant-ikonet (Edit) → lim inn innholdet, **eller**
   dra og slipp den nedlastede filen direkte over den gamle på GitHub
7. Klikk **Commit changes**

Innen 30 sekunder er den nye prosessen synlig for alle!

---

## Tips
- Hold `admin.html`-lenken privat – del den ikke offentlig
- Du kan også redigere `processes.json` direkte i en teksteditor om du foretrekker det
- Ingen database, ingen server – alt er statiske filer
