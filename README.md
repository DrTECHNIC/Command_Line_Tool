# **Задание №2**
Разработать инструмент командной строки для визуализации графа зависимостей, включая транзитивные зависимости. Сторонние средства для получения зависимостей использовать нельзя.

Зависимости определяются для **git-репозитория**. Для описания графа зависимостей используется представление **PlantUML**. Визуализатор должен выводить результат на экран в виде графического изображения графа.

Построить граф зависимостей для коммитов, в узлах которого находятся списки файлов и папок.

Конфигурационный файл имеет формат csv и содержит:
- Путь к программе для визуализации графов.
- Путь к анализируемому репозиторию.

Все функции визуализатора зависимостей должны быть покрыты тестами.
# Установка
Перед началом работы с программой требуется скачать репозиторий и необходимые библиотеки.

Клонирование репозитория:
```Bash
git clone https://github.com/DrTECHNIC/Command_Line_Tool
```
Скачивание библиотеки pillow:
```Bash
pip install pillow
```
Скачивание библиотеки pytest:
```Bash
pip install -U pytest
```
# Запуск
Перед запуском необходимо прописать путь к анализируемому репозиторию в файле [config.csv](https://github.com/DrTECHNIC/Command_Line_Tool/blob/main/config.csv).

Запуск [main.py](https://github.com/DrTECHNIC/Command_Line_Tool/blob/main/main.py):
```Bash
py main.py
```
Запуск [test.py](https://github.com/DrTECHNIC/Command_Line_Tool/blob/main/test.py):
```Bash
pytest -v test.py
```
# Тесты
## Зависимости [первого репозитория](https://github.com/kriru/firstJava), взятого для теста:
![](https://github.com/DrTECHNIC/Command_Line_Tool/blob/main/test_1.png)
## Зависимости [второго репозитория](https://github.com/iam-veeramalla/write_your_first_terraform_project), взятого для теста:
![](https://github.com/DrTECHNIC/Command_Line_Tool/blob/main/test_2.png)
## Зависимости [третьего репозитория](https://github.com/AceLewis/my_first_calculator.py), взятого для теста:
![](https://github.com/DrTECHNIC/Command_Line_Tool/blob/main/test_3.png)
## Общие тесты
![](https://github.com/DrTECHNIC/Command_Line_Tool/blob/main/pytest.png)
