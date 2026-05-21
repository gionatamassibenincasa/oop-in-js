# Foglio di lavoro - Objects First con BlueJS
**Titolo:** Il cerchio magico  
**Durata prevista:** circa 30 minuti  
**Ambiente di lavoro:** BlueJS (simulatore web)  
**Linguaggio di riferimento:** JavaScript

---

## Obiettivi di apprendimento
Al termine dell'attivita dovresti saper:

1. distinguere tra **classe** e **oggetto**;
2. riconoscere lo **stato** di un oggetto osservando ispettore e JSON;
3. invocare i **metodi** di un oggetto con la sintassi tipica di JavaScript;
4. verificare che una modifica allo stato produca subito un effetto visibile nell'interfaccia.

---

## Regole di lavoro

Lavora principalmente nella **console JavaScript** in basso.

- Esegui **un solo comando per volta**.
- Per creare un oggetto usa una dichiarazione come:
  - `const c = new Circle();`
  - `let d = new Circle();`
- Per invocare un metodo usa la sintassi ordinaria:
  - `c.makeVisible();`
  - `c.moveRight();`
  - `c.changeColor();`
- Per selezionare un oggetto nell'interfaccia puoi scrivere solo il suo nome:
  - `c`

Ogni volta che esegui un comando, controlla subito quattro aree:

1. **Banco degli Oggetti**
2. **Visualizzazione Mondo**
3. **Ispettore Oggetto**
4. **JSON Oggetto**

---

## Fase 1 - Creazione e riconoscimento degli oggetti (8 minuti)

### Attivita

1. Crea un primo oggetto con il comando:
   `const c = new Circle();`
2. Crea un secondo oggetto con un nome diverso:
   `let d = new Circle();`
3. Scrivi `c` nella console e osserva quali pannelli cambiano.
4. Scrivi `d` nella console e confronta con il caso precedente.

### Domande guida

1. Quante **classi** vedi nel diagramma? __________
2. Quanti **oggetti** compaiono nel banco dopo i primi due comandi? __________
3. Qual e la differenza tra il nome della classe `Circle` e i nomi `c`, `d`?  
   ____________________________________________________________
4. In quale pannello leggi lo stato interno dell'oggetto in forma tabellare?  
   ____________________________________________________________

---

## Fase 2 - Stato e comportamento (10 minuti)

Lavora sull'oggetto `c`.

### Sequenza di comandi

1. `c.makeVisible();`
2. `c.moveRight();`
3. `c.moveRight();`
4. `c.changeColor();`

Dopo **ogni** comando, fermati e osserva se il cambiamento e immediatamente visibile nel mondo, nell'ispettore e nel JSON.

### Tabella da completare

| Comando eseguito | `isVisible` | `xPosition` | `color` | Cosa cambia nella GUI? |
| :--- | :--- | :--- | :--- | :--- |
| Stato iniziale di `c` | `false` | `20` | `blue` | __________________ |
| Dopo `c.makeVisible();` | ________ | ________ | ________ | __________________ |
| Dopo `c.moveRight();` | ________ | ________ | ________ | __________________ |
| Dopo il secondo `c.moveRight();` | ________ | ________ | ________ | __________________ |
| Dopo `c.changeColor();` | ________ | ________ | ________ | __________________ |

### Domanda di riflessione

Quando invochi un metodo, cambia la **classe** o cambia lo **stato dell'oggetto**?  
____________________________________________________________

---

## Fase 3 - Due oggetti, due storie diverse (7 minuti)

Adesso confronta `c` e `d`.

### Attivita

1. Rendi visibile `d` con `d.makeVisible();`
2. Sposta `d` una sola volta con `d.moveRight();`
3. Cambia colore a `d` due volte.
4. Seleziona prima `c` e poi `d` scrivendo i loro nomi nella console.

### Osservazioni da scrivere

1. `c` e `d` hanno lo stesso stato finale? Perche?  
   ____________________________________________________________
2. Quale prova mostra che gli oggetti della stessa classe possono evolvere in modo indipendente?  
   ____________________________________________________________

---

## Fase 4 - Mini sfida finale (5 minuti)

Usa **solo la console** per ottenere questa configurazione finale:

- `c` visibile, spostato di due passi verso destra;
- `d` visibile, spostato di un passo verso destra;
- `c` e `d` con colori diversi.

### Spazio per i comandi usati

1. ________________________________________
2. ________________________________________
3. ________________________________________
4. ________________________________________
5. ________________________________________

### Verifica finale

Spiega in 3-4 righe come l'interfaccia ti aiuta a capire cosa succede quando scrivi un comando nella console.  
____________________________________________________________  
____________________________________________________________  
____________________________________________________________

---

## Estensione facoltativa

Se hai finito in anticipo, prova questa variante:

1. crea un nuovo oggetto con `let e = new Circle();`
2. rendilo visibile;
3. confronta il suo JSON con quello di `c` e `d`.

Quali campi sono uguali? Quali cambiano?  
____________________________________________________________
