1. **Discutere il concetto di non disconoscibilità nella firma elettronica.**
    Il documento informatico munito di firma digitale o firma elettronica avanzata sembrerebbe in realtà non disconoscibile;
    Infatti per verificare la firma apposta su un foglio è necessario procedere ad un esame grafologico, nel caso di documento informatico sottoscritto con firma digitale basta verificare la corrispondenza della firma con la chiave pubblica del presunto sottoscrittore per accertarne la provenienza. Conseguentemente, il disconoscimento della firma digitale **sarebbe precluso**, perché con la corrispondenza tra la chiave pubblica e la chiave privata vengono accertate  sia la **provenienza** del documento che **l’assenza di alterazioni** del medesimo.
    L’unica ipotesi di falsità materiale che può configurarsi (atteso che le alterazioni materiali del documento sono da escludere grazie alla funzione di hash), è che la firma sia apposta da **persona diversa dal legittimo proprietario** del dispositivo di firma. Di conseguenza, l'oggetto del disconoscimento non sarà relativo alla firma ma all'effettivo utilizzo della firma digitale da parte del titolare. 

2. **Dimostrare:**
$(ab)\ mod\  M = (a \ mod\ M)(b\ mod\ M)\ mod\  M$

    Siano 
   - $a\ mod \ M = x$ con $x < M$
   - $b\ mod \ M = y$ con $y < M$

    Allora $(\exists k, j)$ tale che:
   - $Mk+x=a$
   - $Mj+y=b$

    Pertanto:

    $(ab)\ mod\  M = ((Mk+x)(Mj+y))\ mod\ M=$
    $= ((MkMj+Mky+Mjx+xy))\ mod\ M=$
    $=xy\ mod\ M=(a \ mod\ M)(b\ mod\ M)\ mod\  M$
    rimane $xy$ perché gli altri sono tutti multipli di $M$

3. **La firma grafometrica:**
   comprende la scansione della firma autografa e altri dati biometrici cifrati
4. **Un cifrario a sostituzione monoalfabetica**
   sostituisce ad una n-upla di lettere del testo in chiaro un'altra n-upla di lettere, in base ad una sostituzione che non può mai cambiare man mano che si procede nello scorrimento del testo.
5. **Un MAC (Message Authentication Code)**
    autentica un messaggio con una chiave simmetrica