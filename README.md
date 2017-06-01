# Front-End сборка
Что внутри
<ul>
  <li>Bootstrap 4 grid</li>
  <li>Gulp</li>
  <li>Минификатор картинок</li>
  <li>Спрайт генератор</li>
  <li>библиотека миксинов bourbon.io</li>
</ul>

# Установка
Перед началалом роботы - установим все пакеты и зависимости

```bash
npm i
```

также поставим gulp =) :
```bash
npm i gulp -g
```

# Начало работы


Для запуска сборки:
```bash
gulp
```

# Для запуска спрайт-генератор:

сначала ложим наши спрайты(иконки etc.) в папку:

```bash
./img/spite/
```

после чего пишем:
```bash
gulp sprite
```
спрайты доступны как миксины в - sprite.scss

после чего для подключения спрайта, в scss пишем, @include sprite($'название спрайта') -- например @include sprite($facebook)

# SVG спрайт генератор:

сначала ложим наши спрайты(иконки etc.) в папку:

```bash
./img/svg/
```

после чего пишем:
```bash
gulp svg
```

и готово, для того что б вставить svg в html, достаточно написать команду для вызова pug миксина(в папке templates проверяем что б были подключены миксины)

```bash
+icon(*название иконки с папки*)
```



# Проект запускается на локальном сервере:

```bash
localhost:1337
```

# Пакеты которые есть в проекте

```json
"devDependencies": {
  "gulp": "^3.9.1",
  "gulp-autoprefixer": "^3.1.0",
  "gulp-clean": "^0.3.2",
  "gulp-concat": "^2.6.0",
  "gulp-connect": "^4.1.0",
  "gulp-file-include": "^0.13.7",
  "gulp-newer": "^1.2.0",
  "gulp-plumber": "^1.1.0",
  "gulp-postcss": "^6.1.1",
  "gulp-replace": "^0.5.4",
  "gulp-sass": "^2.3.2",
  "gulp-sourcemaps": "^1.6.0",
  "gulp-uglify": "^1.5.3",
  "gulp-watch": "^4.3.8",
  "gulp.spritesmith": "^6.2.1",
  "node-bourbon": "^4.2.8"
},
"dependencies": {
  "bourbon": "^4.2.7"
}
```
