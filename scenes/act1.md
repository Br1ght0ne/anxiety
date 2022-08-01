# act1

```
SceneSetup.act1();
```

(...300)

n: І ЦЕ ЛЮДСЬКА ТРИВОГА

n: _ТИ_ Є ТРИВОГОЮ

{{if window.localStorage.continueChapter=="replay"}}
(#act1_replay)
{{/if}}

{{if window.localStorage.continueChapter!="replay"}}
(#act1_normal)
{{/if}}



# act1_replay

`hong({mouth:"0_neutral", eyes:"0_neutral"})`

h: Ох, гей! Ми тут знову?

`hong({eyes:"0_neutral"})`

n: ТВОЯ РОБОТА ОБЕРІГАТИ СВОЮ ЛЮДИНУ ВІД *ЗАГРОЗ*

`bb({eyes:"look", mouth:"small_lock"})`

n: ДО РЕЧІ, ПОВТОРНА ГРА НАРАЖАЄ ЇЇ НА *ЗАГРОЗУ* ПРЯМО ЗАРАЗ

n: ШВИДШЕ, ПОПЕРЕДЬ ЇЇ!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Людино! Слухай, ми у небезпеці! Гравець...

[...буде катувати нас знову!](#act1_replay_torture)

[...не знайде іншої кінцівки!](#act1_replay_alternate)

[...отримає лудонаративний дисонанс!](#act1_replay_dissonance)

# act1_replay_torture

```
window.HACK_REPLAY = JSON.parse(localStorage.act4);
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

{{if window.HACK_REPLAY.act1_ending=="fight"}}
b: Він скрутить нас у клубок і ми плакатимемо!
{{/if}}

{{if window.HACK_REPLAY.act1_ending=="flight"}}
b: Він змусить нас розбити телефон, щоб у тебе була панічна атака!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="fight"}}
b: Він змусить нас *НЕ* бити власника вечірки!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="flight"}}
b: Він змусить нас ударити симпатичного анти-злодія власника вечірки!
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="jump"}}
h: Ну, можливо ми не зістрибнемо з даху цьго ра--

{{if window.HACK_REPLAY.a3_ending=="walkaway"}}
b: ВІН ЗАСТАВИТЬ НАС ЗІСТРИБНУТИ.
{{/if}}

`bb({body:"fear"});`

b: ВІН ЗРОБИТЬ ІЗ НАМИ ВСІ ЦІ ЖАХЛИВІ РЕЧІ, А ТОДІ МИ--

(#act1_replay_end)


#act1_replay_alternate

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Звісно, історія *взагальному* така ж, але в кожного розділу є два закінчення, плюс всі варіанти діало--

`bb({body:"fear"});`

b: Гравець буде розчарованим, закривай цю вкладку, видаляй програму, і тоді ми--

(#act1_replay_end)


# act1_replay_dissonance

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Непристойне що тепер?

`bb({eyes:"normal"});`

b: Ця арка історії була про те, що ти можеш *ВИБИРАТИ*, щоб побудувати здорові відносини зі своїм страхом,

`bb({eyes:"normal_right"});`

b: Але повторна гра приведе до минулого закінчення, ваші нові *ВИБОРИ* не враховуються,

`bb({eyes:"narrow_eyebrow"});`

b: Таким чином, можна побачити протиріччя між посилом та механікою гри,

`bb({eyes:"fear"});`

b: Таким чином розгадуючи суть цього закрученого світу,

`bb({body:"fear"});`

b: І тоді ти--

(#act1_replay_end)


# act1_replay_end

`bb({body:"panic"})`

b: ВМРЕЕЕЕЕШШШ

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

h: Окей, повернімось до розділу.

```
Game.clearText();
```

n4: (ДАЙ _СВОЇЙ_ ТРИВОЗІ БЛА БЛА НАЙБІЛЬШ СХОЖЕ ДО _ТВОГО_ СТРАХУ БЛА БЛА ТИ ЗНАЄШ ПРАВИЛА)

```
sfx("squeak");
hong({body:"0_squeeze"});
bb({body:"squeeze"});
```

(#act1_normal_choice)



# act1_normal

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: Ох, чудово, мій вовк повернувся. Фаааантастично.

`hong({eyes:"0_neutral"})`

n: ТВОЯ РОБОТА ОБЕРІГАТИ СВОЮ ЛЮДИНУ ВІД *ЗАГРОЗИ*

`bb({eyes:"look", mouth:"small_lock"})`

n: ДО РЕЧІ, ЦЕЙ БУТЕРБРОД Є *НЕБЕЗПЕКОЮ* НАВІТЬ ЗАРАЗ

n: ШВИДШЕ, ПОПЕРЕДЬ ЇЇ!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Людино! Слухай, ти у небезпеці! І це...

`bb({body:"squeeze"})`

n4: (ДАЙ _СВОЇЙ_ ТРИВОЗІ ВИЙТИ ГРАТИ! ВИБЕРИ НАЙБІЛЬШ СХОЖЕ ДО _СВОГО_ СТРАХУ)

(#act1_normal_choice)

# act1_normal_choice

[Ти знов обідаєш одна! Знову!](#act1a_alone) `bb({body:"squeeze_talk"})`

[Ти не продуктивна поки їси!](#act1a_productive) `bb({body:"squeeze_talk"})`

[Цей білий хліб шкідливий для тебе!](#act1a_bread) `bb({body:"squeeze_talk"})`

# act1a_alone

```
bb({body:"normal", mouth:"small", eyes:"narrow"});
hong({body:"0_sammich"});
```

b: Ти знаєш, що самотність асоціюється з предчасною смертю , так само як викурені 15 сигарет за день?-

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: (Holt-Lunstad 2010, PLoS Medicine)

`hong({eyes:"0_annoyed"})`

h: Ем, дякую за інформацію але--

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: Що означає, якщо ти не будеш тусуватись з кимось *прямо зараз* ти-

`bb({body:"panic"})`

b: ВМРЕЕЕЕЕШШШ

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "alone");
publish("hp_show");
```

(...2500)

`_.fifteencigs = true`

n: ТИ ВИКОРИСТАВ *СТРАХ БУТИ САМОТНЬОЮ*

(#act1b)

# act1a_productive

```
bb({body:"normal", mouth:"small", eyes:"normal"});
hong({body:"0_sammich"});
```

b: Відкрий свій ноутбук і почни щось робити зараз!

`hong({eyes:"0_annoyed"})`

h: Ем, краще щоб крихти не попадали на мою клав--

```
bb({mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Якщо ти нічого не принесеш для цього соціо-тіла, це означає що ти - соціо-паразит!

b: Соціо-тіло піде до соціо-лікаря за ліками, щоб витравити соціо-паразита, а тоді ти--

```
bb({body:"panic", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: ВМРЕЕЕЕЕШШШ

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "bad");
publish("hp_show");
```

(...2500)

`_.parasite = true`

n: ТИ ВИКОРИСТАВ *СТРАХ БУТИ ЖАХЛИВОЮ*

(#act1b)

# act1a_bread

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich", eyes:"0_annoyed"});
```

h: Чи були ці досліди відтво--

```
bb({body:"fear", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Зрозумій, борошно наповнить нашу кров цукром, лікарі ампутують наші кінцівки, і тоді ти-

`bb({body:"panic"})`

b: ВМРЕЕЕЕЕШШШ

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "harm");
publish("hp_show");
```

(...2500)

`_.whitebread = true`

n: ТИ ВИКОРИСТАВ *СТРАХ БУТИ ПОРАНЕНОЮ*

(#act1b)

# act1b

n: ЦЕ НАДЗВИЧАЙНО ЕФЕКТИВНО

`bb({mouth:"smile", eyes:"smile"});`

b: Бачиш, людино? Я твій вірний вовк-захисник!

`bb({body:"pride_talk"});`

b: Довірся своїм відчуттям! Вони завжди праві!

`bb({body:"pride"});`

n: ОПУСТИ ШКАЛУ ЕНЕРГІЇ ЛЮДИНИ ДО НУЛЯ

n: ЩОБ ОБЕРІГАТИ ЇЇ ФІЗИЧНІ + СОЦІАЛЬНІ + МОРАЛЬНІ ПОТРЕБИ, ТИ МОЖЕШ ВИКОРИСТАТИ:

n: СТРАХ *БУТИ ПОРЕНЕНОЮ* #harm#

n: СТРАХ *БУТИ САМОТНЬОЮ* #alone#

n: І СТРАХ *БУТИ ЖАХЛИВОЮ* #bad#

`Game.OVERRIDE_TEXT_SPEED = 1.25;`

n4: (ПІДКАЗКА: ВИБИРАЙ САМЕ ТЕ, ЩО БЛИЗЬКЕ ДО ТЕБЕ, НАЙТЕМНІШІ СТРАХИ!~)

h: ...

```
hong({body:"putaway"});
sfx("rustle");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

(...1000)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h: знаєш що, час чекнути мій мобільний.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: ОБЕРІГАЙ СВОЮ ЛЮДИНУ

n: ВІД СВІТУ. ВІД ІНШИХ ЛЮДЕЙ. ВІД НИХ.

n: ЩАСТИ

(...500)

`Game.clearText()`

(...500)

(#act1c)

# act1c

`music('battle', {volume:0.5})`

n: РАУНД ПЕРШИЙ: *БОРИСЬ!*

`bb({body:"normal", mouth:"normal", eyes:"normal"});`

h: Хах. У Фейсбуці кажуть, що цими вихідними буде вечірка.

`bb({eyes:"uncertain"});`

b: То ті диваки, що влаштовують вечірки *кожні* вихідні дні?

`bb({eyes:"uncertain_right"});`

b: Яку внутрішню пустоту вони намагаються заповнити? Напевно, вони жахливі всередині!

`hong({eyes:"surprise"});`

h: І ще, мене запросили?

`bb({eyes:"fear", mouth:"normal"});`

b: Тоді гаразд!

[Скажи так, інакше ми вмрем від самотності!](#act1c_loner)

[Відмовся, там буде повно отруйних наркотиків!](#act1c_drugs)

[Проігноруй, ми лише там всіх засмутим.](#act1c_sad)

# act1c_loner

{{if _.fifteencigs}}
b: П'ятнадцять сигарет на день, людино! П'ятнадцять!
{{/if}}

{{if !_.fifteencigs}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if !_.fifteencigs}}
b: Ніхто не прийде на твій похорон, вони просто розвіють твій прах в океан, тебе з'їдять кити,
{{/if}}

{{if !_.fifteencigs}}
b: і ти станеш ^ГІМНОМ^ КИТА!
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
b: А тому, ми повинні піти на вечірку!
{{/if}}

{{if _.parasite}}
b: Просто візьми ноутбук, щоб ми працювали, і не були соціо-паразитом.
{{/if}}

{{if _.whitebread}}
b: Доки, поки вони не будуть подавати БІЛИЙ ХЛІБ
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: БОЖЕ. Якщо ти заткнешся, тоді гаразд.

h: Я погоджусь.

{{if _.whalepoop}}
b: ^Гімно^ кита, людино! ^Гімно^ кита!
{{/if}}

`_.partyinvite="yes"`

(#act1d)

# act1c_drugs

`bb({mouth:"small", eyes:"fear"});`

{{if _.whitebread}}
b: або навіть гірше... БІЛИЙ ХЛІБ
{{/if}}

{{if _.whitebread}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if _.whitebread}}
b: У нас буде передоз від метамфетаміну і білого хліба, а тоді вони не зможуть помістити наш жирний труп у крематорій!
{{/if}}

{{if !_.whitebread}}
b: Ти отримаєш передоз від неймовірної кількості наркоти, що всі будуть дивуватись, як ти *вже* забальзамувалася!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.parasite}}
b: Ти не можеш веселитись, тобі потрібно працювати, щоб не бути соціо-паразитом!
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: БОЖЕ. Якщо ти заткнешся, гаразд.

h: Я відмовлюсь.

`_.partyinvite="no"`

(#act1d)

# act1c_sad

`bb({eyes:"uncertain_right", mouth:"normal"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.fifteencigs}}
b: Все що ми робим - плачем у кутку від того, що самотність така ж небезпечна як 15 сигарет.
{{/if}}

{{if _.parasite}}
b: На вечірці ти лише хвилюєшся за свою продуктивність.
{{/if}}

{{if _.whitebread}}
b: Ти постійно хвилюєшся про шкідливу їжу, яка може вбити тебе.
{{/if}}

```
bb({mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"lookaway"});
```

h: бож, дивуюсь чому.

`hong({eyes:"neutral"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: Якщо ми прийдемо - їм буде сумно через нас, але якщо ми відмовимся вони також засмутяться!

`bb({body:"fear", eyes:"fear"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: ТИ ПРИНОСИШ ЛИШЕ ШКОДУ ЛЮДЯМ, ТОМУ ТОБІ МАЄ БУТИ ПОГАНО

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`hong({mouth:"anger", eyes:"anger"});`

h: Ех. Якщо ти заткнешся, гаразд.

h: Я проігнорую запрошення.

`_.partyinvite="ignore"`

(#act1d)

# act1d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"annoyed"});
```

h: Все одно. Досить з мене Фейсбуку. Мені потрібне щось спокійніше, менш тривожне.

`hong({eyes:"neutral"});`

h: Що нового у Твіттері?

`bb({eyes:"look"});`

[Оу ні, подивись на цю жахливу новину!](#act1d_news)

[Оу ні, невже цей твіт насправді про *нас?*](#act1d_subtweet)

[Гей, гіфка кота, що п'є молоко.](#act1d_milk)


# act1d_news

```
bb({eyes:"pained1"});
music(null, {fade:2});
```

b: Боже, таке відчуття, ніби цей світ руйнується, правда?

```
bb({eyes:"pained2"});
hong({mouth:"sad", eyes:"sad"});
```

b: Начебто, все закінчується, вмирає, і ми приречені та не можемо якось запобігти цьому.

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
bb({mouth:"shut"});
```

b: ...

`bb({mouth:"smile", eyes:"smile"});`

b: Давай зробимо ретвіт цієї історії!

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

h: Окей, добре, добре, просто сиди тихіше!

`hong({mouth:"neutral", eyes:"annoyed"});`

h: Ну і чорт з ним, я у Снепчат.

(#act1e)


# act1d_subtweet

`bb({eyes:"fear"});`

b: Це сабтвіт! Підлий, підлий сабтвіт!

`hong({eyes:"annoyed"});`

h: Ні, це не так?

`bb({eyes:"narrow", mouth:"small"});`

b: але якщо вони обговорюють тебе поза спиною?

h: Вони н--

`bb({body:"fear", eyes:"fear", mouth:"normal"});`

b: НАВПРОТИ НАШОЇ СПИНИ

`hong({eyes:"sad", mouth:"sad"});`

h: Я --

`bb({eyes:"narrow", mouth:"small"});`

b: але *якщо*

h: З--

`bb({eyes:"narrow_eyebrow"});`

b: *якщо*

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

h: о-КЕЙ, загляну в Снепчат.

(#act1e)

# act1d_milk

`hong({mouth:"smile", eyes:"neutral"});`

h: Хех, красунчик, хочу це ретвітнути, я ду--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: КОТИ НЕ ПЕРЕТРАВЛЮЮТЬ МОЛОКО, ЯКА ТИ ЖАХЛИВА, ЗА ТЕ ЩО НАСОЛОДЖУЄШСЯ НАСИЛЬСТВОМ

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

h: о-КЕЙ, загляну в Снепчат.

(#act1e)

# act1e

`hong({mouth:"neutral", eyes:"neutral"});`

h: Хех, вчорашнє фото. Тоді *саме так* виглядають всі ці вечірки.

{{if _.partyinvite=="yes"}} (#act1e_said_yes) {{/if}}

{{if _.partyinvite=="no"}} (#act1e_said_no) {{/if}}

{{if _.partyinvite=="ignore"}} (#act1e_said_ignore) {{/if}}

# act1e_said_yes

`hong({mouth:"sad", eyes:"annoyed"});`

h: У-ух, виглядає затісно для моєї тривоги.

h: Можливо, мені потрібно було відмовити?

```
hong({mouth:"neutral", eyes:"neutral"});
bb({mouth:"normal", eyes:"normal"});
```

[Змінити відповідь? Як ^придурок^?!](#act1e_yes_dontchange)

[Зміни відповідь! Там затісно!](#act1e_yes_changetono)

{{if _.subtweet}}
[Та-ак, вони точно нас обговорють.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Зачекай, ти ретвітнула це та нічого не перевірила.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Ти знаєш, що у тебе жахлива постава?](#act1e_ignore_posture)
{{/if}}

# act1e_yes_dontchange

```
bb({eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Вони розраховували на те що ти прийдеш, і тепер ти їх зраджуєш? Ти хочеш вмерти одна?!

{{if _.fifteencigs}}
b: П'ЯТНАДЦЯТЬ. СИГАРЕТ.
{{/if}}

{{if _.whalepoop}}
b: ^ГІМНО^. КИТА.
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

h: Заткнись, заткнись. Я йду і крапка!

(#act1f)

# act1e_yes_changetono

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Ти знаєш наскільки небезпечні тисняви?

```
bb({body:"fear", mouth:"small", eyes:"narrow"});
hong({eyes:"sad", mouth:"sad"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 2003-го року в нічному клубі Род-Айленду була пожежа. Люди запанікували, і тиснява зі 100 людей згоріла в вогні-

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({mouth:"shock"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: ТИ ХОЧЕШ ЩОБ ЦЕ СТАЛОСЬ З ТОБОЮ-

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 2.5;
```

b: СКАЖИ НІ, СКАЖИ НІ, СКАЖИ НІ, СКАЖИ НІ, СКАЖИ Н-


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

h: Заткнись, заткнись, я відмовлюсь! Боже!

(#act1f)

# act1e_said_no

`hong({mouth:"sad", eyes:"sad"});`

h: Гм... це виглядає весело.

h: Мабуть, я краще б погодилась?

`bb({mouth:"normal", eyes:"normal"});`

[Змінити нашу відповідь? Як ^придурок^?!](#act1e_no_dontchange)

[Зміни відповідь! Не помри самотньою!](#act1e_no_changetoyes)

{{if _.subtweet}}
[Та-ак, вони твітять саме про нас.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Зачекай, ти ретвітнула це та нічого не перевірила..](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Ти знаєш, у тебe жахлива постава?](#act1e_ignore_posture)
{{/if}}

# act1e_no_dontchange

`bb({eyes:"anger"})`

b: Всі розразовували на тебе..!

b: ...залишити їх в спокої, щоб у них була прекрасна вечірка без жахливих, нестерпних {{if _.whitebread}}біло-хлібно-жувальних{{/if}} страшил як ти--


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

h: Заткнись, заткнись. Я не погоджусь!

(#act1f)

# act1e_no_changetoyes

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Хронічна самотність збільшує рівень кортизолу з ризиком серцево-судинних захворювань та інсульту!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.fifteencigs}}
b: П'ЯТНАДЦЯТЬ. СИГАРЕТ.
{{/if}}

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Заткнись, заткнись, я погоджусь! Боже!

(#act1f)

# act1e_ignore_subtweet

```
bb({eyes:"fear", mouth:"small"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Всі твої проблемні твіти виплили на чисту воду!

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.7;
```

b: Нас закенселять, викрадуть, прив'яжуть мотузкою до коня, і відправлять на вершину інформаційної гори! 

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

h: Чому ти така?!

(#act1f)

# act1e_ignore_factcheck

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Ти поширюєш фейки! Ти руйнуєш довіру до вільної преси!

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Ти станеш причиною повернення фашизму з уламків демократії!

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

h: Чому ти така?!

(#act1f)

# act1e_ignore_posture

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Ти хочеш скривлений хребет?! Припини горбитись над екраном!

```
bb({body:"meta"});
```

b: Ти теж.

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

h: Чому ти така?!

(#act1f)

# act1e_said_ignore

`hong({mouth:"sad", eyes:"sad"});`

h: Гм... виглядає весело.

h: Мабуть, я не мала б ігнорувати запрошення?

`bb({mouth:"normal", eyes:"normal"});`

[Продовжуй ігнорувати, ти тусуєшся як ^гімно^.](#act1e_ignore_continue)

[Дійсно, скажи так.](#act1e_ignore_changetoyes)

[Дійсно, скажи ні.](#act1e_ignore_changetono)

# act1e_ignore_continue

`hong({eyes:"annoyed"});`

h: Це дещо грубо, так ігнорити людину, чи не так?

`bb({eyes:"normal_right"});`

b: Ну, інші люди завжди ігнорять *мене*, тому

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

b: нехай це буде нічия.

(#act1f)

# act1e_ignore_changetoyes

`hong({eyes:"surprise", mouth:"smile"});`

h: Ти... дозволяєш мені веселитись?

b: Ну, я маю на увазі, що самотність *може* вбити тебе.

`hong({eyes:"neutral", mouth:"neutral"});`

(#act1e_no_changetoyes)

# act1e_ignore_changetono

`bb({eyes:"narrow"});`

b: Тут надто тісно. Натовп небезпечний.

(#act1e_yes_changetono)


# act1f

```
hong({mouth:"neutral", eyes:"neutral"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: Гаразд. М, нове повідомлення з Тіндеру.

`bb({eyes:"uncertain"})`

b: Що, цей жахливий додаток?

`hong({eyes:"annoyed"})`

h: Він не жахливий, тут просто можна зустріти нових лю--

`bb({eyes:"narrow"})`

b: Це - мерзотний додаток.

```
hong({eyes:"surprise", mouth:"smile"});
bb({eyes:"normal"});
```

h: О, у мене збіг! Він виглядає милим!

```
bb({eyes:"narrow_eyebrow"});
hong({eyes:"sad", mouth:"anger"})
```

h: Будь ласка, не руйнуй для ме--

```
bb({body:"panic"});
Game.OVERRIDE_TEXT_SPEED = 2.0;
```

b: НЕБЕЗПЕКА НЕБЕЗПЕКА НЕБЕЗПЕКА НЕБЕЗПЕКА

`bb({body:"fear", eyes:"fear", mouth:"normal"})`

[Тебе *використовують* інші люди.](#act1f_used_by_others)

[Ти *використовуєш* людей.](#act1f_using_others)

[ЦЕ МОЖЕ БУТИ СЕРІЙНИЙ ВБИВЦЯ](#act1f_killer)

# act1f_used_by_others

`bb({body:"point_crotch", eyes:"normal", mouth:"normal"})`

b: Такі зустрічі можуть заповнити низ дірки,

b: але не заповнити усю дірку...

`bb({body:"point_heart", eyes:"pretty", mouth:"small"})`

b: *тут*.

(...1000)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Ти ПОМРЕШ САМОТНЯ

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.hookuphole=true`

(#act1g)

# act1f_using_others

`bb({eyes:"narrow", mouth:"small"})`

b: Ти думаєш, чужі геніталії це покемони для колекціювання?

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

b: ♫ (тема з покемонів)-

(...5600)

```
bb({mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2400;
```

b: ♫ Я хочу бути, най^збоченкою^-

(...500)

```
bb({eyes:"narrow", mouth:"small"});
Game.FORCE_TEXT_DURATION = 2100;
```

b: ♫ Як ніхто ніколи не був-

(...1500)

```
bb({eyes:"pretty"});
Game.FORCE_TEXT_DURATION = 2300;
```

b: ♫ Стегна й ^срака^, розкішні ^цицьки^-

(...500)

```
bb({eyes:"fear", mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2000;
```

b: ♫ з солоденьким ^членом^ та ^яйцями^!-

(...1000)

```
bb({eyes:"smile", mouth:"smile"});
Game.FORCE_TEXT_DURATION = 1000;
```

b: ♫ ЗБОЧЕН-КА! ПІЙМАЛА-

```
Game.FORCE_CANT_SKIP = false;
Game.clearText();
music(false);
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Річ в тому, що ти - маніпулятор.

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
b: Вони заточать тебе в колодязі, і насильно відкормлять білим хлібом так, що тобі не потрібно буде одягатись, а все буде прикрите жиро-костюмом!
{{/if}}

{{if _.parasite}}
b: Вони запустять бладжон та увімкнуть помодоро таймер, і будуть повторювати "ТАКИЙ ПАРАЗИТ ЯК ТИ, МАЄ БУТИ ПРОДУКТИВНІШИМ"
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Вони розірвуть твої м'язи у конфеті, з жил зроблять розтяжки, і твою кров перероблять у пунш!
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Як ЦЕ може бути запрошенням?!
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

h: мені так набридла ця гра.

(...700)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h:
{{if _.fifteencigs}}"самотність вб'є нас"... {{/if}}
{{if _.parasite}}"ми - соціо-паразит"... {{/if}}
{{if _.whitebread}}"не їж це - воно вб'є нас"... {{/if}}
{{if _.subtweet}}"вони говорять за нашою спиною"... {{/if}}
{{if _.badnews}}"світ горить"... {{/if}}
{{if _.hookuphole}}"ми помремо самотні"... {{/if}}
{{if _.serialkiller}}"він - серійний вбивця"... {{/if}}
{{if _.catmilk}}"коти не перетравлюють молоко"... {{/if}}
{{if _.pokemon}}"^гімняна^ пародія..." {{/if}}

h: я хочу лише спокійного життя.

h: я хочу бути вільною від цього... болю.

`bb({eyes:"look_sad"});`

b: Гей... людино...

`Game.OVERRIDE_TEXT_SPEED = 0.5;`

b: Все буде добре.

(...600)

`bb({body:"point_heart", eyes:"look_sad_smile", mouth:"smile"});`

b: Як твій вірний вовк-захисник, я буду оберігати тебе від небезпеки, старатись, щоб ти була в безпеці.

`bb({body:"normal", eyes:"look_sad", mouth:"smile"});`

b: Я обіцяю.

(...600)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({body:"phone1", eyes:"neutral", mouth:"neutral"});
```

h: Останній додаток. Інстаграм. Що там?

`hong({eyes:"sad"});`

h: Тут... ще більше світлин з вечірки.

`hong({mouth:"sad"});`

h: Усі виглядають щасливими. Вільні від думок. Вільні від тривоги.

`hong({mouth:"anger"});`

h: Боже, чому я не можу бути такою? Просто бути *нормальною?*

`bb({eyes:"normal_right"});`

b: Про вечірку цими вихідними. Ось моє ФІНАЛЬНЕ рішення:

`bb({eyes:"normal"});`

[Ти йдеш.](#act1g_go) `Game.OVERRIDE_CHOICE_LINE=true`

[Ти не маєш йти.](#act1g_dont) `Game.OVERRIDE_CHOICE_LINE=true`

# act1g_go

`_.act1g = "go"`

(#act1h)

# act1g_dont

`_.act1g = "dont"`

(#act1h)

# act1h

b: Ти по--

```
bb({eyes:"wat", mouth:"small"});
hong({body:"2_fuck"});
```

h: *^БЛЯТЬ^.*

`hong({body:"2_you"});`

h: ТИ.

(...500)

b: щ

(...1500)

`bb({eyes:"wat_2"});`

b: що?

`hong({body:"phone1", eyes:"anger", mouth:"anger"});`

h: Я ПІДУ на вечірку,

{{if _.act1g=="go"}}
h: Не тому що ти цього хочеш, а бо це *МОЄ* рішення.
{{/if}}

{{if _.act1g=="dont"}}
h: ТОМУ ЩО ти цього мені не дозволяєш.
{{/if}}

```
hong({body:"putaway"});
sfx("rustle");
```

h: Ти НЕ контролюєш мене.

```
sfx("rustle2");
hong({body:"0_sammich", eyes:"0_annoyed", mouth:"0_neutral"});
```

h: А тепер вибач, я буду їсти це бутерброд в ^їбаній^ тишині.

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

[АГГХ ТИ ПОМРЕШ](#act1h_death) `Game.OVERRIDE_CHOICE_LINE = true;`

[АГГХ ВСІ ТЕБЕ НЕНАВИДЯТЬ](#act1h_loneliness) `Game.OVERRIDE_CHOICE_LINE = true;`

[АГГХ ТИ - ЖАХЛИВА ЛЮДИНА](#act1h_worthless) `Game.OVERRIDE_CHOICE_LINE = true;`

# act1h_death

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: ААГГХ ТИ ПОМРЕШ ААГГХХ

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

b: ААГГХ ВСІ НАС НЕНАВИДЯТЬ ААГГХХ

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

b: ААГГХ ТИ - ЖАХЛИВА ЛЮДИНА ААГГХХ

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

n: ВІТАЮ

(...500)

n: ТИ УСПІШНО ОБЕРІГ ФІЗИЧНІ + СОЦІАЛЬНІ + МОРАЛЬНІ ПОТРЕБИ СВОЄЇ ЛЮДИНИ!

n: ПОДИВИСЬ ЯКІ ВОНИ ПРЕКРАСНІ!

(...500)

n: І КОЛИ ВСЯ ЕНЕРГІЯ НА НУЛІ, ТИ МОЖЕШ КОНТРОЛЮВАТИ ВСІ ЇЇ ДІЇ

`bb({mouth:"smile", eyes:"normal"});`

n: ВИБЕРИ СВІЙ ФІНАЛЬНИЙ ХІД

`bb({mouth:"small_lock", eyes:"fear"});`

n: *ПРИКІНЧИ ЇЇ*

[{БОРОТИСЬ: Розбий свій телефон!}](#act1i_phone) `Game.OVERRIDE_CHOICE_LINE=true`

[{БОРОТИСЬ: Скрутись і плач!}](#act1i_cry) `Game.OVERRIDE_CHOICE_LINE=true`

# act1i_phone

`bb({mouth:"normal", eyes:"narrow"})`

b: Твій телефон викликає у тебе тривогу!

`bb({eyes:"anger"})`

b: Цукерберг знищує твоє психічне здоров'я для отримання капіталістичних грошей!

```
bb({body:"fear", eyes:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Накажи свій телефон! Знищ його! Вбий його!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "fight";
```

b: ВБИЙ ВБИЙ ВБИЙ ВБИЙ ВБИЙ ВБИЙ ВБИЙ ВБИЙ ВБИЙ ВБИЙ ВБИЙ ВБИЙ ВБИЙ ВБИЙ ВБИЙ ВБИЙ ВБИЙ ВБИЙ ВБИЙ ВБИЙ ВБИЙ ВБИЙ ВБИЙ ВБИЙ ВБ--

(#act1j)

# act1i_cry

`bb({eyes:"fear", mouth:"normal"})`

b: Увесь світ наповнений небезпекою!

```
bb({body:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Зроби як броненосець! Скрутись у м'ячик для захисту!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "flight";
```

b: СКРУТИСЬ І ПЛАЧ СКРУТИСЬ І ПЛАЧ СКРУТИСЬ І ПЛАЧ СКРУТИСЬ І ПЛАЧ СКРУТИСЬ І ПЛ-- 

(#act1j)

# act1j

`SceneSetup.act1_outro()`
