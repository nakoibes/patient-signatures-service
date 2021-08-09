# Rest-api, позволяющее искать и получать информацио о сигнатурах пациента



## Основные сущности

### Patient

Пациент имеет имя и сигнатуры

### Signature

Сигнатура имеет имя и значение

## Основные API методы

Методы обрабатывают HTTP GET запросы.

Документация находится по адресу http://127.0.0.1:8000/docs

### Получить значения выбранных сигнатур данного пациента

### Получить значения всех сигнатур данного пациента

![image](https://user-images.githubusercontent.com/81371413/128726174-608bd83a-a6ee-4f66-b157-f9d3cc0ea2a7.png)


### Получить среднее значение данный сигнатуры по всем пациентам

![image](https://user-images.githubusercontent.com/81371413/128725834-27635d71-6547-45ad-968f-5ab91a89678b.png)


## Установка через Docker<br>
* Клонируем проект
```bash
sudo docker-compose up -d
```

Доступно по адресу http://127.0.0.1:8000/



## Установка без Docker<br>
* Клонируем проект
* Создаем виртуальное окружение 
```bash
python -m venv venv
```
* Активируем виртуальное окружение
```bash
source venv/bin/activate
```
* Устанавливаем зависимости из requirements.txt
```bash
pip install -r requirements.txt
```
* Запускаем http сервер командой
```bash
uvicorn main:app
```



