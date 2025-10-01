# act1

```
SceneSetup.act1();
```

(...300)

n: E QUESTA È L'ANSIA DELL'UMANA

n: _TU_ SEI L'ANSIA

{{if window.localStorage.continueChapter=="replay"}}
(#act1_replay)
{{/if}}

{{if window.localStorage.continueChapter!="replay"}}
(#act1_normal)
{{/if}}



# act1_replay

`hong({mouth:"0_neutral", eyes:"0_neutral"})`

h: Oh, ehi! Di nuovo qui?

`hong({eyes:"0_neutral"})`

n: IL TUO LAVORO È QUELLO DI PROTEGGERE L'UMANA DAL *PERICOLO*

`bb({eyes:"look", mouth:"small_lock"})`

n: IN VERITÀ, RIGIOCARE A QUESTO GIOCO LA STA METTENDO IN *PERICOLO* PROPRIO ORA

n: VELOCE, AVVISALA!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Umana! Ascolta, siamo in pericolo! Il giocatore...

[...ci vuole torturare di nuovo!](#act1_replay_torture)

[...non troverà un finale alternativo!](#act1_replay_alternate)

[...vedrà un contrasto con la trama!](#act1_replay_dissonance)

# act1_replay_torture

```
window.HACK_REPLAY = JSON.parse(localStorage.act4);
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

{{if window.HACK_REPLAY.act1_ending=="fight"}}
b: Ci farà raggomitolare e piangere!
{{/if}}

{{if window.HACK_REPLAY.act1_ending=="flight"}}
b: Ci farà rompere il telefono per averti dato un attacco di panico!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="fight"}}
b: Ci farà *NON* dare un pugno all'organizzatore della festa!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="flight"}}
b: Ci faranno dare un pugno al simpatico e anti-cattivo organizzatore della festa!!
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="jump"}}
h: Beh, almeno potremmo non saltare dal tetto questa vo--
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="walkaway"}}
b: CI FARÀ SALTARE GIÙ DAL TETTO.
{{/if}}

`bb({body:"fear"});`

b: TUTTE QUESTE COSE TERRIBILI CI ACCADRANNO, E POI NOI--

(#act1_replay_end)


#act1_replay_alternate

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Certo, la storia *completa* è uguale, ma ogni capitolo ha due finali possibili, oltre a tutte le diramazioni nelle rispos--

`bb({body:"fear"});`

b: Il giocatore ne sarà deluso, chiudi questa scheda, cancella il nostro software, e poi noi--

(#act1_replay_end)


# act1_replay_dissonance

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Un... come l'hai chiamato?

`bb({eyes:"normal"});`

b: La trama parlava di come tu puoi *SCEGLIERE* di avere un buon rapporto con la tua paura,

`bb({eyes:"normal_right"});`

b: Ma rigiocare il gioco avrà come risultato la stessa storia, quindi le tue *SCELTE* non importano veramente,

`bb({eyes:"narrow_eyebrow"});`

b: E quindi si mostra una contraddizione tra il messaggio e le meccaniche del gioco,

`bb({eyes:"fear"});`

b: Disgregando il tessuto di questo universo narrativo,

`bb({body:"fear"});`

b: E poi noi--

(#act1_replay_end)


# act1_replay_end

`bb({body:"panic"})`

b: MORIREMOOOOOOOOOOOOOO

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.clearText();
```

(...1001)

```
bb({body:"laugh"});
hong({body:"laugh"});
Game.clearText();
sfx("laugh");
```

(...5001)

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"0_sammich"});
```

h: Ok, torniamo nel personaggio.

```
Game.clearText();
```

n4: (LASCIA CHE LA _TUA_ ANSIA BLA BLA BLA PIÙ SIMILE A COSA DICE LA _TUA_ PAURA BLA BLA TANTO GIÀ LO SAI)

```
sfx("squeak");
hong({body:"0_squeeze"});
bb({body:"squeeze"});
```

(#act1_normal_choice)



# act1_normal

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: Oh, perfetto, il mio lupo è tornato. Faaaaantastico.

`hong({eyes:"0_neutral"})`

n: IL TUO LAVORO È PROTEGGERE L'UMANA DAL *PERICOLO*

`bb({eyes:"look", mouth:"small_lock"})`

n: IN VERITÀ, QUEL SANDWICH LA STA METTENDO IN *PERICOLO* PROPRIO ORA

n: VELOCE, AVVISALA!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Umana! Ascolta, siamo in pericolo! Il pericolo è...

`bb({body:"squeeze"})`

n4: (LASCIA CHE LA _TUA_ ANSIA GIOCHI AL POSTO TUO! SCEGLI LA COSA PIÙ SIMILE A COSA DICE LA _TUA_ PAURA)

(#act1_normal_choice)

# act1_normal_choice

[Stiamo mangiando da soli il pranzo! Di nuovo!](#act1a_alone) `bb({body:"squeeze_talk"})`

[Non siamo produttivi mentre mangiamo!](#act1a_productive) `bb({body:"squeeze_talk"})`

[Quel pane bianco ci fa male!](#act1a_bread) `bb({body:"squeeze_talk"})`

# act1a_alone

```
bb({body:"normal", mouth:"small", eyes:"narrow"});
hong({body:"0_sammich"});
```

b: Lo sai che la solitudine è associata alle morti premature tanto quanto fumare 15 sigarette al giorno?-

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: (Holt-Lunstad 2010, PLoS Medicine)

`hong({eyes:"0_annoyed"})`

h: Uhm, grazie per aver citato le fonti ma--

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: Questo significa che se non usciamo con qualcuno *ora* noi-

`bb({body:"panic"})`

b: MORIREMOOOOOOOOOOOOOO

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "alone");
publish("hp_show");
```

(...2500)

`_.fifteencigs = true`

n: HAI USATO *PAURA DI NON ESSERE AMATA*

(#act1b)

# act1a_productive

```
bb({body:"normal", mouth:"small", eyes:"normal"});
hong({body:"0_sammich"});
```

b: Tira fuori il portatile e lavora ora!

`hong({eyes:"0_annoyed"})`

h: Uhm, preferirei non avere briciole sulla mia tastie--

```
bb({mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Se non contribuiamo ad una società, siamo dei parassiti!

b: La società andrà dal dottore per una medicina contro i parassiti e--

```
bb({body:"panic", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: MORIREMOOOOOOOOOOOOOO

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "bad");
publish("hp_show");
```

(...2500)

`_.parasite = true`

n: HAI USATO *PAURA DI ESSERE UNA CATTIVA PERSONA*

(#act1b)

# act1a_bread

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich", eyes:"0_annoyed"});
```

h: Questi studi sono stati replica--

```
bb({body:"fear", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Il grano lavorato farà schizzare la glicemia e dovranno amputarci tutti gli arti e--

`bb({body:"panic"})`

b: MORIREMOOOOOOOOOOOOOO


```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "harm");
publish("hp_show");
```

(...2500)

`_.whitebread = true`

n: HAI USATO *PAURA DI ESSERE FERITA*

(#act1b)

# act1b

n: È SUPER EFFICACE

`bb({mouth:"smile", eyes:"smile"});`

b: Vedi, umana? Sono la tua fedele guardia-lupo!

`bb({body:"pride_talk"});`

b: Fidati del tuo istinto! I tuoi sentimenti sono sempre validi!

`bb({body:"pride"});`

n: PORTA L'ENERGIA DELLA TUA UMANA A ZERO

n: PER PROTEGGERE I SUOI BISOGNI FISICI + SOCIALI + MORALI, PUOI USARE:

n: PAURA DI *ESSERE FERITA* #harm#

n: PAURA DI *NON ESSERE AMATA* #alone#

n: E PAURA DI *ESSERE UNA CATTIVA PERSONA* #bad#

`Game.OVERRIDE_TEXT_SPEED = 1.25;`

n4: (SUGGERIMENTO: SCEGLI LE OPZIONI CHE TI COLPISCONO LE TUE PAURE PIÙ PROFONDE E OSCURE!~)

h: ...

```
hong({body:"putaway"});
sfx("rustle");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

(...1000)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h: sai forse è ora di controllare il telefono.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: PROTEGGI LA TUA UMANA

n: DAL MONDO. DAGLI ALTRI. DA SE STESSA.

n: BUONA FORTUNA

(...500)

`Game.clearText()`

(...500)

(#act1c)

# act1c

`music('battle', {volume:0.5})`

n: PRIMO ROUND: *LOTTA!*

`bb({body:"normal", mouth:"normal", eyes:"normal"});`

h: Ehm. Il mio feed Facebook dice che c'è una festa questo fine settimana.

`bb({eyes:"uncertain"});`

b: Non è quel pazzo che fa festa *ogni* weekend?

`bb({eyes:"uncertain_right"});`

b: Che vuoto interiore vuole riempire? Deve essere ridotto male, dentro!

`hong({eyes:"surprise"});`

h: E poi, ho ricevuto un invito?

`bb({eyes:"fear", mouth:"normal"});`

b: Bene allora!

[Dici sì, o moriremo di solitudine!](#act1c_loner)

[Dici no, è pieno di droghe velenose!](#act1c_drugs)

[Ignoralo, noi rendiamo le feste tristi e basta.](#act1c_sad)

# act1c_loner

{{if _.fifteencigs}}
b: Quindici sigarette al giorno, umana! Quindici!
{{/if}}

{{if !_.fifteencigs}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if !_.fifteencigs}}
b: E poi nessuno verrà al nostro funerale, butteranno le nostre ceneri nell'oceano, e verremo mangiati da una balena,
{{/if}}

{{if !_.fifteencigs}}
b: e diventeremo CACCA DI BALENA!
{{/if}}

{{if !_.fifteencigs}} `_.whalepoop = true` {{/if}}

(...500)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

{{if !_.fifteencigs}}
b: Quindi sì dovremmo andare alla festa!
{{/if}}

{{if _.parasite}}
b: Ma portiamo il portatile così possiamo lavorare, e non essere un parassita.
{{/if}}

{{if _.whitebread}}
b: Sempre che non ci sia PANE BIANCO
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: ODDIO. Se ti farà stare zitto, allora ok.

h: Dirò sì.

{{if _.whalepoop}}
b: Cacca di balena, umana! Cacca di balena!
{{/if}}

`_.partyinvite="yes"`

(#act1d)

# act1c_drugs

`bb({mouth:"small", eyes:"fear"});`

{{if _.whitebread}}
b: o anche peggio... PANE BIANCO
{{/if}}

{{if _.whitebread}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if _.whitebread}}
b: Andremo in overdose con così tante metanfetamine e pane bianco che non ce la faranno a metterci stare nel forno crematorio!
{{/if}}

{{if !_.whitebread}}
b: Andremo in overdose di così tante droghe che il becchino si chiederà come il nostro corpo può essere *già* pre-imbalsamato!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.parasite}}
b: Inoltre, non possiamo fare festa, dobbiamo lavorare o saremo dei parassiti!
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: ODDIO. Se ti farà stare zitto, allora ok.

h: Dirò no.

`_.partyinvite="no"`

(#act1d)

# act1c_sad

`bb({eyes:"uncertain_right", mouth:"normal"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.fifteencigs}}
b: Tutto ciò che facciamo è piangere in un angolo per quanto la solitudine sia mortale quanto 15 sigarette al giorno.
{{/if}}

{{if _.parasite}}
b: Tutto ciò che facciamo è preoccuparci di quanto dovremmo invece essere produttivi.
{{/if}}

{{if _.whitebread}}
b: Tutto ciò che facciamo è preoccuparci che il cibo non sano ci ucciderà.
{{/if}}

```
bb({mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"lookaway"});
```

h: Uh, chissà perché.

`hong({eyes:"neutral"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: Quindi se andiamo lo faremo sentire in colpa, ma se rifiutiamo il suo invito lo faremo sentire lo stesso in colpa!

`bb({body:"fear", eyes:"fear"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: TUTTO CIÒ CHE FACCIAMO È FAR STARE MALE LE PERSONE, QUINDI DOBBIAMO STARCI MALE

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`hong({mouth:"anger", eyes:"anger"});`

h: ODDIO. Se ti farà stare zitto, allora ok.

h: Ignorerò l'invito.

`_.partyinvite="ignore"`

(#act1d)

# act1d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"annoyed"});
```

h: Comunque. Facebook è troppo. Mi serve qualcosa di più tranquillo, che produca meno ansia.

`hong({eyes:"neutral"});`

h: Che novità ci sono su Twitter?

`bb({eyes:"look"});`

[Oh no, guarda quella terribile notizia!](#act1d_news)

[Oh no, quel tweet è segretamente su di *noi?*](#act1d_subtweet)

[Ehi, una GIF con un gatto che beve del latte](#act1d_milk)


# act1d_news

```
bb({eyes:"pained1"});
music(null, {fade:2});
```

b: Oddio, sembra quasi che il mondo stia bruciando, o sbaglio?

```
bb({eyes:"pained2"});
hong({mouth:"sad", eyes:"sad"});
```

b: Sembra che tutto stia finendo, come se tutto stesse morendo e fossimo tutti condannati e non ci fosse nulla da fare.

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
bb({mouth:"shut"});
```

b: ...

`bb({mouth:"smile", eyes:"smile"});`

b: Retweetiamolo!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.badnews=true`

```
music('battle', {volume:0.5});
hong({mouth:"anger", eyes:"anger"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Ok lo retweeto ma stai zitto!

`hong({mouth:"neutral", eyes:"annoyed"});`

h: Al diavolo, guardiamo Snapchat.

(#act1e)


# act1d_subtweet

`bb({eyes:"fear"});`

b: È un subtweet! Un subdolo, subdolo subtweet!

`hong({eyes:"annoyed"});`

h: Ma forse no?

`bb({eyes:"narrow", mouth:"small"});`

b: e se stessero tutti parlando di noi alle nostre spalle

h: Non lo stan--

`bb({body:"fear", eyes:"fear", mouth:"normal"});`

b: DAVANTI ALLE NOSTRE SPALLE

`hong({eyes:"sad", mouth:"sad"});`

h: Non pe--

`bb({eyes:"narrow", mouth:"small"});`

b: ma *se*

h: C--

`bb({eyes:"narrow_eyebrow"});`

b: *se*

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
hong({mouth:"shut"});
```

h: ...

(...1000)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.subtweet=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: o-KAY, proviamo ad andare su Snapchat.

(#act1e)

# act1d_milk

`hong({mouth:"smile", eyes:"neutral"});`

h: Eh eh sì carino, l'ho appena retweetato, pen--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: I GATTI NON RIESCONO A DIGERIRE IL LATTE E SIAMO DELLE PERSONE TERRIBILI PERCHÉ CI PIACE L'ABUSO SUGLI ANIMALI

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("18p", "bad");
```

(...2500)


`_.catmilk=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: o-KAY, proviamo ad andare su Snapchat.

(#act1e)

# act1e

`hong({mouth:"neutral", eyes:"neutral"});`

h: Ah, foto di ieri notte. Quindi *è così* che sono quelle feste del fine settimana.

{{if _.partyinvite=="yes"}} (#act1e_said_yes) {{/if}}

{{if _.partyinvite=="no"}} (#act1e_said_no) {{/if}}

{{if _.partyinvite=="ignore"}} (#act1e_said_ignore) {{/if}}

# act1e_said_yes

`hong({mouth:"sad", eyes:"annoyed"});`

h: Uff, sembra troppo affollato per la mia ansia.

h: Magari non avrei dovuto accettare l'invito?

```
hong({mouth:"neutral", eyes:"neutral"});
bb({mouth:"normal", eyes:"normal"});
```

[Cambiare la risposta? Come un'idiota?!](#act1e_yes_dontchange)

[Cambia la risposta! È troppo affollato!](#act1e_yes_changetono)

{{if _.subtweet}}
[Sì, stavano sicuramente subtweetando su di noi.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Aspetta abbiamo retweetato senza fact-checking.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Lo sai che hai una cattivissima postura?](#act1e_ignore_posture)
{{/if}}

# act1e_yes_dontchange

```
bb({eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Contavano che noi andassimo e ora tradiamo la loro fiducia? Vuoi morire da sola?!

{{if _.fifteencigs}}
b: QUINDICI. SIGARETTE.
{{/if}}

{{if _.whalepoop}}
b: CACCA. DI. BALENA.
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Basta basta ci vado!

(#act1f)

# act1e_yes_changetono

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Non sai cosa sono le fughe di massa?

```
bb({body:"fear", mouth:"small", eyes:"narrow"});
hong({eyes:"sad", mouth:"sad"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Nel 2003 un nightclub di Rhode Island ha preso fuoco e il panico ha fatto ammassare le persone alle uscite e 100 persone sono morte nel fuoco-

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({mouth:"shock"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: VUOI CHE ACCADA A NOI-

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 2.5;
```

b: DICI NO DICI NO DICI NO DICI NO DICI NO DICI NO DICI NO DICI N-


```
bb({body:"normal", eyes:"fear", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
hong({eyes:"anger", mouth:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Basta basta cambierò la mia risposta in no! Oddio!

(#act1f)

# act1e_said_no

`hong({mouth:"sad", eyes:"sad"});`

h: Hm... sembra molto divertente.

h: Magari non avrei dovuto rispondere no all'invito?

`bb({mouth:"normal", eyes:"normal"});`

[Cambiare la risposta? Come un'idiota?!](#act1e_no_dontchange)

[Cambia la risposta! Non morire da sola!](#act1e_no_changetoyes)

{{if _.subtweet}}
[Sì, stavano sicuramente subtweetando su di noi.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Aspetta abbiamo retweetato senza fact-checking.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Lo sai che hai una cattivissima postura?](#act1e_ignore_posture)
{{/if}}

# act1e_no_dontchange

`bb({eyes:"anger"})`

b: Tutti contavano su di noi!

b: ...di lasciarli in pace e fargli avere una bella festa senza una disgustosa e orribile {{if _.whitebread}}rosicchiatrice di pane bianco{{/if}} strana come t--


```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
bb({body:"normal", eyes:"uncertain", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Basta basta non vado!

(#act1f)

# act1e_no_changetoyes

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: La solitudine cronica aumenta il nostro livello di cortisolo e ci fa rischiare malattie cardiovascolari e infarto!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.fifteencigs}}
b: QUINDICI. SIGARETTE.
{{/if}}

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Basta basta cambierò la mia risposta in sì! Oddio!

(#act1f)

# act1e_ignore_subtweet

```
bb({eyes:"fear", mouth:"small"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Tutti i nostri tweet problematici stanno tornando a farsi sentire!

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.7;
```

b: Ci metteranno alla gogna, ci cancelleranno e ci trascineranno con una corda a cavallo sull'autostrada dell'informazione!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Perché sei così?!

(#act1f)

# act1e_ignore_factcheck

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Stiamo diffondendo disinformazione! Stiamo distruggendo la fiducia nella stampa libera!

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Siamo il motivo per cui il fascismo risorgerà dalle macerie della democrazia!

```
bb({body:"normal", eyes:"anger"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
_.factcheck = true;
```

h: Perché sei così?!

(#act1f)

# act1e_ignore_posture

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Vuoi avere un pretzel come spina dorsale?! Smettila di rannicchiarti sullo schermo!

```
bb({body:"meta"});
```

b: Questo è rivolto anche a te.

```
bb({body:"normal", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Perché sei così?!

(#act1f)

# act1e_said_ignore

`hong({mouth:"sad", eyes:"sad"});`

h: Hm... sembra molto divertente.

h: Magari non avrei dovuto ignorare l'invito?

`bb({mouth:"normal", eyes:"normal"});`

[Continua ad ignorarlo, siamo solo dei guastafeste.](#act1e_ignore_continue)

[Infatti, dici sì.](#act1e_ignore_changetoyes)

[Infatti, dici no.](#act1e_ignore_changetono)

# act1e_ignore_continue

`hong({eyes:"annoyed"});`

h: È un po' maleducato continuare ad ignorarli, no?

`bb({eyes:"normal_right"});`

b: Beh, gli altri *ci* ignorano sempre, quindi

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

b: quindi diciamo che siamo pari.

(#act1f)

# act1e_ignore_changetoyes

`hong({eyes:"surprise", mouth:"smile"});`

h: Mi stai... lasciando divertire?

b: Beh, come ho detto, la solitudine *può* ucciderci.

`hong({eyes:"neutral", mouth:"neutral"});`

(#act1e_no_changetoyes)

# act1e_ignore_changetono

`bb({eyes:"narrow"});`

b: È troppo affollato. La folla è pericolosa.

(#act1e_yes_changetono)


# act1f

```
hong({mouth:"neutral", eyes:"neutral"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: Vabbè. Nuova notifica di Tinder.

`bb({eyes:"uncertain"})`

b: Cosa, l'app di incontri?

`hong({eyes:"annoyed"})`

h: Non è un'app di incontri, è un modo di conoscere nuove perso--

`bb({eyes:"narrow"})`

b: È un'app di incontri.

```
hong({eyes:"surprise", mouth:"smile"});
bb({eyes:"normal"});
```

h: Oh, ho fatto match! E non sembra male!

```
bb({eyes:"narrow_eyebrow"});
hong({eyes:"sad", mouth:"anger"})
```

h: Per favore non rovinarmelo--

```
bb({body:"panic"});
Game.OVERRIDE_TEXT_SPEED = 2.0;
```

b: PERICOLO PERICOLO PERICOLO PERICOLO PERICOLO PERICOLO

`bb({body:"fear", eyes:"fear", mouth:"normal"})`

[Siamo *usati* dagli altri.](#act1f_used_by_others)

[Stiamo *usando* gli altri.](#act1f_using_others)

[IL TUO MATCH È UN SERIAL KILLER](#act1f_killer)

# act1f_used_by_others

`bb({body:"point_crotch", eyes:"normal", mouth:"normal"})`

b: Incontri random potrebbero essere capaci di riempire il buco lì in basso,

b: ma non potranno mai riempire il buco...

`bb({body:"point_heart", eyes:"pretty", mouth:"small"})`

b: *qui*.

(...1000)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Il punto è che MORIREMO DA SOLI

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.hookuphole=true`

(#act1g)

# act1f_using_others

`bb({eyes:"narrow", mouth:"small"})`

b: Pensi che i genitali degli altri siano dei Pokémon da collezionare?

```
bb({body:"sing", eyes:"pretty", mouth:"shut"});
music("pokemon");
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

```
Game.FORCE_TEXT_DURATION = 1000;
Game.FORCE_NO_VOICE = true;
```

b: ♫ (sigla dei pokemon)-

(...5600)

```
bb({mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2400;
```

b: ♫ Voglio essere la più ^puttana^-

(...500)

```
bb({eyes:"narrow", mouth:"small"});
Game.FORCE_TEXT_DURATION = 2100;
```

b: ♫ Come nessun altro mai-

(...1500)

```
bb({eyes:"pretty"});
Game.FORCE_TEXT_DURATION = 2300;
```

b: ♫ Cosce e ^culo^, seno prosperoso-

(...500)

```
bb({eyes:"fear", mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2000;
```

b: ♫ Con ^cazzo^ sudato e palle!-

(...1000)

```
bb({eyes:"smile", mouth:"smile"});
Game.FORCE_TEXT_DURATION = 1000;
```

b: ♫ PERVERTITO-MON! ACCHIAPPALI TU-

```
Game.FORCE_CANT_SKIP = false;
Game.clearText();
music(false);
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Il fatto è che siamo dei manipolatori infami.

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`_.pokemon=true`

(#act1g)

# act1f_killer

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.whitebread}}
b: Ti intrappolerà in un pozzo e ti costringerà a mangiare pane bianco per farti ingrassare e poi usare la tua pelle come vestito!
{{/if}}

{{if _.parasite}}
b: Ti massacrerà con un pomodoro timer e ti dirà "DOVEVI ESSERE PIÙ PRODUTTIVA, PARASSITA"
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Ti scorticherà fino a ridurti in macabri coriandoli, trasformerà le tue interiora in festoni, e mescolerà il tuo sangue in una ciotola per punch!
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Allora, che ne pensi di un invito DEL GENERE?!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.serialkiller=true`

(#act1g)

# act1g

```
bb({body:"normal", mouth:"normal", eyes:"look"});
hong({body:"2_tired"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
music(false);
```

h: ...

(...500)

h: sono stanca di questo gioco.

(...700)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h:
{{if _.fifteencigs}}"la solitudine ci ucciderà"... {{/if}}
{{if _.parasite}}"siamo parassiti della società"... {{/if}}
{{if _.whitebread}}"non mangiarlo, ci ucciderà"... {{/if}}
{{if _.subtweet}}"stanno parlando alle nostre spalle"... {{/if}}
{{if _.badnews}}"il mondo sta bruciando"... {{/if}}
{{if _.hookuphole}}"moriremo soli"... {{/if}}
{{if _.serialkiller}}"è un serial killer"... {{/if}}
{{if _.catmilk}}"i gatti non digeriscono il latte"... {{/if}}
{{if _.pokemon}}una canzone di ^merda^... {{/if}}

h: voglio solo vivere la mia vita.

h: voglio solo essere libera da tutto questo... dolore.

`bb({eyes:"look_sad"});`

b: Ehi... umana...

`Game.OVERRIDE_TEXT_SPEED = 0.5;`

b: Andrà tutto bene.

(...600)

`bb({body:"point_heart", eyes:"look_sad_smile", mouth:"smile"});`

b: Come fedele guardia-lupo, sarò sempre all'erta, e farò il mio meglio per tenerti al sicuro.

`bb({body:"normal", eyes:"look_sad", mouth:"smile"});`

b: Lo prometto.

(...600)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({body:"phone1", eyes:"neutral", mouth:"neutral"});
```

h: Ultima app. Instagram. Cosa c'è?

`hong({eyes:"sad"});`

h: Sono... altre foto di feste.

`hong({mouth:"sad"});`

h: Sembrano tutti così felici. Liberi dalle preoccupazioni. Liberi dall'ansia.

`hong({mouth:"anger"});`

h: Oddio, perché non posso essere come loro? Perché non posso essere *normale?*

`bb({eyes:"normal_right"});`

b: Parlando di feste, riguardo all'invito di questo weekend. Questa è la mia decisione FINALE:

`bb({eyes:"normal"});`

[Dovremmo andare.](#act1g_go) `Game.OVERRIDE_CHOICE_LINE=true`

[Non dovremmo andare.](#act1g_dont) `Game.OVERRIDE_CHOICE_LINE=true`

# act1g_go

`_.act1g = "go"`

(#act1h)

# act1g_dont

`_.act1g = "dont"`

(#act1h)

# act1h

b: --

```
bb({eyes:"wat", mouth:"small"});
hong({body:"2_fuck"});
```

h: *^VAFFANCULO^.*

`hong({body:"2_you"});`

h: A TE.

(...500)

b: c

(...1500)

`bb({eyes:"wat_2"});`

b: cosa?

`hong({body:"phone1", eyes:"anger", mouth:"anger"});`

h: Dirò SÌ all'invito,

{{if _.act1g=="go"}}
h: NON perché tu vuoi che io vada, ma perché *IO* lo voglio.
{{/if}}

{{if _.act1g=="dont"}}
h: Proprio PERCHÉ non vuoi che vada.
{{/if}}

```
hong({body:"putaway"});
sfx("rustle");
```

h: Tu NON mi controlli.

```
sfx("rustle2");
hong({body:"0_sammich", eyes:"0_annoyed", mouth:"0_neutral"});
```

h: Ora scusami ma vorrei mangiare questo panino delizioso in ^fottuta^ pace.

`hong({body:"2_sammich_eat"});`

(...601)

```
sfx("sandwich");
hong({body:"2_sammich_eaten", eyes:"0_lookaway", mouth:"0_chew1"})
```

(...601)

```
bb({body:"normal", eyes:"uncertain", mouth:"shut"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
```

b: ...

```
bb({eyes:"normal_right"});
Game.OVERRIDE_TEXT_SPEED = 1;
```

b: ...

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 4;
```

b: ..................

(...500)

`bb({mouth:"normal"});`

[AHHHH MORIREMO](#act1h_death) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH TUTTI CI ODIANO](#act1h_loneliness) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH SIAMO PERSONE ORRIBILI](#act1h_worthless) `Game.OVERRIDE_CHOICE_LINE = true;`

# act1h_death

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH MORIREMO AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "harm");
```

(...2500)

(#act1i)

# act1h_loneliness

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH TUTTI CI ODIANO AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "alone");
```

(...2500)

(#act1i)

# act1h_worthless

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH SIAMO PERSONE ORRIBILI AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "bad");
```

(...2500)

(#act1i)

# act1i

```
bb({mouth:"smile_lock", eyes:"smile", body:"normal"});
music('battle', {volume:0.5});
```

n: CONGRATULAZIONI

(...500)

n: HAI PROTETTO CON SUCCESSO I BISOGNI FISICI + SOCIALI + MORALI DELLA TUA UMANA

n: MA GUARDALA, QUANTO È RICONOSCENTE!

(...500)

n: ORA CHE LA SUA ENERGIA È A ZERO, PUOI DIRETTAMENTE CONTROLLARE LE SUE AZIONI

`bb({mouth:"smile", eyes:"normal"});`

n: SCEGLI LA TUA MOSSA FINALE

`bb({mouth:"small_lock", eyes:"fear"});`

n: *ELIMINALA*

[{LOTTA: Punisci il tuo telefono stressante!}](#act1i_phone) `Game.OVERRIDE_CHOICE_LINE=true`

[{SCAPPA: Raggomitolati e piangi!}](#act1i_cry) `Game.OVERRIDE_CHOICE_LINE=true`

# act1i_phone

`bb({mouth:"normal", eyes:"narrow"})`

b: Il tuo telefono ti stava provocando un attacco di panico!

`bb({eyes:"anger"})`

b: Zuckerberg e compagnia stanno mandando alla deriva la tua salute mentale per mero denaro accumulato in capitale!

```
bb({body:"fear", eyes:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Punisci il tuo telefono! Distruggilo! Uccidilo!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "fight";
```

b: UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCI--

(#act1j)

# act1i_cry

`bb({eyes:"fear", mouth:"normal"})`

b: Tutto il mondo è pieno di pericoli!

```
bb({body:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Fai come gli armadilli! Raggomitolati come difesa!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "flight";
```

b: RAGGOMITOLATI E PIANGI RAGGOMITOLATI E PIANGI RAGGOMITOLATI E PIANGI RAGGOMITOLATI E PIANGI RAGGOMITOLATI E PIANGI RAGGOMITOLATI E PI-- 

(#act1j)

# act1j

`SceneSetup.act1_outro()`