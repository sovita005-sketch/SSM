# 🧬 SSM Simulator - Simulatore Scuole di Specializzazione Medica

Progressive Web App completa per la preparazione al test SSM con modalità studio ed esame, personalizzazione delle categorie e statistiche dettagliate.

![SSM Simulator](https://img.shields.io/badge/PWA-Ready-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Platform](https://img.shields.io/badge/platform-iOS%20%7C%20Android%20%7C%20Web-lightgrey)

## ✨ Caratteristiche Principali

- 📚 **Supporto per migliaia di domande** - Carica fino a 20.000+ domande in formato JSON
- 🎯 **Modalità Studio** - Feedback immediato con spiegazioni dettagliate dopo ogni risposta
- 🏆 **Modalità Esame** - Simulazione realistica dell'esame SSM senza feedback immediato
- 🔍 **Filtro Categorie** - Seleziona specifiche materie mediche per lo studio mirato
- 📊 **Numero Domande Personalizzabile** - Scegli quante domande affrontare (da 1 a 200)
- 💯 **Statistiche Dettagliate** - Accuratezza, punteggio, risposte corrette/sbagliate
- ⏱️ **Timer Integrato** - Monitora il tempo impiegato durante il quiz
- 📱 **Installabile come App** - Funziona come un'app nativa su iOS e Android
- 🔌 **Funzionamento Offline** - Continua a studiare anche senza connessione internet
- ⚡ **Veloce e Ottimizzato** - Caricamento istantaneo e performance fluide

## 🚀 Installazione

### Su iPhone/iPad:
1. Apri **Safari** e visita il sito
2. Tocca l'icona **"Condividi"** (quadrato con freccia in basso)
3. Scorri e seleziona **"Aggiungi a Home"**
4. Tocca **"Aggiungi"**
5. ✅ L'app SSM Simulator appare sulla tua Home screen!

### Su Android:
1. Apri **Chrome** e visita il sito
2. Tocca **"Installa"** nel banner che appare in basso
3. Oppure: Menu (⋮) → **"Installa app"**
4. ✅ L'app viene aggiunta alla Home screen!

### Su Desktop (Chrome/Edge):
1. Apri il sito nel browser
2. Clicca l'icona **"+"** nella barra degli indirizzi
3. Oppure: Menu → **"Installa SSM Simulator"**
4. ✅ L'app viene installata sul computer!

## 📚 Come Usare il Simulatore

### 1. Carica le tue domande
- Clicca su **"Seleziona File JSON"** nella home
- Scegli il file con le tue domande in formato JSON
- Le domande vengono caricate istantaneamente

### 2. Scegli la modalità
- **Modalità Studio**: Ricevi spiegazioni immediate dopo ogni risposta
- **Modalità Esame**: Simula l'esame reale, risultati a fine quiz

### 3. Personalizza il quiz
- **Seleziona le categorie**: Studia solo le materie che ti interessano
- **Imposta il numero di domande**: Da 1 a 200 domande per sessione
- Le domande vengono mescolate casualmente

### 4. Inizia il quiz
- Rispondi alle domande selezionando una delle opzioni (A-E)
- Usa i pulsanti per navigare tra le domande
- Visualizza le statistiche in tempo reale

### 5. Analizza i risultati
- Vedi tutte le risposte date con correzioni
- Leggi le spiegazioni dettagliate
- Rivedi il tempo impiegato
- Controlla la tua accuratezza

## 🔧 Formato JSON per le Domande

Le domande devono essere in formato JSON seguendo questa struttura:

```json
[
  {
    "id": 1,
    "question": "Quale dei seguenti trattamenti è il più appropriato per...?",
    "answers": [
      "Opzione A",
      "Opzione B",
      "Opzione C",
      "Opzione D",
      "Opzione E"
    ],
    "correctAnswer": 1,
    "explanation": "La risposta B è corretta perché...",
    "category": "Cardiologia",
    "difficulty": "medio"
  },
  {
    "id": 2,
    "question": "Un paziente presenta i seguenti sintomi...",
    "answers": ["..."],
    "correctAnswer": 0,
    "explanation": "...",
    "category": "Neurologia",
    "difficulty": "difficile"
  }
]
```

### Campi obbligatori:
- `id` - Numero identificativo univoco
- `question` - Testo della domanda
- `answers` - Array con 2-5 risposte possibili
- `correctAnswer` - Indice della risposta corretta (0 = prima risposta, 1 = seconda, ecc.)

### Campi opzionali:
- `explanation` - Spiegazione dettagliata della risposta corretta
- `category` - Categoria/materia medica (es: "Cardiologia", "Ortopedia")
- `difficulty` - Livello di difficoltà: "facile", "medio" o "difficile"

## 💻 Tecnologie Utilizzate

- **React 18** - Framework JavaScript per l'interfaccia utente
- **Tailwind CSS** - Framework CSS per lo styling
- **Service Worker** - Per funzionalità offline e cache
- **Web App Manifest** - Per rendere l'app installabile
- **LocalStorage** - Per salvare le domande localmente

## 📱 Compatibilità

- ✅ iOS 12.2+ (Safari)
- ✅ Android 5.0+ (Chrome)
- ✅ Windows 10+ (Chrome, Edge)
- ✅ macOS (Chrome, Safari, Edge)
- ✅ Linux (Chrome, Firefox)

## 🎯 Funzionalità Avanzate

### Navigazione Quiz
- ⬅️ Domanda precedente
- ❌ Annulla risposta
- 📋 Vai al riepilogo
- ✅ Conferma e prosegui

### Statistiche in Tempo Reale
- Numero domande completate
- Risposte corrette/sbagliate
- Accuratezza percentuale
- Timer progressivo

### Personalizzazione
- Selezione multipla categorie
- Slider per numero domande
- Pulsanti rapidi (10, 25, 50, 100, Max)
- Filtraggio intelligente

## 🔐 Privacy e Sicurezza

- ✅ **Nessun dato inviato a server esterni** - Tutto funziona localmente
- ✅ **Nessuna registrazione richiesta** - Usa l'app immediatamente
- ✅ **HTTPS di default** - Connessione sempre sicura
- ✅ **Open Source** - Codice completamente trasparente

## 📈 Roadmap Futura

- [ ] Sincronizzazione cloud (opzionale)
- [ ] Modalità dark mode
- [ ] Export risultati in PDF
- [ ] Grafici di progressione
- [ ]