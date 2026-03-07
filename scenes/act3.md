# act3

```
SceneSetup.act3();
Game.WORDS_HEIGHT_BOTTOM = 205;
sfx("cheers");
```

r: Alla salute!

```
publish("act3",["roofhunter",1]);
publish("act3",["roofhong",1]);
sfx("drinking");
```

(...4001)

```
publish("act3-alpha", ["dizzyhunter",1]);
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",3]);
```

h2: *Ah*, questo ha preso il punto in pieno.

```
publish("act3",["roofhunter",2]);
publish("act3",["roofhong",2]);
```

r: Lo sai, ragazza...

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",6]);
```

h2: Nello specifico, i punti presi in pieno sono la mia amigdala destra e sinistra.

```
publish("act3",["roofhunter",8]);
publish("act3",["roofhong",5]);
```

r: Mi ricordi di quando ero più giovane. Quando ero tormentato dall'animale nella mia testa.

```
publish("act3",["roofhunter",9]);
publish("act3",["roofhong",2]);
```

r: Sono così felice che però ora posso aiutarti ad uccidere il tuo animale nello stesso modo in cui ho ucciso il mio.

```
publish("act3",["roofhunter",2]);
```

r: Ehi, piccola domanda: obbligo o ve--

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",7]);
publish("act3-alpha", ["dizzyhong",0]);
```

h2: OBBLIGO!

```
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",2]);
```

r: Haha! Bene.

```
publish("act3",["roofhunter",21]);
publish("act3",["roofhong",4]);
```

r: Ok. La vedi quella piscina azzurra lì giù?

```
publish("act3-alpha", ["dizzyhong",0]);
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",9]);
```

h2: Sì? Sei piani più in giù?

```
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",8]);
```

r: Salta.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",10]);
```

h2: ...

```
publish("act3",["roofhong",11]);
```

h2: Aspetta, cosa?

```
publish("act3",["roofhong",10]);
publish("act3",["roofhunter",2]);
```

r: L'animale sta iniziando a lamentarsi, o sbaglio?

```
publish("act3",["roofhunter",23]);
```

r: *Nooooo, è pericoloso, non farloooo.*

```
publish("act3",["roofhunter",22]);
```

r: Ma questo è l'esatto motivo per cui ci servono queste esperienze da brivido! Fare festa alla grande! Carpe diem! Farsi di coca sul ^culo^ di una prostituta, #YOLO!

```
publish("act3",["roofhunter",10]);
```

r: Fai vedere a quell'animale che non ce ne sbattono due *^cazz^i* dei suoi piagnistei! Salta.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",13]);
```

h2: Uh, ma, ogni tanto, um... la paura c'è per un motivo...

```
publish("act3",["roofhunter",5]);
publish("act3",["roofhong",12]);
music(null, {fade:2});
```

r: ...

```
publish("act3-alpha", ["dizzyhunter",0]);
publish("act3",["roofhunter",6]);
publish("act3",["dd",1]);
```

r: Scusami, sei caduta per quella propaganda McMindfulness che sostiene che sentirsi male sia *faccia bene?*

```
publish("act3",["roofhunter",17]);
```

r: Quegli ^stronzi^ che gestiscono la società a *noi* lasciano solo ansia e depressione,

```
publish("act3",["roofhunter",18]);
```

r: E poi fanno i TED Talk per dirci di "accettare" di essere ^fottuti^ da loro, e di "ascoltare" il demone sadico nella nostra testa!

```
publish("act3",["roofhunter",6]);
```

r: Ragazza, io so che *tu* lo sai che quell'animale *fa male* alle persone come noi. *Tortura* le persone come noi.

```
publish("act3",["roofhunter",19]);
```

r: Non è nostro amico. È una bestia con la rabbia, che deve, o essere *tranquillizzata*,

```
publish("act3",["roofhunter",20]);
```

r: O ricevere *una pallottola in testa*.

```
publish("act3",["roofhunter",27]);
```

r: Altrimenti, in questo modo lo lascerai vincere.

```
publish("act3",["roofhunter",31]);
publish("act3",["roofhong",14]);
publish("act3",["dd",2]);
```

h2: No. Ti sbagli.

