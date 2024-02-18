**Single Responsibility Principle** или **Принцип единственной ответственности.** Он был реализован в **controller**, а именно:

*Контроллер для бинарного калькулятора **BinaryController.**
Контроллер для калькулятора списков **ListController.***

*Контроллер приложения **AppController.*** 

**Open Closed Principle** или **Принцип открытости/закрытости.**

*Он был реализован в **model.***

**Liskov Substitution Principle** или **Принцип подстановки Барбары Лисков.**

*Он был реализован в **model** и применен к классу **ListCalculator**, так как он у нас является наследуемым от **Calculator**, но методы **sum**(сумма) **product**(умножение) и **div**(деление), возвращают у нас тот же тип **Double***.

**Interface Segregation Principle** или **Принцип разделения интерфейса**.

Был реализован для **model**, а именно разделение **Calculator** на следующие элементы :

*Общее свойство **iCalculator***.

*Интерфейс реализующий бинарный калькулятор **iBinaryCalculator***.

*Интерфейс реализующий калькулятор списков **iListCalculator***.

**Dependency Inversion Principle** или **Принцип инверсии зависимостей.**

*Был использован в **controller** для **Binarycontroller** и **ListController**, так как они не зависят от конкретных реализаций модели. В свою очередь класс **AppController** не зависит от конкретных реализаций **Binarycontroller** и *ListController***

Группа 5450. Малютин Иван