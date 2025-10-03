# act3

```
SceneSetup.act3();
Game.WORDS_HEIGHT_BOTTOM = 205;
sfx("cheers");
```

r: Saúde!

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

h2: *Ah* esse aí bateu na hora.

```
publish("act3",["roofhunter",2]);
publish("act3",["roofhong",2]);
```

r: Sabe, jovem...

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",6]);
```

h2: Para especificar: bateu bem nas minhas amídalas cerebelosas, direita e esquerda.

```
publish("act3",["roofhunter",8]);
publish("act3",["roofhong",5]);
```

r: Você me lembra eu quando era mais jovem. Quando era alguém atormentado por um animal na minha cabeça.

```
publish("act3",["roofhunter",9]);
publish("act3",["roofhong",2]);
```

r: Estou feliz que posso passar isso adiante, ajudar você a matar essa besta como eu matei a minha.

```
publish("act3",["roofhunter",2]);
```

r: Ei, perguntinha: verdade or desaf--

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",7]);
publish("act3-alpha", ["dizzyhong",0]);
```

h2: DESAFIO!

```
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",2]);
```

r: Haha! Beleza.

```
publish("act3",["roofhunter",21]);
publish("act3",["roofhong",4]);
```

r: Então. Tá vendo aquela piscina azulada, lá embaixo?

```
publish("act3-alpha", ["dizzyhong",0]);
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",9]);
```

h2: Tô? Seis andares pra baixo?

```
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",8]);
```

r: Pule dentro dela.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",10]);
```

h2: ...

```
publish("act3",["roofhong",11]);
```

h2: Pera, o que?

```
publish("act3",["roofhong",10]);
publish("act3",["roofhunter",2]);
```

r: O lobo bicha começou a reclamar, não começou?

```
publish("act3",["roofhunter",23]);
```

r: *Ah nããão é perigoso, não faça issooo*

```
publish("act3",["roofhunter",22]);
```

r: Mas isso é exatamento o porquê de precisarmos destes desafios que encaram a morte! Festejar adoidamente! Carpe diem! Colocar platina no nariz, #YOLO!

```
publish("act3",["roofhunter",10]);
```

r: Mostre para aquele furry que a gente tá pouco se f^oden^do com ele enchendo o nosso saco! Cai dentro.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",13]);
```

h2: Uh, às vezes, hum... O Zenith tem razão...

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

r: Perdoe-me, você acabou de cair naquele conto do vigário onde sentimentos ruins são *bons*?

```
publish("act3",["roofhunter",17]);
```

r: O Prazer é o oposto da dor. Portanto você pode usar prazer para vencer a dor, p^orr^a!

```
publish("act3",["roofhunter",18]);
```

r: Como é que aqueles pseudo-budistas do Vale do Silício não enxergam isso c^aralh^o?!

```
publish("act3",["roofhunter",6]);
```

r: Jovem, eu sei que *você* sabe que esse animal de merda apenas *machuca* gente como nós. Ele *tortura* gente como nós.

```
publish("act3",["roofhunter",19]);
```

r: Esse arrombado não é nosso amigo. É uma besta fora de controle, o que significa que ela tem que ser ou *tranquiziliada*,

```
publish("act3",["roofhunter",20]);
```

r: Ou tomar um *tiro de FAL no meio da cara*.

```
publish("act3",["roofhunter",27]);
```

r: Caso contrário, ela vai ganhar.

```
publish("act3",["roofhunter",31]);
publish("act3",["roofhong",14]);
publish("act3",["dd",2]);
```

h2: Não. Você se engana.

```
publish("act3",["roofhunter",13]);
publish("act3",["roofhong",15]);
music('battle_dark', {volume:1.0}, function(){
	music('battle_dark_loop');
});
```

h2: Eu não vou deixar ela ganhar.

```
publish("act3",["roofhunter",25]);
publish("act3-alpha", ["roofhong",0]);
publish("act3-alpha", ["transition",1]);
publish("act3",["dd",6]);
```

r: Aí sim, c^aralh^o! Eu acredito em você, amor! Dá-lhe! <3

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

b: não não não não não não 

n: ESTE CAPÍTULO POSSUI DOIS FINAIS POSSÍVEIS. UM DELES É *MUITO, MUITO RUIM.*

b: NÃO NÃO NÃO NÃO NÃO NÃO NÃO NÃO NÃO NÃO 

n: ESCOLHA SABIAMENTE. PROTEJA SEU HUMANO.

`bb({ eyes:"oh_crap", mouth:"normal_talk", MOUTH_LOCK:true });`

b: Por quê tu tá fazendo isso?

`bb({ mouth:"normal" });`

n: BOA SORTE

```
Game.clearText();
bb({ eyes:"start" });
```

