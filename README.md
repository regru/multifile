#[jQuery Multiple File Upload](http://www.fyneworks.com/jquery/multifile/)

##Fixes
- adds __Multifile.block__ object for main block carry
- adds __Multifile.errors__ object for errors, contains DOM
- __multiple="multiple"__ attribute fix (disappear on input original change)
- BEM classes naming
- restore default __.submit()__ event handler for forms
- __.disableEmpty()__ strongly changed
- adds __.reset()__ method to Multifile object
- adds russian language for basic messages
- adds showError/removeError methods


##Options

```js
multifileName: 'b-file'     // Custom DOM elements name prefix
                            // also className for entire plugin DOM-block
```

DOM will be:
```jade
b-file
  b-file__list
    b-file__list-item
    b-file__list-item
  b-file__wrap
```

```js
wrapper: '.className' // specify wrapper className instead of generating DOM
```
```js
lang: 'en' || 'ru'  // messages language

// and extend it with your own
STRING: {
    ru: {
        remove: 'x',
        denied: 'Нельзя выбрать $ext файл.',
        file: '$file',
        selected: 'Файл выбран: $file',
        duplicate: 'Этот файл уже выбран:\n$file',
        toomuch: 'Общий размер файлов выше допустимого ($size)',
        toolittle: 'Слишком маленький размер файлов ($size)',
        toomany: 'Максимальное кол-во файлов: $max',
        toofew: 'Минимальное кол-во файлов: $max',
        toobig: 'Превышен размер файла ($size)',
        toosmall: 'Слишком маленький размер файла ($size)'
    }
}
```

```js
showErrors: true // append errors in html, false - calls 'error' function
```

