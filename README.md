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
    name="data"           <!-- имя формы -->

    action="/"            <!-- ссылка на страницу скрипта обработчика -->
    method="post"         <!-- метод передачи данных -->
    
    enctype="text/plain"  <!-- метод кодирования данных -->
    accept-charset="UTF-8 <!-- кодировка -->
    
    autocomplete="off"    <!-- автозаполнение -->
    novalidate            <!-- отключение валидации -->    
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
        
        readonly="on"
        pattern="^[9-9]+$"
        
        placeholder=""
           
        autofocus="off"
        autocomplete="off"
        
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
