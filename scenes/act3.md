# act3

```
SceneSetup.act3();
Game.WORDS_HEIGHT_BOTTOM = 205;
sfx("cheers");
```

r: Будьмо!

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

h2: *Ах* саме те, що потрібно.

```
publish("act3",["roofhunter",2]);
publish("act3",["roofhong",2]);
```

r: Знаєш,...

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",6]);
```

h2: Особливо, саме те що потрібне для моєї лівої та правої мигдалини.

```
publish("act3",["roofhunter",8]);
publish("act3",["roofhong",5]);
```

r: Ти нагадуєш мене молодшого. Коли мене також катував звір у моїй голові.

```
publish("act3",["roofhunter",9]);
publish("act3",["roofhong",2]);
```

r: Я так радий, що можу допомогти тобі вбити звіра так, як я вбив свого.

```
publish("act3",["roofhunter",2]);
```

r: Гей, питаннячко: правда чи ді--

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",7]);
publish("act3-alpha", ["dizzyhong",0]);
```

h2: ДІЯ!

```
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",2]);
```

r: Хаха! Добре.

```
publish("act3",["roofhunter",21]);
publish("act3",["roofhong",4]);
```

r: Ок. Бачиш цей голубий басейн внизу?

```
publish("act3-alpha", ["dizzyhong",0]);
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",9]);
```

h2: Так? Вниз на шість поверхів?

```
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",8]);
```

r: Стрибай.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",10]);
```

h2: ...

```
publish("act3",["roofhong",11]);
```

h2: Чекай, що?

```
publish("act3",["roofhong",10]);
publish("act3",["roofhunter",2]);
```

r: Тваринка заскавулила, чи не так?

```
publish("act3",["roofhunter",23]);
```

r: *О ніііі, це небезпечно, не роби цьоогооо.*

```
publish("act3",["roofhunter",22]);
```

r: Але саме тому нам потрібні гострі відчуття! Відривна вечірка! Carpe diem! Вдихати кокс з дупи проститутки, #YOLO!

```
publish("act3",["roofhunter",10]);
```

r: Покажи звірові, що нас не ^їбе^ його ^сучко^виття! Пригай.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",13]);
```

h2: Ем, але інколи, е... у страху є сенс...

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

r: Вибач, ти повелась на пропаганду МсУважності, що говорить відчувати себе погано *нормально*?

```
publish("act3",["roofhunter",17]);
```

r: Мудаки, що керують цим світом нав'язали *нам* тривогу та депресію,

```
publish("act3",["roofhunter",18]);
```

r: Тоді зроби ТЕД промову про те як "прийняти" свою розйобаність, та "обійняти" цього садистського демона в голові!

```
publish("act3",["roofhunter",6]);
```

r: Дитятко, *ти* занаєш, що такі тваринки ранять людей як ми. Вони *тортують* людей як ми.

```
publish("act3",["roofhunter",19]);
```

r: Вони нам не друзі. Це дике чудовисько, яке мє бути *транквилізоване*,

```
publish("act3",["roofhunter",20]);
```

r: Або *всунути пулю в черепок*.

```
publish("act3",["roofhunter",27]);
```

r: Іншими словами, ти даєш йому виграти. 

```
publish("act3",["roofhunter",31]);
publish("act3",["roofhong",14]);
publish("act3",["dd",2]);
```

h2: Ні. Ти не правий.

```
publish("act3",["roofhunter",13]);
publish("act3",["roofhong",15]);
music('battle_dark', {volume:1.0}, function(){
	music('battle_dark_loop');
});
```

h2: Я не дозволю йому виграти.

```
publish("act3",["roofhunter",25]);
publish("act3-alpha", ["roofhong",0]);
publish("act3-alpha", ["transition",1]);
publish("act3",["dd",6]);
```

r: Блять, так! Я вірю в тебе, штучко! Вбий його! <3

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

b: ні ні ні ні ні ні

n: У ЦЬОГО РОЗДІЛУ Є ДВА ЙМОВІРНИХ ЗАКІНЧЕННЯ. ОДНА *ДУЖЕ ПОГАНА.*

b: НІ НІ НІ НІ НІ НІ НІ НІ НІ НІ НІ НІ НІ НІ

n: ВИБИРАЙ ГОЛОВОЮ. ЗАХИСТИ ЛЮДИНУ

`bb({ eyes:"oh_crap", mouth:"normal_talk", MOUTH_LOCK:true });`

b: AAAAAAAAAAAAAAAAAA

`bb({ mouth:"normal" });`

n: УДАЧІ

```
Game.clearText();
bb({ eyes:"start" });
```

