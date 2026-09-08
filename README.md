# Codifica Digitale in TEI/XML: *La Lupa* di Giovanni Verga

Progetto di filologia digitale incentrato sull'edizione, l'annotazione critica e la modellizzazione prosopografica della novella ***La Lupa*** di **Giovanni Verga** (da *Vita dei campi*, 1880), conforme alle linee guida della **Text Encoding Initiative (TEI P5)**.

Il lavoro costituisce la componente applicativa e digitale della mia **Tesi di Laurea Triennale in Lettere Moderne** presso l'Università degli Studi di Catania, focalizzata sull'intersezione tra critica letteraria, questioni di genere e standard computazionali per il testo.

---

## 👤 Autrice
* **Denise Covone**  
  *Elaborato di Tesi di Laurea Triennale in Lettere Moderne*  
  *Università degli Studi di Catania*

  ---

## 🎯 Obiettivi e Focus dell'Annotazione

L'attività di codifica si concentra in particolare su tre livelli analitici:

1. **Modellizzazione Prosopografica (`<listPerson>`):**
   * Strutturazione delle entità biografiche e relazionali dei protagonisti (*Lupa/gnà Pina*, *Maricchia*, *Nanni*).
   * Rilevazione dell'onomastica e dei soprannomi popolari, evidenziando il contrasto tra l'identità anagrafica individuale e l'etichettamento sociale della comunità rurale.

2. **Toponomastica e Simbolismo del Territorio (`<listPlace>`):**
   * Mappatura dei luoghi chiave del paesaggio rurale siciliano (l'*Etna/Mongibello*), analizzati sia nella loro funzione geografica sia come matrici simboliche.

3. **Annotazione Semantica ed Esegetica (`<seg>`):**
   * **Superstizione e giudizio corale:** marcatura delle espressioni legate alla percezione diabolica e sacrilega della protagonista negli occhi della comunità paesana.
   * **Dinamiche di genere e lavoro rurale:** analisi della rottura degli stereotipi patriarcali (il lavoro manuale nei campi riservato agli uomini, la gestione autonoma della casa e della dote).
   * **Pulsione, fatalismo e paremiologia:** tracciamento dei detti popolari (es. *«fra vespero e nona»*) e della progressiva trasformazione del rapporto vittima-carnefice tra Nanni e la Lupa.

---

## ⚙️ Struttura del Documento TEI

* **`teiHeader`:** 
  * `<fileDesc>`: metadati bibliografici sull'edizione di riferimento e attestazione di responsabilità editoriale.
  * `<sourceDesc>`: banche dati entitarie strutturate con `<listPerson>` e `<listPlace>`, collegate direttamente ai nodi testuali tramite identificatori univoci (`xml:id`).
* **`text / body`:**
  * Trascrizione integrale della novella strutturata in paragrafi (`<p>`), con rinvii puntuali mediante l'attributo `ref="#id"` verso le entità marcate nell'header (`<persName>`, `<placeName>`) e categorizzazione tipologica dei segmenti esegetici (`<seg type="...">`).

---

## 🛠️ Tecnologie e Standard
* **Linguaggio di marcatura:** XML (Extensible Markup Language)
* **Standard di codifica:** TEI P5 (Text Encoding Initiative)
