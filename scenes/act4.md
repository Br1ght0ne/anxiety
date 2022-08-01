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

n3: (game auto-saved)

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

h: *видих*

```
hong({body:"hold", eyes:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Ну, і яка до чорта мораль цієї історії?

`hong({body:"one_up", eyes:"annoyed"})`

h: Що ми *вивчили*? Я *була* дурною, мої друзі *використовували* мене, і я майже блять *здохла*.

`hong({body:"normal", eyes:"normal"})`

{{if _.INJURED}}
[Ага, не кажучи вже про рахунок від лікарні.](#act4a_bill)
{{/if}}

{{if !_.INJURED}}
[Ага, не кажучи вже про пошкоджену печінку.](#act4a_liver)
{{/if}}

[Ага, це і *було* найгіршим сценарієм.](#act4a_worst)

[Ага, я був правий.](#act4a_right)

# act4a_bill

`hong({eyes:"annoyed_l", mouth:"narrow"});`

h: Так. Я не думаю, що моє страхування покриє ці "уєбанські похідженьки".

`hong({eyes:"annoyed", mouth:"normal"});`

b: Але... ти вижила!

`hong({eyes:"normal"});`

h: ?

(#act4b)

# act4a_liver

`bb({eyes:"normal_d"});`

b: Ми точно зрізали кілька років твого життя...

`bb({eyes:"surprise"});`

b: Але ти досі *маєш* роки для майбуття! Ти вижила!

```
hong({eyes:"surprise"});
bb({eyes:"normal"});
```

h: ?

(#act4b)

# act4a_worst

`bb({eyes:"normal_d"});`

b: І ще...

h: Гм?

`bb({eyes:"surprise"});`

b: Ти вижила!

(#act4b)

# act4a_right

`bb({eyes:"normal_d"});`

b: Але... ти теж була права.

`hong({eyes:"surprise"});`

h: Гм?

`bb({eyes:"normal"});`

b: Я *був* вовчиком-нитиком. І коли небезпека *дійсно* прийшла, ти - виправдано - не довіряла мені.

`bb({eyes:"surprise_r"});`

b: Але, ти жива!

(#act4b)

# act4b

```
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

b: Незважаючи на все, ти все ще тут.

`hong({eyes:"suspect"});`

{{if _.INJURED}}
h: Ти виглядаєш спокійно, як на того, хто пережив передсмертний досвід.
{{/if}}

{{if !_.INJURED}}
h: Ти виглядаєш спокійно, як на того, хто пережив *перед*передсмертний досвід.
{{/if}}

```
hong({eyes:"normal"});
bb({eyes:"annoyed_d", mouth:"narrow"});
```

b: Ну, це робить все менш страшним у порівнянні. Це також змусило мене задуматись.

`bb({eyes:"normal", mouth:"normal"});`

b: Якщо мій захист сосе, тому що він не захищає тебе...

h: Але мої сварки з тобою *також* сосуть, бо ти просто гучніше кричиш...

`bb({eyes:"normal_r"})`

b: Мабуть...

`bb({eyes:"normal"})`

h: Мабуть, нам не потрібно сперечатись.

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

b: Я не Великий Поганий Вовк. І не вовк-охоронець.

`bb({eyes:"sad_d"})`

b: Я побитий пес з притулку.

`bb({eyes:"sad"})`

b: Ти пережила важкі речі. Можливо, травма або зневага. Тому я іноді реагую надто сильно і кажу:

```
sfx("yaps", {volume:0.6});
bb({body:"yap_1"});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 215;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: YAP YAP YAP YAP YAP
ГАВ ГАВ ГАВ ГАВ ГАВ/БРЕХНЯ БРЕХНЯ БРЕХНЯ #не знаю що тут більше підійде
(...1884)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_CANT_SKIP = false;
bb({body:"normal", mouth:"scream", eyes:"scream_sad"});
```

b: Але, я не *хочу* бути налякани псом! Я хочу оберігати тебе! Я хочу бути хорошим песиком!

`bb({eyes:"sad", mouth:"normal"});`

b: Human... will you help tame this wolf?
Людино, ти допоможеш вгамувати цього вовка? / Людино, ти вгамуєш цього вовка? #o(*￣▽￣*)o
`hong({eyes:"sad"})`

h: Я... Я спробую.

`hong({eyes:"normal_l", body:"chin", mouth:"narrow"})`

h: Окей. Здорові відносини з емоціями. Щоб побудувати відносини потрібно говорити. Давай побазікаєм.

`hong({eyes:"normal", body:"hands_1", mouth:"normal"})`

h: Наступні п’ять хвилин будуть звучати неймовірно банально, але давайте зробим це, поки можем.

```
hong({body:"hands_2", mouth:"normal"});
```

h: Дрогий внутрішній вовк... як *ти* почуваєшся?

n2: СТРАХІВ ВИКОРИСТАНО:

n2: *ПОШКОДЖЕНА* {{_.attack_harm_total}},  *САМОТНЯ* {{_.attack_alone_total}}, *ЖАХЛИВА* {{_.attack_bad_total}}
 
n2: ПРО ЩО ТИ ХОЧЕШ ПОГОВОРИТИ НАСАМПЕРЕД? (ІНШЕ МОЖЕШ ДІЗНАТИСЬ ПІЗНІШЕ)

```
_.a4_fears_discussed = 0;
_.num_thanks = 0;
hong({body:"normal"});
bb({eyes:"normal"});
```

