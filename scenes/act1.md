# act1

```
SceneSetup.act1();
```

(...300)

n: E ISTO É A ANSIEDADE DESTE HUMANO.

n: _VOCÊ_ SERÁ A ANSIEDADE

{{if window.localStorage.continueChapter=="replay"}}
(#act1_replay)
{{/if}}

{{if window.localStorage.continueChapter!="replay"}}
(#act1_normal)
{{/if}}



# act1_replay

`hong({mouth:"0_neutral", eyes:"0_neutral"})`

h: Ah, eae? Estamos aqui denovo?

`hong({eyes:"0_neutral"})`

n: SEU TRABALHO É PROTEGER SEU HUMANO DE *PERIGOS*

`bb({eyes:"look", mouth:"small_lock"})`

n: DE FATO, REPETIR O JOGO ESTÁ OS COLOCANDO EM *PERIGO* AGORA MESMO

n: RÁPIDO, OS AVISE!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Humano! Escute, estamos em perigo! O jogador...

[...vai nos torturar denovo!](#act1_replay_torture)

[...não achará um final alternativo!](#act1_replay_alternate)

[...terá dissonância ludonarrativa!](#act1_replay_dissonance)

# act1_replay_torture

```
window.HACK_REPLAY = JSON.parse(localStorage.act4);
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

{{if window.HACK_REPLAY.act1_ending=="fight"}}
b: Eles nos farão ficar em posição fetal e chorar!
{{/if}}

{{if window.HACK_REPLAY.act1_ending=="flight"}}
b: Eles nos farão quebrar seu celular ao lhe dar um ataque de pânico!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="fight"}}
b: Eles não vão deixar a gente bater na dona da festa!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="flight"}}
b: Eles vão fazer a gente bater na simpática dona anti-herói da festa!
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="jump"}}
h: Bem, talvez assim não iremos pular da cobertura dessa v--
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="walkaway"}}
b: ELES NOS FARÃO PULAR DA COBERTURA.
{{/if}}

`bb({body:"fear"});`

b: TODAS ESTAS COISAS HORRÍVEIS IRÃO ACONTECER CONOSCO, E ENTÃO A GENTE VAI--

(#act1_replay_end)


#act1_replay_alternate

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Claro, a história em sua *inteireza* é a mesma, mas cada capítulo possui dois finais possíveis. Além de todas as opções de dialógo ramificadoras e--

`bb({body:"fear"});`

b: O jogador ficará desapontado, vai fechar a aba do navegador, deletar nosso software, e então a gente vai--

(#act1_replay_end)


# act1_replay_dissonance

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Uma luso-o quê agora?

`bb({eyes:"normal"});`

b: O arco de história foi sobre como você pode *ESCOLHER* construir uma colaboração saudável com seus medos,

`bb({eyes:"normal_right"});`

b: Mas jogar o jogo denovo vai resultar na mesma estória, implicando que suas *ESCOLHAS* não importam,

`bb({eyes:"narrow_eyebrow"});`

b: Mostrará então a contradição entre a mensagem do jogo e suas mecânicas,

`bb({eyes:"fear"});`

b: Que logo desmoronará a construção deste universo narrativo,

`bb({body:"fear"});`

b: E então a gente vai--

(#act1_replay_end)


# act1_replay_end

`bb({body:"panic"})`

b: MOOOOORREEEEEEEEEER

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

h: Tá, vamos voltar aos personagens.

```
Game.clearText();
```

n4: (DEIXE _SUA_ ANSIEDADE BLAH BLAH BLAH QUE MAIS SE ASSEMELHA AO QUE _SEU_ MEDO BLAH BLAH VOCÊ JÁ SABE)

```
sfx("squeak");
hong({body:"0_squeeze"});
bb({body:"squeeze"});
```

(#act1_normal_choice)



# act1_normal

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: Ah legal, meu lobo voltou. Fantááástico.

`hong({eyes:"0_neutral"})`

n: SEU TRABALHO É PROTEGER SEU HUMANO DE *PERIGOS*

`bb({eyes:"look", mouth:"small_lock"})`

n: DE FATO, AQUELE SANDUÍCHE ESTÁ OS COLOCANDO EM *PERIGO* AGORA MESMO

n: RÁPIDO, OS AVISE!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Humano! Escute, estamos em perigo! O problema é que...

`bb({body:"squeeze"})`

n4: (DEIXE A _SUA_ ANSIEDADE SAIR PARA BRINCAR! ESCOLHA AQUILO QUE MAIS SE ASSEMELHA AO QUE _SEU_ MEDO DIZ)

(#act1_normal_choice)

# act1_normal_choice

[Estamos almoçando sozinhos, denovo!](#act1a_alone) `bb({body:"squeeze_talk"})`

[Não estamos produzindo nada ao comer!](#act1a_productive) `bb({body:"squeeze_talk"})`

[Esse pão branco aí é ruim pra gente!](#act1a_bread) `bb({body:"squeeze_talk"})`

# act1a_alone

```
bb({body:"normal", mouth:"small", eyes:"narrow"});
hong({body:"0_sammich"});
```

b: Você não sabe que solidão é associada com mortes prematuras tanto quanto o ato de fumar 15 cigarros ao dia?-

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: (Holt-Lunstad 2010, PLoS Medicine)

`hong({eyes:"0_annoyed"})`

h: Hum, obrigado por citar suas fontes mas--

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: Isso significa que, se nós não nos enturmarmos com alguém *agora mesmo*, a gente vai--

`bb({body:"panic"})`

b: MOOOOORREEEEEEEEEER

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "alone");
publish("hp_show");
```

(...2500)

`_.fifteencigs = true`

n: VOCÊ USOU *MEDO DE SER DESAMADO*

(#act1b)

# act1a_productive

```
bb({body:"normal", mouth:"small", eyes:"normal"});
hong({body:"0_sammich"});
```

b: Puxe o computador aí e trabalhe em alguma coisa agora mesmo!

`hong({eyes:"0_annoyed"})`

h: Hum, eu preferiria não derrubar migalhas no meu teclad--

```
bb({mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Se não estivermos contribuindo ao corpo-da-sociedade, então nós somos um parasita-da-sociedade!

b: O corpo-da-sociedade irá ao doutor-da-sociedade para medicação exterminadora de parasitas-da-sociedade e então a gente vai--

```
bb({body:"panic", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: MOOOOORREEEEEEEEEER

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "bad");
publish("hp_show");
```

(...2500)

`_.parasite = true`

n: VOCÊ USOU *MEDO DE SER ALGUÉM RUIM*

(#act1b)

# act1a_bread

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich", eyes:"0_annoyed"});
```

h: Você tem certeza que estes estudos foram comprov--

```
bb({body:"fear", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Trigo processado irá decolar nosso açúcar no sangue, e então eles terão que amputar todos os nossos membros, e então a gente vai--

`bb({body:"panic"})`

b: MOOOOORREEEEEEEEEER

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "harm");
publish("hp_show");
```

(...2500)

`_.whitebread = true`

n: VOCÊ USOU *MEDO DE SE MACHUCAR*

(#act1b)

# act1b

n: É SUPER EFETIVO

`bb({mouth:"smile", eyes:"smile"});`

b: Viu, humano? Eu sou seu leal lobo-guardião!

`bb({body:"pride_talk"});`

b: Acredite no seu coração! Seus sentimentos são sempre válidos!

`bb({body:"pride"});`

n: REDUZA A BARRA DE ENERGIA DE SEU HUMANO PARA ZERO

n: PARA PROTEGER SUAS NECESSIDADES FÍSICAS + SOCIAIS + MORAIS, VOCÊ PODERÁ USAR:

n: MEDO DE *SE MACHUCAR* #harm#

n: MEDO DE *SER DESAMADO* #alone#

n: E MEDO DE *SER UMA PESSOA RUIM* #bad#

`Game.OVERRIDE_TEXT_SPEED = 1.25;`

n4: (DICA: SELECIONE AS ESCOLHAS QUE PESSOALMENTE ATINGEM SEUS MAIORES, MAIS PROFUNDOS MEDOS!~)

h: ...

```
hong({body:"putaway"});
sfx("rustle");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

(...1000)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h: quer saber, talvez seja hora de olhar meu celular.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: PROTEJA SEU HUMANO.

n: DO MUNDO. DE OUTRAS PESSOAS. DELES MESMOS.

n: BOA SORTE!

(...500)

`Game.clearText()`

(...500)

(#act1c)

# act1c

`music('battle', {volume:0.5})`

n: ROUND 1: *BRIGUE!*

`bb({body:"normal", mouth:"normal", eyes:"normal"});`

h: Huh. Meu feed do facebook diz que vai rolar uma festa este final de semana.

`bb({eyes:"uncertain"});`

b: Aquela pessoa estranha não faz uma festa *todo* final de semana?

`bb({eyes:"uncertain_right"});`

b: Que tipo de vazio eles estão tentando preencher? Eles devem ser uma bagunça por dentro!

`hong({eyes:"surprise"});`

h: E, eu recebi um convite?

`bb({eyes:"fear", mouth:"normal"});`

b: Então!

[Diga sim, ou morreremos de solidão!](#act1c_loner)

[Diga não, será cheio de drogas fatais!](#act1c_drugs)

[Ignore, nós apenas arruinamos festas.](#act1c_sad)

# act1c_loner

{{if _.fifteencigs}}
b: 15 cigarros ao dia, humano! Quinze!
{{/if}}

{{if !_.fifteencigs}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if !_.fifteencigs}}
b: E então ninguém aparecerá no nosso funeral, eles arremessarão nossas cinzas sobre o oceano, seremos comidos por uma baleia,
{{/if}}

{{if !_.fifteencigs}}
b: e nos tornaremos CACA DE BALEIA!
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
b: Mas é, nós devemos ir para aquela festa!
{{/if}}

{{if _.parasite}}
b: Leve o computador para que possamos trabalhar, e não ser um parasita-da-sociedade.
{{/if}}

{{if _.whitebread}}
b: Contanto que eles não sirvam PÃO BRANCO.
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: DEUS. Tá, se isso fizer você calar a boca, tudo bem.

h: Vou dizer sim.

{{if _.whalepoop}}
b: Caca de baleia, humano! Caca de baleia!
{{/if}}

`_.partyinvite="yes"`

(#act1d)

# act1c_drugs

`bb({mouth:"small", eyes:"fear"});`

{{if _.whitebread}}
b: ou até pior... PÃO BRANCO.
{{/if}}

{{if _.whitebread}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if _.whitebread}}
b: Nós teremos uma overdose tão pesada de cocaina e pão branco que eles não irão conseguir caber nossa bunda gorda dentro da fornalha de cremação!
{{/if}}

{{if !_.whitebread}}
b: Nós teremos uma overdose com tantas drogas que o funerário irá se perguntar como que nosso corpo já *havia sido* embalsamado!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.parasite}}
b: Fora isso, não podemos festejar; precisamos trabalhar ou seremos horríveis parasitas-da-socidade!
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: DEUS. Tá, se isso fizer você calar a boca, tudo bem.

h: Vou dizer não.

`_.partyinvite="no"`

(#act1d)

# act1c_sad

`bb({eyes:"uncertain_right", mouth:"normal"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.fifteencigs}}
b: Tudo que fazemos em festas é reclamar em um canto sobre como solidão é tão mortífera quanto fumar 15 cigarros ao dia.
{{/if}}

{{if _.parasite}}
b: Tudo que fazemos em festas é nos preocupar como deveriamos estar sendo produtivos.
{{/if}}

{{if _.whitebread}}
b: Tudo que fazemos em festas é nos preocupar como as opções de comida não saudáveis vão nos matar.
{{/if}}

```
bb({mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"lookaway"});
```

h: ^por^ra me pergunto por que será.

`hong({eyes:"neutral"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: Então se irmos, nós faremos eles se sentirem mal, mas se rejeitarmos o convite nós também iremos fazer eles se sentirem mal!

`bb({body:"fear", eyes:"fear"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: TUDO QUE FAZEMOS FAZ COM QUE AS PESSOAS SE SINTAM MAL, LOGO NÓS DEVEMOS NOS SENTIR MAL

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`hong({mouth:"anger", eyes:"anger"});`

h: Ugh. Se isso fizer você calar a boca, tudo bem.

h: Eu vou ignorar o convite.

`_.partyinvite="ignore"`

(#act1d)

# act1d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"annoyed"});
```

h: De qualquer forma. Facebook é um pouco demais. Preciso de algo mais calmo, menos propício a ansiedade.

`hong({eyes:"neutral"});`

h: O que há no Twitter?

`bb({eyes:"look"});`

[Ah não, olhe este terrível artigo de notícia!](#act1d_news)

[Ah não, seria aquele tweet sobre *nós*?](#act1d_subtweet)

[Olhe, um GIF de um gato bebendo leite](#act1d_milk)


# act1d_news

```
bb({eyes:"pained1"});
music(null, {fade:2});
```

b: Meu Deus, é como se o mundo estivesse em chamas, não é?

```
bb({eyes:"pained2"});
hong({mouth:"sad", eyes:"sad"});
```

b: Parece que está tudo acabando, como se tudo estivesse morrendo e como nós estivéssemos perdidos com nada que possamos fazer a respeito.

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
bb({mouth:"shut"});
```

b: ...

`bb({mouth:"smile", eyes:"smile"});`

b: Mas, vamos retweetar esse artigo!

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

h: Tá bom, eu vou retweetar, mas por favor fique quieto!

`hong({mouth:"neutral", eyes:"annoyed"});`

h: Dane-se, vamos dar uma olhada no Snapchat.

(#act1e)


# act1d_subtweet

`bb({eyes:"fear"});`

b: É um subtweet! Um esperto subtweet sorrateiro!

`hong({eyes:"annoyed"});`

h: Provavelmente não é?

`bb({eyes:"narrow", mouth:"small"});`

b: mas e se eles estiverem falando pelas nossas costas

h: Eles n--

`bb({body:"fear", eyes:"fear", mouth:"normal"});`

b: NA FRENTE DAS NOSSAS COSTAS

`hong({eyes:"sad", mouth:"sad"});`

h: Eu n--

`bb({eyes:"narrow", mouth:"small"});`

b: Mas *e se for*

h: S--

`bb({eyes:"narrow_eyebrow"});`

b: *e se for*

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

h: o-KAY, vou olhar meu Snapchat.

(#act1e)

# act1d_milk

`hong({mouth:"smile", eyes:"neutral"});`

h: Hehe sim é bonitinho, acabei de retweetar, eu ach--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: GATOS NÃO PODEM DIGERIR LEITE SOMOS PESSOAS TERRÍVEIS POR CURTIR O ABUSO DE ANIMAIS

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

h: o-KAY, vou olhar meu Snapchat.

(#act1e)

# act1e

`hong({mouth:"neutral", eyes:"neutral"});`

h: Huh, fotos de ontem a noite. Então *é assim* que aquelas festas semanais são.

{{if _.partyinvite=="yes"}} (#act1e_said_yes) {{/if}}

{{if _.partyinvite=="no"}} (#act1e_said_no) {{/if}}

{{if _.partyinvite=="ignore"}} (#act1e_said_ignore) {{/if}}

# act1e_said_yes

`hong({mouth:"sad", eyes:"annoyed"});`

h: Vish, parece muito cheio de gente para a minha ansiedade.

h: Talvez eu deveria ter dito não para o convite?

```
hong({mouth:"neutral", eyes:"neutral"});
bb({mouth:"normal", eyes:"normal"});
```

[Mudar de idéia? E ser babaca?!](#act1e_yes_dontchange)

[Mudar de idéia! É muito cheio!](#act1e_yes_changetono)

{{if _.subtweet}}
[Poisé, eles estavam subtweetando a gente mesmo.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Espere, nós retweetamos o artigo sem checar fatos.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Sabia que você senta com uma péssima postura?](#act1e_ignore_posture)
{{/if}}

# act1e_yes_dontchange

```
bb({eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Eles estavam contando conosco para ir, e agora estamos traindo a confiança deles? Você quer morrer na solidão?

{{if _.fifteencigs}}
b: QUINZE. CIGARROS.
{{/if}}

{{if _.whalepoop}}
b: CACA. DE. BALEIA.
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

h: Cale a boca cale A BOCA eu vou manter o meu sim!

(#act1f)

# act1e_yes_changetono

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Você nunca ouviu falar de pisoteamento humano?

```
bb({body:"fear", mouth:"small", eyes:"narrow"});
hong({eyes:"sad", mouth:"sad"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Em 2013 uma boate em Santa Maria pegou fogo e o pânico fez com que as pessoas engarrafassem as saídas e 200 pessoas queimaram vivas-

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({mouth:"shock"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: VOCÊ QUER QUE ISSO ACONTEÇA COM A GENTE-

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 2.5;
```

b: DIGA NÃO DIGA NÃO DIGA NÃO DIGA NÃO DIGA NÃO DIGA N-


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

h: Cale a boca cale A BOCA eu vou mudar para não! DEUS!

(#act1f)

# act1e_said_no

`hong({mouth:"sad", eyes:"sad"});`

h: Hm... parece bem legal.

h: Talvez eu não deveria ter dito não para o convite?

`bb({mouth:"normal", eyes:"normal"});`

[Mudar de idéia? E ser babaca?!](#act1e_no_dontchange)

[Mudar de idéia! Não morra na solidão!](#act1e_no_changetoyes)

{{if _.subtweet}}
[Poisé, eles estavam subtweetando a gente mesmo.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Espere, nós retweetamos o artigo sem checar fatos.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Sabia que você senta com uma péssima postura?](#act1e_ignore_posture)
{{/if}}

# act1e_no_dontchange

`bb({eyes:"anger"})`

b: Todos estavam contando conosco!

b: ...em deixá-los em paz para que pudessem ter uma boa festa sem uma pessoa esquisita {{if _.whitebread}}comedora-de-pão-branco{{/if}} bizarra que nem você--


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

h: Cale a boca cale A BOCA eu vou deixar como não!

(#act1f)

# act1e_no_changetoyes

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Solidão crônica aumenta os níveis de cortisol juntamente ao risco de doenças cardivasculares e derrames!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.fifteencigs}}
b: QUINZE. CIGARROS.
{{/if}}

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Cale a boca cale A BOCA eu vou mudar para sim! Deus!

(#act1f)

# act1e_ignore_subtweet

```
bb({eyes:"fear", mouth:"small"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Todos os nossos tweets problemáticos voltaram para nos crucificar!

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.7;
```

b: Nós vamos ser expostos, cancelados, arrastados pela super-rodovia da informação por uma corda de acusações!

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

h: Por que você é assim?!

(#act1f)

# act1e_ignore_factcheck

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Nós estamos espalhando desinformação! Destruindo a integridade da imprensa livre!

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Somos a razão pela qual o fascismo irá se erguer sobre as ruínas da democracia!

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

h: Por que você é assim?!

(#act1f)

# act1e_ignore_posture

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Você quer que sua coluna vire um pretzel?! Pare de ficar que nem um corcunda sobre a tela!

```
bb({body:"meta"});
```

b: Isso significa você também.

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

h: Por que você é assim?!

(#act1f)

# act1e_said_ignore

`hong({mouth:"sad", eyes:"sad"});`

h: Hm... parece bem legal.

h: Talvez eu não deveria ter ignorado o convite?

`bb({mouth:"normal", eyes:"normal"});`

[Continue ignorando, somos terríveis em festas ainda.](#act1e_ignore_continue)

[Na real, diga sim.](#act1e_ignore_changetoyes)

[Na real, diga não.](#act1e_ignore_changetono)

# act1e_ignore_continue

`hong({eyes:"annoyed"});`

h: Mas é um pouco grosso continuar a ignorá-los, não é?

`bb({eyes:"normal_right"});`

b: Bem, outras pessoas sempre ignoram *a gente*, então

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

b: vamos dizer que é um empate.

(#act1f)

# act1e_ignore_changetoyes

`hong({eyes:"surprise", mouth:"smile"});`

h: Você... está deixando que eu me divirta?

b: Bem, digo, solidão *pode* nos matar.

`hong({eyes:"neutral", mouth:"neutral"});`

(#act1e_no_changetoyes)

# act1e_ignore_changetono

`bb({eyes:"narrow"});`

b: É muita gente. Multidões são perigosas.

(#act1e_yes_changetono)


# act1f

```
hong({mouth:"neutral", eyes:"neutral"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: Tanto faz. Nova notificação no Tinder.

`bb({eyes:"uncertain"})`

b: O que, aquele app de sexo?

`hong({eyes:"annoyed"})`

h: Não é um app de sexo, é só um jeito de conhecer novas pess--

`bb({eyes:"narrow"})`

b: É um app de sexo.

```
hong({eyes:"surprise", mouth:"smile"});
bb({eyes:"normal"});
```

h: Oh, recebi um match! Essa pessoa é bonitinha!

```
bb({eyes:"narrow_eyebrow"});
hong({eyes:"sad", mouth:"anger"})
```

h: Por favor não arruine isso pra m--

```
bb({body:"panic"});
Game.OVERRIDE_TEXT_SPEED = 2.0;
```

b: PERIGO PERIGO PERIGO PERIGO PERIGO PERIGO PERIGO 

`bb({body:"fear", eyes:"fear", mouth:"normal"})`

[Nós estamos sendo *usados* por outros.](#act1f_used_by_others)

[Nós estamos *usando* os outros.](#act1f_using_others)

[SEU MATCH É UM ASSASSINO EM SÉRIE](#act1f_killer)

# act1f_used_by_others

`bb({body:"point_crotch", eyes:"normal", mouth:"normal"})`

b: Sexo casual talvez preencha o buraco ali embaixo,

b: mas nunca irá preencher o buraco...

`bb({body:"point_heart", eyes:"pretty", mouth:"small"})`

b: aqui *dentro*.

(...1000)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: O que estou dizendo é que, VAMOS MORRER SOZINHOS

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.hookuphole=true`

(#act1g)

# act1f_using_others

`bb({eyes:"narrow", mouth:"small"})`

b: Você acha que a genitália alheia são como Pokémons para colecionar?

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

b: ♫ (música tema do pokemon)-

(...5600)

```
bb({mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2400;
```

b: ♫ Esse meu jeito de ^fod^er-

(...500)

```
bb({eyes:"narrow", mouth:"small"});
Game.FORCE_TEXT_DURATION = 2100;
```

b: ♫ Ninguém nunca viu igual-

(...1500)

```
bb({eyes:"pretty"});
Game.FORCE_TEXT_DURATION = 2300;
```

b: ♫ A minha vida é prazer-

(...500)

```
bb({eyes:"fear", mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2000;
```

b: ♫ Peitos, r^ol^a e ^an^al!-

(...1000)

```
bb({eyes:"smile", mouth:"smile"});
Game.FORCE_TEXT_DURATION = 1000;
```

b: ♫ PU^TA^-MON! TEMOS QUE PEG-

```
Game.FORCE_CANT_SKIP = false;
Game.clearText();
music(false);
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Quero dizer que somos nojentos e manipuladores.

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
b: Eles vão te prender em um poço e te forçar a comer pão branco para te engordar, e então vestir a sua pele como uma macacão!
{{/if}}

{{if _.parasite}}
b: Eles vão te bater com um temporizador de pomodoro e dizer "VOCÊ DEVERIA TER PRODUZIDO MAIS, PARASITA"
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Eles vão estraçalhar sua carne em confetti, transformar seus orgãos em serpentinas, misturar seu sangue em uma bacia de ponche
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Que tal ISSO como convite de festa?!
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

h: estou ficando doente com este jogo.

(...700)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h:
{{if _.fifteencigs}}"solidão vai nos matar"... {{/if}}
{{if _.parasite}}"somos um parasita-da-sociedade"... {{/if}}
{{if _.whitebread}}"não coma aquilo, vai nos matar"... {{/if}}
{{if _.subtweet}}"eles estão falando pelas nossas costas"... {{/if}}
{{if _.badnews}}"o mundo está em chamas"... {{/if}}
{{if _.hookuphole}}"vamos morrer em solidão"... {{/if}}
{{if _.serialkiller}}"eles são um assassino em série"... {{/if}}
{{if _.catmilk}}"gatos não digerem leite"... {{/if}}
{{if _.pokemon}}uma ^merda^ de paródia musical... {{/if}}

h: eu só quero viver minha vida

h: eu só quero ser livre, livre de toda essa... dor.

`bb({eyes:"look_sad"});`

b: Ei... humano...

`Game.OVERRIDE_TEXT_SPEED = 0.5;`

b: Vai ficar tudo bem.

(...600)

`bb({body:"point_heart", eyes:"look_sad_smile", mouth:"smile"});`

b: Como seu leal lobo-guardão, eu sempre estarei a procura do perigo, fazendo meu melhor para manter você em segurança.

`bb({body:"normal", eyes:"look_sad", mouth:"smile"});`

b: Eu prometo.

(...600)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({body:"phone1", eyes:"neutral", mouth:"neutral"});
```

h: Último app. Instagram. Que que você tem?

`hong({eyes:"sad"});`

h: São... mais fotos de festas.

`hong({mouth:"sad"});`

h: Todo mundo parece tão feliz. Livres de preocupações. Livres de ansiedade.

`hong({mouth:"anger"});`

h: Meu Deus, por que não posso ser como eles? Por que não posso ser *normal?*

`bb({eyes:"normal_right"});`

b: Falando em festas, sobre o convite deste final de semana. Aqui está minha decisão FINAL:

`bb({eyes:"normal"});`

[Devemos ir.](#act1g_go) `Game.OVERRIDE_CHOICE_LINE=true`

[Devemos ficar longe.](#act1g_dont) `Game.OVERRIDE_CHOICE_LINE=true`

# act1g_go

`_.act1g = "go"`

(#act1h)

# act1g_dont

`_.act1g = "dont"`

(#act1h)

# act1h

b: Dev--

```
bb({eyes:"wat", mouth:"small"});
hong({body:"2_fuck"});
```

h: *F^OD^A.*

`hong({body:"2_you"});`

h: -SE.

(...500)

b: o

(...1500)

`bb({eyes:"wat_2"});`

b: o que?

`hong({body:"phone1", eyes:"anger", mouth:"anger"});`

h: Eu vou dizer SIM para aquela festa,

{{if _.act1g=="go"}}
h: NÃO porque você quer, mas porque *EU* quero.
{{/if}}

{{if _.act1g=="dont"}}
h: Precisamente PORQUE você não quer que eu vá.
{{/if}}

```
hong({body:"putaway"});
sfx("rustle");
```

h: Você não me controla.

```
sfx("rustle2");
hong({body:"0_sammich", eyes:"0_annoyed", mouth:"0_neutral"});
```

h: Agora, me dê licença enquanto eu como esse ^caralho^ de sanduíche delicioso em paz.

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

[AHHHH A GENTE VAI MORRER](#act1h_death) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH TODO MUNDO NOS ODEIA](#act1h_loneliness) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH SOMOS PESSOAS HORRÍVEIS](#act1h_worthless) `Game.OVERRIDE_CHOICE_LINE = true;`

# act1h_death

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH A GENTE VAI MORRER AAAAAAHHHHHHH

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

b: AHHHH TODO MUNDO NOS ODEIA AAAAAAHHHHHHH

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

b: AHHHH SOMOS PESSOAS HORRÍVEIS AAAAAAHHHHHHH

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

n: PARABÉNS!

(...500)

n: VOCÊ PROTEGEU AS NECESSARIDADES FÍSICAS + SOCIAIS + MORAIS DO SEU HUMANO COM SUCESSO.

n: ALÁ, OLHE COMO ELES ESTÃO GRATOS

(...500)

n: AGORA QUE A ENERGIA DELES ESTÁ EM ZERO, VOCÊ PODERÁ CONTROLAR SUAS AÇÕES DIRETAMENTE

`bb({mouth:"smile", eyes:"normal"});`

n: ESCOLHA SEU GOLPE FINAL

`bb({mouth:"small_lock", eyes:"fear"});`

n: *ACABE COM ELES*

[{LUTAR: Puna seu celular estressante!}](#act1i_phone) `Game.OVERRIDE_CHOICE_LINE=true`

[{FUGIR: Assuma posição fetal e chore!}](#act1i_cry) `Game.OVERRIDE_CHOICE_LINE=true`

# act1i_phone

`bb({mouth:"normal", eyes:"narrow"})`

b: Seu celular estava prestes a te causar um ataque de pânico!

`bb({eyes:"anger"})`

b: Zuckerberg e compania estão abduzindo sua saúde mental por lucros capitalistas fáceis!

```
bb({body:"fear", eyes:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Entregue punição ao celular! Destrua-o! Mate-o!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "fight";
```

b: MATE-O MATE-O MATE-O MATE-O MATE-O MATE-O MATE-O MATE-O MATE-O MATE-O MATE-O MATE-O MATE-O MATE--

(#act1j)

# act1i_cry

`bb({eyes:"fear", mouth:"normal"})`

b: O mundo inteiro está cheio de perigos!

```
bb({body:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Faça como um tatu-bola! Se englobe em auto-defesa!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "flight";
```

b: ENGLOBE E CHORE ENGLOBE E CHORE ENGLOBE E CHORE ENGLOBE E CHORE ENGLOBE E CHORE ENGLOBE E CHOR--

(#act1j)

# act1j

`SceneSetup.act1_outro()`