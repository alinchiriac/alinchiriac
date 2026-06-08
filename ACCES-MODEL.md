# Model de Acces — Proiecte Alin Chiriac

## Arhitectură

Fiecare proiect are **propriul repository privat** cu acces individual controlat.
Nimeni nu poate vedea altă muncă decât cea la care a primit acces explicit.

## Repository-uri

| Repo | Vizibilitate | Colaboratori |
|------|-------------|---------------|
| `alinchiriac/alinchiriac` | Privat | Doar tu (hub tracking) |
| `alinchiriac/adfaber` | Privat | Invit per persoană |
| `alinchiriac/cursuri-adfaber` | Privat | Invit per persoană |
| `alinchiriac/alinchiriac-ro` | Privat | Invit per persoană |
| `alinchiriac/codeschoolclubs` | Privat | Invit per persoană |
| `alinchiriac/cursuri-codeschoolclubs` | Privat | Invit per persoană |
| `alinchiriac/dev-csc` | Privat | Invit per persoană |
| `alinchiriac/ai4teachers` | Privat | Invit per persoană |

## Cum dai acces unui colaborator

1. Mergi pe GitHub.com la repo-ul specific (ex: `alinchiriac/adfaber`)
2. Settings → Collaborators → Add people
3. Introdu username-ul sau emailul colaboratorului
4. Alege nivelul de acces:
   - **Read** — pot vedea codul, nu pot modifica
   - **Write** — pot face push (recomandat pentru devs)
   - **Maintain** — pot gestiona PR-uri, nu pot schimba setari critice
   - **Admin** — acces complet (doar pentru co-admini de încredere)

## Contextul AI (CLAUDE.md)

Fiecare repo conține un fişier `.claude/CLAUDE.md` cu:
- Descrierea proiectului
- Tehnologiile folosite
- Reguli de lucru specifice
- Instrucțiuni pentru agenții AI

Acest fişier este **vizibil doar colaboratorilor din acel repo**.
Nimeni din alt proiect nu îll poate accesa.

## Permisiuni Claude Code

Când deschizi o sesiune Claude Code pe un repo:
- Claude vede doar fişierele din acel repo
- Contextul (`CLAUDE.md`) este specific proiectului
- Sesiunile sunt izolate — nu se „revarsă” între proiecte

## Reguli generale

- Nu adăuga niciodată chei API, parole sau date sensibile în repo-uri
- Folosesc `.env` local (adăugat în `.gitignore`) pentru secrete
- Revoc accesul imediat după terminarea colaborării
