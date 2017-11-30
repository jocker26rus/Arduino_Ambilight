[![AlexGyver YouTube](http://alexgyver.ru/git_banner.jpg)](https://www.youtube.com/channel/UCgtAOyEQdAyjvm9ATCi_Aig?sub_confirmation=1)
# Arduino_Ambilight
Динамическая фоновая подсветка для монитора компьютера с адаптивной яркостью
Подробности в видео: https://youtu.be/tx5GxvFgkh0

## Папки

- **Библиотеки** - библиотеки для дисплея и прочего, скопировать в  
`C:\Program Files (x86)\Arduino\libraries\` (Windows x64)  
`C:\Program Files\Arduino\libraries\` (Windows x86)
- **Gyver_Ambilight** - прошивка для Arduino, файл в папке открыть в Arduino IDE (читай FAQ)
- **Schemes** - папка со схемами подключения
- **Test pictures** - папка с ядрёными радугами для теста подсветки

## Схема подключения
![СХЕМА](https://github.com/AlexGyver/Arduino_Ambilight/blob/master/Schemes/pc.jpg)

##  Материалы и компоненты
Если товар закончился, то почти всё указанное ниже можно найти здесь http://alexgyver.ru/arduino_shop/ или здесь http://alexgyver.ru/electronics/

* Arduino NANO http://ali.pub/1sun6b
* Лента http://ali.pub/1sun73
* БЕЗПАЕЧНЫЕ УГЛОВЫЕ СОЕДИНИТЕЛЯ ДЛЯ ЛЕНТЫ!!! http://ali.pub/22lb00
* Мощный БП http://ali.pub/1sunn8  http://ali.pub/1sun82  http://ali.pub/1sunol
* Фоторезисторы http://ali.pub/1suna7
* Резисторы ЧипДип 10 кОм https://www.chipdip.ru/product0/41486
* Резисторы ЧипДип 300 Ом https://www.chipdip.ru/product0/29794

## Вам скорее всего пригодится
* Всё для пайки (паяльники и примочки) http://alexgyver.ru/all-for-soldering/
* Недорогие инструменты http://alexgyver.ru/my_instruments/
* Все существующие модули и сенсоры Arduino http://alexgyver.ru/arduino_shop/
* Электронные компоненты http://alexgyver.ru/electronics/
* Аккумуляторы и зарядные модули http://alexgyver.ru/18650/

## Как запустить и настроить
* Загрузка прошивки http://alexgyver.ru/arduino-first/
* Установить ambiBox, настроить по видео

## Настройки в коде
    #define NUM_LEDS 98          // число светодиодов в ленте
    #define DI_PIN 13            // пин, к которому подключена лента
    
    #define start_flashes 0      // проверка цветов при запуске (1 - включить, 0 - выключить)
    
    #define auto_bright 0        // автоматическая подстройка яркости от уровня внешнего освещения (1 - включить, 0 - выключить)
    #define max_bright 255       // максимальная яркость (0 - 255)
    #define min_bright 50        // минимальная яркость (0 - 255)
    #define bright_constant 500  // константа усиления от внешнего света (0 - 1023)
    // чем МЕНЬШЕ константа, тем "резче" будет прибавляться яркость

##  FAQ
### Основные вопросы
В: Как скачать с этого грёбаного сайта?  
О: На главной странице проекта (где ты читаешь этот текст) вверху справа зелёная кнопка **Clone or download**, вот её жми, там будет **Download ZIP**

В: Скачался какой то файл .zip, куда его теперь?
О: Это архив. Можно открыть стандартными средствами Windows, но думаю у всех на компьютере установлен WinRAR, архив нужно правой кнопкой и извлечь.

В: Я совсем новичок! Что мне делать с Ардуиной, где взять все программы?  
О: Читай и смотри видос http://alexgyver.ru/arduino-first/

В: Компьютер никак не реагирует на подключение Ардуины!  
О: Возможно у тебя зарядный USB кабель, а нужен именно data-кабель, по которому можно данные передавать

В: Ошибка! Скетч не компилируется!  
О: Путь к скетчу не должен содержать кириллицу. Положи его в корень диска.

В: Сколько стоит?  
О: Ничего не продаю.

### Вопросы по этому проекту

