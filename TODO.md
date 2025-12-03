# Ordini del giorno

## 26/11

- **Task 2**

  - **Facciamo post-processing?**

    - [ ] togliamo punteggiatura inizio?
    - [ ] compattiamo punteggiatura ripetuta?
    - [ ] compattiamo spazi
    - [ ] rimuoviamo spazi inizio e/o fine?
  - **Discutere di strani aspetti di lemmatization e tokenizzazione**

    - [X] Va bene che i doppi apici (") iniziali diventino `` e quelli finali '' ?
    - [X] I'm diventa i 'm e non i be

    UPDATE: probabilmente hanno senso era solo per segnalarlo
  - **Discutere regex**

    - [ ] Vogliamo inserire `re.compile(r'[ᵃᵇᶜᵈᵉᶠᵍʰⁱʲᵏˡᵐⁿᵒᵖʳˢᵗᵘᵛʷˣʸᶻᴬᴮᴰᴱᴳᴴᴵᴶᴷᴸᴹᴺᴼᴾᴿᵀᵁⱽᵂ]+')` anche se appare una volta tra i tweets e recita:
      "Are you ever at work and just look at someone and you're likeʸᵒᵘ ˡᵒᵒᵏ ˡⁱᵏᵉ ᵃ ᵇⁱᵗᶜʰ "
    - [ ] Vogliamo considerare `re.compile(r'[↕↔→←↑↓⇒⇐⇑⇓⇔⟵⟶⟷⤴⤵]'),` anche se in realtà ci serve solo `↕` dato cche sembra impossibile eliminare l'emoji ️↕️
    - [ ] Come consideriamo i tentativi di emoji sbagliati o emoji straniere particolari come
      "@Ellars It's stupid Russian Federation army force, they're thinking that Chernobyl is still for us a strategic object)))"
      **NB: cercando online ho trovato che ))) è un'emoticon russa/slava equivalente a :) o 😂**
    - [ ] Come vogliamo considerare gli asterischi? a volte sono ad indicare dei bullets e a volte indicano una parola in bold
    - [ ] Come gestiamo i separatori? a volte vengono usati ___ o ::: o ---, secondo me potrebbero diventare singoli spazi
    - [ ] Come gestire l'uso di ~ ? Indica un todo da flirt
    - [ ] A volte usano +, -, _ a inizo frase per simulare una lista