```
publish("act3",["roofhunter",13]);
publish("act3",["roofhong",15]);
music('battle_dark', {volume:1.0}, function(){
	music('battle_dark_loop');
});
```

h2: Non lo lascerò vincere.

```
publish("act3",["roofhunter",25]);
publish("act3-alpha", ["roofhong",0]);
publish("act3-alpha", ["transition",1]);
publish("act3",["dd",6]);
```

r: ^Cazzo^ sì! Credo in te! Uccidilo! <3

(#act3a)



# act3a

```
Game.clearText();
publish("act3-out");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
_.act3_bb_body = 1;
```

(...1500)

```
publish("hp_show");
```

b: no no no no no no

n: QUESTO CAPITOLO HA DUE FINALI POSSIBILI. UNO È *MOLTO, MOLTO BRUTTO.*

b: NO NO NO NO NO NO NO NO NO NO NO NO NO NO

n: SCEGLI SAGGIAMENTE. PROTEGGI LA TUA UMANA

`bb({ eyes:"oh_crap", mouth:"normal_talk", MOUTH_LOCK:true });`

b: AAAAAAAAAAAAAAAAAA

`bb({ mouth:"normal" });`

n: BUONA FORTUNA

```
Game.clearText();
bb({ eyes:"start" });
```

[Umana, potresti letteralmente MORIRE!](#act3a_harm) `Game.OVERRIDE_CHOICE_LINE=true`

[Fare questo è stupido e autodistruttivo!](#act3a_bad) `Game.OVERRIDE_CHOICE_LINE=true`

[Questa gentaglia non è veramente tua amica!](#act3a_alone) `Game.OVERRIDE_CHOICE_LINE=true`

# act3a_harm

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: U--

(#act3a_after)

# act3a_alone

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: F--

(#act3a_after)

# act3a_bad

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: Q--

(#act3a_after)

# act3a_after

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Lo sai, avrei potuto crederti... se non lo avessi già provato a fare migliaia di volte prima.

h: Tu sei il lupo che ha urlato "al lupo".

```
bb({ eyes:"sad" });
```

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_harm"`

[](#act3_fork) `_.SPECIAL_ATTACK="harm"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_alone"`

[](#act3_fork) `_.SPECIAL_ATTACK="alone"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_bad"`

[](#act3_fork) `_.SPECIAL_ATTACK="bad"; Game.OVERRIDE_CHOICE_LINE=true`


# act3_fork

```
Game.clearText();
bb({body:"special_attack"});
sfx("charging");
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
Game.FORCE_CANT_SKIP = false;
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Hai provato anche questo.

b: umana, per favore...

`hong({ eyes:"look_right" });`

h: Oh mi *dispiace* che Big Pharma non approvi la mia automedicazione.

h: Guarda ^stronzo^, abbiamo *tutti* un modo per farti stare ^fottutamente^ zitto.

`hong({ body:"look_up", eyes:"look_up" });`

h: Alcune persone si mettono al lavoro.

`hong({ body:"look_down", eyes:"look_down" });`

h: Altre si buttano nel giro del sesso, della droga, e nel refresh del feed Facebook.

`hong({ body:"normal", eyes:"look_right" });`

h: Altre ancora si buttano su altre persone. 

`hong({ eyes:"angry" });`

h: E io invece mi butterò in quella piscina.

[Sei ubriaca ed è SEI PIANI PIÙ GIÙ](#act3_bad_1_harm)

[Cavolo, ed è questo il ringraziamento che mi dai?!](#act3_bad_1_insult) `bb({eyes:"angry"});`

[Ok, lo ammetto. Ho sbagliato.](#act3_good_1) `bb({mouth:"sorry", eyes:"sorry_down"});`

# act3_bad_1_harm

b: Anche se atterri sull'acqua, la tensione superficiale ti romperà le costole e ti provocherà una commozione cerebrale, *quantomeno!*

h: Eh.

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Una volta ho visto un tipo russo farlo su YouTube.

(#act3_bad_2)

# act3_bad_1_insult

`hong({ eyes:"look_right" });`

h: I- Scusa, il *ringraziamento?*

`bb({ eyes:"angry" });`

b: Questo è esattamente il motivo per cui *esisto!* Perché gli umani non riescono a proteggersi da soli!

b: Ho provato a parare il tuo stupido ^culo^ per tutta la mia vita e tu vuoi sol--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)

# act3_good_1

`hong({ body:"laugh_1" })``

h: heh.

`hong({ body:"laugh_2" })``

h: hahahaha

`hong({ body:"laugh_3" })``

h: HAHAHAHAHAHA

```
bb({ eyes:"sorry"});
hong({ body:"yell_1", mouth:"yell", eyes:"blank" });
```

h: Oh WOW questo è il più grande *^cazzo^* di eufemismo del secolo!

`hong({ body:"yell_2" });`

h: Sì, pila di ^merda^ sanguinolenta in putrefazione! Hai fatto un ^cazzo^ di casino!

`hong({ body:"normal", mouth:"angry", eyes:"angry" });`

h: Altre osservazioni, Signor Ovvio?

[Ma vendicarsi su di me non è la soluzione!](#act3_good_1_fail_revenge) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Ma questa volta ho *davvero* ragione!](#act3_good_1_fail_harm) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Ti ho fatto del male.](#act3_good_2a)


# act3_good_1_fail_revenge

b: Dovresti avere una relazione più sana con le tue emozioni, invece di farle affogare con--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)



# act3_good_1_fail_harm

b: Quindi, per piacere, metti giù la bottiglia e facciamo--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)




# act3_bad_2

`bb({ eyes:"sad" });`

b: per piacere... non farlo...

h: La tua energia sembra piuttosto bassa, caro lupo.

h: Se fossi in te, sceglierei le mie prossime parole con cura.

`bb({ eyes:"normal" });`

[Bene. Non ti proteggerò più.](#act3_bad_2_jump) `bb({ mouth:"ignore", eyes:"ignore" });`

[Ho sempre avuto ragione.](#act3_bad_2_right)

[Mi dispiace.](#act3_good_2b) `bb({mouth:"sorry", eyes:"sorry_down"});`


# act3_bad_2_jump

b: Quindi, vai, salta. E vedrai se ci tengo a te.

`hong({ eyes:"look_right", mouth:"normal", MOUTH_LOCK:true });`

h: ...

```
hong({ eyes:"less_angry", mouth:"normal" });
bb({ eyes:"ignore_oh_crap" });
```

h: Allora ok. Cin cin.

```
bb({ mouth:"normal", eyes:"oh_crap" });
Game.OVERRIDE_TEXT_SPEED = 2;
```

b: NO ASPETTA ERA PSICOLOGIA INVERSA AVRESTI DOVUTO FARE L'*OPPOSTO* DI QUELLO CHE HO DET--

(#act3_bad_3)



# act3_bad_2_right

`bb({ eyes:"angry" });`

b: Tu *ti stai* mettendo in pericolo. I tuoi cosiddetti amici *ti stanno* usando. E *tu* stai usando i tuoi cosiddetti amici.

`bb({ eyes:"sad" });`

b: Quindi per favore, umana... perché non mi credi?!

h: Perché tu non hai mai creduto in *me*.

(#act3_bad_3)


# act3_bad_2_terrible

`bb({ eyes:"angry" });`

b: Altri lupi-guardia hanno avuto umani che hanno speso tempo ad addestrarli pazientemente, per *imparare* a lavorare insieme,

b: Piuttosto che odiare i lupi-guardia per aver provato a proteggerli! Quindi perché non puo--

`bb({ eyes:"normal" });`

h: Risposta sbagliata, ^cazzo^.

(#act3_bad_3)



# act3_bad_3

```
music(null);
hong({body:"drink"});
bb({body:"attacked"});
publish("bb_STOP_VIBRATING");
attackBB("100p");
```

(...2000)

```
hong({ body:"normal", mouth:"normal", eyes:"normal" });
bb({ body:"dead" });
```

(...999)

h: *"L'unica cosa di cui aver paura è la paura stessa."*

`hong({ body:"look_up", mouth:"happy", eyes:"blank" });`

h: *"Non preoccuparti, sii felice"*

`hong({ body:"normal", mouth:"normal", eyes:"normal" });`

h: Tutti i saggi di questa generazione sono d'accordo: le emozioni negative sono *cattive!*

`hong({ eyes:"less_angry" });`

h: Ma dai! È per quello che sono chiamate *negative!*

b: umana... per favore...

`hong({ eyes:"normal" });`

h: Un po' di tempo fa, ho detto: “Voglio solamente essere libera da tutto questo dolore.”

h: E il mio desiderio si è esaudito. Non sento più dolore, paura, o ansia...

h: Non sento assolutamente niente.

`_.a3_ending = "jump";`

(#act3_end)



# act3_good_2a

`bb({mouth:"sorry", eyes:"sorry_down"});`

b: Ero così impegnato a fare in modo che niente ti facesse male, che non mi sono accorto che ero *io* ciò che ti faceva male.

```
bb({ eyes:"sorry"});
hong({ body:"yell_2", mouth:"yell", eyes:"blank" });
```

h: NO. C^AZZO^.

`hong({ body:"yell_1" });`

h: ^MALEDIZIONE^. Ti ci è veramente voluto così tanto per capirlo?!

`hong({ body:"cry", mouth:"cry", eyes:"blank" });`

h: Avresti potuto evitarci così tanti problemi, stupido idiota peloso. Perché non te ne sei accorto prima?...

`_.apologized_for_hurt = true;`

(#act3_good_2q)



# act3_good_2b

`hong({ body:"normal", mouth:"angry", eyes:"look_right" });`

h: ...ti *dispiace.*

`hong({ eyes:"angry", MOUTH_LOCK:true });`

h: ...

h: Ma ti dispiace per *cosa*?

(#act3_good_2q)


# act3_good_2q

`bb({mouth:"sorry", eyes:"sorry"});`

{{if _.apologized_for_hurt}}
(#act3_good_2q_already_apologized)
{{/if}}

{{if !_.apologized_for_hurt}}
(#act3_good_2q_not_already_apologized)
{{/if}}


# act3_good_2q_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"less_angry" });`

[Di non essere stato un buon protettore.](#act3_good_3_protector)

[Mi dispiace di non averti rispettata.](#act3_good_3_respect)

[Mi dispiace.](#act3_good_4)


# act3_good_2q_not_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"angry" }, 0);`

[Mi dispisce di avere un'umana terribile!](#act3_bad_2_terrible) `bb({mouth:"normal", eyes:"normal"})`

[Mi dispiace di non averti rispettata.](#act3_good_3_respect)

[Mi dispiace di averti fatto del male.](#act3_good_3_hurt)



# act3_good_3_protector

`bb({eyes:"sorry_down"});`

b: È il mio dovere avvisarti di pericoli *veri*, ma continuavo ad abbaiare anche alle macchine e al postino.

`bb({eyes:"sorry_up"});`

b: Abbaiare alle ombre. Abbaiare così tanto.

`bb({eyes:"sorry"});`

b: Comprendo che mi vuoi mettere la museruola.

`bb({eyes:"sorry_down"});`

b: Mi dispiace.

(#act3_good_4)



# act3_good_3_respect

`bb({eyes:"sorry_down"});`

b: Sarei dovuto essere il *tuo* fedele cane da guardia, ma ho agito come se tu avessi dovuto *obbedirmi*.

`bb({eyes:"sorry_up"});`

b: C'è differenza tra un protettore e un guardiano della prigione, e io ho superato il limite.

`bb({eyes:"sorry_down"});`

b: Mi dispiace.

(#act3_good_4)



# act3_good_3_hurt

`bb({eyes:"sorry_down"});`

b: Ero così impegnato a fare in modo che niente ti facesse male, che non mi sono accorto che ero *io* ciò che ti faceva male.

`bb({eyes:"sorry_up"});`

b: Ero un cane cattivo.

`bb({eyes:"sorry_down"});`

b: Mi dispiace.

(#act3_good_4)


# act3_good_4

```
music(null,{fade:3});
hong({ eyes:"less_angry", MOUTH_LOCK:true },0);
```

h: ...

```
hong({ body:"stop", mouth:"stop", eyes:"blank" });
```

h: Eh sì, beh, era un'idea stupida questa comunque.

h: Lo ho fatto solo per incasinarti, e, beh, ci sono riuscita.

h: Questa volta siamo pari, ok?

```
bb({ mouth:"sorry", eyes:"sorry" });
bb({ MOUTH_LOCK:true });
```

b: ...

b: Ok.

h: Ok.

n: *PARI*

`_.a3_ending = "walkaway";`

(#act3_end)









# act3_end

```
Game.clearText();
publish("act3-in");
publish("hp_hide");
Game.FORCE_CANT_SKIP = true;
```

{{if _.a3_ending=="walkaway"}}
(#act3_walkaway)
{{/if}}

{{if _.a3_ending=="jump"}}
(#act3_jump)
{{/if}}






# act3_walkaway

```
publish("start-walkaway-anim");
Game.WORDS_HEIGHT_BOTTOM = 205;
```

(...3501)

```
sfx("bottle_toss");
publish('hong-next');
publish("act3",["roofhunter",7]);
```

(...667)

```
publish("act3",["dd",4]);
publish("act3",["roofhunter",26]);
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("concrete_step2");
```

(...667)

```
publish('hong-next');
publish("act3",["roofhunter",27]);
```

`Game.FORCE_CANT_SKIP = false;`

r: Oh *andiamo*. Dopo tutto quello che il tuo animale ti ha fatto, *rinunci?*

r: Che ti succede, ragazza? Hai *paura?*

```
publish('hong-next');
publish("act3",["roofhunter",26]);
```

h2: Sì.

h2: Ho paura.

`publish('hong-next')`

h2: E questo è ok!

`publish('hong-next')`

h2: È giusto avere paura.

`publish('hong-next')`

(...500)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1167)

```
publish('hong-next');
```

(...833)

```
publish('hong-next');
sfx("rustle2");
```

(...1333)

```
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",31]);
sfx("concrete_step4");
```

(...667)

```
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("door");
```

(...1333)

```
publish('hong-next');
sfx("concrete_step2");
```

(...501)

```
publish('hong-next');
Game.FORCE_CANT_SKIP = false;
sfx("lock_door");
publish("act3",["roofhunter",32]);
```

(...2001)

```
publish("act3",["roofhunter",33]);
```

r: Ha davvero chiuso la porta?

```
Game.clearAll();
_.INJURED = false;
Game.WORDS_HEIGHT_BOTTOM = -1;
```

(...2000)

(#act4)




# act3_jump

```
publish("start-jump-anim");
Game.FORCE_TEXT_Y = 300;
```

(...2001)

```
publish('hong-next');
sfx("bottle_toss");
```

(...833)

```
sfx("concrete_step1");
sfx("claps");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",28]);
```
(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step2");
publish('hong-next');
publish("act3",["roofhunter",28]);
```

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",34]);
```

(...1167)

```
sfx("rustle2");
publish('hong-next');
```

(...1001)

`publish('hong-next')`

b: no...

(...501)

`Game.clearText();`

`publish('hong-next')`

(...1333)

```
sfx("quack");
publish('hong-next');
```

(...1333)

`publish('hong-next')`

b: no no no

(...501)

`Game.clearText();`

`publish('hong-next')`

(...2001)

```
sfx("rustle2");
publish('hong-next')
```

(...501)

```
sfx("concrete_step1");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",30]);
```

(...167)

```
sfx("concrete_step2");
publish('hong-next');
```

(...167)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",2]);
publish("act3",["roofhunter",15]);
```

(...167)

```
sfx("bottle_slip");
publish('hong-next');
publish("act3",["dd",3]);
publish("act3",["roofhunter",16]);
```

(...833)

```
sfx("rustle");
publish('hong-next');
```

(...167)

`publish('hong-next')`

(...167)

```
publish('hong-next');
Game.FORCE_TEXT_Y = 325;
Game.OVERRIDE_FONT_SIZE = 50;
```

b: NO!

(...400)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-injury-show");
publish("hide_tabs");
```

(...2000)

```
sfx("hospital1");
publish("act4-injury", [1]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital2");
publish("act4-injury", [2]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital3");
publish("act4-injury", [3]);
```

(...8000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...5500)

`_.INJURED = true;`

(#act4)
