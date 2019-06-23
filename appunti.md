# CIFRARI

Il **CIFRARIO** è un sistema che permette di:

- Cifrare
- Decifrare
- Generare e Gestire chiavi crittografiche.

Può essere:

- Aperto
- Chiuso

Definizioni

- **Plaintext** - testo prima della encryption
- **Ciphertext** - testo dopo l'encryption

## SIMMETRICI (chiavi condivise)

Caratteristiche:
- Mittente e Ricevente hanno la stessa chiave K
- Cifratura e decifratura sono efficienti
- Difficilissimo decifrare senza conoscere la chiave (essendo l'informazione necessaria)

#### Cifrari 'pre-informatici':

- **Character-oriented**
  - **Cifrario di Cesare**
    - monoalfabetici a 1 lettera
  - **Cifrario di Playfair** (monoalfabetico a 2 lettere)
  - **Cifrario di Vigenere** (polialfabetico)
- **Bit-oriented**
  - Cifrario di Vernam e one-time pad
- **A Sostituzione** - un gruppo di caratteri viene sostituito con un altro gruppo di caratteri
- **A Permutazione** - gruppi di caratteri vengono spostati nel testo
- Cifrari *monoalfabetici* a $N$ lettere - Ogni $N$-upla di lettere del testo viene sostituita sempre dalla stessa sequenza di lettere
- Cifrari *polialfabetici* - Una lettere o $N$-upla di lettere può essere **cifrata diversamente** a seconda della sua posizione nel testo

##### Cifrari monoalfabetici a 1 lettera

Come il cifrario di **Cesare**, ma la chiave $K$ identifica una sostituzione per ciascuna lettera (es. a-q, b-q, c-f,...):
*abcdefghilmnopqrstuvz*
*qzfabdeohilmnprstcugv*
**Esistono $N!$ diverse chiavi per $N$ lettere.**
- Non si può provare a decifrare manualmente (brute force) tutte le possibili chiavi (come in **Cesare**)
- Molto deboli a causa di *regolarità* statistiche 
  - **Crittanalisi Statistica** che considera la frequenza delle lettere del testo con la frequenza delle lettere in un linguaggio
  
##### Cifrari monoalfabetici a $N$ lettere

Ogni sequenza di $N$ lettere viene sostituita con una sequenza fissata di $N$ lettere. Per esempio (aa-qe, ab-zi, ba-df, ...)
- Migliore di $N=1$ (a una lettera)
- Rimane possibile **Crittanalisi statistica** (più il testo è lungo e più facile sarà)

##### Cifrario di Playfair (monoalfabetico $N=2$)

- Rimane possibile *Crittanalsi statistica*

##### Cifrari Polialfabetici


## ASIMMETRICI (chiavi diversi per cifratore e decifratore)