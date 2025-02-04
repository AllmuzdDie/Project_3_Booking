# Проект 2. Проект: Предсказание рейтинга отелей на Booking

## Оглавление  
[1. Описание проекта](#Описание-проекта)  
[2. Какой кейс решаем?](#Какой-кейс-решаем)  
[3. Краткая информация о данных](#Краткая-информация-о-данных)  
[4. Этапы работы над проектом](#Этапы-работы-над-проектом)  
[5. Результат](#Результаты)    
[6. Выводы](#Выводы) 

# Описание проекта    
Построение рабочей модели машинного обучения, по выявлению нечестных отелей,
которые накручивают себе рейтинг.


:arrow_up:[к оглавлению](#Оглавление)


# Какой кейс решаем?    
Одна из проблем компании Booking — это нечестные отели, которые накручивают себе рейтинг. Одним из способов обнаружения таких отелей является построение модели, которая предсказывает рейтинг отеля. Если предсказания модели сильно отличаются от фактического результата, то, возможно, отель ведёт себя нечестно, и его стоит проверить.

# Краткая информация о данных
Данные представлены файлом формата `csv` в датасете примерно 386 тысяч записей,
датасет содержит отзывы об отелях от постояльцев, которые их посещали.
 
:arrow_up:[к оглавлению](#Оглавление)


# Этапы работы над проектом  
Проект разделен на 5 этапов и включает в себя:
- Первичный анализ данных
- Очистка и преобразование данных
- Визуализация данных
- Обучение модели и получение метрики качества
- Выводы по проекту


:arrow_up:[к оглавлению](#Оглавление)


# Результаты:  
В результате проведенного анализа, а также пробразования признаков, удалось улучшить точность предсказания по метрике `MAPE` с `0.1412` до `0.1292`

:arrow_up:[к оглавлению](#Оглавление)


# Выводы:  
1. Проведена работа по построению готовой модели машинного обучения для сервиса Booking.
Цель проекта, построение модели предсказания рейтинга отзывов об отеле, т.к. есть основание, что некоторые отели ведут не честную игру и накручивают себе рейтинг.

2. В ходе анализа данных, выяснили, что большая часть отелей в дата-сете представлена отелями из Великобритании.
Вполне закономерно, большая часть постояльцей также британцы.
Выяснили что в целом данные хорошо заполнены, пропуски были только по небольшому количеству записей по признакам широты и долготы.
Выяснили, что целевой признак не распределен по нормальному закону.

3. В ходе работы по преобразованию признаков, использовали продвинутые библиотеки, так например широту и долготу, заполнили
с использование библиотеки Geopy, по адресу отеля нашли примерные координаты и заполнили признаки.

4. Также признаки положительные и отрицательные отзывы обработали с помощью продвинутой библиотеки nltk, с помощью которой, 
определили степень тональности текста и смогли оцифровать призники.
Перевели признак tags в список, а затем с помощью библиотеки nltk, также оцифровали поличенный список.


:arrow_up:[к оглавлению](#Оглавление)


Если информация по этому проекту покажется вам интересной или полезной, то я буду очень вам благодарен, если отметите репозиторий и профиль ⭐️⭐️⭐️-дами