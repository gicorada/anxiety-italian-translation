# act2

`SceneSetup.act2();`

{{if _.badnews && !_.factcheck}}
(#act2-preamble-news1)
{{/if}}

{{if _.badnews && _.factcheck}}
(#act2-preamble-news2)
{{/if}}

{{if _.catmilk}}
(#act2-preamble-cat)
{{/if}}

(#act2-preamble-tinder)


# act2-preamble-news1

```
publish("act2",["dee",3]);
```

s: Ma hai *visto* quella "notizia" su quella cosa orribile che sta accadendo da qualche parte?

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: c-ciao...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",3]);
```

a: Dio, odio le notizie. È tutto sensazionalismo o un clickbait.

```
publish("act2",["dum",2]);
publish("act2",["party_hong","next"]);
```

h2: b... bella festa...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",1]);
```

s: Vero, ma stanno solo seguendo la loro convenienza. Il *vero* problema sono le persone che cliccano il clickbait.

```
publish("act2",["dee",3]);
```

s: Chi retweeterebbe mai una notizia terribile, facendo stare male tutti i suoi amici?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Sì, lo so, vero?

(#act2-preamble-end)


# act2-preamble-news2

```
publish("act2",["dee",3]);
```

s: Ma hai *visto* quella "notizia" che sta andando virale?

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: c-ciao...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",3]);
```

a: Sì, completamente false. Chi è che non lo capirebbe e la retweeterebbe?

```
publish("act2",["dum",2]);
publish("act2",["party_hong","next"]);
```

h2: b... bella festa...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Veramente. Tipo, ehi, apri Google e controlla che sia vera?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Sì, lo so, vero?

(#act2-preamble-end)


# act2-preamble-cat

```
publish("act2",["dee",3]);
```

s: Come stavo dicendo, l'Industria dei Meme sfrutta i gatti.

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: c-ciao...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",1]);
```

a: Elabora la tesi.

```
publish("act2",["dum",0]);
publish("act2",["party_hong","next"]);
```

h2: b... bella festa...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",1]);
```

s: Beh, ieri ho visto qualcuno retweetare una GIF di un gatto che beveva del latte.

```
publish("act2",["dee",3]);
```

s: Non riescono a digerire quella ^merda^! Chi retweeterebbe un *abuso sugli animali* come quello?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Sì, lo so, vero?

(#act2-preamble-end)


# act2-preamble-tinder

```
publish("act2",["dee",1]);
```

s: Quindi non ti ha mai risposto!

```
publish("act2",["dee",0]);
publish("act2",["party_hong","next"]);
```

h2: c-ciao...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",1]);
```

a: Anche se entrambi avete fatto match su Tinder?

```
publish("act2",["dum",0]);
publish("act2",["party_hong","next"]);
```

h2: b... bella festa...

```
publish("act2",["party_hong","next"]);
```

{{if _.serialkiller}}
(#act2-preamble-serialkiller)
{{/if}}

{{if _.hookuphole}}
(#act2-preamble-hookuphole)
{{/if}}

{{if _.pokemon}}
(#act2-preamble-pokemon)
{{/if}}

# act2-preamble-serialkiller

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Sì, non so! Per caso pensava che potessi essere un *serial killer* o simili? Troppo paranoica.

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Sì, lo so, vero?

(#act2-preamble-end)


# act2-preamble-hookuphole

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Sì, non so! Magari pensava che gli incontri non possano riempire il suo buco nel cuore?

s: Smettila di essere così puritana! Apri la tua mente, e poi le tue gambe!

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Sì, lo so, vero?

(#act2-preamble-end)


# act2-preamble-pokemon

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Sì, non so! Non era così attraente, ma sarebbe stata una buona cattura!

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Gotta Catch 'Em All!™

(#act2-preamble-end)


# act2-preamble-end

```
Game.clearText();
publish("act2-out-1");
music(null, {fade:1});
```

(...3000)

```
music('battle', {volume:0.5});
publish("hp_show");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

n: SECONDO ROUND: *LOTTA!*

[Oh no, ci odiano tutti!](#act2a_social)

[Stavi *mangiando con gli occhi* la rossa?](#act2a_perv)

[Ehi, parliamo del senso della vita.](#act2a_meaning)

# act2a_social

`bb({eyes:"sad"})`

b: Stiamo rovinando l’atmosfera di questa festa facendo i tristi mollaccioni!

`bb({eyes:"shock", body:"two_up"})`

b: Stiamo uccidendo l'atmosfera! Stiamo commettendo un atmosfericidio di primo grado!

`bb({eyes:"normal", body:"normal"})`

b: Umana, dobbiamo andarcene *ora* prima che--

```
_.a2_first_danger = 'social';
_.a2_attack_1 = "alone";
```

(#act2b)

# act2a_perv

`bb({eyes:"suspect"})`

b: È troppo più attraente di noi, e significa che se anche solo la *guardiamo*, allora--

`bb({eyes:"shock", body:"two_up"})`

b: SIAMO SCHIFOSI

`bb({body:"normal"})`

b: Siamo dei schifosi, malvagi, cattivi cattivi cattivi terribili terribili perv--

```
_.a2_first_danger = 'perv';
_.a2_attack_1 = "bad";
```

(#act2b)

# act2a_meaning

`bb({body:"one_up", eyes:"normal_r"})`

b: Alla fine, cosa potremmo fare che importi veramente? 

`bb({body:"normal", eyes:"sad"})`

b: Contribuire all'umanità? Tutte le grandi opere decadono come Osimandia. L’amore? La morte farà sempre la sua parte.

`bb({eyes:"sad_r"})`

b: E quanta morte c'è! *Noi* moriremo. *I nostri cari* moriranno.

`bb({eyes:"shock", body:"two_up"})`

b: Cavolo, per la Seconda Legge della Termodinamica anche il nostro *universo* morirà!

`bb({eyes:"suspect", body:"normal"})`

b: Oh, "la morte ci fa apprezzare la vita"? È come dire che la schiavitù è buona perché ci fa apprezzare la libertà!

`bb({body:"one_up"})`

b: Oh, "devi creare tu il tuo senso"? È quello che i culti e i cospirazionisti fanno!

`bb({eyes:"shock", body:"two_up"})`

b: La vita non ha senso, la morte non ha senso, anche *senso* non ha senso! Cosa dovrebbe fare un'anima mortal--

```
_.a2_first_danger = 'meaning';
_.a2_attack_1 = "bad";
```

(#act2b)

# act2b

`bb({eyes:"normal", mouth:"normal", body:"normal", MOUTH_LOCK:true})`

b: ...

`bb({eyes:"suspect"})`

b: Ehm... mi riesci a sentire, umana?

`bb({eyes:"normal", MOUTH_LOCK:true})`

b: ...

`bb({eyes:"shock", mouth:"small_talk", body:"chest", MOUTH_LOCK:true})`

b: *GASP*

`bb({mouth:"small_talk"})`

b: TI DEVO AVVERTIRE DI...

[*Altro* sullo stesso pericolo!](#act2b_louder)

{{if _.a2_first_danger=="social"}}
[Un *altro* pericolo della società!](#act2b_different_social)
{{/if}}

{{if _.a2_first_danger=="perv" || _.a2_first_danger=="meaning"}}
[Un *altro* pericolo morale!](#act2b_different_moral)
{{/if}}

[Stai ignorando il pericolo! Ed è pericoloso!](#act2b_ignore)

# act2b_louder

`_.a2_first_choice = "louder"`

{{if _.a2_first_danger=="social"}}
(#act2b_louder_social)
{{/if}}

{{if _.a2_first_danger=="perv"}}
(#act2b_louder_perv)
{{/if}}

{{if _.a2_first_danger=="meaning"}}
(#act2b_louder_meaning)
{{/if}}

# act2b_louder_social

`bb({eyes:"shock", body:"two_up", mouth:"normal"})`

b: LE EMOZIONI SONO CONTAGIOSE! QUINDI SE NON VAI VIA INFETTERAI TUTTI CON LA TUA MALATTIA MENTALE! 

b: Scatenerai un’epidemia letale di SINDROME DEL TRISTE MOLLACCIONE

`bb({eyes:"suspect", body:"normal", mouth:"normal"})`

b: Dobbiamo andarcene e metterci in quarantena eterna in una stanzina con Netflix e cibo a domicilio!

```
_.a2_second_danger = 'netflix';
_.a2_attack_2 = "alone";
_.a2_hoodie_callback = "una quarantena";
```

(#act2c)

# act2b_louder_perv

`bb({eyes:"suspect", body:"two_up", mouth:"normal"})`

b: NON COMPORTARTI DA SCHIFOSA! È CONTRO LA LEGGE!

`bb({eyes:"judge", body:"judge_1", mouth:"normal"})`

(...201)

```
bb({body:"judge_2"}, 0);
sfx("gravel");
```

(...168)

`bb({body:"judge_1"}, 0)`

(...168)

`bb({body:"judge_2"}, 0)`

(...168)

`bb({body:"judge_1"}, 0)`

(...501)

b: Legge sullo Strano, Sezione 74.5: (1) Qualsiasi persona che osservi (a) quelle spalle muscolose (b) quel sedere sodo (2) sarà da ora conosciuta come

`bb({eyes:"shock", body:"two_up", mouth:"normal"})`

b: "UNA GRANDE PERVERSA E SCHIFOSA E INUTILE"

```
_.a2_second_danger = 'law';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "la legge";
```

(#act2c)

# act2b_louder_meaning

`bb({body:"two_up", mouth:"normal", eyes:"shock"})`

b: In verità, anche se hai un obiettivo nobile nella vita, puoi *comunque* mandare tutto all'aria!

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Alfred Nobel voleva la pace nel mondo e che le culture si capissero tra loro. Quindi ha deciso di facilitare i viaggi.

`bb({eyes:"normal_r"})`

b: Per questo gli serviva un modo di creare velocemente gallerie per i treni. E ha inventato un nuovo materiale, chiamato "dinamite"...

`bb({body:"one_up", eyes:"normal"})`

b: che è stato usato nella Prima Guerra Mondiale per UCCIDERE MILIONI DI PERSONE

`bb({body:"two_up", eyes:"shock"})`

b: È L'EFFETTO FARFALLA, UMANA! QUANTE PERSONE STAI UCCIDENDO SENZA SAPERLO, ORA

```
_.a2_second_danger = 'butterfly';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "la prima guerra mondiale";
```

(#act2c)

# act2b_different_social

`_.a2_first_choice = "different"`

`bb({eyes:"normal_r", body:"point", mouth:"normal"})`

b: In verità, sai cos'è peggio di nessuno che ti ama? Che *tutti* ti amino.

`bb({body:"one_up", eyes:"suspect", mouth:"normal"})`

b: Cioè, diventare una di *questi* animali da festa sempre alla ricerca di divertimento.

`bb({body:"normal", mouth:"small"})`

b: Una vita superficiale con amici superficiali che ti conoscono solo superficialmente!

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: Umana, dobbiamo scappare via da questi zombie della spensieratezza prima che ti trasformino in loro!

```
_.a2_second_danger = 'zombies';
_.a2_attack_2 = "alone";
_.a2_hoodie_callback = "gli zombie";
```

(#act2c)

# act2b_different_moral

`_.a2_first_choice = "different"`

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: Ci sono persone che muoiono in carestie e genocidi *in questo momento* e noi andiamo a feste!

`bb({body:"point", eyes:"closed", mouth:"small"})`

b: Una saggia persona disse, "l'unica cosa necessaria al trionfo del male è che le brave persone non reagiscano."

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: NOI NON STIAMO REAGENDO.

`bb({mouth:"small"})`

b: FACENDO FESTA, STIAMO AIUTANDO *HITLER*.

```
_.a2_second_danger = 'hitler';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "Hitler";
```

(#act2c)

# act2b_ignore

`_.a2_first_choice = "ignore"`

`bb({body:"normal", mouth:"normal", eyes:"suspect"})`

b: Pensi di esser salva solo perché hai tolto le batterie dai rilevatori di monossido di carbonio?

`bb({eyes:"suspect_r"})`

b: Non sentirai nemmeno il veleno! Diventerai sonnolenta e poi--

`bb({body:"scream_c_1"})`

b: MORIRAIIIIIIIIIIIIII

```
_.a2_second_danger = 'ignore';
_.a2_attack_2 = "harm";
_.a2_hoodie_callback = "il monossido di carbonio";
```

(#act2c)

# act2c

```
hong({body:"ignore_sweat"});
bb({eyes:"normal", mouth:"normal", body:"normal", MOUTH_LOCK:true});
```

b: ...

`bb({eyes:"happy", mouth:"smile", body:"chest"})`

b: Oh, grazie a dio, umana! Riesci a sentirmi di nuovo!

`bb({eyes:"closed", body:"point"})`

b: DEVO AVVERTIRTI DI...

{{if _.a2_first_choice=="louder"}}
[*Ancora altro* su questo pericolo!](#act2c_louder)
{{/if}}

{{if _.a2_first_choice!="louder"}}
[*Altro* su questo pericolo!](#act2c_louder)
{{/if}}

{{if _.a2_first_danger=="social"}}
[Un *altro* pericolo della società!](#act2c_different_social)
{{/if}}

{{if _.a2_first_danger=="perv" || _.a2_first_danger=="meaning"}}
[Un *altro* pericolo morale!](#act2c_different_moral)
{{/if}}

[Hai controllato il punch prima di berlo?](#act2c_punch)

#act2c_louder

{{if _.a2_second_danger=="netflix"}}
(#act2c_louder_netflix)
{{/if}}

{{if _.a2_second_danger=="law"}}
(#act2c_louder_law)
{{/if}}

{{if _.a2_second_danger=="butterfly"}}
(#act2c_louder_butterfly)
{{/if}}

{{if _.a2_second_danger=="zombies"}}
(#act2c_louder_zombies)
{{/if}}

{{if _.a2_second_danger=="hitler"}}
(#act2c_louder_hitler)
{{/if}}

{{if _.a2_second_danger=="ignore"}}
(#act2c_louder_ignore)
{{/if}}

# act2c_louder_netflix

`bb({body:"normal", mouth:"normal", eyes:"shock"})`

b: In verità, Netflix & consegna a domicilio non è abbastanza come quarantena! Infetteremmo comunque chi consegna il cibo!

`bb({body:"one_up", mouth:"small"})`

b: Dobbiamo trasferirci nei territori canadesi dello Yukon, e farci consegnare il cibo con un drone!

`bb({body:"two_up", mouth:"normal"})`

b: E poi dovrebbero sterilizzarlo per togliere i nostri GERMI DA MOLLACCIONI

`_.a2_attack_3 = "alone";`

`_.a2_hoodie_callback = "una quarantena";`

(#act2d)

# act2c_louder_law

`bb({eyes:"judge", body:"judge_1", mouth:"normal"})`

(...201)

```
bb({body:"judge_2"}, 0);
sfx("gravel");
```

(...168)

`bb({body:"judge_1"}, 0)`

(...168)

`bb({body:"judge_2"}, 0)`

(...168)

`bb({body:"judge_1"}, 0)`

(...501)

b: La GRANDE PERVERSA E SCHIFOSA E INUTILE sarà condannata a passare 72 ore in uno di quegli attrezzi medievali da gogna

b: sempre che non gli *piaccia* segretamente quel tipo di cose

`bb({body:"scream_a_1"})`

b: perché è una GRANDE PERVERSA E SCHIFOSA E INUTILE

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "la legge";`

(#act2d)

# act2c_louder_butterfly

`bb({body:"normal", mouth:"small", eyes:"suspect"})`

b: EFFETTO FARFALLA! Stai usando un bicchiere di plastica non biodegradabile?

`bb({body:"two_up", mouth:"normal", eyes:"shock"})`

b: BAM, DA UNA DISCARICA ESCE VELENO E UCCIDE UN BAMBINO

`bb({body:"normal", mouth:"small", eyes:"suspect"})`

b: Stai sudando e il tuo cuore sta scoppiando nel petto?

`bb({body:"scream_a_1"})`

b: BAM, MANDI IN BANCAROTTA IL NOSTRO SISTEMA SANITARIO E IN MILIONI MUOIONO

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "l'effetto farfalla";`

(#act2d)

# act2c_louder_zombies

`bb({body:"normal", mouth:"small", eyes:"angry"})`

b: Questi zombie del divertimento barcolleranno verso di te mormorando,

`bb({body:"normal", mouth:"normal", eyes:"shock"})`

b: MI PIACEE. MI PIAAAAAACEE.

`bb({body:"scream_a_1"})`

b: E ti MORDERANNO e ti faranno diventare un FRATELLO SENZA CERVELLO e/o una RAGAZZA DELLA SCIOCCHEZZA

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "gli zombie";`

(#act2d)

# act2c_louder_hitler

`bb({body:"scream_a_1"})`

b: I NAZISTI STANNO SFILANDO DI NUOVO PER LE STRADE A PASSO MILITARE!

`bb({body:"one_up", mouth:"smile", eyes:"happy"})`

b: Dicendo, *bello che i 'bravi ragazzi' siano impegnati con cose tipo 'rilassarsi' e 'curarsi di se'!*

`bb({body:"point", mouth:"smile", eyes:"happy_r"})`

b: *Ora i nostri piani possono proseguire, in quarta come il prossimo Reich!*

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "Hitler";`

(#act2d)

# act2c_louder_ignore

`bb({body:"normal", mouth:"normal", eyes:"normal_r"})`

b: Dai, pensaci, sappiamo se questo edificio *ha* un rilevatore di CO?!

`bb({body:"two_up", mouth:"small", eyes:"normal"})`

b: E se ci stesse avvelenando *PROPRIO ORA?*

`bb({body:"scream_a_1"})`

b: NON VEDREMMO NEMMENO LA MORTE AVVICINARSI. SMETTEREMMO DI ESISTERE PER SEMPRE E ANCORA E ANC--

`_.a2_attack_3 = "harm";`

`_.a2_hoodie_callback = "il monossido di carbonio";`

(#act2d)

# act2c_different_social

`bb({body:"normal", mouth:"normal", eyes:"sad"})`

b: E se fossimo solo *completamente incapaci* di essere amati o di amare?

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: E se qualcosa si fosse rotto dentro di noi tempo fa? O se non fosse mai esistito?

`bb({body:"scream_a_1"})`

b: AHH SIAMO ROTTI! ROTTI ROTTISSIMI COSÌ ROTTI--

`_.a2_attack_3 = "alone";`

(#act2d)

# act2c_different_moral

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: E se fossimo solo *completamente marci?*

`bb({body:"one_up", eyes:"sad"})`

b: Gli altri hanno una bussola verso il bene, ma noi facciamo del "bene" solo se ci sentiamo in colpa o ci vergognamo, al massimo.

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: E se fosse nella nostra natura fare del male agli altri? E se non potessimo evitare di essere *altro* che un fardello per chi ci è vicino?

`bb({body:"scream_a_1"})`

b: AHH SIAMO ROTTI! ROTTI ROTTISSIMI COSÌ ROTTI--

`_.a2_attack_3 = "bad";`

(#act2d)

# act2c_punch

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Non sono irrazionale. Le persone *mettono* droga nelle ciotole da punch. È una cosa che succede veramente.

`bb({eyes:"suspect"})`

b: Umana, ti fa male la testa? I tuoi arti sono molli? Mi sa che stiamo morendo.

`bb({body:"scream_a_1"})`

b: AHHH STIAMO MORENDO! STIAMO MORENDO STIAMO MORENDO STIAMO MO--

`_.a2_attack_3 = "harm";`

`_.a2_hoodie_callback = "le ciotole da punch";`

(#act2d)

# act2d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"attacked"});
attack("20p", _.a2_attack_1);
```

(...401)

```
hong({body:"attacked_2"});
attack("20p", _.a2_attack_2);
```

(...401)

```
hong({body:"attacked_3"});
attack("20p", _.a2_attack_3);
```

(...1001)

h: C^AAAZZO^!

h: C^AZZ^UTISSIMO C^AZZ^-C^AZZ^ONISSIMO *C^AAAAZZO^*

`bb({body:"two_up", mouth:"smile", eyes:"happy"});`

b: Evviva, umana! Sono così contento che riesci a sentirmi di nuovo!

`bb({body:"normal", mouth:"small", eyes:"sad"})`

b: Perché mi stavi ignorando?

`hong({body:"facepalm"})`

h: Santa ^merda^, sei un idiota.

`hong({body:"facepalm_2"})`

h: La conosci quella storiella dei Nativi Americani?

h: "Ci sono due lupi dentro di te, uno è la speranza e uno la disperazione, che lupo vince? Quello a cui dai da mangiare."

```
hong({body:"facepalm_3"});
bb({eyes:"normal"});
```

h: Stavo cercando di farti *morire di fame*, sadistico pezzo di ^merda^!

`hong({body:"smile", mouth:"smile"})`

h: Dannazione, dirò frasi positive allora.

h: *Sono amata. Sono buona. Sono intelligente. Sono bellissima. Sono speciale.*

`bb({eyes:"suspect"});`

[Caspita, quanto sei narcisista!](#act2d_narcissist)

[Lo sai che questo metodo è stato dimostrato *inutile?*](#act2d_disproven)

[ommioddio non dare i crediti di questa storia agli indigeni](#act2d_racist)

# act2d_disproven

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: In verità, si *ritorcono* contro se la persona ha poca stima di se! 

`bb({body:"one_up", mouth:"small", eyes:"normal"})`

b: Ed era uno studio ben eseguito – trial randomizzato, e lo sperimentatore non sapeva a quale gruppo appartenevano i partecipanti.

`bb({body:"two_up", mouth:"small", eyes:"normal_r"})`

b: Risultato: se già hai poca stima di te, dover ripetere delle frasi motivazionali ti fa sentire *peggio* di quando non dici niente!

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: Wood 2009, Psychological Science. Cercalo su Google Scholar, umana,

`bb({body:"scream_b_1"})`

b: QUINDI SMETTILA DI DIFFONDERE FAKE NEWS ANTISCIENTIFICHE

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2d_narcissist

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: *Devi* guardare i tuoi difetti con umiltà per crescere come persona!

`bb({body:"two_up", eyes:"suspect"})`

b: Non puoi spruzzare deodorante in una stanza piena di muffa! Coprire i tuoi difetti li peggiorerà a lungo andare.

`bb({body:"chest", mouth:"smile", eyes:"closed"})`

b: Per fortuna, io, come tua fedele guardia-lupo, posso farti notare i tuoi difetti. E ora, è-

`bb({body:"scream_b_1"})`

b: TUTTO. È TUTTO SBAGLIATO

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2d_racist

`bb({body:"normal", mouth:"normal", eyes:"suspect"})`

b: I Nativi Americani erano *persone vere*, non dei "buoni selvaggi" che puoi nominare a caso per rendere i tuoi consigli scontati più *esotici*.

`bb({eyes:"suspect_r"})`

b: Stai riducendo persone e complesse culture ad una cartolina! È "razzismo benevolo"! 

`bb({body:"scream_b_1"})`

b: SMETTILA DI ESSERE RAZZISTA, MALVAGIA DAGLI OCCHI STRETTI

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2e

h: ^Porca merda^.

`hong({body:"yell", mouth:"yell"})`

h: Sai cosa? Sei *irrazionale*.

h: Tutti sanno che le emozioni sono irrazionali! Specialmente la paura!

`hong({body:"facepalm_2"})`

h: Sei un inutile residuo dell'evoluzione, come la mia appendice o i denti del giudizio!

`hong({body:"yell", mouth:"yell"})`

h: ^Cavolo^, tutta questa metafora del lupo è stupida! Sei solo un miscuglio di neurotrasmettitori nella mia testa.

`hong({body:"cross", mouth:"cross"})`

h: E quindi perché dovrei ascoltare un inutile, irrazionale, inesistente pezzo di ^merda^ come te?!

`bb({eyes:"sad", MOUTH_LOCK:true})`

b: ...

[Cavli, umana. Fa veramente male.](#act2e_hurtful)

[Sono un sentimento. I sentimenti sono validi.](#act2e_valid)

[Umana, siamo *entrambi* "delle sostanze chimiche."](#act2e_rational)

# act2e_hurtful

`bb({body:"chest"})`

b: Faccio *parte* di te, come sai. Quando dici questo, stai facendo del male a *te stessa*.

`bb({body:"scream_a_1"})`

b: Perché ti stai colpendo da sola, umana? BASTA COLPIRTI.

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "harm");
```

(...2500)

(#act2f)

# act2e_rational

`bb({body:"normal", mouth:"normal", eyes:"normal_r"});`

b: Le tue più profonde motivazioni sono dopamina, le tue più grandi felicità serotonina.

`bb({body:"one_up"});`

b: La tua memoria sono modifiche di sinapsi, il tuo ragionamento sono segnali elettrici traballanti.

`bb({eyes:"normal", body:"normal"});`

b: Quindi se io sono "delle sostanze chimiche" significa *che sono* irrazionale... che signifca che *sei* irrazionale!

`bb({body:"two_up", eyes:"shock"});`

b: E se siamo *entrambi* irrazionali, allora non capiremo *mai* come essere contenti e realizzati!

`bb({body:"scream_a_1"})`

b: AHH SIAMO ROTTI! ROTTI ROTTISSIMI COSÌ ROTTI--

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2f)

# act2e_valid

`bb({body:"normal", mouth:"normal", eyes:"suspect"});`

b: Aspetta... "loro" dicono i sentimenti sono validi, che dovresti sempre accettare le tue emozioni.

`bb({eyes:"suspect_r"});`

b: Ma "loro" dicono anche che le emozioni sono irrazionali, e che non bisogna dargli fiducia.

`bb({eyes:"angry"});`

b: Ommioddio, "loro" ci stavano mentendo per tutto il tempo!

`bb({body:"scream_a_1"})`

b: "LORO" CI RIEMPIONO DI CONTRADDIZIONI PER FARCI DIPENDERE DALL'INDUSTRIA DELL'AUTO-AIUTO

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "harm");
```

(...2500)

(#act2f)

# act2f

`hong({body:"defeated", MOUTH_LOCK:true});`

h: ...

h: Lo odio. Dio, fa male, e lo *odio*.

h: Non riesco a calmarti. Non riesco ad ignorarti. Non riesco a combatterti. 

`bb({eyes:"suspect"});`

h: Ogni cosa che faccio, sembra che non riesca a liberarmi di t--

`bb({body:"cry_1"});`

b: Beh, magari perché NON *DOVRESTI* LIBERARTI DI ME.

`bb({body:"cry_2"});`

b: Come pensi che mi senta, *io*, umana?!

`bb({body:"cry_4", mouth:"cry", eyes:"cry"})`

b: Sto facendo il mio meglio per essere il tuo cane da guardia, ma mi vedi sempre come un Grande Lupo Cattivo!

b: E quindi provo ad avvertirti *di più* dei pericoli! *Più* pericoli! *Altri* pericoli!

`bb({eyes:"cry_2"})`

b: Ma anche se provo così tanto a proteggerti, tu *ancora* pensi che sono tuo nemico!

`bb({body:"cry_5"});`

b: Cosa sto facendo di sbagliato?!

`bb({body:"cry_2"});`

b: Lo *so* che faccio schifo in questo. Ma ci sto *provando*, umana!

`bb({body:"cry_3"});`

b: ...ci sto provando.

`bb({body:"cry_6", mouth:"right", eyes:"cry_r_1"});`

b: Non devi per forza ascoltare i miei avvertimenti, o concordare con me, o perfino *volermi bene*.

`bb({eyes:"cry_r_2"});`

b: Io voglio solo... solo che tu sia paziente con me.

`bb({eyes:"cry_r_3"});`

b: Voglio solo che stia con me per un po', invece di girarti e--

```
bb({eyes:"cry_r_4"});
hong({body:"listen"});
```

r: Ehi.

```
hong({body:"look"});
Game.clearText();
publish("act2-in-2");
publish("hp_hide");
music('party1', {volume:0.4, fade:2});
```

(...2000)

```
publish("act2",["party_hunter",2]);
Game.WORDS_HEIGHT_BOTTOM = 230;
```

r: Sembra che tu stia litigando con te stessa, ragazza.

```
publish("act2",["party_hunter",3]);
publish("act2",["party_hong",13]);
```

h2: Si vedeva così tanto?

```
publish("act2",["party_hunter",4]);
publish("act2",["party_hong",14]);
```

r: Stavi, uh, parlando con la tua felpa riguardo {{_.a2_hoodie_callback}} o qualcosa del genere.

```
publish("act2",["party_hunter",13]);
publish("act2",["party_hong",15]);
sfx("rustle", {volume:0.6});
setTimeout(function(){
	publish("act2",["party_hong",16]);
	sfx("concrete_step3", {volume:0.6});
},401);
setTimeout(function(){
	publish("act2",["party_hong",17]);
	sfx("concrete_step4", {volume:0.6});
},801);
```

h2: oddio sono un disastro.

```
publish("act2",["party_hunter",7]);
publish("act2",["party_hong",18]);
sfx("squeak");
```

r: Ehi. Non sei da sola, amica. L'ansia è molto comune.

```
publish("act2",["party_hunter",5]);
publish("act2",["party_hong",19]);
```

{{if _.act1_ending=="fight"}}
r: Cavolo, proprio ieri, ho sentito di qualcuno che ha avuto un crollo nervoso e ha distrutto il suo telefono!
{{/if}}

{{if _.act1_ending=="flight"}}
r: Cavolo, proprio ieri, ho sentito di qualcuno che si è raggomitolato come un armadillo e si è messo a piangere in pubblico!
{{/if}}

```
publish("act2",["party_hunter",2]);
```

r: Ascolta: so com'è avere quell'animale nella propria testa.

```
publish("act2",["party_hunter",8]);
```

r: *Tutti* lo sappiamo. Ed è questo il motivo per cui faccio festa ogni weekend, per dimenticare le preoccupazioni, dimenticarsi di quell'animale.

```
publish("act2",["party_hunter",9]);
publish("act2",["party_hong",20]);
```

h2: ma la mia ansia...

```
publish("act2",["party_hunter",2]);
publish("act2",["party_hong",21]);
```

r: Non preoccuparti, ragazza. Una volta ero come te. Ma poi ho trovato un piccolo trucco per far tacere per sempre quella voce...

```
publish("act2",["party_hunter",3]);
Game.clearText();
music(null, {fade:1});
```

(...2001)

```
publish("act2",["party_hunter",10]);
publish("act2",["party_hong",22]);
sfx("rustle");
```

(...2501)

```
publish("act2",["party_hunter",10]);
publish("act2",["party_hong",23]);
sfx("rustle2");
```

(...1001)

```
publish("act2",["party_hunter",11]);
```

r: La mia miscela speciale. È un po' più forte di... beh, qualsiasi cosa legale in realtà.

```
publish("act2",["party_hunter",12]);
publish("act2",["party_hong",24]);
```

r: Alla salute, ^stronza^!

```
hong({body:"hold"});
bb({body:"normal", mouth:"small", eyes:"wat"});
Game.clearText();
Game.WORDS_HEIGHT_BOTTOM = -1;
publish("act2-out-3");
publish("hp_show");
```

(...3500)

[Oh mio Dio.](#act2g_1) `Game.OVERRIDE_CHOICE_LINE=true`

[Questo è un pessimo meccanismo di difesa.](#act2g_2) `Game.OVERRIDE_CHOICE_LINE=true`

[Non accettare drink dagli sconosciuti.](#act2g_3) `Game.OVERRIDE_CHOICE_LINE=true`

# act2g_1

b: O--

(#act2g)

# act2g_2

b: Q--

(#act2g)

# act2g_3

b: N--

(#act2g)

# act2g

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("40p", "harm");
```

(...2000)

```
hong({body:"forward", mouth:"forward"});
bb({body:"frazzled", mouth:"frazzled", eyes:"frazzled"});
```

h: Mmm, che gusto squisito!

h: Un gusto deciso di “spegni il cervello”, con un delicato retrogusto di “non provare mai più niente”!

b: È una brutta cosa, umana. Davvero, davvero brutta.

[È *così* che inizia una dipendenza.](#act2h_opt1) `Game.OVERRIDE_CHOICE_LINE=true`

[Lo *sapevo* che l'organizzatore era messo male!](#act2h_opt3) `Game.OVERRIDE_CHOICE_LINE=true`

[In più, potrebbero averci messo droga!](#act2h_opt2) `Game.OVERRIDE_CHOICE_LINE=true`


# act2h_opt1

b: È *così* ch--

(#act2h)

# act2h_opt2

b: In più, potreb--

(#act2h)

# act2h_opt3

b: Lo *sapevo* ch--

(#act2h)

# act2h

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("40p", "harm");
```

(...2000)

```
hong({body:"back", mouth:"back"});
bb({body:"panicked", mouth:"panicked", eyes:"panicked"});
```

h: Delizioso, *e* più economico di andare in terapia!

b: UMANA PER FAVORE BASTA

h: Hehehe!

h: E *tu* che cosa hai intenzione di fare, ^stronzo^?

b: Mi dispiace, umana.

b: Dovrò usare il mio ATTACCO SPECIALE

```
bb({body:"special_a"});
music('battle', {volume:0.5});
```

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_harm"`

[](#act2h_attack) `_.SPECIAL_ATTACK="harm"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_alone"`

[](#act2h_attack) `_.SPECIAL_ATTACK="alone"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_bad"`

[](#act2h_attack) `_.SPECIAL_ATTACK="bad"; Game.OVERRIDE_CHOICE_LINE=true`

# act2h_attack

```
bb({body:"special_b_1"});
hong({body:"forward", mouth:"forward"});
sfx("charging");
```

h: E che ^cavolata^ è questa?

h: Hai intenzione di blaterare ancora idiozie contro di me per--

```
bb({body:"special_c"});
sfx("hadouken");
```

(...901)

(#act2i)

# act2i

```
publish("hide_tabs");
publish("show_special_attack");
Game.FORCE_CANT_SKIP = true;
music(null);
stopAllSounds();
```

(...5000)

```
publish("show_tabs");
hong({ body:"final", mouth:"final" });
bb({ body:"normal", mouth:"normal", eyes:"sad" });
attack("100p", _.SPECIAL_ATTACK);
Game.FORCE_CANT_SKIP = false;
setTimeout(function(){
	publish("remove_special_attack");
},30);
```

(...2500)

h: CHE ^DIAVOLO^ ERA

b: Scusami. Ma dovevo farti vedere le conseguenze.

{{if _.SPECIAL_ATTACK=="harm"}}
h: POTEVO *VEDERE* IL MIO CADAVERE. POTEVO *SENTIRE* LA SENSAZIONE DI ESSERE VERAMENTE MORTA.
{{/if}}

{{if _.SPECIAL_ATTACK=="alone"}}
h: POTEVO *VEDERE* LO SGUARDO DI DISGUSTO DI TUTTI. POTEVO *SENTIRE* TUTTO QUELLO CHE DICEVANO.
{{/if}}

{{if _.SPECIAL_ATTACK=="bad"}}
h: POTEVO *SENTIRE* LE MIE COSTOLE ACCARTOCCIARSI. POTEVO *ODORARE* IL SANGUE DISPERSO NELL'ARIA.
{{/if}}

b: Scusami, umana.

n: *ELIMINALA*

[{LOTTA: Dai un pugno all'organizzatore.}](#act2j_fight) `Game.OVERRIDE_CHOICE_LINE=true`

[{SCAPPA: Andiamo via.}](#act2j_flight) `Game.OVERRIDE_CHOICE_LINE=true`

# act2j_fight

`bb({ eyes:"angry" });`

b: Quella psicopatica stava approfittando di te.

b: Stava cercando di rovinarti, farti diventare proprio come lei!

`bb({ body:"yell_angry_1" });`

b: Picchiala quella tipa! Mandala KO!

`bb({ body:"final_1" });`

b: PICCHIALA PICCHIALA PICCHIALA PICCHIALA PICCHIALA PICCHIALA PICCHIALA PICCHIAL--

`_.a2_ending = "fight";`

(#act2k)

# act2j_flight

b: Lo *sapevo* che tutti i festaioli sono messi male, dentro. Alleviano il dolore in modo orribile!

`bb({ body:"yell_1" });`

b: E stanno cercando di convincerti a fare lo stesso! Ti stanno rovinando! Dobbiamo andare via!

`bb({ body:"final_1" });`

b: ANDARE VIA ANDARE VIA ANDARE VIA ANDARE VIA ANDARE VIA ANDARE VIA ANDARE V--

`_.a2_ending = "flight";`

(#act2k)

# act2k

```
Game.clearText();
publish("act2-in-4");
publish("hp_hide");
music('party1', {volume:0.6, fade:1.5});
```

(...2001)

```
publish("act2",["party_hong",26]);
sfx("slide");
```

(...1001)

```
publish("act2",["party_hunter",14]);
Game.WORDS_HEIGHT_BOTTOM = 230;
```

r: Tutto bene, ragazza?

`publish("act2",["party_hunter",13]);`

{{if _.a2_ending=="fight"}}
(#act2k_fight)
{{/if}}

{{if _.a2_ending=="flight"}}
(#act2k_flight)
{{/if}}

# act2k_fight

```
Game.clearText();
publish("act2",["party_hunter",21]);
publish("act2",["party_hong",33]);
music(null);
sfx("hit");
```

(...1000)

```
sfx("record_scratch");
publish("act2",["party_hunter",22]);
publish("act2",["party_hong",34]);
publish("act2",["dee",6]);
publish("act2",["dum",6]);
```

r: T-tu...

```
publish("act2",["party_hunter",23]);
publish("act2",["party_hong",35]);
publish("act2",["dee",5]);
publish("act2",["dum",5]);
music('party1', {volume:0.6, fade:6});
```

r: sei *piccante*.

r: E mi piace. Vieni alla festa il prossimo weekend, tesoro.

```
publish("act2",["party_hunter",19]);
publish("act2",["party_hong",36]);
```

h2: ok ciao, bye, adios, au revoir

r: L'animale magari oggi avrà vinto, ma torna qui, e ti preparerò qualcosa di ancora più forte!

h2: sayōnara, auf wiedersehen, zài jiàn, shalom

r: Io e te, ragazza, faremo vedere alla bestia chi è il vero boss!

(#act2k_end)

# act2k_flight

`publish("act2",["party_hong",36]);`

h2: ok scusa ma devo proprio andare

`publish("act2",["party_hunter",16]);`

r: ^Cazzo^! Oggi ha vinto l’animale, eh?

`publish("act2",["party_hunter",15]);`

h2: no no, è che, mh, devo fare una maratona. devo essere veloce.

`publish("act2",["party_hunter",19]);`

r: Vieni alla mia festa il prossimo weekend, tesoro. Ti preparerò qualcosa di ancora più forte.

h2: ok grazie ma devo proprio correre correre correre

r: Io e te, ragazza, faremo vedere alla bestia chi è il vero boss!

(#act2k_end)

# act2k_end

```
Game.clearText();
publish("act2-out-5");
publish("act2-outro", ["end1"]);
music("hum", {fade:2, volume:0.6});
Game.WORDS_HEIGHT_BOTTOM = -1;
```

(...2500)

```
publish("act2", ["act2_end",2]);
sfx("whoosh");
```

(...1000)

b: Umana! Stai bene?!

```
publish("act2", ["act2_end","next"]);
```

b: Oddio, ci siamo andati *vicini.* Potevamo veramente--

```
Game.clearText();
publish("act2", ["act2_end","next"]);
music(null);
sfx("squeak");
```

(...1500)

```
publish("act2", ["act2_end","next"]);
sfx("hit");
```

(...1000)

h: Tornerò alla festa il prossimo weekend.

h: La prossima volta lotteremo, e non voglio solo *sconfiggerti*...

h: Ti voglio ammazzare, ^cazzo^!

```
Game.clearText();
publish("act2", ["act2_end","next"]);
sfx("concrete_step1");
````

(...901)

```
publish("act2", ["act2_end","next"]);
sfx("concrete_step2", {volume:0.8});
```

(...901)

```
publish("act2", ["act2_end","next"]);
sfx("concrete_step3", {volume:0.5});
```

(...901)

`sfx("concrete_step4", {volume:0.25});`

(...3000)

`_.INTERMISSION_STAGE = 2;`

(#intermission)