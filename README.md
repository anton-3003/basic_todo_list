# basic_todo_list
[![Travis][build-badge]][build]


[build-badge]: https://img.shields.io/travis/anton-3003/basic_todo_list/master.png?style=flat-square
[build]: https://travis-ci.org/anton-3003/basic_todo_list

Это небольшое приложение на Flask, которое представляет собой простйший todo-лист. 
Как начать: 
* склонировать этот репозиторий;
* перейти в папку с ним; 
* создать виртуальное окружение `python -m venv venv`;
* активировать его `source venv/bin/activate` (или `virtualenv venv`)
* установить зависимости `requirements pip install -r requirements.txt`;
* переменную окружения сделать равно текущей директории (текущую директорию можно узнать выполнив команду `pwd`) PYTHONPATH: `export PYTHONPATH=current_folder` (или `set PYTHONPATH=current_folder`)
* Запустить приложение можно с помощью команды `python app.py`. Оно запустится по адресу `http://127.0.0.1:5000/`
* У этого приложения есть следующие эндпоинты: 
  * GET: tasks: возвращает все существующие задачи;
  * GET: /tasks/<int:task_id>: возвращает задачу с заданным id; 
  * POST: /tasks/post: создает задачу. Принимает дату задачи (которая должна быть в будущем) и текст в параметрах запроса. 
  * Запустить тесты можно с помощью команды `pytest tests/test_pytest.py`
