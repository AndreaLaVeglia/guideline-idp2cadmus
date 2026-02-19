# Guida pratica all'utilizzo di Cadmus

INDICE
- [1.1 Aggiunta di item](#11-aggiunta-di-item)
- [1.2 Aggiunta di part](#12-aggiunta-di-part)

Cadmus è un framework di descrizione modulare, nel senso che offre la possibilità di strutturare le informazioni in moduli componibili. In particolare l'architettura di Cadmus è costituita da **_items_** e da **_parts_**.  


## 1.1 Aggiunta di un  _item_

L'_item_ è come una scatola che contiene al suo interno elementi correlati tra loro e riferiti al contenitore che sono le _parts_.  
Dunque possiamo utilizzare l'_item_ per identificare un manoscritto o un'unità codicologica, la cui descrizione analitica si articolerà con l'inserimento di diverse _parts_ (Cf. [Documentazione di Cadmus](https://cadmus.fusi-soft.com/docs/data-architecture)). 

Dunque per aggiungere un ms al database di Cadmus è necessario creare un nuovo _item_, andando sul bottone in basso a sinistra nella visualizzazione dell'editor di Cadmus_NDP.

![aggiunta item](./additem.png)<figcaption>Aggiunta di un item in Cadmus.</figcaption>

### Metadati identificativi (identity)

Per la creazione di un nuovo _item_ bisogna inserire i seguenti metadati obbligatori che costituiscono l'etichetta (_**label**_) dell'_item_: 
- `title` 
- `description` 
- `facet`provvede ad indicare la tipologia di item, specificando dunque se si tratti di manoscritti, disegni o stampe, oppure di un item iconografico o di una persona.

### Flags

I flags sono le "bandierine" che segnalano lo stato editoriale della catalogazione dell'oggetto di riferimento (ms, frg, ...) in Cadmus.

> NB Dal momento della creazione dell'item bibliologico fino al suo completamento, per segnalare agli altri contributori che è ancora in lavorazione, bisogna selezionare lo stato di `draft`. 
Dopo il completamento della scheda si potrà selezionare `complete` e togliere la spunta a `draft`.

## 1.2 Aggiunta di _part_

Un elemento _part_ è un **set di dati** coerente che si riferisce all'item al quale viene correlato (Cf. [Documentazione di Cadmus](https://cadmus.fusi-soft.com/docs/data-architecture)).  
DUnque, dopo aver creato un _item_ si può procedere alla parte fondamentale del lavoro, ossia l'aggiunta delle parti di Cadmus utili a descrivere l'item bibliologico in questione.  
Si veda di seguito lo screenshot di esempio per l'aggiunta di una parte. 

![Aggiunta di Part](addpart.png)<figcaption>Aggiunta di un item in Cadmus.</figcaption>

### 1.2.1 Aggiunta della part `metadata`con EID e autore

La prima part da aggiungere è `metadata` per attribuire all'_item_ un EID (ID human friedly) e le informazioni sui catalogatori

#### EID 

 L'EID è strutturato convenzionalmente secondo le seguenti parti:

1. indica il *facet* 
2. sigla standard della città di provenienza o di edizione;
3. sigla della biblioteca o archivio in cui è contenuto il manufatto da descrivere; 
4. parte numerica della segnatura del manoscritto o dell'incunabolo 

**1** e **2** sono separate da un underscore ( **_** ), le altre parti da un trattino intermedio ( **-** )

Quindi nel caso del manoscritto mediceo l'EID risulta: `ms_fi-bml-86`

>NB tutte le lettere sono minuscole

#### Indicazioni sull'autorialità della scheda

- `author` indica l'autore della catalogazione nell'ambiente Cadmus nel caso in cui abbia fatto un lavoro di catalogazione  "di prima mano"
- `revisor` indica l'autore della catalogazione nell'ambiente Cadmus nel caso in cui abbia fatto un lavoro di catalogazione  "di seconda mano"
- `IDP author` indica l'autore della scheda in IDP (In IDP è visualizzato in fondo alla scheda, alla voce **Autore/i della scheda (sezione IDP)** [corrisponde a `IDP_autoriIDP`])
- `IDP revisor` indica il revisore della scheda in IDP (In IDP è visualizzato in fondo alla scheda, alla voce **Revisore/i della scheda (sezione IDP)** [corrisponde a `IDP_revisoriIDP`])
- `MOL author` indica l'autore della scheda in MOL (In IDP è visualizzato in fondo alla scheda, alla voce **Autore/i della scheda (sezione MOL)** [corrisponde a `IDP_autoriMOL`])
- `MOL revisor` indica il revisore della scheda in MOL (In IDP è visualizzato in fondo alla scheda, alla voce **Revisore/i della scheda (sezione MOL)** [corrisponde a `IDP_revisoriMOL`])  

[torna all'indice](#linee-guida-per-il-trasferimento-di-schede-da-idp-a-cadmus)

## 4. Aggiunta della bibliografia (references)


[torna all'indice](#linee-guida-per-il-trasferimento-di-schede-da-idp-a-cadmus)



