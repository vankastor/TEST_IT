# Test_it
ab test library for python

from ABTest import ABTest

# Чтобы использовать нашу библиотеку, необходимо импортировать ее и создать объект класса ABTest. Затем вызовите метод transform_data() для преобразования данных в соответствии с выбранной метрикой. После этого вызовите метод test(), передав необходимые параметры, включая уровень значимости и метод проведения теста. Вот пример кода, который показывает, как использовать библиотеку для проведения AB теста с метрикой "quantitative":

# Создаем объект класса ABTest, указывая путь к файлу и тип метрики
test = ABTest('test_data.csv', 'quantitative')

# Преобразовываем данные в соответствии с выбранной метрикой
test.transform_data()

# Проводим AB тест с уровнем значимости 0.05 и методом проведения теста 'two-sided'
test.test(alpha=0.05, alternative='two-sided')

# В результате выполнения этого кода мы получим сообщение о том, является ли изменение значимым или нет. Если изменение значимо, то можно сделать вывод о том, что тестирование было успешным и изменение имеет смысл внедрять в бизнес-процессы.
