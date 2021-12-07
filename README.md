# cognitive-platform

## Краткое описание

Система видео аналитики, способная распознавать, сопровождать, классифицировать и предсказывать траектории движения до 200 объектов одновременно. Каждый объект снабжается своим уникальным id, который не теряется, когда одновременно движутся более 200 объектов. Система работает быстрее чем реальное время благодаря оболочке pytorch детектора объектов, способной использовать все имеющиеся видеокарты и работать в несколько потоков.

Детекция объектов происходит на базе YOLO darknet либо SSD, обученных на базе собственной разметки, использующей как реальные, так и синтетические данные. Синтетические данные формировались на базе 3D моделирования

Предсказание траектории происходит на базе LSTM. Классификация поведения объектов происходит на базе алгоритмов, использующих методы линейной алгебры. Индивидуальный дескриптор каждого объекта, позволяющий одновременно отслеживать много объектов в условиях их временного исчезновения или затемнения, строится на базе технологии triplet loss, реализованной в pytorch.
 
## Библиотеки

Модуль os – предоставляет множество функций для работы с операционной системой, причем их поведение, как правило, не зависит от ОС, поэтому программы остаются переносимыми. Здесь будут приведены наиболее часто используемые из них.

Numpy – библиотека с открытым исходным кодом для языка программирования Python. Возможности: поддержка многомерных массивов; поддержка высокоуровневых математических функций, предназначенных для работы с многомерными массивами

Модуль Random – предоставляет функции для генерации случайных чисел, букв, случайного выбора элементов последовательности.

Matplotlib – библиотека на языке программирования Python для визуализации данных двумерной (2D) графикой (3D графика также поддерживается). Получаемые изображения могут быть использованы в качестве иллюстраций в публикациях

SciPy – библиотека Python с открытым исходным кодом, предназначенная для решения научных и математических проблем. Она построена на базе NumPy и позволяет управлять данными, а также визуализировать их с помощью разных высокоуровневых команд.

Time – модуль для работы со временем в Python

Sklearn – библиотека машинного обучения для языка программирования Python.

PIL – библиотека языка Python, предназначенная для работы с растровой графикой

Torchvision – Библиотека для компьютерного зрения

PyTorch – фреймворк машинного обучения для языка Python с открытым исходным кодом, созданный на базе Torch. Используется для решения различных задач: компьютерное зрение, обработка естественного языка.