# Первичный анализ, преобразование, исследование зависимостей визуализация и очистка данных
Оглавление
Описание данных
Описание проекта
Установка проекта
Использование проекта
Авторы
Выводы
Дополнительные материалы
Описание данных
Файл с исходными данными (файл в формате csv, разделитеь- запятая) вы можете скачать здесь

Это и есть начальный датасет, который предстоить обработать. Он находится на Google диске.

Так же там находится и промежуточный DataFrame. При нормальном ходе расчетов в проекте, он не понадобится. В случае не штатной ситуации ссылка на него находится в соответствующем разделе проекта.

Описание проекта
Компания HeadHunter хочет построить модель, которая бы автоматически определяла примерный уровень заработной платы, подходящей пользователю, исходя из информации, которую он указал о себе. Для построения этой модель, данные необходимо преобразовать, исследовать и очистить. В этом и состоит задача данного проекта.

Наш проект состоит из четырёх частей:

1. Базовый анализ структуры данных

2. Преобразование данных

3. Разведывательный анализ

4. Очистка данных

Преобразование данных - это процесс преобразования данных к виду, удобному для из визуализации и анализа.

Визуализация данных – это процесс отображения преобразованных данных в виде различного рода диаграмм и графиков, с целью выявления взаимозависимостей признаков.Это начальный этап для построения различных моделей.

Очистка данных - это процесс поиска и борьбы с аномалиями данных, включая пропуски, выбросы и некорректные данные.

Основные этапы и цели преобразования данных:

избавление от пропусков
Получение отфильтрованных наборов данных, с целью убрать явные аномалии.
Получение различного рода сгруппированных промежуточных наборов данных и сводных таблиц.
Создание новых признаков в удобном для анализа формате и удаление неинформативных признаков.
О структуре проекта:

data - папка с исходными табличными данными, как было указано ранее, основной файл с исходными данными находится на Google диске, в силу ограничениий GitHub
images - папка с изображениями диаграмм, необходимых для оформления проекта
HHproject.ipynb - jupyter-ноутбук, содержащий основной код проекта, в котором демонстрируются методы подготовки, визуализации и анализа данных
Используемые версии и библиотеки.
Python (3.10.11):
numpy (1.26.4)
pandas (2.2.1)
plotly (5.20.0)
Установка проекта
git clone https://github.com/loktiev/HeadHunterProject.git
Использование проекта
Вся информация о работе представлена в jupyter-ноутбуке HHProject.ipynb. Т.к. в GitHub файлы plotly могут не отображаться, копии всех диаграмм находятся в папке inages и отображаются дополнительно в соответствующих местах проекта.

Авторы
Борис Локтиев
Выводы
В результате обратки первичных данных, был получен Dataset,очищенный от неинформативных признаков и записей, готовый для дальнейшего построения модели предсказания предполагаемого уровня зарплаты у соискателей в компании HeadHunter. Обнаружен ряд взаимозависимостей между некоторыми признаками (Уровень образования, Опыт в (мес), готовность к командировкам и т.д.) и целевым признаком (ЗП (руб)). А также, отсутствие явной корреляции между другими признаками, например уровень зарплаты слабо зависит от готовности работать на постоянной основе, полный рабочий день.

Дополнительные-материалы
https://pandas.pydata.org/

https://github.com

https://realpython.com/python-pep8

https://plotly.com/python/
