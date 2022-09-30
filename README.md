# Color System Converter
>Назначение проекта – создать приложение, позволяющее получать численные представления цветов в различных цветовых пространствах и поддерживать связь этих значений при изменении любой из цветовых компонент в любом из пространств.

>Для создания приложения был использован фреймворк Qt и язык C++.

>Для отображения и взаимодействия с пользователем был написан абстрактный класс colorSystem, который включает в себя переменное число полей ввода, а также слайдер для плавного изменения значений поля. От этого класса были снаследованы такие классы, как RGBSystem, CMYKSystem, …, LABSystem, обеспечивающие полный функционал требуемой цветовой системы. 

>Для контроля взаимодействия цветовых систем был написан класс colorSystemController, обеспечивающий корректное изменение значений всех цветовых систем при изменении любого из полей произвольной системы.

>Главным средством перевода значений из одной системы в другую является класс QColor, являющийся частью Qt. Были написаны дополнительные функции для поддержки систем XYZ и LAB fromRGBtoXYZ и fromXYZtoLAB. 
