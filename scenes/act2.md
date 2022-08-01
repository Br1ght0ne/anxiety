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

s: Ти *бачила* цю "історію з новин", про ці жахливі речі, що десь стались?

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: х-хай...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",3]);
```

a: Боже, я ненавиджу новини. Лише одні сенсації та клікбейти.

```
publish("act2",["dum",2]);
publish("act2",["party_hong","next"]);
```

h2: к... класна вечірка...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",1]);
```

s: Так, але вони все це роблять для винагороди. *Справжня* проблема - люди, що довіряють клікбейтам.

```
publish("act2",["dee",3]);
```

s: Хто ретвітить такі жахливі історії, які псують друзям настрій?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Егх, я ніби знаю?

(#act2-preamble-end)


# act2-preamble-news2

```
publish("act2",["dee",3]);
```

s:  Ти *бачила* цю "новину", що стала популярною?

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: х-хай...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",3]);
```

a: Так, повна ^лажа^. Хто такому повірить і буде ретвітити?

```
publish("act2",["dum",2]);
publish("act2",["party_hong","next"]);
```

h2: к... класна вечірка...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Серйозно чувак. Типу, привіт, може відкриєш Гугл і чекниш факти?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Егх, напевно?

(#act2-preamble-end)


# act2-preamble-cat

```
publish("act2",["dee",3]);
```

s: Як я і говорю. Індустрійний Мемний Комплекс експлотує котів.

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: х-хай...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",1]);
```

a: Доведи свою тезу.

```
publish("act2",["dum",0]);
publish("act2",["party_hong","next"]);
```

h2: х... хороша вечірка...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",1]);
```

s: Ну, вчора хтось ретвітнув гіфку кота, який пив молоко.

```
publish("act2",["dee",3]);
```

s: Вони не перетравлюють це ^гівно^! Хто ретвітить таке *насильство над тваринами*?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Егх, правда?

(#act2-preamble-end)


# act2-preamble-tinder

```
publish("act2",["dee",1]);
```

s: Вона так і не відповіла!

```
publish("act2",["dee",0]);
publish("act2",["party_hong","next"]);
```

h2: х-хай...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",1]);
```

a: Навіть коли у вас метч в Тіндері?

```
publish("act2",["dum",0]);
publish("act2",["party_hong","next"]);
```

h2: к... класна вечірка...

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

s: Еге ж! Вона що, думає я якийсь *серійний вбивця*, або типу того? Параноїк.

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Егх, правда?

(#act2-preamble-end)


# act2-preamble-hookuphole

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Ага! Напевно вона думає, що такі зустрічі не зможуть заповнити дірку в її серці?

s: Припини бути такою обережною! Відкрий свій розум, а згодом ноги!

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Егх, правда?

(#act2-preamble-end)


# act2-preamble-pokemon

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Ага! Вона не гаряча штучка, але була б прекрасним уловом!

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Я спіймаю їх всіх!™

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

n: РАУНД ДРУГИЙ: *БОРИСЬ!*

[О ні, вони всі нас ненавидять!](#act2a_social)

[Ти *дивилась* на цього рижого?](#act2a_perv)

[Гей, давай поговоримо про значення життя.](#act2a_meaning)

# act2a_social

`bb({eyes:"sad"})`

b: Ти портиш всім настрій на цій вечірці, тим що ти настільки відстійна!

`bb({eyes:"shock", body:"two_up"})`

b: Ми вбиваєм цей прекрасний вайб! Ти вчинила вайб-вбивство першого ступеня!

`bb({eyes:"normal", body:"normal"})`

b: Людино, тобі потрібно йти *зараз* пер--

```
_.a2_first_danger = 'social';
_.a2_attack_1 = "alone";
```

(#act2b)

# act2a_perv

`bb({eyes:"suspect"})`

b: Вони привабливіші за нас, якщо ти просто *подивишся* на них, тоді--
 
`bb({eyes:"shock", body:"two_up"})`

b: ТИ СТРАШИЛА

`bb({body:"normal"})`

b: Ти страшна, зла, погана, погана, жахлива, жахлива збоче--

```
_.a2_first_danger = 'perv';
_.a2_attack_1 = "bad";
```

(#act2b)

# act2a_meaning

`bb({body:"one_up", eyes:"normal_r"})`

b: В решті-решт, що ти можеш зробити *дійсно* вагоме? 

`bb({body:"normal", eyes:"sad"})`

b: Зробити внесок для людства? Всі великі роботи руйнуються, як Озимандія. Кохання? Смерть завжди розлучить.

`bb({eyes:"sad_r"})`

b: І скільки там смерті! *Ти* помреш. *Твої кохані* теж помруть.

`bb({eyes:"shock", body:"two_up"})`

b: Чорт, Другий Закон Термодинаміки доказує, що навіть наш *всесвіт* помре!

`bb({eyes:"suspect", body:"normal"})`

b: Ох, "смерть змушує цінити життя"? Це те саме, як "рабство хороше, бо так ми більше цінуєм нашу волю"!

`bb({body:"one_up"})`

b: Ох, "тобі потрібно знайти своє призначення"? Саме це роблять конспірологи та окультисти!

`bb({eyes:"shock", body:"two_up"})`

b: У життя нема значення, у смерті нема значення, навіть у *значення* нема значення! Що смертна душа повинна--

```
_.a2_first_danger = 'meaning';
_.a2_attack_1 = "bad";
```

(#act2b)

# act2b

`bb({eyes:"normal", mouth:"normal", body:"normal", MOUTH_LOCK:true})`

b: ...

`bb({eyes:"suspect"})`

b: Ем... ти мене чуєш, людино?

`bb({eyes:"normal", MOUTH_LOCK:true})`

b: ...

`bb({eyes:"shock", mouth:"small_talk", body:"chest", MOUTH_LOCK:true})`

b: *АХ*

`bb({mouth:"small_talk"})`

b: Я МАЮ ЗАСТЕРЕГТИ ТЕБЕ ПРО...

[*БІЛЬШЕ* ПРО ЦЮ ЗАГРОЗУ!](#act2b_louder)

{{if _.a2_first_danger=="social"}}
[Про *іншу* моральну загрозу!](#act2b_different_social)
{{/if}}

{{if _.a2_first_danger=="perv" || _.a2_first_danger=="meaning"}}
[Про *іншу* моральну загрозу!](#act2b_different_moral)
{{/if}}

[Ти ігноруєш загрозу! Це небезпечно!](#act2b_ignore)

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

b: ЕМОЦІЇ ЗАРАЗНІ! ТОМУ, ЯКЩО ТИ НЕ ПІДЕШ, ТИ ЗАРАЗИШ УСІХ СВОЄЮ ПСИХІЧНОЮ ХВОРОБОЮ! 

b: Ти створиш смертельну пандемію СИНДРОМУ ЗАНУДИ

`bb({eyes:"suspect", body:"normal", mouth:"normal"})`

b: Тобі потрібно йти звідси, обмежети себе від всіх навіки, у маленькій кімнатці з Нетфліксом і доставкою їжі!

```
_.a2_second_danger = 'netflix';
_.a2_attack_2 = "alone";
_.a2_hoodie_callback = "a quarantine";
```

(#act2c)

# act2b_louder_perv

`bb({eyes:"suspect", body:"two_up", mouth:"normal"})`

b: НЕ БУДЬ СТРАШИЛОЮ. ЦЕ ПРОТИ ЗАКОНУ!

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

b: Закон Слимаків, Секція 74.5: (1) Люди, що дивляться на (а) ці накачені плечі, (б) округлу ^жопку^, (2) повинні бути всім відомі як

`bb({eyes:"shock", body:"two_up", mouth:"normal"})`

b: "ОГИДНІ СМІТТЄВІ ЗБОЧЕНЦІ"

```
_.a2_second_danger = 'law';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "the law";
```

(#act2c)

# act2b_louder_meaning

`bb({body:"two_up", mouth:"normal", eyes:"shock"})`

b: Врешті, навіть якщо ти знайдеш шляхетних сенс у житті, ти *досі* можеш все зіпсувати!
 
`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Альфред Нобель хотів миру у світі, щоб усі культури розуміли одне одного. Він намагався полегчити подорожі.

`bb({eyes:"normal_r"})`

b: Він шукав дешевий метод створення тунелів для поїздів. Так і винайшли новий матеріал - "динаміт"...

`bb({body:"one_up", eyes:"normal"})`

b: який був використаний в Першій Світовій Війні ДЛЯ ВБИВСТВ 

`bb({body:"two_up", eyes:"shock"})`

b: ЦЕ ЕФЕКТ МЕТЕЛИКА, ЛЮДИНО! СКІЛЬКОХ ЛЮДЕЙ ТИ ВИПАДКОВО ВБИВАЄШ ПРЯМО ЗАРАЗ

```
_.a2_second_danger = 'butterfly';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "World War I";
```

(#act2c)

# act2b_different_social

`_.a2_first_choice = "different"`

`bb({eyes:"normal_r", body:"point", mouth:"normal"})`

b: Ти знаєш, що може бути гіршим, коли ніхто не любить тебе? Коли ти *всім* подобаєшся.

`bb({body:"one_up", eyes:"suspect", mouth:"normal"})`

b: Ось так, стати *цією* тваринкою, що полює на задоволення.

`bb({body:"normal", mouth:"small"})`

b: Дрібне життя, з дрібними друзями, які знають лише дрібну тебе!

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: Людино, тобі потрібно втікти від цих зомбі-задоволень, перед тим, як станеш однією з них!

```
_.a2_second_danger = 'zombies';
_.a2_attack_2 = "alone";
_.a2_hoodie_callback = "zombies";
```

(#act2c)

# act2b_different_moral

`_.a2_first_choice = "different"`

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: Цілі сім'ї помирають під час геноциду *саме зараз*, а ми веселимось!

`bb({body:"point", eyes:"closed", mouth:"small"})`

b: Мудра людина колись сказала, -"Єдине, що потрібно для тріумфу зла - це те, щоб добрі люди нічого не робили"

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: ТИ НІЧОГО НЕ РОБИШ.

`bb({mouth:"small"})`

b: ВЕЧІРКОЮ, МИ ДОПОМАГАЄМ *ГІТЛЕРУ*.

```
_.a2_second_danger = 'hitler';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "Hitler";
```

(#act2c)

# act2b_ignore

`_.a2_first_choice = "ignore"`

`bb({body:"normal", mouth:"normal", eyes:"suspect"})`

b: Ти думаєш, що ти в безпеці, тільки тому що висунула батарейки з детектора чадного газу?

`bb({eyes:"suspect_r"})`

b: Ти навіть не відчуєш запаху отрути! Ти просто відчуєш себе сонною і тоді ти --

`bb({body:"scream_c_1"})`

b: ВМРЕЕЕЕЕШШШШ

```
_.a2_second_danger = 'ignore';
_.a2_attack_2 = "harm";
_.a2_hoodie_callback = "carbon monoxide";
```

(#act2c)

# act2c

```
hong({body:"ignore_sweat"});
bb({eyes:"normal", mouth:"normal", body:"normal", MOUTH_LOCK:true});
```

b: ...

`bb({eyes:"happy", mouth:"smile", body:"chest"})`

b: О, дякую тобі боже, людино, ти знову можеш чути мене!

`bb({eyes:"closed", body:"point"})`

b: Я МАЮ ЗАСТЕРЕГТИ ТЕБЕ ПРО...

{{if _.a2_first_choice=="louder"}}
[*ЩЕ БІЛЬШЕ* ПРО ЦЮ ЗАГРОЗУ!](#act2c_louder)
{{/if}}

{{if _.a2_first_choice!="louder"}}
[*БІЛЬШЕ* ПРО ЦЮ ЗАГРОЗУ!](#act2c_louder)
{{/if}}

{{if _.a2_first_danger=="social"}}
[Про *іншу* соціальну загрозу!](#act2c_different_social)
{{/if}}

{{if _.a2_first_danger=="perv" || _.a2_first_danger=="meaning"}}
[Про *іншу* моральну загрозу!](#act2c_different_moral)
{{/if}}

[Ти перевірила цей пунш перед тим як пити?](#act2c_punch)

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

b: І ще, Нетфлікс та доставка їжі недостатньо ізольовані! Ти можеш заразити особу з доставки!

`bb({body:"one_up", mouth:"small"})`

b: Ти маєш переїхати до території Канадського Юкону, щоб твою їжу доставляли дроном!

`bb({body:"two_up", mouth:"normal"})`

b: І тоді вони будуть дезінфікувати дрон, щоб позбутись ЗБУДНИКІВ ЗАНУДИ

`_.a2_attack_3 = "alone";`

`_.a2_hoodie_callback = "a quarantine";`

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

b: ВЕЛИКИЙ ОГИДНИЙ ЗБОЧЕНЕЦЬ повинен бути заключеним 72 години, в цих середньовічних засобах для публічного приниження

b: хіба, вони можуть секретно *захоплюватись* таким

`bb({body:"scream_a_1"})`

b: тому що вони ВЕЛИЧЕЗНІ ОГИДНІ ЗБОЧЕНЦІ

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "the law";`

(#act2d)

# act2c_louder_butterfly

`bb({body:"normal", mouth:"small", eyes:"suspect"})`

b: ЕФЕКТ МЕТЕЛИКА! Ти використовуєш пластикову чашку?

`bb({body:"two_up", mouth:"normal", eyes:"shock"})`

b: БАМ, ЗВАЛИЩЕ ПОВНЕ ОТРУТИ, ЯКЕ ВБИВАЄ ДІТЕЙ

`bb({body:"normal", mouth:"small", eyes:"suspect"})`

b: Ти потієш і у тебе шалено б'ється серце?

`bb({body:"scream_a_1"})`

b: БАМ, ТИ ОБАНКРУТИЛА МЕДИЦИНУ І МІЛЬЙОНИ ПОМИРАЮТЬ
 
`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "the butterfly effect";`

(#act2d)

# act2c_louder_zombies

`bb({body:"normal", mouth:"small", eyes:"angry"})`

b: Ці зомбі-насолоди оточуть тебе, і будуть мугикати:

`bb({body:"normal", mouth:"normal", eyes:"shock"})`

b: ВПОДОБААЙКИ. ВПОДОБААЙКИ.

`bb({body:"scream_a_1"})`

b: І тоді вони ВКУСЯТЬ ТЕБЕ і ти станеш БРО БЕЗМІЗГІВ і/або ^ШЛЬОНДРОЮ^ БЕЗГОЛОВОЮ!

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "zombies";`

(#act2d)

# act2c_louder_hitler

`bb({body:"scream_a_1"})`

b: НАЦИСТИ ПРЯМО ЗАРАЗ КРОКУЮТЬ ВУЛИЦЯМИ

`bb({body:"one_up", mouth:"smile", eyes:"happy"})`

b: Говорячи: *добре, що ці «хороші люди» розслабилися з «розслабленням» та «доглядом за собою»!*

`bb({body:"point", mouth:"smile", eyes:"happy_r"})`

b: *Тепер наші плани можуть відійти, рейх за розкладом!*

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "Hitler";`

(#act2d)

# act2c_louder_ignore

`bb({body:"normal", mouth:"normal", eyes:"normal_r"})`

b: Якщо подумати, чи *є* в цій будівлі детектор чадного газу?!

`bb({body:"two_up", mouth:"small", eyes:"normal"})`

b: А якщо ми всі отруємся *У ЦЮ МИТЬ?*

`bb({body:"scream_a_1"})`

b: МИ НАВІТЬ НЕ ПОМІТИМО ПІДСТУП СМЕРТІ, МИ ПЕРЕСТАНЕМ ІСНУВАТИ НАВІКИ, І ВІКИ, І ВІ--

`_.a2_attack_3 = "harm";`

`_.a2_hoodie_callback = "carbon monoxide";`

(#act2d)

# act2c_different_social

`bb({body:"normal", mouth:"normal", eyes:"sad"})`

b: Що, якщо ти просто *в принципі нездатна* колись бути коханою, або кохати іншого?

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: А якщо, щось безповоротно зламалося всередині тебе уже давно? Або взагалі ніколи не існувало в тебе?

`bb({body:"scream_a_1"})`

b: АГХ ТИ ЗЛАМАНА! ТАКА, ТАКА, ТАКА ЗЛАМА--

`_.a2_attack_3 = "alone";`

(#act2d)

# act2c_different_moral

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Що, якщо ти просто *фундаментально гнила?*

`bb({body:"one_up", eyes:"sad"})`

b:  У інших є внутрішній привід робити добро, а ти це робиш через вину чи сором, якщо взагалі щось робиш.

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: А якщо це у твоїй природі шкодити іншим? Що, якщо ми не можемо бути нічим *іншим*, як тягарем для близьких?

`bb({body:"scream_a_1"})`

b: АГХ ТИ ЗЛАМАНА! ТАКА, ТАКА, ТАКА ЗЛАМА--

`_.a2_attack_3 = "bad";`

(#act2d)

# act2c_punch

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Я не ірраціональний. Люди *роблять* наркотичні пунші. Це реальна річ, яка насправді відбувається.

`bb({eyes:"suspect"})`

b: Людино, у тебе болить голова? Твої кінцівки ослаблені? Я думаю ти помираєш.

`bb({body:"scream_a_1"})`

b: АГГХ, ТИ ПОМИРАЄШ! ТИ ПОМИРАЄШ, ТИ ПОМИРАЄШ, ТИ ПОМИ--

`_.a2_attack_3 = "harm";`

`_.a2_hoodie_callback = "punch bowls";`

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

h: Б^ЛЯЯТЬ^!

h: БЛ^ЯДСЬ^КЕ Б^ЛЯ^ТЬ Б^ЛЯДУН^СТВО *Б^ЛЯЯЯЯЯ^ТЬ*

`bb({body:"two_up", mouth:"smile", eyes:"happy"});`

b: Ура, людино! Я такий радий, що ти можеш чути мене!

`bb({body:"normal", mouth:"small", eyes:"sad"})`

b: Чому ти мене ігнорувала?

`hong({body:"facepalm"})`

h: Божечки, який ти йолоп.

`hong({body:"facepalm_2"})`

h: Ти знаєш цю притчу місцевих американців?

h: "Всередині нас живе два вовка, один з них - надія, інший - відчай, хто виграє? Той, якого ти кормиш."

```
hong({body:"facepalm_3"});
bb({eyes:"normal"});
```

h: Я надіялась ти *зголоднієш*, ти садист-^гівнюк^!

`hong({body:"smile", mouth:"smile"})`

h: Да пішло воно, я краще повторю позитивні афірмації.

h: *Мене люблять. Я хороша. Я розумна. Я красива. Я неповторна.*

`bb({eyes:"suspect"});`

[Божечки, це так нарцисично!](#act2d_narcissist)

[Ти знаєш, що афірмації не допомагають?*](#act2d_disproven)

[омг, не приписуй рандомні притчі до місцевих](#act2d_racist)

# act2d_disproven

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: Фактично, вони мають *зворотній ефект* для людей з ниизькою самооцінкою! 

`bb({body:"one_up", mouth:"small", eyes:"normal"})`

b: Це було добре продумане дослідження –  контрольоване дослідження, експериментатор не знав, хто в якій групі.

`bb({body:"two_up", mouth:"small", eyes:"normal_r"})`

b: Результат: якщо у вас вже була низька самооцінка, при повторі афірмацій, ви почуваєтеся *гірше*, ніж якби ви взагалі нічого не говорили!

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: Вуд 2009, психологія. Подивись у гуглі, людино,

`bb({body:"scream_b_1"})`

b: А ТОДІ ПРИПИНИ ПОШИРЮВАТИ НЕНАУКОВІ ФЕЙКИ

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2d_narcissist

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Тобі *потрібно* бачити свої недоліки, щоб рости як особистість!

`bb({body:"two_up", eyes:"suspect"})`

b: Не можна розпилювати освіжувач у запліснявілій кімнаті! Приховування недоліків потім зробить тебе гіршою.

`bb({body:"chest", mouth:"smile", eyes:"closed"})`

b: На щастя, я твій вірний вовк-захисник, можу вказати тобі на них. І прямо зараз, це-

`bb({body:"scream_b_1"})`

b: ВСЕ. ВСЕ НЕ ТАК

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2d_racist

`bb({body:"normal", mouth:"normal", eyes:"suspect"})`

b: Корінні американці - *люди*, не "шляхетні дикуни". Ти не можеш кидатись назвами, щоб твоє печиво-удачі було *екзотичніше*.

`bb({eyes:"suspect_r"})`

b: Ти змішуєш особистостей та складні культури у одну мішанину! Це - "доброзичливий расизм"!

`bb({body:"scream_b_1"})`

b: ПРИПИНИ БУТИ РАСИСТКОЮ ЖИРНООКА ТРЯПКА

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2e

h: ^ЇБАТЬ^.

`hong({body:"yell", mouth:"yell"})`

h: Знаєш що? Ти *ірраціональний*.

h: Всі знають - емоції ірраціональні! Особливо страх!

`hong({body:"facepalm_2"})`

h: Ти - еволюційний непотріб, як мій апендицит чи зуб мудрості!

`hong({body:"yell", mouth:"yell"})`

h: ^Сука^, вся ця вовча метафора дурна! Ти просто купка нейро-хімічних зв'язків у моїй голові.

`hong({body:"cross", mouth:"cross"})`

h: Чому я маю прислуховуватись до ірраціонального, не існуйочого шматку непотребу як ти?!

`bb({eyes:"sad", MOUTH_LOCK:true})`

b: ...

[Мда, людино. Це боляче.](#act2e_hurtful)

[Я - почуття. Почуття важливі.](#act2e_valid)

[Людино, ми *двоє* просто хімікати.](#act2e_rational)

# act2e_hurtful

`bb({body:"chest"})`

b: Я *частина* тебе. Коли ти таке говориш, ти раниш *себе*.

`bb({body:"scream_a_1"})`

b: Чому ти б'єш себе, людино? ПРИПИНИ БИТИ СЕБЕ.

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

b: Твій найбільший мотиватор - дофамін, твоя щира радість - серотонін.

`bb({body:"one_up"});`

b: Твої спогади — це синаптичні ваги, твої причини — несправні електричні сигнали.

`bb({eyes:"normal", body:"normal"});`

b: Тому, те що я "хімічний зв'язок" означає *мою* ірраціональність... тоді *ти* ірраціональна!

`bb({body:"two_up", eyes:"shock"});`

b: І якщо ми *обоє* ірраціональні, тоді ми *ніколи* не зрозумієм як бути задоволеними і щасливими!

`bb({body:"scream_a_1"})`

b: АГГХ, МИ ПОЛОМАНІ! МИ ТАКІ, ТАКІ, ТАКІ ПОЛОМАНІ--

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

b: Стривай... "вони" говорять, що почуття важливі, ти завжди маєш приймати їх.

`bb({eyes:"suspect_r"});`

b: Але "вони" також говорять, що емоції ірраціональні, та їм не можна довіряти.

`bb({eyes:"angry"});`

b: Божечки, "вони" брехали нам увесь цей час!

`bb({body:"scream_a_1"})`

b: "ВОНИ" НАБИВАЛИ НАС СУПЕРЕЧНОСТЯМИ, ЩОБ МИ БУЛИ ЗАЛЕЖНІ ВІД ІНДУСТРІЇ САМОДОПОМОГИ

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

h: Я ненавиджу це. Боже, так сильно *ненавиджу*.

h: Я не можу заспокоїти тебе. Я не можу ігнорувати. Я не можу подолати.

`bb({eyes:"suspect"});`

h: Що б я не робила, я не можу позбутися теб--

`bb({body:"cry_1"});`

b: Ну, мабуть, ти НЕ *ПОВИННА* ПОЗБУВАТИСЬ МЕНЕ.

`bb({body:"cry_2"});`

b: Як ти думаєш, що я відчуваю, людино?!

`bb({body:"cry_4", mouth:"cry", eyes:"cry"})`

b: Я з усіх сил намагаюся бути твоїм охоронцем, але ти дивишся на мене як на Злого Вовка!

b: Тому я *намагаюся* попередити про небезпеку! *Більше* небезпеки! *Іншої* небезпеки!

`bb({eyes:"cry_2"})`

b: Але як би я не намагався захистити тебе, ти *досі* думаєш, що я твій ворог!

`bb({body:"cry_5"});`

b: Що я роблю не так?!

`bb({body:"cry_2"});`

b: Я *знаю*, я поганий у цьому. Але я *намагаюсь*, людино!

`bb({body:"cry_3"});`

b: ...Я намагаюсь.

`bb({body:"cry_6", mouth:"right", eyes:"cry_r_1"});`

b: Тобі не потрібно прислуховуватись до мене, або погоджуватись, або навіть *любити* мене.

`bb({eyes:"cry_r_2"});`

b: Я просто... все, чого я хочу, це щоб ти була зі мною.

`bb({eyes:"cry_r_3"});`

b: Я просто хочу, щоб ти посиділа зі мною деякий час, а не відверталась і--

```
bb({eyes:"cry_r_4"});
hong({body:"listen"});
```

r: Гей.

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

r: Виглядаєш ніби ти б'єшся із собою, дитино.

```
publish("act2",["party_hunter",3]);
publish("act2",["party_hong",13]);
```

h2: Це так очевидно?

```
publish("act2",["party_hunter",4]);
publish("act2",["party_hong",14]);
```

r: Ти бурмотіла у свою товстовку про {{_.a2_hoodie_callback}} типу того.

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

h2: о боже, я безнадійна

```
publish("act2",["party_hunter",7]);
publish("act2",["party_hong",18]);
sfx("squeak");
```

r: Гей. Ти не одна, подруго. Тривога дуже поширена.

```
publish("act2",["party_hunter",5]);
publish("act2",["party_hong",19]);
```

{{if _.act1_ending=="fight"}}
r: Чорт, тільки вчора я почув, що хтось у кампусі мав нервовий зрив і розбив свій телефон!
{{/if}}

{{if _.act1_ending=="flight"}}
r: Чорт, тільки вчора я почув, як хтось згорнувся в клубок як броненосець і заплакав на публіці!
{{/if}}

```
publish("act2",["party_hunter",2]);
```

r: Слухай: я знаю, як це мати таку тваринку у своїй голові.

```
publish("act2",["party_hunter",8]);
```

r: Ми *всі* знаєм. Тому я влаштовую ці вечірки кожні вихідні, щоб забути турботи, забути ту тваринку.

```
publish("act2",["party_hunter",9]);
publish("act2",["party_hong",20]);
```

h2: але моя тривога...

```
publish("act2",["party_hunter",2]);
publish("act2",["party_hong",21]);
```

r: Не хвилюйся, дитино. Раніше я був таким, як ти. Але я знайшов хитрість, щоб змусити цей голос замовкнути...

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

r: Моя власна суміш. Це сильніше за...ну, все легальне.

```
publish("act2",["party_hunter",12]);
publish("act2",["party_hong",24]);
```

r: До дна, ^су-у-чко^!

```
hong({body:"hold"});
bb({body:"normal", mouth:"small", eyes:"wat"});
Game.clearText();
Game.WORDS_HEIGHT_BOTTOM = -1;
publish("act2-out-3");
publish("hp_show");
```

(...3500)

[О.Мій.Бог.](#act2g_1) `Game.OVERRIDE_CHOICE_LINE=true`

[Це поганий механізм коплення.](#act2g_2) `Game.OVERRIDE_CHOICE_LINE=true`

[Не бери напоїв від незнайомців.](#act2g_3) `Game.OVERRIDE_CHOICE_LINE=true`

# act2g_1

b: O--

(#act2g)

# act2g_2

b: Ц--

(#act2g)

# act2g_3

b: Н--

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

h: Ммм, яка вишукана палітра!

h: Насичений аромат "затикання свого розуму" з тонким присмаком "ніколи нічого більше не відчування"!

b: Це погано, людино. Це дуже, дуже погано.

[*Саме так* починається залежність.](#act2h_opt1) `Game.OVERRIDE_CHOICE_LINE=true`

[Я *знав*, що власник був ^прийобаний^!](#act2h_opt3) `Game.OVERRIDE_CHOICE_LINE=true`

[А ще, вони могли всунути наркотики!](#act2h_opt2) `Game.OVERRIDE_CHOICE_LINE=true`


# act2h_opt1

b: *Сам та*--

(#act2h)

# act2h_opt2

b: А ще, вони мо--

(#act2h)

# act2h_opt3

b: Я *знав*, щ--

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

h: Смачно, *і* дешевше за терапію!

b: ЛЮДИНО, ЗУПИНИСЬ

h: Хе-хе-хе!

h: І що *ти* збираєшся робити з цим, ^лошок^?

b: Мені так шкода, людино.

b: Мені доведеться використати СПЕЦІАЛЬНУ АТАКУ

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

h: Що за ^лайно^?

h: Ти будеш напихати мені більше дурних *слів*--

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

h: ЩО ЦЕ ^ДО ЧОРТА^ БУЛО

b: Вибач. Мені потрібно було показати наслідки.

{{if _.SPECIAL_ATTACK=="harm"}}
h: Я МОГЛА *БАЧИТИ* СВІЙ ТРУП. Я МОГЛА *ВІДЧУВАТИ* ЩО ТАКЕ БУТИ МЕРТВОЮ.
{{/if}}

{{if _.SPECIAL_ATTACK=="alone"}}
h: Я МОГЛА *БАЧИТИ* ПОГЛЯД ОГИДИ КОЖНОГО. Я МОГЛА *ЧУТИ* ВСЕ, ЩО ВОНИ СКАЗАЛИ.
{{/if}}

{{if _.SPECIAL_ATTACK=="bad"}}
h: Я МОГЛА *ЧУТИ* ХРУСКІТ РЕБЕР. Я МОГЛА *ВІДЧУВАТИ* КРОВ У ПОВІТРІ.
{{/if}}

b: Вибач, людино.

n: *ПРИПИНИ*

[{БИТИСЬ: вдарити власника.}](#act2j_fight) `Game.OVERRIDE_CHOICE_LINE=true`

[{ВІДЛЕТІТИ: піти з вечірки.}](#act2j_flight) `Game.OVERRIDE_CHOICE_LINE=true`

# act2j_fight

`bb({ eyes:"angry" });`

b: Цей психопат скористався тобою.

b: Вони намагалися розвести тебе, зробити такою самою, як і вони!

`bb({ body:"yell_angry_1" });`

b: Вдарь цього ^придурка^! Вибийте його чортові ноги!

`bb({ body:"final_1" });`

b: БИЙ, БИЙ, БИЙ, БИЙ, БИЙ, БИЙ, БИЙ, БИЙ, БИЙ, БИЙ, БИЙ, БИЙ, БИЙ, БИЙ, БИЙ, БИЙ, БИЙ, БИ--

`_.a2_ending = "fight";`

(#act2k)

# act2j_flight

b: Я *знав*, що всі ці вечірки були ^хуйовими^. Усі вони притупляють свій біль жахливими речами!

`bb({ body:"yell_1" });`

b: І вони примушують тебе робити те саме! Вони знищують тебе! Нам треба йти звідси!

`bb({ body:"final_1" });`

b: БІЖИ, БІЖИ, БІЖИ, БІЖИ, БІЖИ, БІЖИ, БІЖИ, БІЖИ, БІЖИ, БІЖИ, БІЖИ, БІЖИ, БІ--

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

r: Все нормально?

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

r: Т-ти...

```
publish("act2",["party_hunter",23]);
publish("act2",["party_hong",35]);
publish("act2",["dee",5]);
publish("act2",["dum",5]);
music('party1', {volume:0.6, fade:6});
```

r: *фетешистка*.

r: Мені таке подобається. Приходи наступний раз, красуню.

```
publish("act2",["party_hunter",19]);
publish("act2",["party_hong",36]);
```

h2: окей, бувай, ciao, adios, au revoir

r: Звір, можливо, сьогодні й переміг, але повертайся, я тобі змішаю щось ще міцніше!

h2: sayōnara, auf wiedersehen, zài jiàn, shalom

r: Ми з тобою, покажемо звірові, хто головний!

(#act2k_end)

# act2k_flight

`publish("act2",["party_hong",36]);`

h2: ок, вибач, мені потрібно бігти

`publish("act2",["party_hunter",16]);`

r: ^Блін^. Тварина сьогодні перемогла, га?

`publish("act2",["party_hunter",15]);`

h2: ні, ні, просто треба пробігти марафон. швидко.

`publish("act2",["party_hunter",19]);`

r: Приходи наступний раз, красуню. Я тобі змішаю щось ще міцніше!

h2: ок, дякую, я біжу...

r: Ми з тобою, покажемо звірові, хто головний!

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

b: Людина! Ти впорядку?!

```
publish("act2", ["act2_end","next"]);
```

b: Боже, це було *близько.* Ми дійсно могли б--

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

h: Я піду на вечірку наступні вихідні.

h: Наступного разу, коли битимося, я збираюся не *перемогти* тебе...

h: Я збираюсь ^бляд^ськи *вбити* тебе.

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
