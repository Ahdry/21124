# 21124
домашнее задание  Распаковка позиционных параметров 2024

# 1. Функция с параметрами по умолчанию
def print_params(a=1, b='строка', c=True):
    print(a, b, c)

# Вызовы функции с разным количеством аргументов
print_params()  # Выводит: 1 строка True
print_params(10)  # Выводит: 10 строка True
print_params(b=25)  # Выводит: 1 25 True
print_params(c=[1, 2, 3])  # Выводит: 1 строка [1, 2, 3]

# 2. Распаковка параметров
values_list = [3.14, 'пример', False]
values_dict = {'a': 42, 'b': 'слово', 'c': None}

# Передаем список и словарь в функцию
print_params(*values_list)  # Выводит: 3.14 пример False
print_params(**values_dict)  # Выводит: 42 слово None

# 3. Распаковка + отдельные параметры
values_list_2 = [54.32, 'Строка']
print_params(*values_list_2, 42)  # Выводит: 54.32 Строка 42

