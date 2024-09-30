# Document Object Model (DOM) в JavaScript

## Введение
Document Object Model (DOM) — это программный интерфейс для HTML и XML документов. Он представляет документ в виде дерева узлов, где каждый узел соответствует части документа.

## Основные концепции

### Дерево DOM
DOM представляет HTML документ как дерево узлов. Каждый элемент, атрибут и текст в документе является узлом.

### Узлы
- **Элементные узлы**: Представляют HTML теги.
- **Текстовые узлы**: Представляют текст внутри элементов.
- **Атрибутные узлы**: Представляют атрибуты элементов.

### Доступ к элементам
Для доступа к элементам DOM используются различные методы:
- `document.getElementById(id)`
- `document.getElementsByClassName(className)`
- `document.getElementsByTagName(tagName)`
- `document.querySelector(selector)`
- `document.querySelectorAll(selector)`

### Манипуляция элементами
С помощью DOM можно изменять структуру, стиль и содержание документа:
- **Создание элементов**: `document.createElement(tagName)`
- **Добавление элементов**: `parentNode.appendChild(node)`
- **Удаление элементов**: `parentNode.removeChild(node)`
- **Изменение атрибутов**: `element.setAttribute(name, value)`
- **Изменение стилей**: `element.style.property = value`

### События
DOM позволяет обрабатывать события, такие как клики, ввод текста и загрузка страницы:
- `element.addEventListener(event, function)`
- `element.removeEventListener(event, function)`

## Примеры кода

### Изменение текста элемента
```javascript
document.getElementById("myElement").innerText = "Новый текст";
let newElement = document.createElement("div");
newElement.innerText = "Привет, мир!";
document.body.appendChild(newElement);
document.getElementById("myButton").addEventListener("click", function() {
    alert("Кнопка нажата!");
});

```

