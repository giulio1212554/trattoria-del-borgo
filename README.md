# Trattoria del Borgo — Web App Ristorante

Applicazione web completa per ristorante con **area pubblica** e **dashboard admin**.

## Funzionalità

### Area Pubblica
- **Home** con hero, filosofia, piatti iconici, orari e contatti
- **Menu digitale interattivo** con ricerca e filtri (senza glutine, vegetariano, vegano)
- **Sistema di prenotazione** tavoli con conferma immediata

### Area Admin (password: `admin123`)
- **Panoramica** giornaliera (prenotazioni, coperti, stato tavoli)
- **Gestione prenotazioni** (filtri, aggiunta manuale, modifica, assegnazione tavolo)
- **Mappa sala** con stato in tempo reale (Libero / Prenotato / Occupato)
- **CRUD Menu** (aggiungi, modifica, esaurisci/riattiva piatti)
- **Impostazioni** ristorante

## Come usare

1. Apri `index.html` nel browser (o servi la cartella con un server statico)
2. Oppure da terminale nella cartella:
   ```bash
   npx serve .
   ```
3. Vai su `/admin` e accedi con password: **admin123**

## Note tecniche

- Stack: HTML + Tailwind CSS (CDN) + JavaScript vanilla
- Persistenza dati: `localStorage` del browser
- Le modifiche fatte in Admin si riflettono subito sul sito pubblico
- Dati di esempio già popolati (menu italiano completo, 10 tavoli, prenotazioni di test)
- Design mobile-first, palette calda (panna / antracite / terracotta / verde oliva)

## Struttura file

```
ristorante/
├── index.html          # Home pubblica
├── menu.html           # Menu interattivo
├── prenota.html        # Form prenotazione
├── admin/
│   └── index.html      # Dashboard admin
├── css/
│   └── style.css       # Stili custom
├── js/
│   └── data.js         # Store dati + localStorage
└── README.md
```