[Я боюсь, що мене поранять.](#act4_harm)

[Я боюсь, бути самотньою.](#act4_alone)

[Я боюсь, бути жахливою.](#act4_bad)

# act4_harm

```
_.a4_talked_about_harm = true;
_.a4_fears_discussed += 1;
```

`bb({eyes:"normal_d"})`

b: Я хочу захистити твою потребу у фізичній безпеці,

`bb({eyes:"sad_d"})`

b: Але *весь світ* здається таким небезпечним. Повний трагедій та зла.

`bb({eyes:"sad"})`

{{if _.a4_fears_discussed==1}}
b: Не знаю, досить *мені* вибирати що говорити далі. Що *ти* скажеш, людино?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Повернімось до тебе, людино. Як ти гадаєш?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Що ти думаєш, людино?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Ти маєш рацію. Тож захищаймося.](#act4_harm_skills)

[Давайте піддамо себе *більшій* небезпеці.](#act4_harm_exposure)

[Дякую.](#act4_thanks) `_.thanks_for = "physical safety";`

# act4_harm_skills

`bb({eyes:"look_down", body:"paw"})`

b: Але... як? У мене є ікла і кігті, але я лише метафора.

```
bb({ body:"normal", eyes:"normal" });
hong({ body:"one_up", eyes:"surprise" });
```

h: Ми могли б навчитись самозахищатись? Приєднатися до групи, де люди захищають один одного? Поліпшити здоров’я і особисті межі?

```
bb({ eyes:"annoyed_r" });
hong({ body:"normal", eyes:"normal" });
```

b: Мабуть, але...

[З чого навіть почати?](#act4_harm_skills_start)

[А якщо це не спрацює?](#act4_harm_skills_work)

[А якщо ми перегнем з "безпекою"?](#act4_harm_skills_overboard)

# act4_harm_skills_start

`bb({ eyes:"sad_d" })`

b: Тут так багато роботи, стільки ми повинні виправити в собі. З чого взагалі потрібно *почати*?

`hong({ body:"shrug", eyes:"surprise" })`

h: Ми починаєм прямо зараз.

`bb({ eyes:"normal", mouth:"narrow" })`

b: E?

```
bb({ body:"normal", mouth:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal"});
```

h: Зараз ми прекрасно спілкуємось. Що допомагає нам краще виявити небезпеку, з меншою кількістю помилок,

`hong({ eyes:"surprise" });`

h: І *це* захистить нас від болю!

`hong({ eyes:"normal", mouth:"normal" });`

h: Тому *це* - тренування з самооборони.

`bb({ eyes:"normal_r" })`

b: Хех. Я очікував більшого:

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

h: Правда, неможливо на 100% захистити себе...

`hong({ body:"one_up" });`

h: Але навіть 1% прогресу все одно чогось вартий, правда?

```
bb({ eyes:"annoyed" });
hong({ normal:"one_up" });
```

b: Ти бачиш, що стакан не на 99% порожній, а на 1% повний?

`bb({ eyes:"normal" });`

h: Це вже чогось варте, якщо ти застрягнеш в пустелі.

`bb({ eyes:"closed" });`

b: Гаразд. Тоді, до дна.

(#act4_something_else)

# act4_harm_skills_overboard

`bb({ body:"chest", eyes:"annoyed" })`

b: Я маю на увазі, ти ігнорувала мої попередження, тому що *я* перестарався із безпекою! 

`bb({ body:"normal", eyes:"normal" })`

h: Ну, ти правий. Ми мали б дотримуватися безпеки в міру. Все в міру.

`bb({ eyes:"suspect" })`

b: Вибач, *ВСЕ* у мірі?

`hong({ eyes:"annoyed" })`

h: *Помірна кількість речей* в мірі.

```
bb({ eyes:"closed" });
hong({ eyes:"normal" });
```

b: Дякую, що робиш свої твердження рекурсивно самоузгодженими.

(#act4_something_else)


# act4_harm_exposure

`bb({ mouth:"scream_talk", eyes:"scream", MOUTH_LOCK:true });`

b: *ЩО*

```
bb({ mouth:"narrow", eyes:"suspect" });
hong({ body:"one_up" });
```

h: Я маю на увазі, скажімо, собака боїться грому.

`hong({ body:"hands_1" });`

h: Один прийом, яким дресирують, це відтворити запис грому на низькій гучності, а потім дати частування псу, щоб він був спокійним.

`hong({ body:"hands_2" });`

h: Протягом кількох днів дресирувальник поступово збільшує гучність, поки собака не подолає страх перед громом.

```
hong({ body:"normal", eyes:"surprise" });
bb({ mouth:"normal", eyes:"normal" });
```

h: Це називається "терапія тривалого впливу"!

`hong({ body:"point", eyes:"normal" });`

h: Оскільки ти собака, це має працювати і на тобі, так? Усі ссавці мають однакову реакцію - «бийся або біжи».

`hong({ body:"normal" });`

[Якщо ми *занадто* знизимо чутливість?](#act4_harm_exposure_overboard)

[Що робити, якщо ми піддамося *небезпеці*?](#act4_harm_exposure_hurt)

[Я вовк, не собака.](#act4_harm_exposure_dog) `bb({ eyes:"suspect" })`

# act4_harm_exposure_dog

h: І я продемонструю тобі доброту і терпіння, поки ти не станеш домашнім милим цуценям.

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"sad", mouth:"smile" })`

b: Лінь.

(#act4_something_else)

# act4_harm_exposure_overboard

`bb({ eyes:"annoyed" })`

b: Ми *щойно* бачили, що станеться, якщо ти заглушиш свій страх - ти потрапиш в *дійсно* небезпечні ситуації.

`bb({ eyes:"angry_r", body:"one_up" })`

b: Крім того, *зменшення* чутливості не перетворить нас на психопатів?

`bb({ mouth:"scream", eyes:"scream", body:"two_up" })`

b: Soon we'll give ourselves treats while watching snuff murder porn!
Незабаром ми будемо ласувати, дивлячись вбивче порно #ось тут і не знаю як нормально передати
`hong({ eyes:"annoyed" })`

h: Я... думаю, що є межа між цим і громом.

`bb({ body:"normal", mouth:"normal", eyes:"suspect" })`

b: Але саме *де*, людино? *Де?!*

`hong({ eyes:"surprise", body:"one_up" })`

h: Я не знаю. Але *ти* можеш допомогти мені!

`hong({ eyes:"normal", body:"normal" })`

h: Працюючи та домовляючись, ми намалюємо ці межі.

`bb({ body:"paw", mouth:"narrow", eyes:"closed" })`

b: Добре. Але в мене немає великих пальців, тож ти будеш рисувати.

(#act4_something_else)

# act4_harm_exposure_hurt

`bb({ body:"two_up", eyes:"angry_r" })`

{{if _.INJURED}}
b: Наприклад: ми щойно зістрибнули з чортового *даху!*
{{/if}}

{{if !_.INJURED}}
b: Наприклад: ми майже зістрибнули з чортового *даху!*
{{/if}}

```
hong({ eyes:"annoyed" });
bb({ body:"normal", eyes:"annoyed" });
```

h: Ехх, ти правий. Ти *можеш* зайти далеко.

`hong({ eyes:"normal" });`

h: Але тому, коли ми проводимо експозиційну терапію, ми починаємо з малого і робимо невеликі кроки вгору.

h: Перед тим як натрапити на *реальну* небезпеку - зупинимось.

`bb({ eyes:"annoyed_r", mouth:"narrow" });`

b: Так, я розумію межу між чуттям гучного грому і стоянням під час шторму, з високим гострим капелюхом.

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

b: Зачекай, без аргументів за чи проти того, що я відчуваю? Просто... «дякую»?

`hong({ eyes:"surprise", body:"shrug" })`

h: Так! Дякую, що турбуєшся про моє {{_.thanks_for}}.

```
bb({ eyes:"closed_annoyed", MOUTH_LOCK:true });
hong({ eyes:"normal", body:"normal" });
```

b: ...

h: Все добре?

`bb({ eyes:"super_sad", mouth:"narrow" });`

b: Ти ніколи не говорила *дякую* мені.

`hong({ mouth:"smile" });`

h: Ооу, ти великий, волохатий панічний вовк.

(#act4_something_else)

# act4_thanks_2

h: Навіть якщо ти приймаєш все до серця, я ціную, що ти піклуєшся про моє {{_.thanks_for}}.

`bb({ eyes:"annoyed" })`

b: Зачекай... ти не просто повторюєш "дякую", щоб уникнути розмови про страхи, чи не так?

```
bb({ eyes:"normal" });
hong({ eyes:"annoyed", body:"chin" });
```

h: Ну, це складно пояснити, і я не завжди маю заготовлені відповіді.

`hong({ eyes:"annoyed_l", body:"one_up" })`

h: Життя не дає нам список із трьох готових відповідей для діалогу.

`hong({ eyes:"normal", mouth:"smile", body:"normal" })`

h: Але зараз, я можу хоча б подякувати.

b: Ну, і тобі дякую, що ти терпляче мене вислухала.

`bb({ eyes:"closed" });`

b: Ти малий лисий м'язовий ссавець.

(#act4_something_else)

# act4_thanks_3

h: Навіть якщо твоє скиглення лякає мене, ти просто намагаєшся оберігти моє {{_.thanks_for}}.

`bb({ eyes:"smile_r" });`

b: Окей, якщо ти продовжиш лестити мені ось так, в інтернеті з’являться дивні уявлення про нас.

```
bb({ eyes:"smile" });
hong({ eyes:"annoyed" });
```

h: Камон, я просто вразливий студент, а ти великий страшний вовк. Найгіршим що --

`hong({ eyes:"normal", body:"point" });`

h: Власне, не відповідай на це.

(#act4_something_else)




# act4_alone

```
_.a4_talked_about_alone = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"sad_d" });`

b: Я хочу переконатися, що ти задовільниш цю потребу належати комусь...

`bb({ eyes:"sad_u" });`

b: Але я хвилююсь, що якби хтось, коли-небудь знав нас - *реальних* нас – ми б усіх відлякали.

`bb({ eyes:"sad" });`

{{if _.a4_fears_discussed==1}}
b: Не знаю, досить *мені* вибирати, що говорити далі. Що *ти* скажеш, людино?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Знову, повернемось до тебе, людино. Як ти гадаєш?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Є якісь ідеї, людино?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Я погоджуюсь: давай попрацюєм над нашим соціо-життям.](#act4_alone_skills)
 
[Я думаю що подобаюсь людям. Давай дізнаємось?](#act4_alone_experiment)

[Дякую.](#act4_thanks) `_.thanks_for = "social belonging";`

# act4_alone_skills

```
bb({ eyes:"normal" });
hong({ body:"chin" });
```

h: Ми могли б практикуватись, як ставити запитання, слухати та співпереживати, бути відкритими та вразливими, тощо?

`hong({ eyes:"normal_l" });`

h: Або удосконалити соціальні звички, як-от планування часу з друзями або регулярне відвідувати зустрічей?

`hong({ body:"one_up" });`

h: Також можна навчитися відмовляти людям.

`hong({ eyes:"normal" });`

h: Або навчитись розпізнавати коли ми людям *не* огидні, чи вони втомилися або тримають ^Суче^ лице.

```
hong({ body:"normal" });
bb({ eyes:"annoyed_r" });
```

b: Це забагато варіантів. Але про "соціальне життя"...

[Але це *маніпулятивно?*](#act4_alone_skills_manipulative)

[Чи не зробить це нас *вразливими до маніпуляцій?* ](#act4_alone_skills_manipulated)

[А якщо ми зазнаємо невдачі?](#act4_alone_skills_fail)

# act4_alone_skills_manipulative

`bb({ eyes:"suspect" });`

b: Хіба серійні вбивці, які читають емоції своїх жертв, чудові в «співпереживанні»?

`bb({ eyes:"annoyed" });`

b: Чи Чарльз Менсон схиляв до себе людей і впливав на них?

`hong({ eyes:"annoyed", body:"chin" });`

h: Ні, ти правий.

h: "Соціальні навички" нічого не значуть, якщо ми не піклуємось *про* людей.

`hong({ body:"normal" });`

h: Просто, не будь таким виродком.

`bb({ eyes:"annoyed", mouth:"smile" });`

b: Це як мотиваційний підпис на плакаті.

`hong({ body:"shrug", mouth:"narrow" });`

h: “Не будь виродком.™”

(#act4_something_else)

# act4_alone_skills_manipulated

`bb({ eyes:"angry" })`

b: Ми станемо вхідним килимком, який буде говорити «Будь ласка» і «дякую», коли люди витиратимуть об нас ноги!

`bb({ mouth:"scream", eyes:"scream" })`

b: Ми будем цілувати стільки срак, що це буде виглядати наче ми накрасились коричневою помадою. 

```
bb({ mouth:"normal", eyes:"normal" });
hong( body:"chin" });
```

h: Егх, ти правий. "Соціальні навички" - це не тільки про задовільняння інших, а це ще й про встановлення *меж.*

`hong( body:"one_up" });`

h: Ми не можемо запрошувати інших додому, якщо у нас немає стін, які б підтримували наш дім.

```
hong( eyes:"angry", mouth:"narrow" });
bb( eyes:"annoyed", mouth:"smile" });
```

h: І ще... щодо: помадна ментальна картинка...*ее??*

(#act4_something_else)

# act4_alone_skills_fail

`bb({ eyes:"annoyed" });`

h: Ми можемо провалитись. Насправді, ми *провалимось*

```
bb({ eyes:"normal" });
hong({ eyes:"surprise", body:"shrug" });
```

h: Це - нормально! Ми вчимось на помилках!

`hong({ body:"normal", eyes:"normal" });`

h: Давай провалимось разом, еге?

`bb({ eyes:"normal_r" });`

b: Звісно, я думаю... при найгіршому сценарії, ми можемо виїхати з міста і створити нову ідентичність.
 
`bb({ eyes:"normal" });`

h: Ага, я думаю, це буде коштувати лише 2 біткоіни в ці дні.

(#act4_something_else)

# act4_alone_experiment

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Ми можем спробувати якісь експерименти!

`hong({ body:"chin" });`

h: Ми можем запросити друзів на прогулянку, відновіти спілкування зі старим другом, або поспілкуватисья з баристою.

`hong({ body:"normal" });`

h: Я думаю, ми можем бути більш приємними, ніж підозрюємо.

`bb({ eyes:"annoyed" });`

[А якщо це малі, дешеві "перемоги"?](#act4_alone_experiment_cheap)

[А якщо це стане тягарем для інших?](#act4_alone_experiment_burden)

[Але короткі розмови це не *ми*!](#act4_alone_experiment_real_us)

# act4_alone_experiment_real_us

`bb({ eyes:"sad" });`

b: Якщо ми натягнем піддільну усмішку, ми ніколи дійсно ні з ким не зв'яжимось,

`bb({ eyes:"super_sad" });`

b: *Але* якщо ми відкриємось, інші люди побачуть наш пошматований стан!

`hong({body:"chin", mouth:"narrow", MOUTH_LOCK:true})`

h: ...

```
hong({body:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Перекрутись.

b: Що.

`hong({body:"hands_1"})`

h: Коли собаки показують любов та довіру, вони роблять себе вразливими, оголивши животик.

`hong({body:"one_up"})`

h: Можливо, ми *недостатньо* впевнені, щоб бути занадто вразливими, але з достатньою підготовкою,

`hong({body:"normal", eyes:"surprise"})`

h: Одного дня, ми зможем показувати людям наше я - зруйноване, але людське.

```
hong({eyes:"normal"});
bb({ eyes:"super_sad", mouth:"smile", body:"chest" });
```

b: Я перекручусь, якщо ти даш мені щось смачненьке.

`bb({ eyes:"normal", mouth:"normal" });`

h: Ні.

(#act4_something_else)


# act4_alone_experiment_cheap

b: Говорити "привіт" до баристи, це не виступ гідний золотої медалі на Соціально-Метеликовій олімпіаді.

```
hong({ body:"point", eyes:"surprise" });
bb({ eyes:"normal" });
```

h: Це для *нас!*

`hong({ body:"one_up", eyes:"annoyed" });`

h: На соціальній арені ми навіть не в пір'їнковій ваговій категорії, ми типу... кварки.

`hong({ body:"normal", eyes:"normal" });`

h: Якщо ми починаєм з малих, дешевих перемог, нехай так і буде. Перед тим як ступити 1000 кроків ми робимо 1.

b: Ага! Мабуть, після "Привіт", ми зможемо сказати...

`bb({ body:"two_up", mouth:"smile", eyes:"smile_u" });`

b: *"Як ти?"*

`hong({ body:"shrug", mouth:"smile", eyes:"surprise_l" });`

h: *"Таке собі!"*

(#act4_something_else)

# act4_alone_experiment_burden

`bb({ eyes:"suspect_r" })`

b: Напевно, бариста захоче зробити гімняну каву, не *експеримент*, щоб побачити, що наші соціальні навички сосуть.

`bb({ eyes:"annoyed" })`

h: Ну, якщо ми *станемо* зайвим тягарем ...

```
hong({ eyes:"surprise" });
bb({ eyes:"normal" });
```

h: Це теж буде непогано!

`hong({ eyes:"normal" });`

h: Ми можем навчитись як правильно запитувати людей про кмфортні для них речі, вчитись як дотримуватись чужих меж.

```
hong({ eyes:"annoyed_l", mouth:"narrow" });
bb({ eyes:"annoyed", mouth:"smile" });
```

h: Знаєш, ці всі "міжособові навички", ^гімно^ яке ми бачим в брошурах для консультантів.

(#act4_something_else)



# act4_bad

```
_.a4_talked_about_bad = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"annoyed_r" })`

b: Я хочу захищати твої моральні потреби, що спонукають ставати кращою людиною,

`bb({ eyes:"sad_d" })`

b: Але глибоко всередині, ми настільки фундаментально...поломані.

`bb({ body:"two_up", eyes:"angry" })`

{{if _.INJURED}}
b: І не говори, що це *не* так. Ми зістрибнули з *даху*.
{{/if}}

{{if !_.INJURED}}
b: І не говори, що це *не* так. Ми майже зістрибнули з *даху*.
{{/if}}

`bb({ body:"normal", eyes:"sad" })`

{{if _.a4_fears_discussed==1}}
b: Не знаю, досить *мені* вибирати, що говорити далі. Що *ти* скажеш, людино?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Знов, повернімось до тебе, людино. Що ти думаєш?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Більше думок, людино?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Ми поломані. Давай виправим це.](#act4_bad_fix)

[Ми поломані. Давай приймем це.](#act4_bad_accept)

[Дякую.](#act4_thanks) `_.thanks_for = "moral well-being";`

# act4_bad_fix

```
bb({eyes:"normal"});
hong({body:"chin"});
```

h: Ми могли б поступово створювати кращі звички, привести своє життя до того, що ми цінуємо,

`hong({body:"one_up"});`

h: Якщо потрібно, ми можем отримати професійну допомогу - терапевт або психолог.

`hong({body:"normal"});`

h: Є шляхи починити це.

[А якщо ми не зможем все виправити?](#act4_bad_fix_cant)

[А якщо ми *перестараємось?*](#act4_bad_fix_too_much)

[Ми не можемо дозволити собі професійну допомогу.](#act4_bad_fix_afford)

# act4_bad_fix_cant

`hong({eyes:"annoyed"});`

h: Егх, я думаю ти правий.

h: Ми не можем все виправити.

`bb({mouth:"scream", eyes:"scream_sad"});`

b: Аахг, я знав, ми завжди будемо поломаними!

`hong({eyes:"surprise"});`

h: Але ми можемо як мінімум бути *менш* зруйнованими.

```
bb({mouth:"normal", eyes:"annoyed"});
hong({eyes:"sad", mouth:"smile"});
```

h: Шрами заживають з часом, але не до кінця. І це нормально.

`bb({eyes:"annoyed_r"});`

b: Напевно. Але,

```
Game.FORCE_TEXT_Y = 460;
Game.clearText();
publish("act4-sexy", [true]);
```

b: Шрами - *сексуальні.*

```
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-sexy", [false]);
bb({body:"chest", mouth:"smile_talk", MOUTH_LOCK:true, eyes:"sexy"}, 0);
hong({eyes:"normal", mouth:"normal"}, 0);
```

h: Будь ласка, не починай.

(#act4_something_else)

# act4_bad_fix_too_much

`bb({ eyes:"angry_d" })`

b: Це дико признавати, але... якась частина мене *хоче* мати цей розлад.

`bb({ eyes:"angry" })`

b: Типу, без цього, ми ж будемо *нецікавими?*

`bb({ eyes:"sad_r", body:"one_up" })`

b: Без болячок, чи не стане наше мистецтво сірим та ніяким?

`bb({ eyes:"sad_u", body:"two_up" })`

b: Без розладу ми не зможемо зв’язатися з нашими друзями, які так само страждають?

`bb({ eyes:"sad", body:"chest" })`

b: Якщо ми коли-небудь будемо задоволені життям, чи не припинимо ми змушувати себе творити?

`hong({ MOUTH_LOCK:true })`

h: ...

h: Якщо ми навіть боїмось... "бігти від страхів"...

h: Я не думаю що ми від них втечем.

`bb({ eyes:"smile_u", body:"normal", mouth:"smile" })`

b: Оу, так! Хуу! Яке полегшання!

(#act4_something_else)

# act4_bad_fix_afford

`bb({ body:"one_up", eyes:"sexy", mouth:"normal" })`

b: "Док, я переживаю, що плачу 100$/год. лише щоб почути від Вас *що ви відчуваєте від цього?*"

`bb({ body:"paw", eyes:"closed", mouth:"narrow" })`

b: "Мм-гмм. І як ви себе почуваєте?"

```
bb({ body:"normal", eyes:"normal", mouth:"normal" });
hong({ eyes:"sad" });
```

h: Егх, це цілком розумне переживання.

`hong({ eyes:"annoyed", mouth:"sad" });`

h: І справді прикро, не всі можуть слідкувати за психічним здоров'ям.

`hong({ eyes:"normal", mouth:"normal" });`

h: Але, ще досі є дешеві або безплатні варіанти:

`hong({ body:"chin" })`

h: Групи підтримки, онлайн терапія, студентські/некомерційні оздоровчі центри...

`hong({ body:"hands_1" })`

h: Звички як медитація, хороший сон, регулярне спілкування з друзями, дізнаватися нові речі...

`hong({ body:"hands_2" })`

h: Ходити в бібліотеку, щоб брати зошити з доказової психотерапії...

`hong({ body:"one_up" })`

h: Є безмежна кількість ресурсів, кінці кіців!

```
hong({ body:"normal" });
bb({ eyes:"annoyed", mouth:"narrow" });
```

b: Ну, *ця* четверта стіна довго не простояла.

`hong({ body:"point" });`

h: Деякі речі більш важливі, ніж розповідь. Такі як психічне здоров'я.

(#act4_something_else)


# act4_bad_accept

```
bb({ eyes:"normal" });
hong({ eyes:"normal_l", body:"one_up", mouth:"narrow" });
```

h: Я маю на увазі, саме це говорять терапевти? Прийняти всі свої емоції, навіть негативні?

```
bb({ eyes:"annoyed" });
hong({ eyes:"normal", body:"normal", mouth:"normal" });
```

b: Зачекай.

["Прийняти", як *здатись*?](#act4_bad_accept_give_up)

["Прийняти", як *погодитись*?](#act4_bad_accept_approve)

["Прийняти", як *сприймати буквально*?](#act4_bad_accept_literally)

# act4_bad_accept_give_up

`bb({ eyes:"angry", body:"one_up" });`

b: Ти думаєш, Мартін Лютер Кінг сказав би: "Чорт, Ми не можемо сидіти в передній частині автобуса, давай просто *приймімо* це?"
`bb({ eyes:"angry_r", body:"two_up" });`

b: Чому Індустрійний Комплекс Самодопомоги думає, що розмахування білим прапором є *глибокою мудрістю?* 

`bb({ eyes:"annoyed", body:"normal" });`

h: Я думаю терапевти думали "прийняти" погані речі як те, що вони існують, і це важко змінити,

h: Але не обов’язково відмовлятися від прагнення до змін.

`bb({ eyes:"suspect" });`

b: Тоді, терапевти мають говорити *визнавати*, а не *приймати*.

`hong({ body:"chin", eyes:"annoyed" });`

h: Ага, це *прийняти* дещо спантеличує.

`bb({ eyes:"closed", mouth:"narrow" });`

b: Ну, я *визнаю* це.

(#act4_something_else)

# act4_bad_accept_approve

`bb({ eyes:"angry" });`

b: Типу, *добре* що ми поломані, чи що? Ні!

`bb({ eyes:"angry_r", body:"one_up" });`

b: Всі ці чортові ґоллівудські сценаристи, що романтизують психічні хвороби, повні ^лайна^!

`bb({ eyes:"angry", body:"two_up" });`

b: Мати психічні порушення - *^хуйово!^*Це краде в людей *життя!* Чому ми маємо "приймати" таке?!

`bb({ body:"normal" });`

h: Я думаю, терапевти мають на увазі «приймати» наші емоції, як бути терплячими з ними.

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Як спроби вибратись в сипучих пісках змушує тебе тонути швидше, і вирішення - просто спокійно лежати,

`hong({ eyes:"surprise" });`

{{if _.INJURED}}
h: Боротьба проти тебе, мій страхо, привела мене до стрибку з даху.
{{/if}}

{{if !_.INJURED}}
h: Боротьба проти тебе, мій страхо, майже привела мене до стрибку з даху.
{{/if}}

`hong({ body:"normal", eyes:"normal" });`

h: Натомість рішення в тому, щоб робити те, що ми робимо зараз – не боротись, а терпляче бути один з одним.

`bb({ eyes:"annoyed" });`

b: Тоді вони мають говорити *це*, замість такого проблематичного поняття, як "приймати".

`hong({ body:"chin", eyes:"annoyed" });`

h: Ага, якщо подумати, "приймати" ^хріново^.

`bb({ eyes:"closed_annoyed", mouth:"narrow" });`

b: Я не приймаю "приймання".

(#act4_something_else)

# act4_bad_accept_literally

`bb({ eyes:"sad", body:"one_up" });`

b: Але, ми вже *знаємо*, ти не маєш сприймати мене буквально!

`bb({ eyes:"sad_u", body:"two_up" });`

b: Уся *проблема* в тому, що я хочу тобі допомогти, але я не вмію підбирати правильні слова!

`bb({ eyes:"sad", body:"normal" });`

h: Я думаю терапевти сприймають "прийняття" своїх емоцій як: "Не ігноруйте їх."

`hong({ eyes:"surprise", body:"one_up" });`

h: Слухати себе, працювати *з* собою, але не сприймати все 100% правдою.

```
hong({ eyes:"normal", body:"normal" });
bb({ eyes:"annoyed", mouth:"normal" });`
```

b: Тоді терапевти мають говорити *це* замість якогось милистого, незрозумілого "приймати". 

`hong({ body:"chin", eyes:"annoyed" });`

h: Ну, гадаю вони також ^уїбани^ в підбиранні слів.

(#act4_something_else)




# act4_something_else

```
bb({ body:"normal", mouth:"normal", eyes:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal" });
```

{{if _.a4_fears_discussed==1}}
h: Може є ще щось, про що ти хочеш побалакати?
{{/if}}

{{if _.a4_fears_discussed==2}}
h: Щось ще навантажує твоє серце?
{{/if}}

{{if _.a4_fears_discussed==3}}
(#act4_something_else_2)
{{/if}}

{{if _.a4_talked_about_harm!=true}}
[Я боюсь, що нас поранять.](#act4_harm)
{{/if}}

{{if _.a4_talked_about_alone!=true}}
[Я боюсь, що ми залишимось одні.](#act4_alone)
{{/if}}

{{if _.a4_talked_about_bad!=true}}
[Я боюсь, що ми будемо жахливими.](#act4_bad)
{{/if}}

[Нє, все впорядку.](#act4c_prelude)

# act4_something_else_2

h: Окей, ми обговорили вже всі свої страхи.

b: Ага, їх тільки три.

h: Ага, саме три.

b: Прекрасно.

(#act4c)

# act4c_prelude

h: Прекрасна розмова, команда.

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

b: Це не просто якась *гра*, розумієш.

`bb({eyes:"angry_d", body:"one_up"})`

b: Налагоджувати здорові взаємовідносини зі своїми емоціями не так легко, як нажимати кнопки на екрані.

`bb({eyes:"sad", body:"normal"})`

b: Чи *дійсно*, ми можемо зійтись?

b: *Працювати* разом, як команда?

`hong({eyes:"sad", body:"one_up"})`

h: Ну,

```
hong({eyes:"surprise_l"});
bb({eyes:"normal"});
```

a: В-вибачте...

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

a: Н-не-непроти, якщо я присяду біля тебе пообідати?

`publish("act4", ["alshire", 1]);`

{{if _.TOP_FEAR=="harm"}}
s: *Це* твій краш? Чому вона сидить одна, як якийсь божевільний серійний вбивця? 
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: Питаєш в краша, чи можеш сидіти поряд? Ти знаєш, наскільки *по-жебрацькому* ми звучимо?!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: *Це* твій краш? Ми перервали її спокій та тишу! Ми просто зайвий тягар для неї!
{{/if}}

`publish("act4", ["alshire", 2]);`

a: Я- Я маю-- це, нормально якщо ти відмовиш, я просто...

`publish("act4", ["alshire", 3]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "h2"`

[Зачекай, я бачила тебе на вечірці?](#act4d_recognition) `publish("act4", ["hong_to_alshire",1])`

[Звісно! Присідай.](#act4d_yes) `publish("act4", ["hong_to_alshire",2])`

[Вибач, мені потрібно побути зараз одній.](#act4d_no) `publish("act4", ["hong_to_alshire",8])`

# act4d_recognition

`publish("act4", ["hong_to_alshire",2]);`

h2: Так, ти була на дивані! На першій вечірці я пішла до...

`publish("act4", ["hong_to_alshire",10]);`

{{if _.a2_ending=="fight"}}
h2: Де у мене була панічна атака і я вдарила організатора.
{{/if}}

{{if _.a2_ending=="flight"}}
h2: Де у мене була панічна атака, і я побігла поки плакала.
{{/if}}

```
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Зачекай людино, ми може засильно нагружуємо.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ах, я не хотіла тебе засмутити!

`publish("act4", ["hong_to_alshire",4]);`

h2: Просто пам'ятаю дружнє лице, і все.

```
publish("act4", ["hong_to_alshire",5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: АГХХ, Я ЗНАЛА! ВОНА НЕБЕЗПЕЧНИЙ ПАНІЧНОВМОТИВОВАНИЙ ПСИХ!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: АГХХ, ПЕРШЕ ВРАЖЕННЯ, ЯКЕ МИ СТВОРИЛИ БУЛО "ПОДИВИСЬ НА МОЮ ТРАВМУ"!ЦЕ ЗНАЧИТЬ ВОНА НАС НЕНАВИДИТЬ!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: АГХХ, МИ ЗАСТАВИЛИ ЇЇ ЗАПАМ'ЯТАТИ ТРАВМАТИЧНУ ПОДІЮ. НАША ПРИСУТНІСТЬ ТРАВМУЄ ІНШИХ.
{{/if}}

(#act4e)

# act4d_yes

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Зачекай, людино, їй мабуть нелегко.

```
publish("act4", ["hong_to_alshire", 6]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ах, я не наполягаю!

`publish("act4", ["hong_to_alshire", 4]);`

h2: Просто говорю, ти можеш присісти, якщо хочеш.

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: ВОНА *НАДТО* ДРУЖНЯ! ЯК ТЕД БАНДІ, СЕРІЙНИЙ ВБИВЦЯ!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: ЦЕ ПРОСТО ЇЇ ГРА! НІХТО *ДІЙСНО* НЕ ХОЧЕ БУТИ БЛИЗЬКИМИ З НАМИ!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: АГХХ, МИ ЗАВЖДИ ЗМУШУЄМО ІНШИХ ПОЧУВАТИСЯ НІЯКОВО! МИ МУСОР ЦІЄЇ ЗЕМЛІ!
{{/if}}

(#act4e)

# act4d_no

```
publish("act4", ["hong_to_alshire", 9]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Зачекай людино, ми може засильно нагружуємо.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ах, не хочу показатись грубою!

`publish("act4", ["hong_to_alshire", 6]);`

h2: Мені потрібен час, щоб зрозуміти себе. Не сприймай це як особисту відмову.

```
publish("act4", ["hong_to_alshire", 7]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: ЯКІ ХВОРІ, ПОВЕРНУТІ ДУМКИ ЇЇ ДОЛАЮТЬ?! ЩО ЗА ТЕМНІ БАЖАННЯ ЗАПОВНЮЮТЬ СЕРЦЕ ЦІЄЇ ПСИХОПАТКИ?!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: НАМ ВІДМОВИЛИ! НАС НІКОЛИ НЕ БУДУТЬ ЛЮБИТИ!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: МИ ПЕРЕРВАЛИ ЇЇ РОЗДУМИ! ТЕПЕР ВОНА НАЗАВЖДИ ЗАЛИШИТЬСЯ ТРАВМОВАНОЮ, І ЦЕ ВСЕ НАША ПРОВИНА!
{{/if}}

(#act4e)

# act4e

```
Game.WORDS_HEIGHT_BOTTOM = 195;
publish("act4", ["alshire", 6]);
```

s: БІЖИ БІЖИ БІЖИ БІЖИ БІЖИ БІЖИ БІЖИ БІЖИ БІЖИ БІЖИ БІЖИ БІЖИ

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

h: Хех. Це було дивно. І що було в її голові.

`publish("act4", ["hong_closer", 2]);`

h: І так, що ти говорив?

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 6]);
```

b: Ее, я забув? Щось про команду і роботу?

```
publish("act4", ["bb_closer", 0]);
publish("act4", ["hong_closer", 3]);
```

h: ¯\_(ツ)_/¯

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 4]);
```

b: Вони говорять, що ти маєш "примиритися" зі своїми емоціями, так наче вони "воєнні кримінали".

`publish("act4", ["bb_closer", 7]);`

b: Але я хочу *більше* для нас, аніж простий мир! Я хочу щоб ми були *союзниками!*

`publish("act4", ["bb_closer", 3]);`

b: Я хочу бути хорошим охоронним псом. Так як голод і спрага попереджують про твої фізичні потреби,

`publish("act4", ["bb_closer", 8]);`

b: Я хочу бути сигналом для тебе про твої *психологічні* потреби: безпека, прив'язаність, доброта.

`publish("act4", ["bb_closer", 1]);`

b: Але... Я не справляюсь з цим, тому мені потрібно, щоб ти мене тренерувала.

`publish("act4", ["bb_closer", 4]);`

b: Я не "завжди вагомий," чи "завжди ірраціональний." Я просто... намагаюсь зі всіх сил. Тому будь ласка,

`publish("act4", ["bb_closer", 30]);`

b: Допоможи мені допомогти тобі!

`publish("act4", ["bb_closer", 6]);`

b: Хоча, навчити старого пса новим трюкам займе *деякий* час. Мабуть *роки.*

`publish("act4", ["bb_closer", 3]);`

b: І інколи я буду повертатись до своїх старих звичок.

`publish("act4", ["bb_closer", 2]);`

b: Гавкати на тіні. Лякати тебе своїми словами. Я можу навіть показувати нав'язливі картинки... речей.

`publish("act4", ["bb_closer", 9]);`

b: Вибач! Я побитий безпритульний пес! А такі пси інколи сруть тобі на ліжко!

`publish("act4", ["bb_closer", 4]);`

b: Але якщо тобі хватить терпіння.. і просто залишишся і посидиш зі мною...

`publish("act4", ["bb_closer", 8]);`

b: Мабуть, ти вгамуєш цього вовка.

`publish("act4", ["bb_closer", 0]);`

`Game.clearText();`

(...1000)

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Хороший пес.](#act4f-pat-bb) `Game.OVERRIDE_CHOICE_SPEAKER = "h"; publish("act4", ["hong_closer", 2]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "b"`

[Хороша людина.](#act4f-pat-hong) `Game.OVERRIDE_CHOICE_SPEAKER = "b"; publish("act4", ["bb_closer", 8]);`

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
b: АААА ТИ ДОСІ ЇСИ ОДНА, П'ЯТНАДЦЯТЬ СИГАРЕТ АААА
{{/if}}

{{if _.parasite}}
b: ТИ ДОСІ НЕ ПРОДУКТИВНА ПОКИ ЇСИ, МИ СОЦІО-ПАРАЗИТИ АААААА
{{/if}}

{{if _.whitebread}}
b: ААААА ТИ ЇСИ БІЛЬШЕ БІЛОГО ХЛІБУ ААААА
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

b: ГАВ ГАВ ГАВ ГАВ ГАВ

(#credits)
