# HTML5 tags

#### Семантическая вёрстка

Семантическая вёрстка — подход к разметке, который опирается не на содержание сайта, а на смысловое предназначение каждого блока и логическую структуру документа.&#x20;

#### Как разметить страницу с точки зрения семантики

1. Крупные смысловые блоки на каждой странице сайта: `<header>, <main>, <footer>`
2. Крупные смысловые разделы в блоках: `<nav>, <section>, <article>, <aside>`
3. Заголовок всего документа и заголовки смысловых разделов: `<h1>-<h6>`
4. Мелкие элементы в смысловых разделах: списки, таблицы, параграфы и переносы, формы, цитаты, контактная информация и прогресс.
5. Фразовые элементы: изображения, ссылки, кнопки, видео, время и мелкие текстовые элементы.

#### Зачем это нужно

* чтобы соответствовать спецификации HTML
* чтобы поднять сайт в поисковиках
* чтобы сделать доступным для скринридеров

#### Семантика HTML5 на уровне структуры страницы

* `<header>` предназначен для создания «шапок» — всего сайта или какой-то части контента, например, статьи.
* `<footer>` обозначает нижнюю часть страницы или блока — «подвал». Обычно здесь находятся контакты, ссылки на разделы сайта, копирайт.
* `<nav>` задает навигацию по сайту. В контейнер `<nav>` помещаются основные ссылки, по которым пользователь сможет быстро перейти на нужный раздел сайта.
* `<main>` обозначает главное содержимое страницы, которое больше нигде не повторяется на сайте.
* `<article>` обозначает законченный и самодостаточный раздел документа, описывающий какую-то сущность: статью, товар, карточку пользователя и т. д.
* `<section>` смысловой раздел документа. Как правило, но не всегда, разделы имеют заголовок. Неотделяемый, в отличие от `<article>`.
* `<aside>` размечает блок с дополнительным содержимым. В этот тег оборачивается контент, не обязательный для понимания основной информации на сайте: виджеты с оценкой, поиск по сайту, список тем и рубрик.

#### Семантика HTML5 на уровне текста

* `<em>` определяет текст, на который сделан особый акцент, меняющий смысл предложения.
* `<strong>` указывает на важность отмеченного текста. Он может использоваться для выделения предупреждений или части документа, которую пользователь должен увидеть раньше остального. При этом обозначение части текста тегом `<strong>` не должно изменять смысла предложения.
* `<mark>`  ****  представляет текст, выделенный в справочных целях из-за своей актуальности в определённом контексте. Например, он может быть использован на странице с результатом поиска, в которой выделяется каждый экземпляр искомого слова.
* `<time>` служит для разметки дат, времени или периода времени: в содержимое тега идёт формат для человека, а в атрибут `datetime` версия для машин.
* `<details>` используется для хранения дополнительной информации, которую можно скрыть или показать по требованию пользователя. По умолчанию содержимое тега не отображается, для изменения статуса применяется атрибут `open`.  Первый дочерний элемент `<details>` — `<summary>`, который определяет содержание дополнительной информации, используется в качестве метки для виджета раскрытия.

#### Теги HTML5 описывающие новые технологии

* `audio` добавляет, воспроизводит и управляет настройками аудиозаписи на веб-странице.
* `video` добавляет, воспроизводит и управляет настройками видеоролика на веб-странице.
* `source` вставляет звуковой или видеофайл для тегов `audio` и `video`.
* `canvas` создает область, в которой при помощи JavaScript можно рисовать разные объекты, выводить изображения, трансформировать их и менять свойства. При помощи тега можно создавать рисунки, анимацию, игры и др.
