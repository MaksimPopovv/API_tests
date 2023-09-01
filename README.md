# Проект курса [Тестирование ПО: Автоматизация и Программирование на Python. API](https://stepik.org/course/127716/promo#toc)

---

Проект по автоматизации тестирования API c логированием и созданием отчетов в Allure

## Структура проекта

- `tests/` - директория с тестами
- `utils/` - директория с методами для отправки и проверки запросов
- `logs/` - директория с логами (появляется после запуска тестов)
- `tests_results/` - директория с отчетами Allure (появляется после запуска тестов)

## Установка и настройка

1. Создайте виртуальное окружение:
   ```shell
   python -m venv venv && cd venv
   
2. Клонируйте репозиторий
   ```shell
   git clone https://github.com/MaksimPopovv/API_tests.git && cd API_tests

3. Установите зависимости из файла requirements.txt:
   ```shell
   pip install -r requirements.txt

4. Для запуска тестов используйте команду:
   ```shell
   python -m pytest -s -v
   
5. Для просмотра отчета в Allure:
   ```shell
   python -m pytest --alluredir=test_results/ tests/test_google_maps_api.py && allure serve test_results