[Dan, isso é SUICÍDIO!](#act3a_harm) `Game.OVERRIDE_CHOICE_LINE=true`

[Você vai causar um estrago em você e nos outros!](#act3a_bad) `Game.OVERRIDE_CHOICE_LINE=true`

[A Hunter é uma puta louca!](#act3a_alone) `Game.OVERRIDE_CHOICE_LINE=true`

# act3a_harm

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: H--

(#act3a_after)

# act3a_alone

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: v--

(#act3a_after)

# act3a_bad

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: A--

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

h: Sabe, talvez eu até acreditaria em você... se você não tivesse agido assim um zilhão de vezes antes.

h: Você é o pequeno lobinho indefeso e vulnerável que *tenta* me defender.

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

h: Você tentou essa besteira de "me mostrar", também.

b: Danton. cara, tu toma remédio tarja preta, beber essa merda poderia ter te matado antes...

`hong({ eyes:"look_right" });`

h: Ah, me *desculpe* se a Indústria Farmacêutica não aprova minha auto-medicação.

h: Olha, c^uzã^o, todos *nós* temos um jeito de fazer você fechar essa sua matraca.

`hong({ body:"look_up", eyes:"look_up" });`

h: Algumas pessoas se arremessam no trabalho.

`hong({ body:"look_down", eyes:"look_down" });`

h: Algumas pessoas se arremessam no sexo, nas drogas, em atualizar a feed de seus Facebooks.

`hong({ body:"normal", eyes:"look_right" });`

h: Algumas pessoas se arremessam em outras pessoas. 

`hong({ eyes:"angry" });`

h: Agora eu, eu vou me arremessar naquela piscina.

[Você bebeu e a piscina é funda, e se suas pernas ficarem dormentes?!](#act3_bad_1_harm)

[Porra, esse é isso que eu ganho?!](#act3_bad_1_insult) `bb({eyes:"angry"});`

[Me desculpe...](#act3_good_1) `bb({mouth:"sorry", eyes:"sorry_down"});`

# act3_bad_1_harm

b: Mesmo que você acerte a água, dessa altura a tensão de superfície irá quebrar suas costelas e te dar uma concussão *no mínimo!*

b: Fora que você provávelmente vai tocar o fundo da piscina, suas pernas vão ficar dormentes e você vai se afog-

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

h: Eu vi um Russo fazer isso no Youtube uma vez.

(#act3_bad_2)

# act3_bad_1_insult

`hong({ eyes:"look_right" });`

h: Com Licença,  *agradecimento?!*

`bb({ eyes:"angry" });`

b: Isso aqui é exatamente o porquê de *eu existir*! Devido ao fato de que não dá para confiar em humanos para se manterem seguros!

b: Estive tentando proteger esse seu rego burro minha vida inteira! E é isso que eu recebo?!

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

h: Ah NOSSA, esse é a desculpinha mais f^odid^a do século!

`hong({ body:"yell_2" });`

h: Sim, sua abominação peluda e desalmada! Você fez besteira pra c^aralh^o!

`hong({ body:"normal", mouth:"angry", eyes:"angry" });`

h: Alguma outra observação, Capitão Óbvio?

[Se vingar de mim é a resposta?](#act3_good_1_fail_revenge) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Mas desta vez, eu *realmente* estou certo!](#act3_good_1_fail_harm) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Eu machuquei você.](#act3_good_2a)


# act3_good_1_fail_revenge

b: Você precisa ter uma relação mais saudável com suas emoções, ao invés de afogá-las co--

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

b: V--

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

b: por favor... não faça...

h: Sua barra de energia aí tá parecendo bem baixa, lobo.

h: Se eu fosse você, escolheria minhas próximas palavras com cuidado.

`bb({ eyes:"normal" });`

[Tá. Cansei de proteger você, eu espero que você morra, é, que assim seja.](#act3_bad_2_jump) `bb({ mouth:"ignore", eyes:"ignore" });`

[Estive certo este tempo todo.](#act3_bad_2_right)

[Me desculpe.](#act3_good_2b) `bb({mouth:"sorry", eyes:"sorry_down"});`


# act3_bad_2_jump

b: Tudo bem, vá em frente e pule. Se é assim que acaba, QUE ACABE LOGO.

`hong({ eyes:"look_right", mouth:"normal", MOUTH_LOCK:true });`

h: ...

```
hong({ eyes:"less_angry", mouth:"normal" });
bb({ eyes:"ignore_oh_crap" });
```

h: Beleza então. Bola de canhão.

```
bb({ mouth:"normal", eyes:"oh_crap" });
Game.OVERRIDE_TEXT_SPEED = 2;
```

b: DEIXA ESSA GARRAFA LONGE PELO MENOS!

(#act3_bad_3)



# act3_bad_2_right

`bb({ eyes:"angry" });`

b: Você *está* se colocando em perigo. Seus supostos "amigos" *estão* apenas te usando. E *você* está apenas usando seus supostos amigos.

`bb({ eyes:"sad" });`

b: Então por favor, Danton... por que você não acredita em mim?!

h: Porque você nunca acreditou em *mim*.

(#act3_bad_3)


# act3_bad_2_terrible

`bb({ eyes:"angry" });`

b: Outros lobos-guardiões tem humanos que tiram tempo para treiná-los com paciência, para *aprender* a trabalhar juntos.

b: Já você, você é um humano *cruel pra caralho*, que só grita e exige que eu fique quieto! Eu espero que esse seja seu fim!

`bb({ eyes:"normal" });`

h: Resposta errada, bichinho hipócrita.

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

h: *"A única coisa que devemos temer é o próprio medo."*

`hong({ body:"look_up", mouth:"happy", eyes:"blank" });`

h: *"Não se preocupe, seja feliz!"*

`hong({ body:"normal", mouth:"normal", eyes:"normal" });`

h: Todos os sábios da nossa era concordam: emoções negativas são *ruins!*

`hong({ eyes:"less_angry" });`

h: Duh! Por isso que elas se chamam *negativas*!

b: Porra, Danton, pensa direito, carai'!

`hong({ eyes:"normal" });`

h: Um tempo atrás, eu mesmo disse: “só quero ser livre de toda essa dor”

h: Eu consegui meu desejo. Não sinto mais dor, medo, ou ansiedade...

h: Se eu morrer, que assim seja. Eu não me arrependo de nada.

`_.a3_ending = "jump";`

(#act3_end)



# act3_good_2a

`bb({mouth:"sorry", eyes:"sorry_down"});`

b: Estive tão obsecadamente à procura de coisas que iriam machucar você, que eu não percebi que *eu* poderia estar causando machucados.

```
bb({ eyes:"sorry"});
hong({ body:"yell_2", mouth:"yell", eyes:"blank" });
```

h: NÃO ME DIGA!

`hong({ body:"yell_1" });`

h: P^ORR^A. Sério que levou todo esse tempo para você entender isso?!

`hong({ body:"cry", mouth:"cry", eyes:"blank" });`

h: Você poderia ter evitado tanto problema, seu grande e felpudo *arrombado*. Por que você não se tocou disso antes?...

`_.apologized_for_hurt = true;`

(#act3_good_2q)



# act3_good_2b

`hong({ body:"normal", mouth:"angry", eyes:"look_right" });`

h: ...você está pedindo *desculpas.*

`hong({ eyes:"angry", MOUTH_LOCK:true });`

h: hm...

h: Desculpas pelo *quê*?

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

[Me desculpe, por não ser um protetor.](#act3_good_3_protector)

[Me desculpe, por não te dar o mínimo de respeito.](#act3_good_3_respect)

[Me desculpe por tudo.](#act3_good_4)


# act3_good_2q_not_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"angry" }, 0);`

[Me desculpe, por ter um humano HORRÍVEL!](#act3_bad_2_terrible) `bb({mouth:"normal", eyes:"normal"})`

[Me desculpe, por não te respeitar.](#act3_good_3_respect)

[Me desculpe, por te machucar](#act3_good_3_hurt)



# act3_good_3_protector

`bb({eyes:"sorry_down"});`

b: É meu dever avisar você sobre perigo *real*, mas eu simplesmente ficava latindo para os carros e o entregador de cartas.

`bb({eyes:"sorry_up"});`

b: Latindo para as sombras. Latindo demais.

`bb({eyes:"sorry"});`

b: Faz todo sentido você querer me colocar em uma mordaça.

`bb({eyes:"sorry_down"});`

b: Me desculpe.

(#act3_good_4)



# act3_good_3_respect

`bb({eyes:"sorry_down"});`

b: Eu deveria ser *seu* leal cão-de-guarda, mas eu agi como se você tivesse que obedecer à *mim*.

`bb({eyes:"sorry_up"});`

b: Existe diferença entre um protetor e um escravagista, e eu passei desse limite.

`bb({eyes:"sorry_down"});`

b: Me desculpe.

(#act3_good_4)



# act3_good_3_hurt

`bb({eyes:"sorry_down"});`

b: Estive tão obsecadamente a procura de coisas que iriam machucar você, que eu não percebi que *eu* poderia estar te machucando...

`bb({eyes:"sorry_up"});`

b: Eu fui um cachorro mau.

`bb({eyes:"sorry_down"});`

b: Me desculpe.

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

h: É, bem, isso aqui foi uma má idéia de qualquer forma.

h: Só fiz isso para botar você para baixo, e, bem, eu te coloquei bem pra baixo.

h: Vamos chamar isso de um empate, tá bem?

```
bb({ mouth:"sorry", eyes:"sorry" });
bb({ MOUTH_LOCK:true });
```

b: ...

b: Tá bem.

h: Tá bem.

n: *EMPATE*

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

r: Ahh *coé*. Depois de tudo que aquele merda fez contigo, você vai *desistir?*

r: Que que têm, jovem? Está com *medo?*

```
publish('hong-next');
publish("act3",["roofhunter",26]);
```

h2: Sim.

h2: Estou com medo, e pra caralho.

`publish('hong-next')`

h2: E não há problema nisso, lá no fundo eu tava certo, tu é uma babaca anti-furry que me colocou em perigo.

`publish('hong-next')`

h2: Vai tomar no teu cu, Hunter, vai se foder.

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

r: Aquilo foi a porta trancando? Ih rapaz, agora fudeu.

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

b: Danton...

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

b: Tira a porra da garrafa primeiro.

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

b: PORRA O QUE EU FALEI?!

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
