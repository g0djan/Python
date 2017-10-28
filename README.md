# Тестирование сортировок
Версия 3.0
Автор Рылов Г.А. telegram: @g0djan
# Описание
C помощью данного проекта можно осуществить тестирование различных сортировок по таким параметрам как:
  * Время работы
  * Количество сравнений
  * Количество перестановок
# Требования
  * Python версии 3+ (3.6 подойдет - 146%)
  * numpy
  * scipy
  * matplotlib
# Состав
  * main.py - стартовый фал проекта
  * sorts_test.py - тестирование производительности
  * make_charts - построение графиков
  * array_generators - генерирование данных для тестирования
  * tests/- тестирование корректности сортировок
  * test_data/ - сгенерированные данные
  * sorts/ - тестируемые сортировки
  * results/ - данные полученные в ходе тестирования
  * Docs/ - картинки с построенными графиками и анализ результатов
# Запуск
  * Справка по запуску ./main.py --help
  * Пример запуска ./main.py 4097 2 20 descending ascending random
# О реализации
Все тестирование производительности и прочих ништяков осуществляется в sorts_test.py 
по сути умеет брать упакованные данные(с помошью pickle), распаковывать и запускать на них данные сортировки переданное в аргументах 
число раз, вернет результаты в виде среднего времени тестирования на этих данных и доверительный интервал
