## Формы 

### Тег **`<form>`**

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
                                                    
### Тег **`<inpup>`**

```html
    <input
        type=""
        
        name=""
        value=""
        
        form=""
        
        step=""
        min=""
        max=""
        
        placeholder=""
        
        readonly="on"
        
        autofocus="off"
        autocomplete="off"
        
        pattern="^[9-9]+$"
        
        disabled
        required
    >    
```

Типы инпутов можно поделить на несколько групп:

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
