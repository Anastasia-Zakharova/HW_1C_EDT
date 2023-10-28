# **Задание к занятию "1C:EDT"**

## _Задание 1._ **Установка EDT**

1. Консоль java version
   
![My scrin 1](http://dl3.joxi.net/drive/2023/10/26/0055/3282/3628242/42/a7dfa893e1.jpg)

2. Значения переменных сред

![My scrin 2](http://dl3.joxi.net/drive/2023/10/24/0055/3282/3628242/42/ae49e1a562.jpg)

3. Файл настроек

![My scrin 3](http://dl3.joxi.net/drive/2023/10/25/0055/3282/3628242/42/b976e9994f.jpg)

4. Рабочая область EDT

![My scrin 4](http://dl3.joxi.net/drive/2023/10/26/0055/3282/3628242/42/b6340e5091.jpg)

## _Задание 2._ **Анализ ошибок конфигурации**

1. Отбор ошибок по текущему объекту

![My scrin 5](http://dl4.joxi.net/drive/2023/10/27/0055/3282/3628242/42/221a028769.jpg)

2. Исправление ошибок по текущему объекту Документ "ДЗ_Доставка"
   
   _2.1 Модуль Менеджера Документа "ДЗ_Доставка"_
   
   2.1.1 **Ошибки** Переменные не определены [Толстый клиент]

   (то есть не определены Общие модули)

   ![My scrin 6](http://dl4.joxi.net/drive/2023/10/27/0055/3282/3628242/42/a58b40e2c3.jpg)

   Исправила путем добавления дополнительной проверки

   ![My scrin 7](http://dl3.joxi.net/drive/2023/10/27/0055/3282/3628242/42/9eafbd8f60.jpg)

   2.1.2 **Предупреждение** Используется не рекомендуемый метод

   Нужно заменить ТекущаяДата() на ТекущаяДатаСеанса()

   ![My scrin 8](http://dl3.joxi.net/drive/2023/10/27/0055/3282/3628242/42/3b347faf37.jpg)

   2.1.3 **Предупреждение** Отсутствует комментарий к экспортной процедуре "ДобавитьКомандыПечати"

   Нужно добавить комментарий. Но тут возникла масса сложностей:

   - Сначала ругался на параметры
   - Описала параметры, начал ругаться на типы параметров
   - Описала типы параметров, начал ругаться на тире и просил заменить на минус
   - В итоге перестал ругаться на комментарий, стал ругаться на Определение параметра
   - В результате так и не смогла самостоятельно решить эту проблему
   
   ![My scrin 9](http://dl3.joxi.net/drive/2023/10/28/0055/3282/3628242/42/4bf47c0c10.jpg)

   2.1.4 **Предупреждение** Отсутствует комментарий к экспортной процедуре "Печать"
   Нужно добавить комментарий. 
   Но тут возникла масса сложностей те же что и в пункте 2.1.3

   - Комментарий к процедуре взяла из БСП.
   - Опять долго мучалась, но тут ему Массив и СписокЗначений не нравяться. 
   - **Тип Коллекции должен содержать тип элемента коллекции**
   - Может дело в знаках ;. 
   - Пробую убирать их опять перестает ругать комментарий, но ругается на Определение параметра. 
   - В итоге опять замкнутый круг, а подсмотреть не получается.В Документе "ЗаказПокупателя" тоже нет комментариев к данным процедурам
   - И открыть проверку выдает пустоту
  
   ![My scrin 10](http://dl4.joxi.net/drive/2023/10/28/0055/3282/3628242/42/4fcbff384d.jpg)


   _2.2 Модуль Объекта Документа "ДЗ_Доставка"_

   **Ошибка** Переменная не определена [Толстый клиент]

   ![My scrin 11](http://dl3.joxi.net/drive/2023/10/28/0055/3282/3628242/42/7bca358635.jpg)

   Исправила путем добавления дополнительной проверки

   ![My scrin 12](http://dl4.joxi.net/drive/2023/10/28/0055/3282/3628242/42/4f93aeb200.jpg)

   _2.3 Модуль ФормыДокумента Документа "ДЗ_Доставка"_

   **Предупреждение** Область не стандартная для текущего типа модуля

   ![My scrin 13](http://dl4.joxi.net/drive/2023/10/28/0055/3282/3628242/42/031a2b3599.jpg)

   Исправила название области

   ![My scrin 14](http://dl3.joxi.net/drive/2023/10/28/0055/3282/3628242/42/b20fcc01eb.jpg)

   _2.4 Модуль ФормыСписка Документа "ДЗ_Доставка"_

   **Предупреждение** Область не стандартная для текущего типа модуля

   ![My scrin 15](http://dl4.joxi.net/drive/2023/10/28/0055/3282/3628242/42/a350158405.jpg)

   Исправила области

   ![My scrin 16](http://dl4.joxi.net/drive/2023/10/28/0055/3282/3628242/42/024c80a64e.jpg)

   _2.5 Основные Документ "ДЗ_Доставка"_

   **Предупреждение** Не заполнено представление объекта и списка

   ![My scrin 17](http://dl4.joxi.net/drive/2023/10/28/0055/3282/3628242/42/69cebc91fc.jpg)

   Заполнила представления

   
   В Итоге осталось три **Предупреждения** с Определениями Параметров
   
   ![My scrin 18](http://dl4.joxi.net/drive/2023/10/28/0055/3282/3628242/42/08397aeda8.jpg)

   _Пожалуйста, помогите мне с комментариями и описаниями параметров в данных процедурах._

   **Спасибо!**

   

