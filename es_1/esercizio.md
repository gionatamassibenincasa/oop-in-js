# Esercitazione Guidata: Introduzione alla Programmazione Orientata agli Oggetti
**Ambiente di lavoro:** BlueJS (Simulatore Web)  
**Durata:** 60 minuti  
**Linguaggio di riferimento:** JavaScript (Approccio *Objects-First*)

---

## 🎯 Obiettivi dell'Esercitazione
1. Comprendere la differenza fondamentale tra **Classe** (il modello) e **Oggetto** (l'istanza).
2. Capire cos'è lo **Stato** di un oggetto (i suoi attributi/campi).
3. Capire cos'è il **Comportamento** di un oggetto (i suoi metodi/funzioni).
4. Sperimentare l'indipendenza degli oggetti (modificare un oggetto non influenza gli altri).

---

## 🚀 Fase 1: Esplorazione dell'Ambiente (15 minuti)

1. Apri il file `index.html` fornito dal docente nel tuo browser.
2. Osserva la struttura dello schermo:
   * **Diagramma delle Classi:** L'area grigia principale. Il box giallo `Circle` rappresenta la **Classe**.
   * **Banco degli Oggetti (Object Bench):** L'area in basso dove prenderanno vita i nostri oggetti.
   * **Visualizzazione Mondo:** Lo schermo nero sulla destra dove vedremo gli effetti grafici.
   * **Ispettore Oggetto:** La tabella che mostra i dati interni dell'oggetto selezionato.

### ✍️ Domande di Riflessione (Fase 1):
* Fai click sulla classe `Circle` e seleziona `new Circle()`. Ripeti l'operazione una seconda volta.
* *Quante classi sono presenti nel diagramma?* __________
* *Quanti oggetti sono apparsi in basso nel banco degli oggetti?* __________

---

## 🛠️ Fase 2: Metodi e Stato (15 minuti)

Un **Oggetto** è composto da due elementi fondamentali: i **Metodi** (le azioni che sa fare) e lo **Stato** (le sue caratteristiche in un preciso momento).

1. Fai click destro sull'oggetto rosso `circle1` posizionato nel banco in basso.
2. Apparirà un menu con una lista di funzioni: quelli sono i suoi **Metodi**.
3. Clicca sul metodo `makeVisible()`. 
4. Ora fai un click normale (sinistro) su `circle1` e osserva la tabella dell'**Ispettore Oggetto** a destra.

### ✍️ Compila la Tabella dello Stato:
Esegui i metodi richiesti su `circle1` e annota come cambiano i valori nell'ispettore:

| Azione (Invocazione del Metodo) | Valore di `isVisible` | Valore di `xPosition` | Valore di `color` |
| :--- | :--- | :--- | :--- |
| **Appena creato (Stato iniziale)** | `false` | `20` | `blue` |
| **Dopo `makeVisible()`** | __________ | __________ | __________ |
| **Dopo `moveRight()` (eseguito 2 volte)** | __________ | __________ | __________ |
| **Dopo `changeColor()`** | __________ | __________ | __________ |

---

## 🏁 Fase 3: La Sfida del Semaforo (20 minuti)

Ora che hai capito come interagire con gli oggetti, usa il simulatore per risolvere questo problema logico e visivo.

### 📝 Richiesta:
Configura il banco degli oggetti e il mondo visivo per riprodurre un **Semaforo Orizzontale**. Alla fine dell'esercizio il tuo schermo nero dovrà mostrare tre cerchi affiancati con i seguenti colori, da sinistra a destra: **Rosso, Verde, Magenta**.

### 🛠️ Passaggi da seguire:
1. Crea tre oggetti distinti dalla classe `Circle` (si chiameranno `circle1`, `circle2`, `circle3`).
2. Rendi tutti e tre gli oggetti visibili nel mondo tramite il metodo corretto.
3. Utilizza i metodi `moveRight()` e `changeColor()` sui singoli oggetti in modo indipendente per posizionarli e colorarli correttamente.
   * *Suggerimento:*
