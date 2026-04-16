<div id="header" align="center">
  <h1>Проект «<span style='color:green'>Со Смыслом</span>» поиск по изображениям</h1>
</div>


## Описание проекта:

> Пользователи хостинга «<span style='color:green'>Со Смыслом</span>» размещают свои фотографии на хостинге и сопровождают их полным описанием: 
+ указывают место съёмок,
+ модель камеры и т. д.

> Отличительная особенность сервиса — описание: его может предоставить не только тот, кто размещает фотографию, но и другие пользователи портала.
> Отдел занимается экспериментом по разработке поиска референсных фотографий для фотографов. 
Суть поиска заключается в следующем: пользователь сервиса вводит описание нужной сцены.
Чтобы эксперимент получил право на жизнь, нужно защитить его перед руководителем компании. Для защиты необходимо презентовать так называемый PoC (Proof of Concept, Проверка концепции) — продемонстрировать, что такой проект практически осуществим. 
## Cтек технологий:
<img src="https://img.shields.io/badge/Scikit--Learn:_-1.6.1-purple">
<img src="https://img.shields.io/badge/Pandas:_-2.2.3-slategrey">
<img src="https://img.shields.io/badge/Python:_-3.13.0-greem">
<img src="https://img.shields.io/badge/FastAPI:_-0.119.0-green">
<img src="https://img.shields.io/badge/Uvicorn:_-0.37.0-red">
<img src="https://img.shields.io/badge/Poetry:_-2.0.0-blue">

## Как развернуть проект на локальной машине:


### 1. Клонируем проект:
```
git clone git@github.com:OsKaLis/fotohos.git
```
### 2. Переходим в директорию проекта:
```
cd fotohos/
```
### 3. Необходимо проверить установленную версию Python:
```
python3 -V
```
- Если у вас версия 3.13.*, то можно переходить к шагу 4.
- Если версия не 3.13.*, то необходимо её установить.
### 4. Устанвка `poetry`:
```
pip install poetry
```
- [Не большое руководство по `poetry`](https://habr.com/ru/articles/740376/)
### 5. Проверка что `poetry` установлен:
```
poetry -V
```
### 6. Запускаем виртуальное окружение из папки "fotohos":
``` 
poetry shell
```
### 7. Устанавливаем установка зависимости для окружения:
```
poetry install
```
### 8. Переходим в директорию проекта:
```
cd project_fastapi/
```
### 9. Запускаем проекта локально: 
```
poetry run uvicorn main:app --reload
```
### 10. Перейти по адресу
```
http://127.0.0.1:8000/
```

## Инструкция по работе с приложением
> 1. Запускаем приложение из папки (project_fastapi) - [ poetry run uvicorn main:app --reload ]
> 2. Перейти по адресу [ http://127.0.0.1:8000/ ]
> 3. Выбираем фаил в формате (*.csv) с полями:

| Порядковый № | Поле                                 | Значение |
|--------------|--------------------------------------|-------|
| 1            | Age                                  | Возраст |
| 2            | Cholesterol                         | Показатель холестерина |

> 4. Нажать кнопку [ Загрузить ]
> 5. Скачать готовый фаил с аброботкой результата 
> 6. Если есть ещё файлы для обработки нажать [ Новый запрос ]

## Демонстрация работы:
### Стартовая страница
![Стартовый интерфейс](https://github.com/OsKaLis/predictions_of_heart_attack_risk/blob/ca14cff9bca2ed58b81815d4caad905aaefa2490/project_fastapi/img/index.png)
### Выбор файла
![Выбор файла](https://github.com/OsKaLis/predictions_of_heart_attack_risk/blob/ca14cff9bca2ed58b81815d4caad905aaefa2490/project_fastapi/img/open_file.png)
### После нажатия на кнопру [Загрузить]
![Получение результата](https://github.com/OsKaLis/predictions_of_heart_attack_risk/blob/ca14cff9bca2ed58b81815d4caad905aaefa2490/project_fastapi/img/result.png)

## Сылка на документацию:
```
http://127.0.0.1:8000/docs
```
![Информация по эндпоинтам](https://github.com/OsKaLis/predictions_of_heart_attack_risk/blob/ca14cff9bca2ed58b81815d4caad905aaefa2490/project_fastapi/img/help.png)

## Автор: Юшко Ю.Ю.
