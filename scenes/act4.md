# act4

```
SceneSetup.act4();
publish("SAVE_GAME", ["act4"]);
Game.FORCE_CANT_SKIP = true;
```

(...5001)

```
publish("set_how_many_prompts", [1]);
Game.FORCE_CANT_SKIP = false;
Game.CLICK_TO_ADVANCE = true;
```

n3: (salvataggio automatico effettuato)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
var hong_frame = _.INJURED ? 9 : 0;
publish("act4", ["hong_walks_in",hong_frame]);
sfx("grass_step1", {volume:0.1});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.2});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.25});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.3});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...1667)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...1333)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.20});
```

(...167)

```
publish("act4_hong_sits");
```

(...66)

```
publish("act4", ["hong_transition", "next"]);
sfx("squeak");
```

(...133)

`publish("act4", ["hong_transition", "next"]);`

(...1333)

```
publish("act4", ["hong_transition", "next"]);
sfx("rustle");
```

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1001)

```
publish("act4", ["hong_transition", "next"]);
```

(...333)

```
publish("act4", ["hong_transition", 9]);
sfx("sandwich");
```

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1466)

`publish("act4-out-1");`

(...201)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

```
publish("act4-show-chars");
Game.FORCE_CANT_SKIP = false;
```

(...901)

`hong({body:"sigh_1"})`

(...601)

```
hong({body:"sigh_2"});
bb({eyes:"look_down"});
```

h: *sigh*

```
hong({body:"hold", eyes:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Quindi quale ^cazzo^ era il morale di questa storia?

`hong({body:"one_up", eyes:"annoyed"})`

h: Che cosa abbiamo *imparato*? Che io *ero* una stupida, i miei "amici" mi *stavano* usando, e che siamo quasi *morti*.

`hong({body:"normal", eyes:"normal"})`

{{if _.INJURED}}
[Sì, e non dimenticare il conto dell'ospedale.](#act4a_bill)
{{/if}}

{{if !_.INJURED}}
[Sì, e non dimenticare i danni al fegato.](#act4a_liver)
{{/if}}

[Sì, *era* lo scenario peggiore.](#act4a_worst)

[Sì, avevo ragione.](#act4a_right)

# act4a_bill

`hong({eyes:"annoyed_l", mouth:"narrow"});`

h: Giusto. Mi sa che la mia assicurazione non copre "essere un'idiota".

`hong({eyes:"annoyed", mouth:"normal"});`

b: Ma... siamo sopravvissuti!

`hong({eyes:"normal"});`

h: ?

(#act4b)

# act4a_liver

`bb({eyes:"normal_d"});`

b: Abbiamo sicuramente accorciato la nostra vita di qualche anno...

`bb({eyes:"surprise"});`

b: Ma almeno ce l'*abbiamo* ancora una vita! Siamo sopravvissuti!

```
hong({eyes:"surprise"});
bb({eyes:"normal"});
```

h: ?

(#act4b)

# act4a_worst

`bb({eyes:"normal_d"});`

b: Ma...

h: Hm?

`bb({eyes:"surprise"});`

b: Siamo sopravvissuti!

(#act4b)

# act4a_right

`bb({eyes:"normal_d"});`

b: Ma... avevi ragione anche tu.

`hong({eyes:"surprise"});`

h: Hm?

`bb({eyes:"normal"});`

b: Io *ero* il lupo che ha urlato "al lupo". Quindi quando un *vero* pericolo si è avvicinato, tu – comprensibilmente – non mi hai creduto.

`bb({eyes:"surprise_r"});`

b: Ma, siamo sopravvissuti!

(#act4b)

# act4b

```
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

b: Nonostante tutto, siamo ancora qui.

`hong({eyes:"suspect"});`

{{if _.INJURED}}
h: Sembri piuttosto calma considerando che sei quasi morta.
{{/if}}

{{if !_.INJURED}}
h: Sembri piuttosto calma considerando che sei quasi quasi-morta.
{{/if}}

```
hong({eyes:"normal"});
bb({eyes:"annoyed_d", mouth:"narrow"});
```

b: Beh, rende tutto il resto meno spaventoso. E mi ha anche fatto pensare.

`bb({eyes:"normal", mouth:"normal"});`

b: Se lottare contro di te fa schifo, perché non ti protegge...

h: Ma *anche* lottare contro di te fa schifo, perché ti fa solo urlare di più...

`bb({eyes:"normal_r"})`

b: Quindi magari...

`bb({eyes:"normal"})`

h: Magari non dobbiamo lottare.

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
```

(...301)

`publish("smash",[0]);`

(...2001)

```
publish("smash",[1]);
sfx("smash_glass");
```

(...2601)

```
publish("smash",[2]);
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

(...2001)

`Game.FORCE_CANT_SKIP = false;`

(#act4b_2)

# act4b_2

```
music('dontfight',{fade:5, volume:0.6});
bb({eyes:"annoyed_d"});
```

b: Non sono un Grande Lupo Cattivo. Ma non sono neanche un lupo da guardia.

`bb({eyes:"sad_d"})`

b: Sono un malconcio cane da canile.

`bb({eyes:"sad"})`

b: Abbiamo passato momenti difficili. Magari traumi o abbandono. È per questo che reagisco in modo esagerato ogni tanto e:

```
sfx("yaps", {volume:0.6});
bb({body:"yap_1"});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 215;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: YAP YAP YAP YAP YAP

(...1884)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_CANT_SKIP = false;
bb({body:"normal", mouth:"scream", eyes:"scream_sad"});
```

b: Ma non *voglio* essere un cane codardo! Voglio proteggerti! Voglio essere un buon cane!

`bb({eyes:"sad", mouth:"normal"});`

b: Umana... vorresti domare questo lupo?

`hong({eyes:"sad"})`

h: Ci... Ci voglio provare.

`hong({eyes:"normal_l", body:"chin", mouth:"narrow"})`

h: Ok. Relazioni sane con le proprie emozioni. Alle relazioni serve comunicazione. Quindi, comunichiamo.

`hong({eyes:"normal", body:"hands_1", mouth:"normal"})`

h: I prossimi cinque minuti saranno super sdolcinati, ma fingiamo fino alla fine.

```
hong({body:"hands_2", mouth:"normal"});
```

h: Caro lupo interiore... come *ti* senti?

n2: TOTALE PAURE USATE:

n2: *ESSERE FERITA* {{_.attack_harm_total}}, *NON ESSERE AMATA* {{_.attack_alone_total}}, *ESSERE UNA CATTIVA PERSONA* {{_.attack_bad_total}}

n2: DI CHE PAURA VUOI PARLARE PER PRIMA? (LE ALTRE PUOI SCEGLIERLE DOPO)

```
_.a4_fears_discussed = 0;
_.num_thanks = 0;
hong({body:"normal"});
bb({eyes:"normal"});
```

[Ho paura di essere ferita.](#act4_harm)

[Ho paura che resterò da sola.](#act4_alone)

[Ho paura di essere una cattiva persona.](#act4_bad)

# act4_harm

```
_.a4_talked_about_harm = true;
_.a4_fears_discussed += 1;
```

`bb({eyes:"normal_d"})`

b: Io voglio proteggere la tua sicurezza fisica,

`bb({eyes:"sad_d"})`

b: Ma il *mondo intero* sembra così pericoloso. Pieno di tragedie e malvagità.

`bb({eyes:"sad"})`

{{if _.a4_fears_discussed==1}}
b: Non lo so, facciamo che adesso scegli *tu* di cosa parlare. Che ne dici, umana?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Ancora, è il tuo turno, umana. Che ne pensi?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Vuoi altre riflessioni, umana?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Hai ragione. Proteggiamoci.](#act4_harm_skills)

[Esponiamoci a *più* pericolo.](#act4_harm_exposure)

[Grazie.](#act4_thanks) `_.thanks_for = "sicurezza fisica";`

# act4_harm_skills

`bb({eyes:"look_down", body:"paw"})`

b: Ma... come? Ho zanne e artigli, ma è solo una metafora.

```
bb({ body:"normal", eyes:"normal" });
hong({ body:"one_up", eyes:"surprise" });
```

h: Possiamo imparare l'autodifesa? Entrare in una comunità che si protegge a vicenda? Migliorare la nostra salute e lavorare sui confini personali?

```
bb({ eyes:"annoyed_r" });
hong({ body:"normal", eyes:"normal" });
```

b: Magari, ma...

[Da cosa possiamo partire?](#act4_harm_skills_start)

[E se ancora non funziona?](#act4_harm_skills_work)

[E se esageriamo con la "sicurezza"?](#act4_harm_skills_overboard)

# act4_harm_skills_start

`bb({ eyes:"sad_d" })`

b: C'è così tanto da fare, così tanto che dobbiamo sistemare di noi. Da dove dovremmo *partire*?

`hong({ body:"shrug", eyes:"surprise" })`

h: Stiamo partendo già ora.

`bb({ eyes:"normal", mouth:"narrow" })`

b: Eh?

```
bb({ body:"normal", mouth:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal"});
```

h: Ci stiamo esercitando con una buona comunicazione proprio ora. Che ci aiuterà a riconoscere meglio il pericolo, con meno falsi positivi,

`hong({ eyes:"surprise" });`

h: E *questo* ci aiuterà a proteggerci dal male!

`hong({ eyes:"normal", mouth:"normal" });`

h: Quindi: questo *è* allenamento all'autodifesa.

`bb({ eyes:"normal_r" })`

b: Huh. Mi aspettavo anche del:

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
hong({ eyes:"sad", mouth:"smile" });
bb({ body:"karate_1" });
sfx("hiya");
```

(...1001)

`Game.FORCE_CANT_SKIP = false;`

(#act4_something_else)

# act4_harm_skills_work

`bb({ eyes:"normal" });`

h: Vero, non c'è un modo per proteggerci al 100%...

`hong({ body:"one_up" });`

h: Ma anche per un miglioramento dell'1% ne vale la pena, giusto?

```
bb({ eyes:"annoyed" });
hong({ normal:"one_up" });
```

b: Stai vedendo il bicchiere non come 99% vuoto, ma 1% pieno?

`bb({ eyes:"normal" });`

h: Ma ne vale la pena se sei assetato e bloccato in un deserto.

`bb({ eyes:"closed" });`

b: Beh. Alla salute, allora.

(#act4_something_else)

# act4_harm_skills_overboard

`bb({ body:"chest", eyes:"annoyed" })`

b: Intendo, il motivo per cui ignoravi i miei avvertimenti è che *io* ho esagerato! 

`bb({ body:"normal", eyes:"normal" })`

h: Nah, hai ragione. Vogliamo avere sicurezza con moderazione. Tutto con moderazione

`bb({ eyes:"suspect" })`

b: Scusa, *TUTTO* con moderazione?

`hong({ eyes:"annoyed" })`

h: *Un numero moderato di cose* con moderazione.

```
bb({ eyes:"closed" });
hong({ eyes:"normal" });
```

b: Grazie per aver reso almeno le tue dichiarazioni coerenti.

(#act4_something_else)


# act4_harm_exposure

`bb({ mouth:"scream_talk", eyes:"scream", MOUTH_LOCK:true });`

b: *COSA*

```
bb({ mouth:"narrow", eyes:"suspect" });
hong({ body:"one_up" });
```

h: Intendo, diciamo che un cane è spaventato dai tuoni.

`hong({ body:"hands_1" });`

h: Un trucco che hanno gli addestratori è riprodurre una registrazione di tuoni a volume basso, e poi dare una ricompensa al cane per essere stato calmo.

`hong({ body:"hands_2" });`

h: In più giorni, l'addestratore aumenta il volume di un po', fino a quando il cane non ha più paura dei tuoni.

```
hong({ body:"normal", eyes:"surprise" });
bb({ mouth:"normal", eyes:"normal" });
```

h: Si chiama terapia dell'esposizione!

`hong({ body:"point", eyes:"normal" });`

h: E visto che sei un cane, funzionerà anche con te, giusto? Tutti i mammiferi hanno lo stesso comportamento di lotta o fuga.

`hong({ body:"normal" });`

[E se ci desensibilizziamo *troppo*?](#act4_harm_exposure_overboard)

[E se siamo esposti a un *vero* pericolo?](#act4_harm_exposure_hurt)

[Sono un lupo, non un cane.](#act4_harm_exposure_dog) `bb({ eyes:"suspect" })`

# act4_harm_exposure_dog

h: E ti tratterò con gentilezza e pazienza finché non sarai addomesticato e diventerai un cucciolo carino.

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"sad", mouth:"smile" })`

b: Che tenerezza.

(#act4_something_else)

# act4_harm_exposure_overboard

`bb({ eyes:"annoyed" })`

b: Abbiamo *appena* visto quello che succede se ignori le tue paure – ti metti in situazioni che sono *davvero* pericolose.

`bb({ eyes:"angry_r", body:"one_up" })`

b: Detto questo, essere *troppo* desensibilizzati non ci farà diventare psicopatici?

`bb({ mouth:"scream", eyes:"scream", body:"two_up" })`

b: Presto ci ricompenseremo da soli mentre guardiamo porno sadici con omicidi!

`hong({ eyes:"annoyed" })`

h: Io... penso che ci sia della differenza tra questo e i tuoni.

`bb({ body:"normal", mouth:"normal", eyes:"suspect" })`

b: Ma esattamente *dove*, umana? *Dove?!*

`hong({ eyes:"surprise", body:"one_up" })`

h: Non lo so. Ma *tu* puoi aiutarmi!

`hong({ eyes:"normal", body:"normal" })`

h: Lavorando insieme, la scriveremo quella differenza.

`bb({ body:"paw", mouth:"narrow", eyes:"closed" })`

b: Ok. Ma non ho i pollici opponibili, quindi di sicuro scriverai tu.

(#act4_something_else)

# act4_harm_exposure_hurt

`bb({ body:"two_up", eyes:"angry_r" })`

{{if _.INJURED}}
b: Ad esempio: siamo saltati giù da un *tetto!*
{{/if}}

{{if !_.INJURED}}
b: Ad esempio: siamo quasi saltati giù da un *tetto!*
{{/if}}

```
hong({ eyes:"annoyed" });
bb({ body:"normal", eyes:"annoyed" });
```

h: Nah hai ragione. Uno *può* esagerare.

`hong({ eyes:"normal" });`

h: Ma questo è esattamente il motivo per cui, se facciamo la terapia di esposizione, partiremo da poco e faremo piccoli passi avanti.

h: E poco prima di raggiungere un *vero* pericolo, ci fermiamo.

`bb({ eyes:"annoyed_r", mouth:"narrow" });`

b: Sì, il limite secondo me è tra i tuoni forti, ed essere in mezzo alla tempesta con un alto cappello a punta.

(#act4_something_else)

# act4_thanks

`_.num_thanks += 1`

{{if _.num_thanks==1}}
(#act4_thanks_1)
{{/if}}

{{if _.num_thanks==2}}
(#act4_thanks_2)
{{/if}}

{{if _.num_thanks==3}}
(#act4_thanks_3)
{{/if}}

# act4_thanks_1

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"annoyed" })`

b: Aspetta, nessuna discussione per o contro di come mi sto sentendo? Solo... "grazie"?

`hong({ eyes:"surprise", body:"shrug" })`

h: Sì! Grazie per aver mostrato la tua preoccupazione per la mia {{_.thanks_for}}.

```
bb({ eyes:"closed_annoyed", MOUTH_LOCK:true });
hong({ eyes:"normal", body:"normal" });
```

b: ...

h: Tutto bene?

`bb({ eyes:"super_sad", mouth:"narrow" });`

b: Non mi hai mai detto *grazie* prima.

`hong({ mouth:"smile" });`

h: Aww, sei un grande peloso confuso lupo impanicato.

(#act4_something_else)

# act4_thanks_2

h: E anche se reagisci eccessivamente, apprezzo che tu ti preoccupi per la mia {{_.thanks_for}}.

`bb({ eyes:"annoyed" })`

b: Aspetta... non starai ripetendo "grazie" per evitare di parlare delle tue paure, spero?

```
bb({ eyes:"normal" });
hong({ eyes:"annoyed", body:"chin" });
```

h: Beh, è complicato, e io non ho sempre una risposta pronta.

`hong({ eyes:"annoyed_l", body:"one_up" })`

h: Non è che la vita ti da una lista di tre risposte già pronte.

`hong({ eyes:"normal", mouth:"smile", body:"normal" })`

h: Ma per adesso, posso almeno ringraziarti.

b: Bene, grazie anche a te, per avermi ascoltato pazientemente.

`bb({ eyes:"closed" });`

b: Piccola mammifera senza peli.

(#act4_something_else)

# act4_thanks_3

h: Anche se il tuo straparlare mi spaventa, stai semplicemente cercando di proteggere la mia {{_.thanks_for}}.

`bb({ eyes:"smile_r" });`

b: Ok, se continui ad adularmi così, l'internet si farà delle strane idee su di noi.

```
bb({ eyes:"smile" });
hong({ eyes:"annoyed" });
```

h: Eddai, sono solo una vulnerabile ragazzina in età da scuole superiori, e tu sei un grande, spaventoso lupo. Che cosa potrebbe mai succe--

`hong({ eyes:"normal", body:"point" });`

h: Anzi, forse meglio non saperlo.

(#act4_something_else)




# act4_alone

```
_.a4_talked_about_alone = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"sad_d" });`

b: Voglio essere sicuro che tu possa soddisfare quel profondo bisogno umano di appartenenza.

`bb({ eyes:"sad_u" });`

b: Ma sono preoccupato che se qualcuno saprà chi siamo – chi siamo *veramente* – si spaventerà e se ne andrà.

`bb({ eyes:"sad" });`

{{if _.a4_fears_discussed==1}}
b: Non lo so, facciamo che adesso scegli *tu* di cosa parlare. Che ne dici, umana?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Ancora, è il tuo turno, umana. Che ne pensi?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Vuoi altre riflessioni, umana?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Sono d'accordo: lavoriamo sulla nostra vita sociale.](#act4_alone_skills)

[Penso che piacciamo alle persone invece. Proviamo?](#act4_alone_experiment)

[Grazie.](#act4_thanks) `_.thanks_for = "social belonging";`

# act4_alone_skills

```
bb({ eyes:"normal" });
hong({ body:"chin" });
```

h: Potremmo fare pratica sulla capacità di fare domande, ascoltare ed empatizzare, essere aperti e vulnerabili, eccetera?

`hong({ eyes:"normal_l" });`

h: O su avere una routine sociale, come passare del tempo con gli amici o incontrarsi regolarmente?

`hong({ body:"one_up" });`

h: Potremmo anche imparare come non stare troppo male quando siamo rifiutati da qualcuno.

`hong({ eyes:"normal" });`

h: O imparare a capire quando le persone *non* ci stanno rifiutando, ma sono solo stanche o hanno una faccia ^stronza^ anche a riposo.

```
hong({ body:"normal" });
bb({ eyes:"annoyed_r" });
```

b: Queste sono molte possibilità. Ma, sulle "skill" sociali...

[Non è *manipolazione?*](#act4_alone_skills_manipulative)

[Non ci renderà più *facili da manipolare?*](#act4_alone_skills_manipulated)

[E se falliamo comunque?](#act4_alone_skills_fail)

# act4_alone_skills_manipulative

`bb({ eyes:"suspect" });`

b: I serial killer che riescono a capire le emozioni delle loro vittime, non sono forse bravi nell'"empatia"?

`bb({ eyes:"annoyed" });`

b: Charles Manson non si è guadagnato amici e ha influenzato persone?

`hong({ eyes:"annoyed", body:"chin" });`

h: No, hai ragione.

h: Le "skill" sociali non significano niente se non ci occupiamo davvero *delle* persone.

`hong({ body:"normal" });`

h: In breve, non essere un ^coglione^.

`bb({ eyes:"annoyed", mouth:"smile" });`

b: Questo è proprio un contenuto da poster motivazionale:

`hong({ body:"shrug", mouth:"narrow" });`

h: “Non Essere Un ^Coglione^™”

(#act4_something_else)

# act4_alone_skills_manipulated

`bb({ eyes:"angry" })`

b: Diventeremo degli zerbini, ringrazieremo anche chi si pulisce le scarpe su di noi!

`bb({ mouth:"scream", eyes:"scream" })`

b: Baceremo così tanti sederi, che sembrerà che ci mettiamo il rossetto marrone!

```
bb({ mouth:"normal", eyes:"normal" });
hong( body:"chin" });
```

h: Nah, hai ragione. Le "skill" sociali non sono solo fare i comodi degli altri, è anche segnare dei *confini.*

`hong( body:"one_up" });`

h: Non possiamo invitare gli altri a casa nostra, se la casa non ha i muri che la tengono su.

```
hong( eyes:"angry", mouth:"narrow" });
bb( eyes:"annoyed", mouth:"smile" });
```

h: E poi... l'immagine mentale del rossetto marrone... *schifo??*

(#act4_something_else)

# act4_alone_skills_fail

`bb({ eyes:"annoyed" });`

h: Potremmo fallire. Anzi, *sicuramente* falliremo.

```
bb({ eyes:"normal" });
hong({ eyes:"surprise", body:"shrug" });
```

h: E questo va bene! Il fallimento è il modo in cui ognuno impara qualsiasi cosa nuova!

`hong({ body:"normal", eyes:"normal" });`

h: Quindi falliamo insieme, ok?

`bb({ eyes:"normal_r" });`

b: Ok, immagino... nel caso peggiore, basta cambiare città e identità.

`bb({ eyes:"normal" });`

h: Sì, penso che ormai costi solo due bitcoin di questi tempi.

(#act4_something_else)

# act4_alone_experiment

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Possiamo fare qualche tentativo!

`hong({ body:"chin" });`

h: Possiamo chiedere ad un amico di uscire insieme, riscrivere ad un vecchio compagno, o anche solo chiacchierare con un barista.

`hong({ body:"normal" });`

h: Secondo me, potremmo risultare più simpatici di quanto pensiamo.

`bb({ eyes:"annoyed" });`

[E se queste fossero solo piccole "vittorie"?](#act4_alone_experiment_cheap)

[E se questo fosse solo un peso per gli altri?](#act4_alone_experiment_burden)

[Ma chiacchierare così non è il *vero* me!](#act4_alone_experiment_real_us)

# act4_alone_experiment_real_us

`bb({ eyes:"sad" });`

b: Con solo un timido sorriso, non ci connetteremo mai davvero con altre persone,

`bb({ eyes:"super_sad" });`

b: *Ma* se ci apriamo, gli altri vedranno il disastro che abbiamo dentro!

`hong({body:"chin", mouth:"narrow", MOUTH_LOCK:true})`

h: ...

```
hong({body:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Vieni qui.

b: Come.

`hong({body:"hands_1"})`

h: Quando i cani vogliono mostrare amore e fiducia, si rendono vulnerabili ed espongono la pancia.

`hong({body:"one_up"})`

h: Magari non siamo ancora *così* sicuri da essere troppo vulnerabili, ma con abbastanza addestramento,

`hong({body:"normal", eyes:"surprise"})`

h: Un giorno potremmo mostrare agli altri il vero noi – disastrosi, ma umani.

```
hong({eyes:"normal"});
bb({ eyes:"super_sad", mouth:"smile", body:"chest" });
```

b: Farò una capriola se mi darai una ricompensa.

`bb({ eyes:"normal", mouth:"normal" });`

h: No.

(#act4_something_else)


# act4_alone_experiment_cheap

b: Salutare il barista non è esattamente da medaglia d'oro in Socialità Olimpica.

```
hong({ body:"point", eyes:"surprise" });
bb({ eyes:"normal" });
```

h: È per *noi!*

`hong({ body:"one_up", eyes:"annoyed" });`

h: Nell'arena della società, non siamo nemmeno pesi leggeri, siamo tipo... pesi atomici.

`hong({ body:"normal", eyes:"normal" });`

h: Se partiamo da piccoli, piccoli passi, è perché dobbiamo farlo. Dobbiamo salire il primo gradino prima di salire gli altri 1000.

b: Proprio così! Magari dopo aver detto "Ciao", potremmo aggiungere...

`bb({ body:"two_up", mouth:"smile", eyes:"smile_u" });`

b: *"Come stai?"*

`hong({ body:"shrug", mouth:"smile", eyes:"surprise_l" });`

h: *"Niente di che!"*

(#act4_something_else)

# act4_alone_experiment_burden

`bb({ eyes:"suspect_r" })`

b: Magari il barista vuole solo fare del dannato caffè, non fare parte di un *esperimento* per le nostre capacità sociali.

`bb({ eyes:"annoyed" })`

h: Beh, se effettivamente capiamo di *essere* un disturbo...

```
hong({ eyes:"surprise" });
bb({ eyes:"normal" });
```

h: È bene saperlo!

`hong({ eyes:"normal" });`

h: Possiamo imparare come chiedere proattivamente agli altri che cosa gli va bene, per saperlo e per rispettare i confini personali.

```
hong({ eyes:"annoyed_l", mouth:"narrow" });
bb({ eyes:"annoyed", mouth:"smile" });
```

h: Sai, tutte quelle cavolo di "capacità interpersonali" delle brochure.

(#act4_something_else)



# act4_bad

```
_.a4_talked_about_bad = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"annoyed_r" })`

b: Voglio difendere il tuo bisogno morale di diventare una persona migliore,

`bb({ eyes:"sad_d" })`

b: Ma sembra quasi che, nel profondo, siamo come... rotti.

`bb({ body:"two_up", eyes:"angry" })`

{{if _.INJURED}}
b: E non dirmi che *non* siamo rotti. Siamo saltati giù da un *tetto*.
{{/if}}

{{if !_.INJURED}}
b: E non dirmi che *non* siamo rotti. Siamo quasi saltati giù da un *tetto*.
{{/if}}

`bb({ body:"normal", eyes:"sad" })`

{{if _.a4_fears_discussed==1}}
b: Non lo so, facciamo che adesso scegli *tu* di cosa parlare. Che ne dici, umana?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Ancora, è il tuo turno, umana. Che ne pensi?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Vuoi altre riflessioni, umana?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Quindi, siamo rotti. Aggiustiamoci.](#act4_bad_fix)

[Quindi, siamo rotti. Accettiamolo.](#act4_bad_accept)

[Grazie.](#act4_thanks) `_.thanks_for = "capacità morale";`

# act4_bad_fix

```
bb({eyes:"normal"});
hong({body:"chin"});
```

h: Potremmo, con piccoli passi, prendere abitudini migliori, avvicinarci con la nostra vita a quello in cui crediamo,

`hong({body:"one_up"});`

h: E se necessario possiamo cercare un aiuto professionale – uno psicologo, un analista.

`hong({body:"normal"});`

h: Ci sono i modi di aggiustarci.

[E se non possiamo davvero aggiustarci?](#act4_bad_fix_cant)

[E se ci aggiustiamo *troppo*?](#act4_bad_fix_too_much)

[Non possiamo permetterci un aiuto professionale.](#act4_bad_fix_afford)

# act4_bad_fix_cant

`hong({eyes:"annoyed"});`

h: Nah, immagino che tu abbia ragione.

h: Non possiamo aggiustare tutto.

`bb({mouth:"scream", eyes:"scream_sad"});`

b: Ahhh lo sapevo saremo per sempre rotti!

`hong({eyes:"surprise"});`

h: Ma possiamo almeno essere *meno* rotti.

```
bb({mouth:"normal", eyes:"annoyed"});
hong({eyes:"sad", mouth:"smile"});
```

h: Le ferite guariscono con il tempo, ma non spariscono mai. E questo va bene.

`bb({eyes:"annoyed_r"});`

b: Immagino. E comunque,

```
Game.FORCE_TEXT_Y = 460;
Game.clearText();
publish("act4-sexy", [true]);
```

b: Le ferite sono *sexy.*

```
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-sexy", [false]);
bb({body:"chest", mouth:"smile_talk", MOUTH_LOCK:true, eyes:"sexy"}, 0);
hong({eyes:"normal", mouth:"normal"}, 0);
```

h: Per piacere non farlo.

(#act4_something_else)

# act4_bad_fix_too_much

`bb({ eyes:"angry_d" })`

b: Sembra strano da ammettere, ma... una parte di me *vuole* avere questo disturbo.

`bb({ eyes:"angry" })`

b: Intendo, senza di lui, non saremmo troppo *noiosi?*

`bb({ eyes:"sad_r", body:"one_up" })`

b: Senza il disturbo, la nostra arte non divenerebbe insipida?

`bb({ eyes:"sad_u", body:"two_up" })`

b: Senza il disturbo, non saremmo in grado di connetterci con i nostri amici che invece ce l'hanno, il disturbo?

`bb({ eyes:"sad", body:"chest" })`

b: Se ci accontenteremo mai della nostra vita, non ci fermerebbe dal fare nuove cose importanti?

`hong({ MOUTH_LOCK:true })`

h: ...

h: Se abbiamo paura di... "esaurire le paure"...

h: Non penso che esauriremo mai le paure.

`bb({ eyes:"smile_u", body:"normal", mouth:"smile" })`

b: Oh, yeah! Whew! Che sollievo!

(#act4_something_else)

# act4_bad_fix_afford

`bb({ body:"one_up", eyes:"sexy", mouth:"normal" })`

b: "Dottore, sono ansioso di star pagando $100 all'ora solo per sentirmi chiedere da te *e questo come ti fa sentire?*"

`bb({ body:"paw", eyes:"closed", mouth:"narrow" })`

b: "Mm-hmm. E questo come ti fa sentire?"

```
bb({ body:"normal", eyes:"normal", mouth:"normal" });
hong({ eyes:"sad" });
```

h: Nah, è una paura più che ragionevole.

`hong({ eyes:"annoyed", mouth:"sad" });`

h: E fa davvero schifo che la salute mentale non sia accessibile a molti.

`hong({ eyes:"normal", mouth:"normal" });`

h: Ma comunque, ci sono delle opzioni economiche o gratuite:

`hong({ body:"chin" })`

h: Gruppi di supporto, terapia online, centri non profit e per studenti...

`hong({ body:"hands_1" })`

h: Avere delle abitudini come la meditazione, dormire bene, parlare regolarmente con gli amici, imparare nuove cose...

`hong({ body:"hands_2" })`

h: Andare in biblioteca per prendere in prestito libri su terapie psicologiche...

`hong({ body:"one_up" })`

h: C'è una enorme lista di risorse, considerato tutto!

```
hong({ body:"normal" });
bb({ eyes:"annoyed", mouth:"narrow" });
```

b: Beh *quella* quarta parete non è durata molto.

`hong({ body:"point" });`

h: Alcune cose sono più importanti di delle convenzioni narrative. Come la salute mentale.

(#act4_something_else)


# act4_bad_accept

```
bb({ eyes:"normal" });
hong({ eyes:"normal_l", body:"one_up", mouth:"narrow" });
```

h: Intendo, questo è quello che dicono gli psicologi, giusto? Accettare le tue emozioni, anche quelle negative?

```
bb({ eyes:"annoyed" });
hong({ eyes:"normal", body:"normal", mouth:"normal" });
```

b: Wait.

["Accettare" come *rinunciare*?](#act4_bad_accept_give_up)

["Accettare" come *approvare*?](#act4_bad_accept_approve)

["Accettare" come *letteralmente*?](#act4_bad_accept_literally)

# act4_bad_accept_give_up

`bb({ eyes:"angry", body:"one_up" });`

b: Pensi che Martin Luther King avrebbe detto, "Accidenti non possiamo sederci nella parte davanti del bus, *accettiamolo*?"

`bb({ eyes:"angry_r", body:"two_up" });`

b: Perché l'industria dell'auto-aiuto pensa che sventolare bandiera bianca sia segno di una *profonda saggezza?*

`bb({ eyes:"annoyed", body:"normal" });`

h: Penso che gli psicologi intendano "accettare" le cose negative come: riconoscere che esistono e che sono difficili da cambiare,

h: Ma non necessariamente rinunciare una possibilità di cambiamento.

`bb({ eyes:"suspect" });`

b: Quindi dovrebbero dire *riconoscere*, non *accettare*.

`hong({ body:"chin", eyes:"annoyed" });`

h: A pensarci, "accettare" è un po' vago.

`bb({ eyes:"closed", mouth:"narrow" });`

b: Beh, lo *riconosco*.

(#act4_something_else)

# act4_bad_accept_approve

`bb({ eyes:"angry" });`

b: Come se fosse *buono* che siamo rotti, o simili? No!

`bb({ eyes:"angry_r", body:"one_up" });`

b: Tutti questi autori di Hollywood che romanticizzano le malattie mentali sono schifose!

`bb({ eyes:"angry", body:"two_up" });`

b: Avere una malattia mentale *fa schifo!* Si prende le *vite* delle persone! Perché dovremmo "accettare" questo?

`bb({ body:"normal" });`

h: Penso che gli psicologi intendano "accettare" le emozioni come: avere pazienza con loro.

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Come quando dimenarti nelle sabbie mobili ti fa solo andare più a fondo, e la soluzione è di sdraiarsi e avere pazienza,

`hong({ eyes:"surprise" });`

{{if _.INJURED}}
h: Lottare contro di te, la mia paura, mi ha portata a saltare giù da un tetto.
{{/if}}

{{if !_.INJURED}}
h: Lottare contro di te, la mia paura, mi ha portata a quasi saltare giù da un tetto.
{{/if}}

`hong({ body:"normal", eyes:"normal" });`

h: Invece, la soluzione è fare quello che stiamo facendo ora – non lottare, ma avere pazienza nella nostra relazione.

`bb({ eyes:"annoyed" });`

b: E dovrebbero dire *questo* invece di una parola problematica come "accettare".

`hong({ body:"chin", eyes:"annoyed" });`

h: A pensarci, "accettare" fa un po' schifo come parola.

`bb({ eyes:"closed_annoyed", mouth:"narrow" });`

b: Non accetto "accetto".

(#act4_something_else)

# act4_bad_accept_literally

`bb({ eyes:"sad", body:"one_up" });`

b: Ma già *sai* che non dovresti prendermi mai alla lettera!

`bb({ eyes:"sad_u", body:"two_up" });`

b: Il *problema* è che io voglio aiutarti, ma faccio schifo a trovare le parole per farlo!

`bb({ eyes:"sad", body:"normal" });`

h: Penso che gli psicologi intendano "accettare" le emozioni come: "non lottare o ignorarle."

`hong({ eyes:"surprise", body:"one_up" });`

h: Per ascoltare te stesso, lavora *con* te stesso, ma non prendere quello che dici come verità assoluta.

```
hong({ eyes:"normal", body:"normal" });
bb({ eyes:"annoyed", mouth:"normal" });`
```

b: E dovrebbero dire *questo* invece di una parola vaga e confusa come "accettare".

`hong({ body:"chin", eyes:"annoyed" });`

h: Immagino che anche loro facciano schifo a trovare le parole.

(#act4_something_else)




# act4_something_else

```
bb({ body:"normal", mouth:"normal", eyes:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal" });
```

{{if _.a4_fears_discussed==1}}
h: Comunque, altro di cui vuoi parlare?
{{/if}}

{{if _.a4_fears_discussed==2}}
h: Quindi, hai altro a cuore di cui vuoi discutere?
{{/if}}

{{if _.a4_fears_discussed==3}}
(#act4_something_else_2)
{{/if}}

{{if _.a4_talked_about_harm!=true}}
[Ho paura di ricevere del male.](#act4_harm)
{{/if}}

{{if _.a4_talked_about_alone!=true}}
[Ho paura di essere solo.](#act4_alone)
{{/if}}

{{if _.a4_talked_about_bad!=true}}
[Ho paura di essere una persona cattiva.](#act4_bad)
{{/if}}

[Nah, sono a posto per ora.](#act4c_prelude)

# act4_something_else_2

h: Ok, mi sa che abbiamo parlato di tutte le nostre paure.

b: Sì, esistono sono solo tre paure.

h: Esatto, proprio tre.

b: Comodo!

(#act4c)

# act4c_prelude

h: Bella chiacchierata, ragazzi.

(#act4c)

# act4c

```
Game.clearText();
music(null,{fade:3});
bb({body:"normal", eyes:"normal", mouth:"normal", MOUTH_LOCK:true},0);
hong({body:"normal", eyes:"normal", mouth:"normal"},0);
```

b: ...

`hong({MOUTH_LOCK:true},0)`

h: ...

`bb({eyes:"annoyed_d"})`

b: Questo non è un *gioco*, lo sai.

`bb({eyes:"angry_d", body:"one_up"})`

b: Creare una relazione sana con le tue emozioni non è semplice come cliccare dei pulsanti su uno schermo.

`bb({eyes:"sad", body:"normal"})`

b: *Possiamo* davvero andare d'accordo?

b: *Possiamo* lavorare insieme, come un team?

`hong({eyes:"sad", body:"one_up"})`

h: Bene,

```
hong({eyes:"surprise_l"});
bb({eyes:"normal"});
```

a: S-scusa...

```
Game.clearText();
publish("act4-in-2");
music('campus', {volume:0.5, fade:1});
```

(...2101)

(#act4d)

# act4d

`Game.WORDS_HEIGHT_BOTTOM = 221;`

`publish("act4", ["alshire", 0]);`

a: T-ti d-dispiacerebbe se mi sedessi con te per il pranzo?

`publish("act4", ["alshire", 1]);`

{{if _.TOP_FEAR=="harm"}}
s: *Questa* è la tua crush? Perché è seduta da sola come un serial killer psicopatico?
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: Chiedere alla tua crush se puoi sederti con lei? Lo sai quanto *patetiche* sembriamo?!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: *Questa* è la tua crush? Abbiamo disturbato la sua tranquillità! Siamo un peso!
{{/if}}

`publish("act4", ["alshire", 2]);`

a: I- intendo- è, è ok se è un no, solo...

`publish("act4", ["alshire", 3]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "h2"`

[Aspetta, non eri al party?](#act4d_recognition) `publish("act4", ["hong_to_alshire",1])`

[Certo! Vieni qui.](#act4d_yes) `publish("act4", ["hong_to_alshire",2])`

[Scusa, mi serve stare da sola ora.](#act4d_no) `publish("act4", ["hong_to_alshire",8])`

# act4d_recognition

`publish("act4", ["hong_to_alshire",2]);`

h2: Sì, eri sul divano! Alla prima festa a cui sono andata...

`publish("act4", ["hong_to_alshire",10]);`

{{if _.a2_ending=="fight"}}
h2: Quella in cui ho avuto un attacco di panico e ho dato un pugno al padrone di casa.
{{/if}}

{{if _.a2_ending=="flight"}}
h2: Quella in cui ho avuto un attacco di panico e sono corsa via piangendo.
{{/if}}

```
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Aspetta umana, potremmo starla mettendo a disagio.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, non volevo accusarti di niente!

`publish("act4", ["hong_to_alshire",4]);`

h2: Stavo solo cercando di ricordare una faccia familiare.

```
publish("act4", ["hong_to_alshire",5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: AHHHHH LO SAPEVO! È UNA PERICOLOSA PSICOPATICA ATTRATTA DAL PANICO!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: AAHHH IL PRIMO INCONTRO CHE ABBIAMO AVUTO È STATO "AVERE VISTO I MIEI TRAUMI"! SIGNIFICA CHE CI ODIA!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AAAHHH ABBIAMO FATTO RICORDARE A QUALCUNO UN EVENTO TRAUMATICO. GIÀ SOLO LA NOSTRA PRESENZA FERISCE GLI ALTRI.
{{/if}}

(#act4e)

# act4d_yes

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Aspetta umana, sembra a disagio.

```
publish("act4", ["hong_to_alshire", 6]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, nessuna pressione ovvio!

`publish("act4", ["hong_to_alshire", 4]);`

h2: Dicevo, puoi sederti qui se vuoi.

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: È *TROPPO* AMICHEVOLE! COME TED BUNDY, IL SERIAL KILLER!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: STA SOLO FINGENDO DI ESSERE CARINA! NESSUNO VUOLE *DAVVERO* ESSERE VICINO A NOI!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AHHH METTIAMO SEMPRE GLI ALTRI IN IMBARAZZO! SIAMO SOLO UNA MACCHIA NEL MONDO!
{{/if}}

(#act4e)

# act4d_no

```
publish("act4", ["hong_to_alshire", 9]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Aspetta umana, potremmo starla mettendo a disagio.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, non volevo essere scortese!

`publish("act4", ["hong_to_alshire", 6]);`

h2: Mi serve solo del tempo per elaborare le mie emozioni. Non prenderla sul personale, per piacere.

```
publish("act4", ["hong_to_alshire", 7]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: CHE SCHIFOSI, CONTORTI PENSIERI STA ELABORANDO?! CHE DESIDERI OSCURI RIEMPIONO IL SUO CUORE?!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: SIAMO STATI RIFIUTATI COME PERSONA! NESSUNO CI AMERÀ MAI!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: ABBIAMO INTERROTTO LA SUA ELABORAZIONE DELLE EMOZIONI! ADESSO SARÀ TRAUMATIZZATA A VITA ED È TUTTA COLPA NOSTRA!
{{/if}}

(#act4e)

# act4e

```
Game.WORDS_HEIGHT_BOTTOM = 195;
publish("act4", ["alshire", 6]);
```

s: CORRI CORRI CORRI CORRI CORRI CORRI CORRI CORRI CORRI CORRI

```
Game.clearText();
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["alshire", 10]);
sfx("pop");
```

(...1001)

```
publish("act4", ["alshire", 11]);
sfx("alshire_run");
```

(...2601)

```
publish("act4-out-3");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
```

(...1201)

`publish("act4-jumpcut-hong");`

h: Huh. È stato strano. Chissà cosa stava succedendo nella sua testa.

`publish("act4", ["hong_closer", 2]);`

h: Comunque, stavi dicendo?

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 6]);
```

b: Uh, mi sono dimenticato? Qualcosa sul lavorare in gruppo?

```
publish("act4", ["bb_closer", 0]);
publish("act4", ["hong_closer", 3]);
```

h: ¯\_(ツ)_/¯

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 4]);
```

b: Dicono che devi "fare pace" con le tue emozioni, come se le tue emozioni fossero *criminali di guerra*.

`publish("act4", ["bb_closer", 7]);`

b: Ma io vorrei fare qualcosa in *più* della semplice pace! Vorrei che fossimo *alleati!*

`publish("act4", ["bb_closer", 3]);`

b: Vorrei essere un buon cane da guardia. Come fame e sete sono indicatori per i tuoi bisogni fisiologici,

`publish("act4", ["bb_closer", 8]);`

b: Io voglio essere l'indicatore per i tuoi bisogni *psicologici* – i tuoi bisogni di sicurezza, appartenenza e buona volontà.

`publish("act4", ["bb_closer", 1]);`

b: Ma... faccio schifo in questo, quindi devi addestrarmi.

`publish("act4", ["bb_closer", 4]);`

b: Non sono "sempre giusto," né "sempre irrazionale." Sto solo... cercando di fare il mio meglio. Quindi, per favore,

`publish("act4", ["bb_closer", 30]);`

b: Aiutami ad aiutarti!

`publish("act4", ["bb_closer", 6]);`

b: Anche se, insegnare ad un vecchio cane nuovi trucchi ci *metterà* del tempo. Anche *anni.*

`publish("act4", ["bb_closer", 3]);`

b: E quindi ogni tanto potrei tornare irrazionale, tornare alle mie vecchie abitudini.

`publish("act4", ["bb_closer", 2]);`

b: Abbaierò alle ombre. Ti spaventerò con le mie parole. Potrei anche mostrarti delle immagini invasive di... qualche cosa.

`publish("act4", ["bb_closer", 9]);`

b: Mi dispiace! Sono un cane malconcio da canile! I cani malconci la fanno sul tuo letto ogni tanto!

`publish("act4", ["bb_closer", 4]);`

b: Ma se sei paziente con me... e ti siedi e resti con me...

`publish("act4", ["bb_closer", 8]);`

b: Magari puoi addomesticare questo lupo.

`publish("act4", ["bb_closer", 0]);`

`Game.clearText();`

(...1000)

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Good dog.](#act4f-pat-bb) `Game.OVERRIDE_CHOICE_SPEAKER = "h"; publish("act4", ["hong_closer", 2]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "b"`

[Good human.](#act4f-pat-hong) `Game.OVERRIDE_CHOICE_SPEAKER = "b"; publish("act4", ["bb_closer", 8]);`

# act4f-pat-hong

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 13]);
```

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...6501)

`publish("act4", ["bb_closer", 15]);`

(...1001)

(#act4f)

# act4f-pat-bb

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 10]);
```

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...6501)

`publish("act4", ["bb_closer", 12]);`

(...1001)

(#act4f)

# act4f

```
Game.FORCE_CANT_SKIP = false;
publish("act4", ["bb_closer", 16]);
publish("act4", ["hong_closer", 5]);
```

{{if _.fifteencigs}}
  b: AAAAA STAI MANGIANDO ANCORA DA SOLA, QUINDICI SIGARETTE AAAAA
{{/if}}

{{if _.parasite}}
b: AAAAA NON SEI ANCORA PRODUTTIVA MENTRE MANGI SIAMO PARASSITI DELLA SOCIETÀ AAAAA
{{/if}}

{{if _.whitebread}}
b: AAAAA MANGI ANCORA SEMPRE PANE BIANCO AAAAA
{{/if}}

```
publish("act4", ["bb_closer", 18]);
publish("act4", ["hong_closer", 6]);
sfx("yaps", {volume:0.6});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 205;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: YAP YAP YAP YAP YAP

(#credits)
