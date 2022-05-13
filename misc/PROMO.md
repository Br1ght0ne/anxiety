# intro

`SceneSetup.intro();`

# intro-play-button

[<div class="mini-icon" pic="play1"></div> ГРАТИ! <div class="mini-icon" pic="play2"></div>](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: дурень

`publish("show_options_bottom")`

# intro-start-2

`clearText()`

(...1000)

`publish("intro-to-game-2")`

n2: ЦЕ - ЛЮДИНА

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

`SceneSetup.act1();`

(...300)

n: І ЦЕ ЛЮДСЬКА ТРИВОГА

n: _ТИ_ Є ТРИВОГОЮ

[Ти знов обідаєш одна! Знову!](#act1a_alone)

[Ти не продуктивна поки їси!](#act1a_productive)

[Цей білий хліб шкідливий для тебе!](#act1a_bread)

# act1a_alone

`bb({mouth:"small", eyes:"narrow"})`

b: Ти знаєш, що самотність асоціюється з предчасною смертю , так само як викурені 15 сигарет за день?-

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: (Holt-Lunstad et al, 2010, PLoS Medicine)

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: Ем, дякую за інформацію але--

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: Що означає, якщо ти не будеш тусуватись з кимось *прямо зараз* ти-

`bb({body:"panic"})`

b: ВМРЕЕЕЕЕШШШ

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("20p", "alone");
publish("hp_show");
```

(...2500)
