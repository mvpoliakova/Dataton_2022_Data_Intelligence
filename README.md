# Dataton_2022_Data_Intelligence
# Бактериемия у пациентов многопрофильного стационара.
## Авторы:
Белякова Людмила, Гаврилюк Степан, Евтеев Андрей, Ефременкова Ольга, Пирогов Евгений, Полякова Марина
## Описание:
В датасете представлены данные посева крови пациентов многопрофильного стационара за 3 года: 2017, 2018 и 2019.
На основании собранных данных о контаминации материала; времени (в рабочих днях), затраченном на получение результата; антибиотикограмм; систем, которые применялись в работе; эпизодах задержки материала из отделения на срок более суток; диагнозах; отделениях; видах и родах микроорганизмов есть вероятность получить предсказания для решения следующих задач:
- определение продолжительности культивирования образцов;
- выяснение сопоставимости диагнозов, отделений с высеваемостью и микробным пейзажем;
- мониторинг антибиотикорезистентности;
- целесообразность отказа от мануальных сред;
- обоснование необходимости дежурств персонала в выходные дни и вечерние смены.
## Структура репозитория:
 В файлах Excel с названиями "кров 2017 год", "кров 2018 чув", "кров 2018", "кров 2019 год", "кров 2019" содержатся исходные данные датасета.  
 В файле blood.xlsx объединены все исходные данные.   
 Jupyter Notebook dataton_clearing содержит предобработку данных, результатом которой являются файлы blood_data.csv и blood_culture.csv.   
 Итоговый результат представлен в формате Jupyter Notebook и имеет название data_intelligence_bact.
## Blood_dictionary
- год
- Месяц
- чув по групп - представлены антибиотикограммы всех положительных высевов
- N - внутренний номер пациента/анализа
- Отдел - Отделения: РНМ - реанимация, Гастр - гастроэнтерологическое отделение, Гин - гинекология, Гл - глазное отделение, Кард - кардиология, ЛОР - оториноларингологическое отделение, Невр - неврология, Нефр - нефрологическое отделение, НХО - нейрохирургическое отделение, Ожог - ожоговое отделение, П-ка - поликлиника, Пульм - пульмонология, Ревм - ревматология, Тер - терапевтическое отделение, Тр - травматологическое отделение, Ур - урология, Хир - хирургия, ЧЛХ - челюстно-лицевая хирургия, Энд - эндокринология
- DS - диагноз: Абсцесс, АДТ - Автодорожная травма, АМПУТ - Ампутация, Ангина, Анемия, Аппенд - Аппендицит, Атероск - Атеросклероз, БА - Бронхиальная астма, ГБ - Гипертоническая болезнь, Б/Эндокард - Бактериальный эндокардит, Бак. Инф. - Бактериальная инфекция, БХП - Хроническая болезнь почек, Волчанка, Восп - Воспаление, Выкид - Выкидыш, Г/нефр - Гломерулонефрит, Гематома, Гематурия, Гепат - Гепатит, Гиб/плод - Гибель плода, Гидронефроз, Гидроцеф - гидроцефалия, Грыжа, Дерматит, Диверт - Дивертикулит, Дисфун - дисфункция мочевого пузыря, ЖКБ - желче-каменная болезнь, ЖКК - Желудочно-кишечное кровотечение, ИБС - Ишемическая болезнь сердца, ИМ - Инфаркт миокарда, Карб - Карбункул, Катар - Кататравма, Киста, Колит, Колосто - Колостома, Кома, Крона - болезнь Крона, Кровотечение, Кров г/м - Кровоизлияние в головной мозг, Лейкоз, ЛНГ - лихорадка неясного генеза, Менин - Менингит, Миелит, Миома, МКБ - Мочекаменная болезнь, Невр - невралгия, Некроз, Нефро - Нефропатия, Обслед - Обследование, Ожог, ОКН - острая кишечная непроходимость, ОКС - острый коронарный синдром, ОНМК - острое нарушение мозгового кровообращения, ОПН - Острая почечная недостаточность, Опух - рак, ОРВИ, ОРХИТ - орхит, Остеом - Остеомиелит, Отит, отр/уретр - уретрит, П/к - Почечная колика, П/род - Послеродовое состояние, Панкр - Панкреатит, Перелом, Перит - Перитонит, Перфор - Перфорация кишечника, Пиело - Пиелонефрит, Плеврит, Пневм - Пневмония, Полип, ПОН - полиорганная недостаточность, ПОХ - поясничный остеохондроз, Прост - Простотит, Псориз - Псориаз, Пульм - пневмония, РА - Ревматоидный артрит, Рак, Р/К рана - колото-резаная рана, Сальп - Сальпингит, СД - Сахарный диабет, Свищ, Сепсис, Синусит, СКВ - Системная красная волчанка, Сочет - Сочетанная травма, Спайки, Стеноз, ТБС - туберкулез, Тромб - Тромбоз, ТТЖ - Тупая травма живота, ТЭЛА - Тромбоэмболия лёгочной артерии, Флег - Флегмона, Фурун - Фурункул, ХБП - Хроническая болезнь почек, ХОБЛ - Хроническая обструктивная болезнь легких, Холец - Холецистит, ХПН - Хроническая почечная недостаточность, Хр/Язва - Хроническая язва, ЦВБ - цереброваскулярная болезнь, Цирроз, Цистит, ЧМТ - Черепно-мозговая травма, ШОК - Шок неуточненный, Эндометрит, Энцефалопатия, Эпистатус, Язв/ж - Язва желудка
- Заб. - забор материала: 1 - материал доставлялся в лаборатории более 24 часов, 2 - 48 часов.
- Посев - количество календарных дней, требуемых для окончательного результата.  
- Среда - Используемые среды: "б" - bactec, коммерческая среда парные флаконы, автоматизированный анализ. "с" - среда по автору Сирокко, мануальный анализ.
- Брак -  контаминация.
- вид - вид микроорганизма
- род - род микроорганизма
