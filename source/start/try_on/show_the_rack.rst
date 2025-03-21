Show the rack
+++++++++++++++

Ранее мы научились создавать *new objects* в kuwaiba, в том числе размещать 
телекоммуникационные шкафы на различных энергетических объектах и добавлять в них
оборудование. 
Но можем ли мы увидеть, как выглядит шкаф с оборудованием, который мы установили?

Да, можем!

Какие данные необходимо учитывать, чтобы kuwaiba правильно отобразила вид шкафа?
--------------------------------------------------------------------------------

 Необходимо соблюдение трех условий:

1. Для стойки (шкафа) должно быть установлено допустимое целое числовое значение 
   атрибута **rackUnits** (к примеру, 42U').

2. Атрибут **rackUnitsNumberingDescending** должен существовать среди полей в 
   свойствах стойки (шкафа) и иметь 2 варианта значений: ``true`` и ``false``.
   Этот атрибут указывает на порядок возрастания (если **false**) или убывания
   (если **true**).

3. Атрибуты **rackUnits** и **position** должны быть заполнены и иметь целое 
   значение, отличное от 0. 
   Атрибут **position** означает номер юнита, на котором стоит оборудование в 
   стойке, **rackUnits** - сколько юнитов занимает. Как правило, производитель
   указывает количество юнитов.

Как посмотреть вид шкафа с оборудованием?
------------------------------------------

Для отображения стойки (шкафа) в вертикальном разрезе (вид сбоку) необходимо
встать на строку объекта **Rack**, открыть **Views** в свойствах, затем щелкнуть
на ``Rack View``. 

Если все было заполнено правильно для всего оборудования внутри шкафа, программа
отобразит следующий вид (пример):

.. image:: /res/try_on/rack_view.PNG

