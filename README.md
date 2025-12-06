# ⚡ FICES Reality Check

![Version](https://img.shields.io/badge/version-1.0.0-red)
![License](https://img.shields.io/badge/license-MIT-green)
![Platform](https://img.shields.io/badge/platform-iOS%20%7C%20Android%20%7C%20Web-blue)

**Il validatore di idee brutalmente onesto per FICES SRL**

Un'applicazione web che analizza le tue idee aziendali con spietatezza chirurgica, fornendo 5 soluzioni alternative e una super consulenza dettagliata che nessun consulente ti direbbe mai con questa franchezza.

## 🎯 Cos'è FICES Reality Check?

FICES Reality Check è uno strumento di validazione idee progettato specificamente per piccole-medie imprese nel settore costruzioni e produzione industriale. Invece di dirti quello che vuoi sentire, ti dice **la verità nuda e cruda** su:

- **Fattibilità reale** della tua idea
- **Costi nascosti** che nessuno considera
- **Tempi realistici** (non quelli dei sogni)
- **Rischi concreti** che potresti affrontare
- **5 soluzioni alternative** dal "fai il minimo" al "non fare niente"

## ✨ Caratteristiche Principali

### 🎤 Riconoscimento Vocale
- **Input vocale** in italiano per registrare idee parlando
- Supporto completo iOS Safari e Android Chrome
- Trascrizione automatica in tempo reale

### 🔍 Analisi Brutalmente Onesta
- Algoritmo di valutazione basato su complessità, costi e tempi
- Score di fattibilità da 1 a 10
- Moltiplicatori dinamici per costi e timeline

### 💡 5 Soluzioni Alternative
1. **Soluzione Pragmatica Base** - Il minimo indispensabile
2. **Soluzione Excel/Macro** - Economica e veloce (spesso la migliore)
3. **Soluzione Professionale Completa** - Enterprise-grade (spesso eccessiva)
4. **Soluzione Ibrida Pragmatica** - Il compromesso intelligente
5. **Soluzione "Non Fare Niente"** - A volte è la scelta più saggia

### 📊 Super Consulenza Dettagliata (8 Sezioni)

#### 1. 📋 Analisi Dettagliata dell'Idea
- Breakdown completo della complessità
- Score interpretativi e metriche
- Significato pratico per la tua azienda

#### 2. ⚠️ Rischi Reali
- Rischi tecnici, operativi e finanziari
- Probabilità di fallimento calcolata
- Costi nascosti (+30% minimo garantito)

#### 3. 💰 Breakdown Costi Nascosti
- Costi iniziali (hardware, licenze, setup)
- Costi ricorrenti annuali (manutenzione, supporto)
- Costi interni (tempo persone, formazione)

#### 4. 📅 Timeline Realistica
- Fase per fase con tempi reali
- Regola d'oro: aggiungi sempre +50%
- Considerazione del carico di lavoro esistente

#### 5. 🎯 Procedure Step-by-Step
- 6 fasi operative dettagliate
- Dalla validazione al go-live
- Checkpoint di controllo

#### 6. ✅ Fattibilità Contestuale
- Analisi specifica per il tuo contesto aziendale
- Punti di forza e criticità
- Raccomandazioni pratiche

#### 7. 🔧 Risorse Necessarie
- Persone (interne ed esterne)
- Tecnologia e infrastruttura
- Conoscenze richieste

#### 8. 💀 Verdetto Finale Senza Filtri
- Raccomandazione chiara: PROCEDI / CAUTELA / STOP
- La domanda che conta: "Sopravvivi se fallisce?"
- Prossimi passi concreti

### ✏️ Modifica Soluzioni
- Modifica costi, tempi, fattibilità di ogni soluzione
- Duplica soluzioni per creare varianti
- Salvataggio modifiche in tempo reale

## 🚀 Come Usare

### Opzione 1: GitHub Pages (Consigliata)

1. **Fork questo repository**
2. **Vai su Settings** → **Pages**
3. **Seleziona** branch `main` come source
4. **Attendi 1-2 minuti** per il deploy
5. **Apri** `https://TUO-USERNAME.github.io/fices-reality-check/fices-reality-check.html`

### Opzione 2: Netlify (Più Veloce)

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/TUO-USERNAME/fices-reality-check)

1. Clicca il pulsante sopra
2. Connetti il tuo account GitHub
3. Deploy automatico in 30 secondi
4. Ricevi il tuo URL personalizzato

### Opzione 3: Locale (Solo Test)

```bash
# Clona il repository
git clone https://github.com/TUO-USERNAME/fices-reality-check.git

# Apri con un server HTTP locale
cd fices-reality-check
python -m http.server 8000

# Apri browser su
http://localhost:8000/fices-reality-check.html
```

⚠️ **NOTA**: Su iOS/Safari, il riconoscimento vocale richiede **HTTPS**. Il file locale (`file://`) NON funzionerà per il microfono.

## 📱 Compatibilità

### ✅ Completamente Supportato
- **iOS 12+** (Safari) - iPhone 6s e superiori
- **Android 5+** (Chrome)
- **Desktop** (Chrome, Safari, Edge, Firefox)

### 🎤 Riconoscimento Vocale
- **iOS**: Safari (richiede HTTPS)
- **Android**: Chrome
- **Desktop**: Chrome, Edge

### 📐 Responsive Design
- iPhone SE (375px)
- iPhone 16 Pro (393px)
- iPhone 16 Pro Max (430px)
- iPad e Tablet
- Desktop (1920px+)

## 🔒 Requisiti Tecnici

### Per il Riconoscimento Vocale su iOS:
1. **HTTPS obbligatorio** (non funziona con HTTP o file://)
2. **Connessione internet** attiva
3. **Permessi microfono** concessi in Safari
4. **iOS 12 o superiore**

### Come Abilitare il Microfono su iOS:
1. Impostazioni iOS → Safari
2. Tocca "Microfono"
3. Seleziona "Consenti"
4. Ricarica la pagina

## 🛠️ Tecnologie Utilizzate

- **HTML5** - Struttura
- **CSS3** - Styling responsive e animazioni
- **Vanilla JavaScript** - Logica e interazioni
- **Web Speech API** - Riconoscimento vocale
- **Local Storage** - Persistenza dati (opzionale)

**Zero dipendenze esterne** - Funziona completamente offline (eccetto riconoscimento vocale)

## 📖 Personalizzazione

### Modifica l'Algoritmo di Analisi

Apri `fices-reality-check.html` e trova la funzione `performBrutalAnalysis()`:

```javascript
function performBrutalAnalysis(idea) {
    // Modifica i moltiplicatori di costo/tempo
    let costMultiplier = 1;
    let timeMultiplier = 1;
    
    // Aggiungi le tue regole personalizzate
    if (keywords.includes('tua-parola-chiave')) {
        costMultiplier += 0.5;
    }
    
    // ... resto della logica
}
```

### Modifica le Soluzioni Predefinite

Trova l'array `solutions` nella stessa funzione:

```javascript
const solutions = [
    {
        title: "La Tua Soluzione",
        cost: 10000,
        time: 45,
        feasibility: 8,
        description: "Descrizione della soluzione",
        brutal: "La verità brutale"
    },
    // ... altre soluzioni
];
```

### Cambia i Colori e lo Stile

Nel tag `<style>`, modifica le variabili di colore:

```css
/* Colore primario (rosso) */
#ff4444 → il-tuo-colore

/* Colore successo (verde) */
#00aa00 → il-tuo-colore

/* Colore warning (arancione) */
#ffaa00 → il-tuo-colore
```

## 🤝 Contribuire

Contribuzioni sono benvenute! Se vuoi migliorare FICES Reality Check:

1. **Fork** il progetto
2. **Crea** un branch per la tua feature (`git checkout -b feature/AmazingFeature`)
3. **Commit** le tue modifiche (`git commit -m 'Add some AmazingFeature'`)
4. **Push** al branch (`git push origin feature/AmazingFeature`)
5. **Apri** una Pull Request

### Idee per Contribuzioni
- [ ] Supporto multilingua (Inglese, Spagnolo)
- [ ] Esportazione PDF della consulenza
- [ ] Salvataggio analisi in cloud
- [ ] Template specifici per settori
- [ ] Integrazione con tool di project management
- [ ] Modalità dark/light theme
- [ ] Statistiche aggregate delle analisi

## 🐛 Bug e Problemi

Hai trovato un bug? Apri una [Issue](https://github.com/TUO-USERNAME/fices-reality-check/issues) descrivendo:
- Il problema riscontrato
- I passi per riprodurlo
- Browser e sistema operativo utilizzati
- Screenshot (se rilevante)

## 📜 Licenza

Questo progetto è rilasciato sotto licenza **MIT**.

```
MIT License

Copyright (c) 2024 FICES SRL

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## 👤 Autore

**FICES SRL**
- Sede: Lecce, Italia
- Settore: Costruzioni, Cave, Calcestruzzo, Conglomerati Bituminosi

## 🙏 Ringraziamenti

- Ispirato dalla necessità di prendere decisioni aziendali basate su dati reali, non entusiasmo
- Progettato per PMI che non possono permettersi errori costosi
- Creato con l'obiettivo di salvare tempo, soldi e mal di testa

## 📞 Supporto

Per domande o supporto:
- 📧 Email: [tua-email@fices.it]
- 🌐 Website: [https://fices.it]
- 💬 Issues: [GitHub Issues](https://github.com/TUO-USERNAME/fices-reality-check/issues)

---

## ⚡ Quick Start

```bash
# 1. Clone
git clone https://github.com/TUO-USERNAME/fices-reality-check.git

# 2. Deploy su GitHub Pages
# Settings → Pages → Source: main branch → Save

# 3. Apri
https://TUO-USERNAME.github.io/fices-reality-check/fices-reality-check.html
```

**Fatto! L'app è online e funzionante. Zero configurazione richiesta.**

---

## 📊 Statistiche Progetto

- **Dimensione**: ~50 KB (file singolo)
- **Dipendenze**: 0 (zero)
- **Tempo caricamento**: <1 secondo
- **Browser supportati**: 95%+ utenti globali
- **Mobile-first**: Ottimizzato per iPhone/Android

---

<div align="center">

**Smetti di sognare. Inizia a validare.**

[![Star on GitHub](https://img.shields.io/github/stars/TUO-USERNAME/fices-reality-check?style=social)](https://github.com/TUO-USERNAME/fices-reality-check/stargazers)

</div>
