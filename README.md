# Spesa Multisupermercato

Web app locale per gestire liste della spesa e un semplice riepilogo spese. Pensata per Alì ma configurabile per altri siti (Esselunga, Coop, Conad, Amazon Fresh, ecc.). Funziona interamente in locale (LocalStorage).

## Funzioni principali
- Lista della spesa strutturata (prodotto, marca, quantità, pezzi, prezzo max)
- Salvataggio multiplo di liste (crea, rinomina, elimina, salva)
- Import/Export lista (CSV/JSON)
- Stima prezzi (euristica locale + link a metaricerca)
- Modalità Ricerca: copia automatica della query negli appunti e apertura sito
- Riepilogo spese: aggiunta, storico, export/import JSON, grafico mensile
- Impostazioni: scelta sito del supermercato (preset + personalizzato)

## Uso
1. Scheda “Lista”
   - Incolla la tua lista nell’area di testo e premi “Crea righe”
   - Oppure premi “Esempio” e poi “Crea righe”
   - Modifica campi e usa “Stima” per provare a valorizzare “Max”
   - “Salva” salva la lista attiva. “Salva come nuova” crea una nuova lista.
   - “Reset” svuota la lista attiva

2. Scheda “Ricerca”
   - Premi “Avvia Ricerca Automatica”
   - “Apri Sito (nuova scheda)” apre il sito configurato
   - La query dell’articolo corrente è copiata negli appunti

3. Scheda “Riepilogo”
   - Inserisci Data, N. articoli e Costo per ogni spesa
   - Vedi totali mese/anno, media e grafico mensile

4. Scheda “Impostazioni”
   - Scegli un preset (Alì, Esselunga, Coop, Conad, Amazon Fresh) o URL personalizzato
   - Salva e usa i pulsanti di test per aprire il sito

## Scorciatoie
- Ctrl/⌘ + Shift + O = Apri sito in nuova scheda
- Ctrl/⌘ + Shift + N = Passa al prossimo articolo in Ricerca

## Dati
Tutto è salvato in locale via LocalStorage:
- Liste: `spesa_ali_lists_v1`
- Lista legacy: `spesa_ali_list_v4`
- Impostazioni: `spesa_ali_settings_v1`
- Spese: `spesa_ali_expenses_v1`

## Pubblicazione su GitHub Pages (solo web)
1. Crea repo su GitHub (Public)
2. Add file > Create new file > `index.html` e incolla il codice della pagina
3. Settings > Pages > Deploy from a branch > main / root > Save
4. Apri l’URL che appare (attendi 1–2 minuti)

Suggerimenti: se provi l’app dentro un’anteprima/iframe, alcuni pulsanti di apertura sito potrebbero essere limitati dal browser. Apri sempre l’app in una scheda piena.
