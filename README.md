# HTML 

- Структура документа
- Формы

## Структура документа

- `<!DOCTYPE>`
- `<html>`
- - `<base>`
- - <details>
    <summary>`<base>`</summary>

    1. First item must be preceeded with an empty line.
    2. Markdown renders **perfectly**.
    3. Extra item.

    </details>
- - `<meta>`
- - `<link>`
- - `<style>`
- - `<script>`
- - `<title>`
- `<body>`


### `<!DOCTYPE>`

Указывает браузеру тип документа

### `<html>`

Корневой элемент всего документа

### `<head>`

Может включать в себя теги:

`<base>`  
`<meta>`  
`<link>`  
`<style>`  
`<script>`  
`<title>`  

### `<base>`

Тег указывает, который будет подставляеться в начало всех относительных путей.

```html
    <base href=""> 
```

#### атрибуты:

```html
    <base
        href=""
        targer=""
    >
```

### `<meta>`

Мета-данные документа

#### атрибуты:

```html
    <meta
        charset="UTF-8" 
        
        http-equiv=""
        viewport="content=width=device-width, initial-scale=1.0"
        
        description="..."
        autor="..."
        name="keyword" content="qwerty, wasd, xwz"
    >
```

### `<link>`

Подгружает на страницу содержимое внешнего файла

```html
<link rel="stylesheet" href="main.css">
```

#### атрибуты:

```html
<link
    rel="stylesheet" <!-- указание на тип содержимого --> 
    
    href="main.css"  <!-- ссылка на внешний файл --> 
    
    sizes="25x25"    <!-- размер фавиконки -->
    
    media=""         <!-- аналог css директивы @media-->
>
```

### `<style>`

Задает глобальные стили прямо внутри html документа

```html
<style>
    .class {
        color: red;
    }
</style>
```

#### атриибуты:

```
    <style
        media=""
    >
    </style>
```

### `<script>`

Подключает внешниt скрипты к странице, а также позваляет писать программный код внутри тега

```html
<script type="text/javascript" src="main.js"></script>

<script type="text/javascript">
    console.log('hello world')
</script>
```

#### атрибуты:

```html
<script
    src="" <!-- путь к внешнему файлу-->
    
    type="" <!-- тип содержимого -->
    
    async="" <!-- загружает скрипт асинхронно с основной страницей -->
    
    defer="" <!-- загружает скрипт только после загрузки основной страницы -->
    
    language="javascript"
>
</script>
```

***

## Формы 

- тег `<form>`
- тег `<input>`
- теги `<option>, <select>, <optgroup> и <datalist>`
- теги `<fieldset> и <legend>`
- тег  `<label>`

### Тег **`<form>`**

Создает форму для заполнения и ее отправки на сервер

```html

<form name="data" novalidate>
    <input type="text" name="login">
    <br>
    <br>
    <input type="submit" value="send">
</form>
```

#### атрибуты

```html

<form
    name="data"            <!-- имя формы -->

    action="/"             <!-- ссылка на страницу скрипта обработчика -->
    method="post"          <!-- метод передачи данных -->
    
    enctype="text/plain"   <!-- метод кодирования данных -->
    accept-charset="UTF-8" <!-- кодировка -->
    
    autocomplete="off"     <!-- автозаполнение -->
    novalidate             <!-- отключение валидации -->    
>
</form>
```

### Тег **`<input>`**

создает поле ввода (текстовое или иное другое)

```html
<input type="text" name="login">
```

#### атрибуты

```html
    <input
        type=""
        
        name=""
        value=""
        
        form=""
        
        step=""
        min=""
        max=""
        minlength=""
        maxlength=""
        
        placeholder=""
        
        readonly="on"
          
        autofocus="off"
        autocomplete="off"
       
        pattern="^[9-9]+$"
       
        disabled
        required
    >    
```

#### Типы инпутов

#### текстовые 

```html
    <input type="text">
    <input type="email">
    <input type="search">
    <input type="password">
    <input type="number">
    <input type="tel">
    <input type="url">

```

#### кнопки 

```html
    <input type="button"> <!-- обычная кнопка -->
    <input type="submit"> <!-- отправка форы-->
    <input type="reset">  <!-- сброс всех данных в полях ввода-->
    <input type="image>   <!-- отправка изображения -->
```

#### элементы

```html
    <input type="checkbox"> 
    <input type="radio"> 
    <input type="range"> 
    <input type="color"> 
    <input type="file"> 
```

#### дата и время

```html
    <input type="date"> 
    <input type="time"> 
```

#### Теги **`<option>, <select> и <optgroup>`**

#### Тег **`<label>`**

используется для связи и создания подписи к полю ввода (input)

```html
<label for="login"> 
    login 
</label>
<input type="text" name="login">
```

## изображения

### `<img>`

Добавляет изображение на страницу

```html
<img src="/path/to/image" alt="описание">
```

#### атрибуты:  

```html
<img
    src="" <!-- путь к файлу-->    
    alt="" <!-- описание. отображается, если не загрузилась картинка -->    
    width=""  <!-- ширина изображения -->
    height="" <!-- высота изображения -->
    
    srcset=""
    sizes=""
    
    loading="lazy" <!-- начинает загрузку картинки, только в случае необходимости -->
    
    decoding="auto" <!-- режим декодирования изображения -->
>
```

### `<figure>` и `<figcaption>`

Используются для создания карточки изображения с подписью

```html
<figure>
    <img src="image.jpg" alt="img">
    
    <figcaption>
        Слон на фоне заката <!-- подпись к изображению -->
    </figcaption>
</figure>
```

### `<picture>`

Используется для подгрузки изображения в соответствии с устройством пользователя

```html
<picture>
    <source srcset="320.jpg" media="(max-width: 800px)">
    <img src="640.jpg" alt="Абстрактное изображение">
</picture>
```

## ссылки

### `<a>`

Добавляет ссылку на страницу 

```html
a href="path/to/page">нажми на меня</a>
```

### атрибуты:

```htnl
<a
    href="" <!-- адрес ссылки -->
    
    target="_self" <!--определяет где откроется новая сслыка (_blank) --> 
    
    download="" <!-- скачать содержимое ссылки-->
    
    title="" <-- отображает значение при наведении на ссылку -->
>
```

- структура документа
- `<!-DOCTYPE>`
- `<html>`
- `<head>`
    - `<base>`
    - `<meta>`
    - `<style>`
    - `<script>`
    - `<title>`
- `<body>`
    - <-- текст -->
    - `<h1>...<h6>` 
    - `<p>`
    - `<i>`
    - `<em>`
    - `<b>`
    - `<strong>`
    - `<small>`
    - `<sub>`
    - `<sup>`
    - `<mark>`
    - `<code>`
    - `<pre>`
    - `<br>`
    - `<hr>`
    - <-- ссылки -->
    - `<a>`
    - <-- списки -->
    - `<ul>` (`ol`)
        - `<li>`
    - `<dl>`
        - `<dt>`
        - `<dd>`
    - <-- форма -->
    - `<form>`
        - `<label>`
        - `<input>` (`<textarea>`)
        - `<button>`
        - `<select>` (`<datalist>`)
            - `<optgroup>`
                - `<option>`
        - `<fieldset>`
            - `<legend>`
    - <-- медиа -->
    - `<img>`
    - `<audio>`
    - `<video>`
    - `<embed>`
    - `<object>`
    - `<source>`
    - `<canvas>`
    - <-- разное -->
    - `<meter>`
    - `<output>`
    - `<progress>`
    - `<details>`
        - `<summary>`
    - <-- семантика -->
