# ISA-106 і важливість автоматизації ручних процедур

ISA-106 and the Importance of Automating Manual Procedures

**Автор**: Дейв Емерсон

**Авторський переклад**: Олександр Пупена

**Оригінал:**[ **ISA-106 and the Importance of Automating Manual Procedures**](http://www.yokogawa.com/us/technical-library/resources/media-publications/isa-106-and-the-importance-of-automating-manual-procedures/)

Я маю багаторічний досвід в розробці систем керування технологічними процесами, починаючи з автоматизації процесів неперервного виробництва, а пізніше і процесів порційного виробництва. Автоматизація порційного виробництва (Batch) в значній мірі базується на послідовності операцій і станів. У меншій мірі така послідовність операцій і змін станів існує і в багатьох неперервних процесах.

Природнім здавалося б поширення уроків, отриманих в області автоматизації процесів порційного виробництва на неперервні процеси, і я пам'ятаю обговорення цієї концепції з колегами на технічних конференціях. У 1999 році я отримав можливість втілити в життя цю ідею на практиці. Коли нова технологія була комерціалізована, ми адаптували систему керування реактором порційного типу на заводі з неперервним виробництвом. Оперативний персонал цього заводу мав більш ніж 10-річний досвід експлуатації процесів порційного виробництва з високим ступенем їх автоматизації. Вони розуміли перевагу систем автоматизації, побудованих на базі стано-орієнтованого керування (з використанням станів і переходів), тому рішуче підтримали ідею впровадження автоматизації процедур для нового процесу неперервного типу.

Сенс в автоматизації процедур з’явився тоді, коли було прийнято рішення розробити процедури для декількох продуктів, а також для нового процесу. Оригінальні програми керування процесами порційного типу також стали міцною основою для автоматизації нового неперервного процесу. Завод був запущений в кінці 2000 і на ньому використовувалися автоматизовані процедури для запуску, зупинки, перезавантаження і зміни швидкості. Пізніше ми додали автоматизовану процедуру деінвентаризації і оптимізатор швидкості, а також інші функції і відповідні процедури. Додаткові зміни проводилися при появі в процесі виготовлення другого продукту.

Цей досвід змусив мене твердо повірити в необхідності автоматизації процедур, і нижче я буду ділитися своїм досвідом, як давній користувач цього підходу. Я сподіваюся, що зможу спонукувати вас здійснити автоматизацію процедур і на вашому процесі для отримання додаткових вигод, як і ми зробили свого часу.

## Чому автоматизація процедури?

Ідея автоматизації процедур не є новою, і не представляє собою якусь теоретичну концепцію. Вона існувала впродовж багатьох років, в основному в керуванні процесами порційного і напів-порціного типу виробництва, однак деякими далекоглядними користувачами використовувалась і в процесах непереврного типу виробництва. Насамперед це стосується автоматизації конкретних задач в процесі, в яких, як правило, вимагається багато ручних операцій. Автоматизація процедур потрібна тому, що багато проблем виникають саме при ручному втручанні (рисунок 1).

![img](https://web-material3.yokogawa.com/1/5920/details/c51d58f8bbaf88eec52f34a2f6327b7510d4aec1.gif)

**Рис.1.** У доповіді, опублікованій в 2012 році в Energy Practice of Marsh Ltd., підрозділ страхової компанії Marsh McLennan, розглядає п'ятирічний коефіцієнт втрат (з поправкою на інфляцію) з 1972 по 2011 рік в нафтопереробній промисловості. Інциденти під час запусків і зупинок продовжують залишатися найбільш важливим фактором, що впливають на втрати.

Є реальні переваги в такому застосуванні для процесів неперервних вробництв, і навіть поверховий аналіз показує ці можливості. Автоматизація процедури корисна не тільки в хімічній і нафтовій промисловостях, але в будь-якому процесі з наявними послідовними операціями. Автоматизація процедур була застосована до широкого діапазону процесів від операцій на морських добувних платформах до крекінг-печей по переробці ядерних матеріалів.

Процедури в тій чи іншій формі існують для всіх типів процесів. Іноді вони записані на папері, іноді зберігаються в цифровому вигляді в системі керування документами, а іноді - знаходяться тільки в чиїйсь голові (досвідні знання). Добре відпрацьовані написані процедури забезпечують безпечне та послідовне функціонування. Насправді, в деяких галузях, записані процедури є також юридичною вимогою (т.зв. стандартні експлуатаційні процедури, SOP, *примітка перекладача*). Однак, наявність процедур і їх виконання нерідко є зовсім різними речами. Для того, щоб отримати максимальну вигоду від будь-якої процедури, потрібно завжди точно дотримуватися її. Таким чином, основою для головної переваги автоматизації процедури є примушення чіткого дотримання виконання цієї процедури.

## Переваги автоматизації процедур

Автоматизація процедур забезпечує дотримання послідовної роботи процесу, що призводить до підвищення якості та більш високої пропускної здатності. Оператори можуть робити меншу кількість помилок і працювати без затримок, максимально використовуючи усі наявні ресурси. Це легко оцінюється додатковими прибутками та економією - а це хороший показник для менеджерів!

Що ще більш важливо, автоматизація процедур сприяє безпечній експлуатації. Як згадувалося раніше, це знижує ймовірність помилки оператора. У одному з досліджень співробітники Консорціуму ASM виявили, що приблизно одна третина випадків була викликана неправильним використання процедур або їх повною відсутністю. Крім того, процедури що виконуються рідше, були менш знайомі операторам, тому вони більш схильні до виникнення помилки. Ці ситуації зазвичай відбуваються в анормальному режимі функціонування, де більший ризик виникнення небезпечного інциденту (і, ймовірно, його наслідки). Автоматизація процедур також надає засоби для керованої зупинки, яка є менш небезпечною, ніж критична аварійна зупинка.

Автоматизація процедур підвищує безпечність технологічного процесу за рахунок автоматизованого керування системою зупинки і тривоговою системою. Автоматизація процедур також допомагає координувати базову систему керування технологічними процесами (BPCS) і систему протиаварійного захисту (СПАЗ, SIS), забезпечуючи розпізнання ними функцій, специфічних для даного робочого стану. Це особливо важливо під час перехідних процесів або процесів, де умови рівноваги змінюються через зміну марки продукції або сировини. За допомогою автоматизації процедури, в поєднанні з відповідним програмуванням СПАЗ (SIS) може виключити необхідність ручного запуску в обхід блокування.

Керування тривогами сильно впливає на ситуаційну обізнаність оператора і, отже, на безпечну експлуатацію. Тут автоматизація процедури також може бути використана для допомоги в керуванні тривогами, наприклад, визначити, які сигнали тривоги активні або неактивні у відповідний час, і уникнути "дратівливого" помилкового спрацювання, яке плутає операторів. Особливо це актуально в ненормальних умовах, наприклад, при аварійній зупинці.

Прибуток від підвищення рівня безпеки часто буває важко кількісно оцінити в фінансовому еквіваленті, але втрати від небезпечного функціонування очевидно дуже болісні. Збитки від небезпечних інцидентів тільки в США оцінюються в \$10 млрд. на рік. Поодинокі події можуть коштувати компаніям понад \$2 млрд, не кажучи вже про багато втрачених життів.

Раніше ми розглядали питання про знайомство оператора з процедурами та вплив на здатність операторів правильно виконувати ці процедури. Як ми всі знаємо, наші трудові ресурси сильно змінюються тоді, коли старші оператори з 30-річним або більше досвідом експлуатації йдуть на пенсію, і змінюються свіжою кров’ю без досвіду. Старші оператори, з якими я працював, як правило робили хорошу роботу наставництва з новими операторами, але передача знань ніколи не буває повною. Автоматизація процедур є відмінним інструментом для збереження знань, і наявність добре документованих процедур та автоматизації цих процедур значно зменшує проблеми зміни кадрів (рис.2)

![img](https://web-material3.yokogawa.com/1/5920/details/a0376fe279c603e321b67139f7c6be82a00f6cf3.gif)

**Рис.2.** Багато процедур погано задокументовані, і різні оператори можуть трактувати їх по-різному. Частиною задачі автоматизації таких процедур є визначення найкращої практики і включення цих підходів в наступні послідовності.

## Перший Крок реалізації: Планування

Як і з будь-яким інженерним проектом, попередньо проведений час на означення області дій буде компенсуватися на пізніших стадіях проекту. Є одна важлива деталь, яку потрібно вирішувати з самого початку, оскільки це життєво важливо для всіх областей дій. Для того щоб зробити проект успішним, ви повинні мати на заводі «свій» експлуатаційний персонал. Зрештою, не ви будете запускати завод, а вони. Якщо експлуатаційники не сприймають вигоду від автоматизації процедур, то вони не будуть використовуватися в повній мірі. Як мінімум, необхідно взяти в команду проекту одного досвідченого оператора.

Для того, щоб домогтися успіху в автоматизації процедури, необхідно спочатку визначити які процедури необхідно автоматизувати. Якщо процедури добре документовані і перевірені – це вже є хорошим фундаментом. Якщо таких немає, то ви повинні самі створити такі процедури, а це є не тривіальною задачею. Пріоритетною може бути створення процедури для єдиного правильного шляху запуску заводу, однак, часто такий кращий запуск вже сам по собі є величезним кроком вперед. Навіть якщо існують добре задокументовані методики, рекомендується детально їх оглянути, щоб переконатися, що вони насправді є правильними процедурами.

Команда із добре обізнаних в процесі експлуатації осіб повинні переглянути існуючі процедури для перевірки їх повноти і правильності. Команда повинна також запросити ідеї по вдосконаленню процедур. Акцент треба робити на процедурах без операцій в усталеному режимі, так як саме такі є найбільш вигідним для автоматизації. Насправді, було б доцільно провести огляд існуючих процедур з обговоренням того, що підпадає під область автоматизації. Це залежить від декількох факторів, у тому числі частота операцій, складність і наслідки неправильного виконання. Ці фактори також можуть впливати на пріоритет виконання.

Ви можете спробувати приступити до повної автоматизації процесу, від запуску до зупинки і всіх можливостей між ними. Незважаючи на те, що це може бути кінцевою метою, ваші шанси на успіх будуть кращими, якщо ви почнете з дещо меншого.

Для автоматизації перших процедур виберіть операції з високою частотою появи та середньої складності. Ця комбінація критеріїв дасть вам хорошу нагоду для демонстрації можливостей і переваги автоматизації процедури. Крім того, невелика складність задачі, і часте її використання дасть вам можливість доволі швидко усунути помилки при налагодженні за декілька підходів.

З іншого боку, ви очевидно не хочете вирішувати якусь тривіальну проблему, так як поєднання частоти і складності дасть вам широкі можливості для налагодження, а потім демонстрації корисності автоматизації процедури. Іншим фактором є можливість застосувати першу автоматизовану процедуру для декількох операцій або апаратів.

Іншим важливим рішенням є ступінь автоматизації даної процедури. Існує широкий спектр реалізації, від системи, яка просто інструктує операторів на кожному кроці і, можливо, підтверджує його завершення – до такої, в якій оператор ініціює виконання натисканням на кнопку запуску, а потім дозволяє системі виконувати все без сторонньої допомоги, відзвітувавши після завершення.

Це рішення торкнеться запропонованого обладнання в процесі, тому що деякі операції, ймовірно, мають компоненти (запірні клапани, насоси), які не можуть бути віддалено активовані. У цих випадках система автоматизації повинна буде направляти оператору команди про те, чим і як керувати в конкретний момент часу.

Використання існуючих ручних керуючих органів без заміни на автоматичні може бути особливо актуальним в вашому першому проекті, так як керівництво заводу необхідно буде спочатку переконати у потрібності автоматизації процедур, без додаткових затрат на дистанційно керовані запірні вентилі. У деяких випадках керівництво може мати упередження проти віддалено запуску насосів.

Пов'язаний з цим є також розгляд того, що оператору буде дозволено під час виконання автоматизованої процедури. Чи може оператор перевизначити процедуру без її відключення? Чи може він або вона змінити завдання або режими регулятору? З мого досвіду, відповідь на обидва ці питання повинна бути "ні", тому що автоматизація процедури багато в чому залежить від умов, які слідують з написаного в цій процедурі. Проте, оператор повинен мати можливість взяти на себе керування тоді, коли щось піде не так. У цьому випадку переконайтеся, що оператор може отримати доступ до всіх регуляторів, так що він або вона може робити те, що повинно бути зроблено.

## Другий крок реалізації: Розроблення

Я, як правило, виступаю за таку систему, що автоматизована в максимально можливій мірі в межах фізичних можливостей процесу. За необхідності, ви можете спочатку знайти компроміс для часткової автоматизації, тобто повністю автоматизувати тільки деякі операції, які в подальшому можуть бути включені у велику загальну систему автоматизації.

Якщо ви успішно автоматизували невелику частину дій, особливо демонструючи оперативному персоналу корисність автоматизації процедур, ви отримаєте важливих союзників в підтримку майбутніх проектів автоматизації. Ці невеликі модулі, якщо вони належним чином розроблені, можуть бути об'єднані в більш велику загальну процедуру. Ранні перемоги, навіть якщо маленькі, мають стратегічне значення в загальних зусиллях.

Існуючі апаратні засоби на вашому підприємстві також можуть бути вагомим фактором у вашому виборі. Хоча автоматизовані запірні клапани і насоси можуть більш повно автоматизувати процедуру, це може бути важко виправдати додавши їх в свій перший проект. Майте на увазі, що відсутність їх не виключає можливості автоматизації, вона просто впливає на область діяльності.

Незалежно від ступеня автоматизації, яку Ви обираєте, життєво важливо, щоб система інформувала і включала в процес керування оператора. Потенційна проблема непоінформованих операторів, швидше за все, є в повністю автоматизованих системах. Корисними є повідомлення, які відображаються на консолях операторів для передачі статусної інформації. Також корисними є повідомлення з підказками або керуючими інструкціями, які вимагають квитування або підтвердження оператором, особливо в важливих переходах, таких як початок і кінець процедури. Деталі реалізації залежать від можливостей вашої системи автоматизації.

Поінформованість оператора також може бути поліпшена шляхом навчання. Якщо оператор знає, чого очікувати, то легше слідувати процедурам автоматизації. Якщо ваша автоматизація є частиною заміни системи або міграції проекту, переконайтеся, що оператори тренувалися як в новій системі, так в конкретній області застосування. Термін навчання також має важливе значення. В ідеалі, оператор повинен мати можливість використати отримані знання на практиці якомога швидше після завершення навчання.

Як і в разі автоматизації періодичних процесів, модульність є потужним інструментом. Якщо розбити загальну процедуру на більш дрібні модулі процедур, ви можете розробити менш складну програму, ніж це було б для більшої операції. Зрештою, ви можете об'єднати їх в загальній реалізації. Таким чином, ви можете створити для вашої кінцевої мети повну автоматизацію всіх операцій. Ви також побачите, що налагодження невеликих модулів набагато простіше, ніж налагодження монолітних програм.

Залежно від вашого процесу, модулі повинні бути призначені для багаторазового використання. Як правило, деякі конструктивні особливості повторюються протягом усього процесу, так само повторюється процедура для виконання цих процесів. Це може бути простою процедурою, як запуск або зупинка насоса, або складною, як функціонування крекінг установки або колони.

Наприклад, в установці для олефінів зазвичай існує кілька крекінг печей тієї ж конструкції. Автоматизація процедури і її компоненти правильно написаної для однієї печі можуть бути повторно використані на всіх печах (наприклад, з використанням загальної логіки). Це міркування також застосовується для різних заводів і виробничих площадок всього підприємства.

І, нарешті, необхідно розглянути питання керування винятками (exception). Що ви робите, коли клапан не переходить в задану позицію? Як повинна реагувати на несподіваний стан процесу автоматизація, чи це повинен зробити оператор? Як виявити ці винятки? Як повернутися після усунення проблеми до нормального функціонування? Керування винятками, особливо логіка відновлення, є основною частиною будь-якого проекту автоматизації. Для винятків можуть бути написані процедури, але вони можуть бути невизначеними і важко автоматизуватися, тому що ви просто не можете передбачити все, що може статися під час таких аномальних станів.

Ви можете вибрати для автоматизації режим "неповної відмови" і повернути процес назад під контроль оператору, але тільки у випадку попередньої узгодженості з ним. У цьому випадку, ви також повинні вирішити, якщо для процедури бажаною є неповторювана логіка, ви повинні розглянути як автоматизація буде синхронізуватися з процесом.

Якщо виняток є критичним, може знадобитися завершення процесу, яке буде приведене в дію системою ПАЗ (SIS) або, можливо, програмою керованого відключення BPCS. Знову ж таки, необхідно враховувати синхронізацію систем SIS і BPCS. Правильна відповідь на ці питання залежить від вашого процесу і можливостей автоматизації.

## Третій крок реалізації: Введення в експлуатацію

Безумовно, для автоматизації процедур необхідне налагодження програм. Ви можете зробити велику частину цього в офлайні, наприклад, під час стендових випробувань. Тим не менше необхідно буде налагоджувати процедуру і під час запуску в полі (на об’єкті). За допомогою високо-інтегрованого моделювання процесу під час тестування можна звести до мінімуму налагодження в полі, але це не усуне його повністю. У багатьох випадках ваш технологічний процес не буде звертати увагу на результати імітаційного моделювання, і буде вести себе зовсім інакше. Модульні й багаторазово використовувані компоненти автоматизації можуть скоротити час налагодження та повинні використовуватися щоразу, коли це можливо.

Оскільки операційні зміни стану в неперервному процесі відбуваються рідше, ніж в періодичному, може бути менше можливостей для виконання і налагодження деякої частини системи автоматизації. Цей фактор може приводити до більшого часу повного її введення в дію. Про це треба обов'язково повідомити керівництву, щоб ніхто не очікував чудес в перший же день.

Процес налагодження також включає координацію і синхронізацію взаємодії між різними компонентами системи автоматизації, таких як BPCS і SIS. Це те місце, де проблеми синхронізації можуть підняти свої потворні голови, і ви повинні бути готові до їх вирішення.

І, нарешті, треба планувати додаткове навчання оператора при введенні в експлуатацію, так як підготовка на живій системі є самою ефективною. Це також хороший час для закріплення операторами раніше отриманих знань при формальному тренуванні.

## Ресурси

У тій чи іншій мірі, більшість великих постачальників систем керування, які беруть участь в роботі комітету зі стандартизації ISA106, а також деякі системні інтегратори знайомі з поняттями автоматизації процедури. Учасники, які означені в якості членів з правом голосу є найбільш активними і обізнаними про ці методи. Деякі з них також мають досвід застосування цієї технології.

Звичайно, основним ресурсом для ознайомлення автоматизації процедур є вихідні документи комітету ISA106. Перший технічний звіт ISA-TR106.00.01-2013 доступний в ISA на[ www.isa.org/store/products/product-detail/?productId=115958](http://www.isa.org/store/products/product-detail/?productId=115958) (платний, примітка перекладача). Він охоплює моделі і термінологію і вводить концепції автоматизації процедур. Комітет у даний час розробляє другий технічний звіт по робочим процесам.

Склад Комітету відкритий для всіх зацікавлених сторін, так що ви можете взяти участь в розробці стандартів. Це має дві основні переваги: по-перше, ви можете брати участь в дискусіях з багатьма визнаними експертами в цій галузі, навіть якщо тільки в якості слухача; і по-друге, ви будете мати можливість розглянути і прокоментувати роботи комітету перед публікацією матеріалу.

Для того, щоб приєднатися до Комітету в якості інформаційного члена, зверніться до ISA ([www.isa.org/isa106](http://www.isa.org/isa106) ) з проханням про членство, або по електронній пошті[ crobinson@isa.org](mailto:crobinson@isa.org) . Для участі в цьому комітеті членство ISA не потрібно.

Автоматизація процедур добре зарекомендувала себе. Правильно спроектовані і запрограмовані процедури поліпшать повторюваність, використання і безпеку вашого процесу. Мій 14-річний досвід експлуатації неперервних процесів, керованих автоматизованими процедурами підтверджує це. Я вірю в це, тому що бачив своїми очима, що автоматизована процедура може зробити. Я вважаю що і ви будете мати ті ж переваги у ваших процесах, якщо будете користуватися цими підходами.

## Точка зору постачальника ISA106

By Dave Emerson

З багатьох причин в створення технічних звітів ISA-106 і в розробку стандартів були залучені значна група постачальників систем керування технологічними процесами. Однією з основних дискусійних точок стала "велика перезміна", коли старші інженери замінюються молодими працівниками, а саме ідея захоплення досвідних знань цих досвідчених інженерів і операторів, перш ніж вони залишають об’єкт. Це широко обговорюється, але збереження досвіду системою автоматизації та технологічних операцій є дійсно складним завданням.

Стандарти автоматизації процедур полегшують цей процес. Вони забезпечують основу для створення досвідних знань в автоматизованих процедурах. Це особливо важливо для вирішення таких процедур, як запуск заводу, зупинка, зміна класу продуктів і подібних операцій, так як багато досліджень показали, що установки особливо уразливі для інцидентів безпеки, викликаних недосвідченістю операторів, що виконують незнайомі функції ручного налаштування в цей час.

Стандарт ISA-106 буде слугувати каркасом для побудови правильних процедур в системі автоматизації на основі накопичених знань оператора. Ретельна автоматизація може зробити такі процедури простішими, більш послідовними і більш безпечними, які уникають проблем, пов'язаних з недосвідченістю операторів, що роблять поганий вибір.

Існує ще багато того, що належить зробити при записі усіх частин серії ISA-106, тому ми вітаємо вашу участь. Приєднуйтеся до цієї важливої роботи, і нехай ваш голос буде почутий в цьому процесі.

Дейв Емерсон є редактором комітету ISA 106 і директором Центру розвитку США компанії Yokogawa.