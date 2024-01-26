# GWO-CNN-on-CIFAR10
Обучение нейронной сети генетическим Алгоритмом Серых Волков на примере датасета CIFAR10

Алгоритм Серых Волков представляет собой метаэвристический оптимизационный алгоритм, вдохновленный социальным поведением волков. Этот алгоритм базируется на идеях исследования и кооперации волков в природе, чтобы эффективно искать оптимальные решения в пространствах поиска задач оптимизации.
Основные Принципы и Идеи:

1.	Имитация Социального Поведения Волков:	Алгоритм Серых Волков моделирует основные аспекты социальной иерархии волчьих стаек, такие как исследование территории, сотрудничество при охоте и устранение слабых звеньев.
2.	Структура Алгоритма:	Популяция в GWO представляет собой группу "волков", каждый из которых представляет потенциальное решение. Волки разделяются на три категории: Альфа (альфа-волк, наилучший индивид), Бета (бета-волк) и Гамма (гамма-волк). Все остальные волки оценивают свое положение в социальной иерархии и обновляют свое поведение в соответствии с позициями альфа, бета и гамма.
3.	Операторы Обновления Положения Волков:	Каждый волк в популяции обновляет свое положение, подражая поведению альфа, бета и гамма в зависимости от социальной иерархии. Это позволяет эффективнее искать оптимальные решения, используя информацию от лучших индивидов в популяции.
4.	Функция Приспособленности:	Функция приспособленности определяет качество решения и оценивается для каждого волка. Она используется для определения иерархии в популяции и влияет на выбор поведенческих стратегий.
Операционные Этапы Алгоритма:
1.	Инициализация:	Начальная позиция каждого волка задается случайным образом в пространстве поиска. Определяются начальные значения альфа, бета и гамма.
2.	Обновление Позиций Волков:	Каждый волк обновляет свою позицию в пространстве поиска, основываясь на положении альфа, бета и гамма. Это происходит в соответствии с определенными формулами, использующими случайные коэффициенты.
3.	Оценка Приспособленности и Обновление Иерархии:	Приспособленность каждого волка оценивается с использованием целевой функции. Иерархия в популяции обновляется на основе значений приспособленности, и лучшие индивиды выбираются для ролей альфа, бета и гамма.
4.	Проверка Критерия Остановки:	Алгоритм продолжает свою работу, обновляя позиции и иерархию, пока не выполнен критерий остановки, такой как достижение максимального числа итераций или достижение заданного уровня приспособленности.

Применение и Преимущества:
Алгоритм Серых Волков широко применяется для решения задач оптимизации в различных областях, таких как инженерия, экономика, биология и другие. Его преимущества включают способность эффективного обхода пространства поиска, относительную простоту реализации и низкую зависимость от настроек параметров.
Блок схема алгоритма серых волков представлена в виде описания и рисунка 1.4.1.
1.	Начало
2.	Инициализация параметров алгоритма
3.	Генерация начальной популяции серых волков
4.	Оценка приспособленности каждого волка в популяции
5.	Цикл оптимизации
5.1.	Выбор альфа-волка (лучшего)
5.2.	Выбор бета-волка (второго лучшего)
5.3.	Выбор дельта-волка (третьего лучшего)
5.4.	Обновление позиций серых волков
5.5.	Оценка приспособленности новых позиций
5.6.	Обновление позиции альфа-волка
5.7.	Обновление позиций бета и гамма-волков
5.8.	Обновление параметров алгоритма (например, коэффициентов обновления)
5.9.	Проверка критерия остановки или достижения заданного числа итераций
6.	Конец

Результаты алгоритма:
Массив наилучших коэффициентов: [64., 0.84558199, 0.2660136, 0.17869458, 59.53132977, 0.82140753, 0.12719702, 0.10799177, 64., 0.652868, 0.25502293, 0., 45.35843488, 0.46322832, 0.1188171, 0.56635476, 0.31149802, 0.]
Точность: 
Epoch 1/5
1563/1563 [==============================] - 264s 167ms/step - loss: 1.2911 - accuracy: 0.5383
Epoch 2/5
1563/1563 [==============================] - 261s 167ms/step - loss: 0.8182 - accuracy: 0.7144
Epoch 3/5
1563/1563 [==============================] - 260s 166ms/step - loss: 0.6645 - accuracy: 0.7680
Epoch 4/5
1563/1563 [==============================] - 266s 170ms/step - loss: 0.5564 - accuracy: 0.8068
Epoch 5/5
1563/1563 [==============================] - 278s 178ms/step - loss: 0.4790 - accuracy: 0.8339
313/313 [==============================] - 15s 47ms/step - loss: 0.6422 - accuracy: 0.7858
Точность на тестовых данных: 0.7857999801635742
