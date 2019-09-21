# radiation_meter_software
Radiation Meter Software

Приложение, созданное в рамках проекта [ESP Radiation Meter](https://github.com/avdeevsv91/esp_radiation_meter). Основная функция - уведомление пользователя при привышении заданных границ радиационного фона.

## Настройки

### Общее

***Язык интерфейса*** - русский или английский;

***Источник данных*** - COM порт или HTTP запрос;

***Минимальная точность данных*** - минимальное значение в процентах, при котором учитываются поступающие данные;

***Размер буфера данных*** - количество значений, отображаемых на графике;

***Сворачивать в системный трей*** - при сворачивании приложения оно прячется в системный трей;

***Отключить кнопку выхода*** - при нажатии на крестик окно будет сворачиваться, а не закрываться.

### COM порт

***Выберите COM порт*** - номер порта для подключения;

***Скорость*** - скорость порта;

***Биты данных*** - биты данных порта;

***Стоповые биты*** - стоповые биты порта;

***Четность*** - четность порта.

### HTTP запрос

***URL*** - адрес для запроса;

***GET/POST*** - метод запроса;

***POST данные*** - данные, посылаемые вместе с POST запросом;

***User-Agent*** - строка идентификации клиента;

***Интервал*** - время (в секундах) между запросами;

***Метод*** - метод обработки ответа от сервера;

***Точность/Радиация*** - выражение выделения значения, составленное по правилам выбранного метода обработки;

***Ед.изм.*** - единица измерения показаний радиационного фона.

    г.Воронеж (по данным Росатома)
    
    URL (GET): http://www.russianatom.ru/data_source/get_indications_by_id.php?id=34&terr_id=9&order=24  
    XML выражение (радиация): //response/archive/date[position() = last()]/@value  
    Ед.изм.: мкР/ч  

### Автозагрузка

***Запускать вместе с Windows*** - добавить программу в автозагрузку операционной системы;

***В свернутом виде*** - запускать в свернутом виде;

***В развернутом виде*** - запускать в максимальном размере окна;

***Подключаться автоматически*** - подключаться к выбранному источнику данных сразу после запуска.

### Допуски

***Повышенный уровень*** - уровень радиации, выше нормы, но не являющийся опасным;

***Опасный уровень*** - уровень радиации, при долгосрочном находжении в котором, способен причинить вред здоровью.

### Уведомления

***Голосовые оповещения*** - использовать голосовые оповещения при превышении значений допусков;

***Всплывающие сообщения*** - при превышении значений допусков показывать сообщения в системном трее.
