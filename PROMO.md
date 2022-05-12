# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[ГРАТИ!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: Перед початком, як *тобі* подобається читати?

`publish("show_options_bottom")`

# intro-start-2

n3: Тепер, почнемо нашу історію...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: ЦЕ - ЛЮДИНА

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

```
SceneSetup.act1();
publish("hide_tabs");
music('battle', {volume:0.5});
```

(...300)

n: І ЦЕ ЛЮДСЬКА ТРИВОГА

n: _ТИ_ Є ТРИВОГА

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Ні. Ні, ні, не слухаю. Потрібно перевірити мобільний.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: ТВОЯ РОБОТА ОБЕРІГАТИ СВОЮ ЛЮДИНУ ВІД *ЗАГРОЗИ*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: Ох! Ти колись так проскролиш своє життя у Твітері! Знову!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: Еге, чому я просто не буду частіше сидіти і слухати свої думки.

`hong({eyes:"neutral"});`

n: ШВИДШЕ, ПОПЕРЕДЬ ЇЇ ПРО *ЗАГРОЗУ!*

```
bb({eyes:"look"});
```

[Оу ні, подивись на цю жахливу новину!](#act1d_news)

[Оу ні, невже цей твіт насправді про *нас?*](#act1d_subtweet)

[Гей, гіфка кота, що п'є молоко.](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: Хех, це мило, я--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: КОТИ НЕ ПЕРЕТРАВЛЮЮТЬ МОЛОКО, ЯКІ МИ ЖАХЛИВІ ЗА ТЕ ЩО НАСОЛОДЖУЄМСЯ НАСИЛЬСТВОМ

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



