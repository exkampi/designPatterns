# The design patterns
## Overview

* Observer
    * Customized observer
    * Native Java observer
    * Swing observer
* Decorator
    - Customized decorator 
    - java.io
* Factory

__Архитектуры должны быть открытыми для расширения, но закрыты для изменения! Необходимо определить аспекты, которые будут изменяться, и отделить их от тех, которые останутся неизменными.__

## Observer
* Паттерн "Наблюдатель" определяет отношение один-ко-многим между объектами.
* Субъекты обновляют наблюдателей через единый интерфейс.
* Субъект ничего не знает о наблюдателях - кроме того, что они реализуют интерфейс Observer.
* При использовании паттерна возможен как запрос, так и активная доставка данных от субъекта(запрос считается более "правильным").
* Работа кода не должна зависеть от порядка оповещения наблюдателей.
* Java содержит несколько реализаций паттерна "Наблюдатель", включая обобщенную реализацию java.util.Observable.
* Встречается во многих других местах как Listener(JavaBeans, RMI и др.).

## Decorator
Динамически наделяет объект новыми возможностями и является гибкой альтернативой наследования в области расширения функциональности.

* Следует предусмотреть возможность расширения без изменения существующего кода.
* Композиция и делегирование часто используется для динамического добавления нового поведения.
* Типы декораторов соответствуют типам декорируемых компонентов(соответствие достигается путем наследования или реализации интерфейса).
* Декораторы изменяют поведение компонентов, добавляя новую функциональность до и (или) после (или даже вместо) вызовов методов компонентов.
* Компонент может декорироваться любым количеством декораторов.
* Декораторы обычно прозрачны для клиентов компонента (если клиентский код не зависит от конкретного типа компонента).

## Factory

