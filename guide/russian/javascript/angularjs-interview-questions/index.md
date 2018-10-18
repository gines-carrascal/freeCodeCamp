---
title: Angularjs Interview Questions
localeTitle: Вопросы интервью Angularjs
---
# Вопросы интервью Angularjs

Вот список понятий, которые часто задают в интервью Angularjs.

*   Что такое AngularJS?
*   Что такое контроллер просмотра модели (MVC)?
*   Двусторонняя привязка данных
*   Что такое инъекция зависимости и как она работает?
*   Что такое $ scope в AngularJS?
*   Что такое $ rootScope в AngularJS?
*   Как реализовать маршрутизацию в угловом?
*   Объяснить директивы
*   Как мы можем создать настраиваемую директиву в Angular?
*   Объясните разницу между обслуживанием и фабрикой
*   Объясните услугу $ q, отложенные и обещания

# Примеры вопросов и ответов

Вопрос: Перечислите Директивы в AngularJS? Ответ: ngBind, ngModel, ngClass, ngApp, ngInit, ngRepeat

Вопрос: Что такое $ scope в AngularJS? Ответ: $ scope в AngularJS - это объект, который относится к модели приложения. Это объект, который связывает представление (элемент DOM) с контроллером. В контроллере доступ к данным модели осуществляется через объект $ scope. Как известно, AngularJS поддерживает шаблон MV \*, объект $ scope становится моделью MV \*.

Вопрос: Что такое SPA (одностраничное приложение) в AngularJS? Ответ. Приложения с одной страницей (SPA) - это веб-приложения, которые загружают одну страницу HTML и динамически обновляют эту страницу, когда пользователь взаимодействует с приложением. SPA используют AJAX и HTML для создания гибких и гибких веб-приложений без постоянной перезагрузки страницы. Однако это означает, что большая часть работы происходит на стороне клиента, в JavaScript. Одна страница HTML здесь означает страницу ответа UI с сервера. Источником могут быть ASP, ASP.NET, ASP.NET MVC, JSP и т. Д. Однако одностраничное веб-приложение поставляется в виде одной страницы в браузере и обычно не требует перезагрузки страницы, поскольку пользователь переходит к различным частям приложения. Это обеспечивает более быструю навигацию, более эффективные сетевые передачи и лучшую общую производительность для конечного пользователя.

Вопрос: Что такое маршрутизация в AngularJS? Ответ. Маршрутизация является основной функцией в AngularJS. Эта функция полезна при создании SPA (Single Page Application) с несколькими видами. В приложении SPA все представления представляют собой разные Html-файлы, и мы используем Routing для загрузки различных частей приложения, и полезно разделить приложение логически и сделать его управляемым. Другими словами, Routing помогает нам разделить наше приложение на логические представления и связать их с разными контроллерами.

Вопрос: Объясните директиву ng-repeat. Ответ. Директива ng-repeat является наиболее часто используемой и очень полезной функцией Directular. Он выполняет итерацию по набору элементов и создает элементы DOM. Он постоянно контролирует источник данных для повторной обработки шаблона в ответ на изменение.

Вопрос: В чем разница между ng-If и ng-show / ng-hide. Ответ: директива ng-If отображает только элемент DOM, если условие истинно. где ng-show / ng-hide директива визуализирует элемент DOM, но он изменяет класс ng-hide / ng-show, чтобы сохранить видимость элемента на странице.

Вопрос: Как вы отменяете тайм-аут с помощью AngularJs? Ответ: $ timeout - оболочка AngularJs для window.setTimeout, вы отменяете тайм-аут, применяя функцию:
```
$timeout.cancel(function (){ 
  // write your code. 
 }); 
```

Вопрос: Что такое инъекция зависимостей? Ответ: Dependency Injection (DI) - это шаблон разработки программного обеспечения, который касается того, как компоненты получают свои зависимости. Подсистема инжектора AngularJS отвечает за создание компонентов, разрешение их зависимостей и предоставление их другим компонентам по запросу.

Вопрос: Объясните директиву ng-App. Ответ. Директива ng-app запускает приложение AngularJS. Он определяет корневой элемент. Он автоматически инициализирует или загружает приложение, когда загружается веб-страница, содержащая приложение AngularJS. Он также используется для загрузки различных модулей AngularJS в приложении AngularJS.

Вопрос: Объясните директиву ng-init Ответ. Директива ng-init инициализирует данные приложения AngularJS. Он используется, чтобы поместить значения в переменные, которые будут использоваться в приложении. Например: В приведенном ниже примере мы инициализировали массив стран, используя синтаксис JSON для определения массива стран.

```html

<div ng-app = "" ng-init = "countries = [{locale:'en-US',name:'United States'}, {locale:'en-GB',name:'United Kingdom'}, {locale:'en-FR',name:'France'}]"> 
   ... 
 </div> 
```

Вопрос: Как вы делитесь данными между контроллерами? Ответ. Создайте службу AngularJS, которая будет хранить данные и вводить их внутри контроллеров. Использование сервиса - самый чистый, быстрый и простой способ тестирования. Однако есть несколько других способов реализации обмена данными между контроллерами, например: - Использование событий - Использование $ parent, nextSibling, controllerAs и т. Д. Для прямого доступа к контроллерам - Использование $ rootScope для добавления данных (не очень хорошая практика)

Вопрос: В чем разница между директивами ng-if и ng-show / hide? Ответ: ng-if будет создавать и отображать элемент DOM, когда его условие истинно, если условие ложно или изменяется на false, оно не создаст или не уничтожит созданный. ng-show / hide всегда будет генерировать элемент DOM, но он применит свойство отображения css, основанное на оценке состояния.

#### Дополнительная информация:

Здесь вы можете найти другие вопросы и ответы:

*   [Интервью с AngularJS](https://www.tutorialspoint.com/angularjs/angularjs_interview_questions.htm)
*   [10 Интервью с AngularJS](https://www.upwork.com/i/interview-questions/angularjs/)
*   [50 самых важных вопросов интервью AngularJS для 100% успеха](http://www.techbeamers.com/latest-angularjs-interview-questions-answers/)