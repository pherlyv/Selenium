# Selenium

## Поиск элементов с помощью CSS-селекторов [Список](https://wp-kama.ru/id_5875/30-css-selektorov.html#css-selektory "Список всех селекторов")


|Селектор| Пример | Описание примера  |
|:-:|:-:|:-:|
| `*` | `*`  | Все элементы |
| `#id` |  `#firstname` | Элемент с `id="firstname"`  |
|  `.class` |  `.intro` | Все элементы с `class="intro"`  |
|  `.class1.class2` |  `.name1.name2` | Все элементы с `class="name1 name2"`  |
|  `.class1 .class2` |  `.name1 .name2` | Все элементы с `class="name2"` у <br> которых родитель с `class="name1"`  |
|  `tag` |  `p` | 	Все `<p>` элементы  |
|  `tag.class` |  `p.intro` | Все `<p>` элементы с class="intro"  |
|  `tag, tag` |  `div, p` | Все `<div>` и все `<p>` элементы  |
|  `tag tag` |  `div p` | Все `<p>` внутри всех `<div>`  |
|  `tag > tag` |  `div > p` | Все `<p>` прямой родитель которых `<div>`  |
|  `tag + tag` |  `div + p` | `<p>` который находятся сразу после `<div>`  |
|  `tag ~ tag` |  `div ~ p` | Все `<p>` которые находятся после `<div>`  |
|  `[attribute]` |  `[target]` | Все элементы с `target="что-либо"`  |
|  `[attribute = value]` |  `[target=_blank]` | Все элементы с `target="_blank"`  |`
|  `[attribute ^= value]` |  `a[href^="https"]` | 	Каждый `<a>` атрибут `href` которого начинается с `"https"`  |
|  `[attribute $= value]` |  `a[href$=".pdf"]` | Каждый `<a>` атрибут `href` которого заканчивается `".pdf"`  |
|  `[attribute *= value]` |  `a[href*="w3schools"]` | Каждый `<a>` атрибут `href` которого <br> содержит подстроку `"w3schools"`  |
|  `[attribute ~= value]` |  `[title~=flower]` | Все элементы в атрибуте `title` которых есть слово `"flower"` |
|  `:active` |  `a:active` | 		Активная ссылка  |
|  `::after` |  `p::after` | 	Вставляет псевод-элемент в начале каждого `<p>` элемента  |
|  `::before` |  `p::before` | 		Вставляет псевод-элемент в конце каждого `<p>` элемента  |
|  `:checked` |  `input:checked` | 	Все выбранные `<input type="checkbox">` элементы  |
|  `:default` |  `input:default` | 	Все `<input>` элементы  |
|  `:disabled` |  `input:disabled` | 	Все `<input disabled>` элементы  |
|  `:empty` |  `p:empty` | 	Все пустые `<p>`, в которых нет пробелов, <br> текста или других элементов  |
|  `:enabled` |  `input:enabled` | 	Все активные (не disabled) элементы `<input>`  |
|  `:first-child` |  `p:first-child	` | Первый элемент в списке родительского элемента |
|  `:first-of-type` |  `p:first-of-type` | 	Первый `<p>` элемент в списке родительского элемента  |
|  `::first-letter` |  `p::first-letter` | 	Первая буква каждого `<p>` элемента  |
|  `::first-line` |  `p::first-line` | 	Первая линия каждого `<p>` элемента  |
|  `:focus` |  `input:focus` | 	`<input>` в котором находится курсор  |
|  `:focus-visible` |  `a:focus-visible` | Фокус сработает, только если на кнопку <br> перешли с клавиатуры через TAB  |
|  `:focus-within` |  `div:focus-within` | Сработает на блоке, когда его <br> внутренний элемент находится в фокусе  |
|  `:hover` |  `a:hover` | 	Сслыка на которую наведена мышка.  |
|  `:in-range` |  `	input:in-range` | 	Все `<input>` со значением в пределах <br> указанного в min/max диапазона  |
|  `:out-of-range` |  `input:out-of-range` | 	Все `<input>` со значением за пределами <br> указанного в min/max диапазона  |
|  `:indeterminate` |  `input:indeterminate` | 	Все `<input>` в статусе indeterminate  |
|  `:invalid` |  `input:invalid` | 	Все `<input>` с недопустимым значением  |
|  `:lang(language)` |  `p:lang(it)` | 	Все `<p>` с `lang="it"`  |
|  `:last-child` |  `p:last-child` | 	Последний элемент в списке родительского элемента  |
|  `:last-of-type` |  `	p:last-of-type ` | 	Последний `<p>` в списке родительского элемента  |
|  `:link` |  `a:link` | 	Все непосещенные ссылки  |
|  `:not(selector)` |  `:not(p)` | 	Все не `<p>` элементы  |
|  `:not(:only-child)` |  `div:not(:only-child)` | 	Все `<div>` внутри которых больше одного элемента  |
|  `:nth-child(n)` |  `p:nth-child(2)` | 	Второй элемент в списке родительского элемента  |
|  `:nth-of-type(n)` |  `p:nth-of-type(2)` | 	Второй `<p>` в списке родительского элемента  |
|  `:nth-last-child(n)` |  `p:nth-last-child(2)` | 	Второй элемент в списке родительского <br> элемента (счет идет с конца)  |
|  `:nth-last-of-type(n)` |  `p:nth-last-of-type(2)` | 	Второй `<p>` в списке родительского <br> элемента (счет идет с конца)  |
|  `:only-child` |  `p:only-child` | 	Единственный `<p>` у родителя <br> (других элементов быть не может)  |
|  `:only-of-type` |  `p:only-of-type` | 	Один `<p>` у родителя (других элементы могут быть)  |
|  `:optional` |  `	input:optional` | 	Все `<input>` у которых нет артибута `"required"`  |
|  `:required` |  `input:required` | 	Все `<input>` у которых указан атрибут `"required"`  |
|  `:out-of-range` |  `input:out-of-range` | 	Все `<input>` со значением выходящим за указанный рэндж  |
|  `::placeholder	` |  `input::placeholder` | 	Все `<input>` у которых указан атрибут `"placeholder"`  |
|  `:read-only` |  `input:read-only` | Все `<input>` у которых указан атрибут `"readonly"`  |
|  `:read-write` |  `input:read-write` | Все `<input>` у которых не указан атрибут `"readonly"`  |
|  `:root` |  `:root` | Корень документа  |
|  `::selection` |  `::selection` | Выберет текущее выделение текста мышкой  |
|  `:target` |  `#news:target` | Выберет элемент с `id="news"` когда к нему пришил по клику |
|  `:valid` |  `iinput:valid` | Все `<input>` с валидным значением  |
|  `:valid` |  `a:visited` | Все посещенные ссылки  |