[Людино, ти можеш ПОМЕРТИ тут!](#act3a_harm) `Game.OVERRIDE_CHOICE_LINE=true`

[Це тупо та самодеструктивно!](#act3a_bad) `Game.OVERRIDE_CHOICE_LINE=true`

[Ці хворі не твої реальні друзі!](#act3a_alone) `Game.OVERRIDE_CHOICE_LINE=true`

# act3a_harm

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: Л--

(#act3a_after)

# act3a_alone

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: Ц--

(#act3a_after)

# act3a_bad

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: Ц--

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

h: Знаєш, я майже повірила тобі... якби ти так не робив би зілліони разів у минулому.

h: Ти вовк що скиглить, вовче.

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

h: Ти вже це пробував.

b: людино, будь ласка...

`hong({ eyes:"look_right" });`

h: О, *вибач* Великий Фармацевт не схвалює моє самолікування.

h: Подивися, ^мудак^, у нас *всіх* є спосіб заткнути тебе ^нахуй^.

`hong({ body:"look_up", eyes:"look_up" });`

h: Деякі люди кидаються в роботу.

`hong({ body:"look_down", eyes:"look_down" });`

h: Хтось у секс, наркотики, чи оновлення стрічки у Фейсбуці.

`hong({ body:"normal", eyes:"look_right" });`

h: Інші кидаються на інших людей.

`hong({ eyes:"angry" });`

h: А я кину себе у цей басейн.

[Ти п'яна, і вниз ШІСТЬ ПОВЕРХІВ](#act3_bad_1_harm)

[Чорт, і це подяка, яку я отримую?!](#act3_bad_1_insult) `bb({eyes:"angry"});`

[Ок, добре. Я проєбався.](#act3_good_1) `bb({mouth:"sorry", eyes:"sorry_down"});`

# act3_bad_1_harm

b: Навіть якщо ти приземлишся на воду, різниця густоти поверхні розломає твої ребра, а в голові буде, - *нарешті!*

h: Ех.

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

h: Я бачила як кацап таке робив в Ютубі колись.

(#act3_bad_2)

# act3_bad_1_insult

`hong({ eyes:"look_right" });`

h: Я- Стоп, *дякую?*

`bb({ eyes:"angry" });`

b: Саме для цього я і *існую*! Людям не можна довіряти їх власне життя!

b: Я намагаюсь оберігти твою дурну жопку все твоє життя, і тепер ти збираєшс--

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

h: хех.

`hong({ body:"laugh_2" })``

h: хахахаха

`hong({ body:"laugh_3" })``

h: АХАХАХАХААХ

```
bb({ eyes:"sorry"});
hong({ body:"yell_1", mouth:"yell", eyes:"blank" });
```

h: Оу ВАУ, ца найбільш *їбуче* пониження століття!

`hong({ body:"yell_2" });`

h: Ага, ти - гниюча купа, покрита кров'ю лайна! Ти проєбався!

`hong({ body:"normal", mouth:"angry", eyes:"angry" });`

h: Ще примітки, Капітан Очевидність?

[Але помста - це не вихід!](#act3_good_1_fail_revenge) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Але цього разу я *дійсно* правий!](#act3_good_1_fail_harm) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Я ранив тебе.](#act3_good_2a)


# act3_good_1_fail_revenge

b: Тобі потрібні здорові відносини з своїми емоціями, а не топити їх --

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

b: Тому будь ласка, постав пляшку і давай--

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

b: будь ласка... не...

h: Твоя енергетична шкала жахливо занижена, вовче.

h: На твоєму місці, свої наступні слова я б обирала обережно.

`bb({ eyes:"normal" });`

[Гаразд. З мене досить.](#act3_bad_2_jump) `bb({ mouth:"ignore", eyes:"ignore" });`

[Я був правим увесь час.](#act3_bad_2_right)

[Вибач.](#act3_good_2b) `bb({mouth:"sorry", eyes:"sorry_down"});`


# act3_bad_2_jump

b: Тому, іди та стрибай. Побачиш як я переживаю.

`hong({ eyes:"look_right", mouth:"normal", MOUTH_LOCK:true });`

h: ...

```
hong({ eyes:"less_angry", mouth:"normal" });
bb({ eyes:"ignore_oh_crap" });
```

h: Ок тоді. Погнали.

```
bb({ mouth:"normal", eyes:"oh_crap" });
Game.OVERRIDE_TEXT_SPEED = 2;
```

b: ЩО, СТРИВАЙ, ЦЕ РЕВЕРСИВНА ПСИХОЛОГІЯ, ТИ МАЛА ЗРОБИТИ *ПРОТИЛЕЖНЕ* ТОМУ ЩО Я ГОВОР--

(#act3_bad_3)



# act3_bad_2_right

`bb({ eyes:"angry" });`

b: Ти *вже* у небезпеці. Твої так звані друзі *використовують* тебе. І *ти* використовуєш своїх, так званих, друзів.

`bb({ eyes:"sad" });`

b: Тому будь ласко, людино... чому ти не віриш мені?!

h: Тому що, ти ніколи не віриш у *мене*.

(#act3_bad_3)


# act3_bad_2_terrible

`bb({ eyes:"angry" });`

b: Інші вовки мають людей, які не спішать, щоб терпляче їх тренувати, щоб *вчитися* працювати разом,

b: Замість того, щоб ненавидіти своїх вовків за захист! То чому б ти не міг просто--

`bb({ eyes:"normal" });`

h: Неправильна відповідь.

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

h: *"Єдине, чого варто боятися, це сам страх."*

`hong({ body:"look_up", mouth:"happy", eyes:"blank" });`

h: *"Не хвилюйся, будь щасливою!"*

`hong({ body:"normal", mouth:"normal", eyes:"normal" });`

h: Усі мудрі люди нашого часу погоджуються: негативні емоції *шкідливі!*

`hong({ eyes:"less_angry" });`

h: Егх! Саме тому їх називають *негативними!*

b: людино...будь ласка..

`hong({ eyes:"normal" });`

h: Недавно я говорила: "Я просто хочу бути вільною від цього болю."

h: Моє бажання виконалось. Я не відчуваю болю, страху чи тривоги...

h: Я не відчуваю зовсім.

`_.a3_ending = "jump";`

(#act3_end)



# act3_good_2a

`bb({mouth:"sorry", eyes:"sorry_down"});`

b: Я був настільки одержимий тим, щоб ніщо тобі не зашкодило, що не усвідомлював, *я* створював біль.

```
bb({ eyes:"sorry"});
hong({ body:"yell_2", mouth:"yell", eyes:"blank" });
```

h: НІ.ЄБАТЬ.

`hong({ body:"yell_1" });`

h: ЧОРТ. Тобі потрібно було стільки часу, щоб зрозуміти це?!

`hong({ body:"cry", mouth:"cry", eyes:"blank" });`

h: Ти б запобіг стільком проблемам, ти, велика, пухнаста дурашка. Чому ти не зрозумів цього раніше ?...

`_.apologized_for_hurt = true;`

(#act3_good_2q)



# act3_good_2b

`hong({ body:"normal", mouth:"angry", eyes:"look_right" });`

h: ...ти *вибачаєшся.*

`hong({ eyes:"angry", MOUTH_LOCK:true });`

h: ...

h: Вибачаюсь за *що*?

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

[Вибач, що я не хороший захисник.](#act3_good_3_protector)

[Вибач, що не поважав тебе.](#act3_good_3_respect)

[Вибач.](#act3_good_4)


# act3_good_2q_not_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"angry" }, 0);`

[Вибач, я жахливий!](#act3_bad_2_terrible) `bb({mouth:"normal", eyes:"normal"})`

[Вибач, що не поважав тебе.](#act3_good_3_respect)

[Вибач, що ранив тебе.](#act3_good_3_hurt)



# act3_good_3_protector

`bb({eyes:"sorry_down"});`

b: Це мій обов'язок попереджувати про *небезпеку*, але я продовжував гарчати на машини та поштарів.

`bb({eyes:"sorry_up"});`

b: Гарчав на тіні. Так багато.

`bb({eyes:"sorry"});`

b: Має сенс, те що ти хочеш заткнути мені морду.

`bb({eyes:"sorry_down"});`

b: Вибач.

(#act3_good_4)



# act3_good_3_respect

`bb({eyes:"sorry_down"});`

b: Я мав бути *твоїм* вірним захисником, але на ділі поводився неначе ти мала підкорятись *мені*.

`bb({eyes:"sorry_up"});`

b: Є різниця між захисником і тюремним наглядачем, і я переступив межу.

`bb({eyes:"sorry_down"});`

b: Вибач.

(#act3_good_4)



# act3_good_3_hurt

`bb({eyes:"sorry_down"});`

b: Я був одержимий захистом тебе від болю, ніколи не зупинявся, щоб усвідомити, що *я* завдав його тобі.

`bb({eyes:"sorry_up"});`

b: Я був поганим псом.

`bb({eyes:"sorry_down"});`

b: Вибач.

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

h: Таак, ну, це була тупа ідея від початку.

h: Я зробила це лише , щоб зруйнувати тебе, і, ну, я змогла.

h: Давай закінчим це все нічиєю, ок?

```
bb({ mouth:"sorry", eyes:"sorry" });
bb({ MOUTH_LOCK:true });
```

b: ...

b: Ок.

h: Окей.

n: *Нічия*

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

r: Ох, *ало*. Після всього що ця тварюка зробила, ти просто *здаєшся?*

r: Що таке? Ти *злякалася?*

```
publish('hong-next');
publish("act3",["roofhunter",26]);
```

h2: Так.

h2: Я налякана.

`publish('hong-next')`

h2: І це нормально!

`publish('hong-next')`

h2: Нормально бути наляканою.

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

r: Вона що, просто закрила двері?

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

b: ні...

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

b: ні ні ні

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

b: НІ!

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
