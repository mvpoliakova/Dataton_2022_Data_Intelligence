# Dataton_2022_Data_Intelligence
# Бактериемия у пациентов многопрофильного стационара.
В датасете представленны данные посева крови пациентов многопрофильного стационара за 3 года: 2017, 2018 и 2019 года.
На основании собранных данных о контаминации материала; времени (в рабочих днях), затраченном на получение результата; антибиотикограмм; систем, которые применялись в работе; эпизодах задержки материала из отделения на срок более суток; диагнозах; отделениях; видах и родах микроорганизмов можно попытаться сделать предсказания для решения следующих задач:
- определения продолжительности культивирования образцов;
- выяснения сопоставимости диагнозов, отделений с высеваемостью и микробным пейзажем;
- мониторинга антибиотикорезистентности;
- целесообразности отказа от мануальных сред;
- обоснования необходимости дежурств персонала.
# Blood_data_dictionary
- год
- Месяц
- чув по групп - представлены антибиотикограммы всех положительных высевов
- N - внутренний номер пациента/анализа
- Отдел - Отделения: РНМ - реанимация, Гастр - гастроентерологическое отделение, Гин - гинекология, Гл - глазное отделение, Кард - кардиология, ЛОР - оториноларингическое отделение, Невр - неврология, Нефр - нефрологическое отделение, НХО - нейрохирургическое отделение, Ожог - ожоговое отделение, П-ка - поликлиника, Пульм - пульмонология, Ревм - ревматология, Тер - терапевтическое отделение, Тр - травматологическое отделение, Ур - урология, Хир - хирургия, ЧЛХ - челюстно-лицевая хирургия, Энд - эндокринология
- DS - диагноз: Абсцесс, АДТ - Автодорожная травма, АМПУТ - Ампутация, Ангина, Анемия, Аппенд - Аппендицит, Атероск - Атеросклероз, БА - Бронхиальная астма, ГБ - Гипертоническая болезнь, Б/Эндокард - Бактериальный эндокардит, Бак. Инф. - Бактериальная инфекция, БХП - Хроническая болезнь почек, Волчанка, Восп - Воспаление, Выкид - Выкидыш, Г/нефр - Гломерулонефрит, Гематома, Гематурия, Гепат - Гепатит, Гиб/плод - Гибель плода, Гидронефроз, Гидроцеф - гидроцефалия, Грыжа, Дерматит, Диверт - Дивертикулит, Дисфун - дисфункция мочевого пузыря, ЖКБ - желче-каменная болезнь, ЖКК - Желудочно-кишечное кровотечение, ИБС - Ишемическая болезнь сердца, ИМ - Инфаркт миокарда, Карб - Карбункул, Катар - Кататравма, Киста, Колит, Колосто - Колостома, Кома, Крона - болезнь Крона, Кровотечение, Кров г/м - Кровоизлияние в головной мозг, Лейкоз, ЛНГ - лихорадка неясного генеза, Менин - Менингит, Миелит, Миома, МКБ - Мочекаменная болезнь, Невр - невралгия, Некроз, Нефро - Нефропатия, Обслед - Обследование, Ожог, ОКН - острая кишечная непроходимость, ОКС - острый коронарный синдром, ОНМК - острое нарушение мозгового кровообращения, ОПН - Острая почечная недостаточность, Опух - рак, ОРВИ, ОРХИТ - орхит, Остеом - Остеомиелит, Отит, отр/уретр - уретрит, П/к - Почечная колика, П/род - Послеродовое состояние, Панкр - Панкреатит, Перелом, Перит - Перитонит, Перфор - Перфорация кишечника, Пиело - Пиелонефрит, Плеврит, Пневм - Пневмония, Полип, ПОН - полиорганная недостаточность, ПОХ - поясничный остеохондроз, Прост - Простотит, Псориз - Псориаз, Пульм - пневмония, РА - Ревматоидный артрит, Рак, Р/К рана - колото-резаная рана, РНМ, Сальп - Сальпингит, СД - Сахарный диабет, Свищ, Сепсис, Синусит, СКВ - Системная красная волчанка, Сочет - Сочетанная травма, Спайки, Стеноз, ТБС - туберкулез, Тромб - Тромбоз, ТТЖ - Тупая травма живота, ТЭЛА - Тромбоэмболия лёгочной артерии, Флег - Флегмона, Фурун - Фурункул, ХБП - Хроническая болезнь почек, ХОБЛ - Хроническая обструктивная болезнь легких, Холец - Холецистит, ХПН - Хроническая почечная недостаточность, Хр/Язва - Хроническая язва, ЦВБ - цереброваскулярная болезнь, Цирроз, Цистит, ЧМТ - Черепно-мозговая травма, ШОК - Шок неуточненный, Эндометрит, Энцефалопатия, Эпистатус, Язв/ж - Язва желудка
- Заб. - это не заболевание а забор материала, часто поступали пробы через 24ч после взятия и более. Это было сопряженно выходными днями 5/2. 1 - материал доставлялся в лаборатории более 24 часов, 2 - 48 часов. Такие ситуации возникали зачастую в пятницы, когда не успевали доставить материал, соответственно в понедельник от него больному  было уже мало толку. Учет данного показателя ввел, для того, что бы обосновать дежурства в лаборатории на выходных и ввести вечернею смену.
Посев - Сколько календарных дней потребовалось для окончательного результата.  
Среда - Используемые среды: "б" - bactec, коммерческая среда парные флаконы, импортная. "с" - среда со стаканчиком, по автору Сирокко, наша.
Брак -  лишние затраты, контаминация. "444" - Работа с Сирокко подразумевает, что на протяжении всего следования ежедневно надо микроскопировать флаконы, каждый артефакт, дефект покраски и т. д. приводит к тому, что (для подстраховки ибо кровь) ставят дополнительную чашку с антибиотиками (лишние траты ресурсов и времени) "б" контаминация - епидермальный стафилококк, споровая культура, коринны - т.к. флаконы парные, у бального с истиной бактериурией будут прорастать оба, если один и с перечисленными культурами, то это контаминация.
вид - вид микроорганизма
род - род микроорганизма

-
