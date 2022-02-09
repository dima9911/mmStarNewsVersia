# Инструкция для подключения виджета Старметрики

 1. Поместите где нужно в `body` тег `div` с каким либо айди. Например `block1`
```
<body>
...
  <div id="block1"></div>
...
</body>
```
2. Подключите скрипт Старметрики и инициализацию виджета перед закрывающимся тегом `body`
#### divID - сюда нужно указать атрибут `id` тега `div`, куда нужно установить виджет `(шаг 1)`
```
<html>
  <body>
    ...
    <div id="block1"></div>
    ...
    <script src="//starmetrics.ru/widget/mmStarNewsWidget.js"></script>
    <script>
      const Widget1 = new mmStarWidget({
          divID: 'block1'
      });
    </script>
  </body>
</html>
```

3. _(* необязательно)_ Виджетов можно установить несколько. Для этого нужно разместить несколько тегов `div` с разными `id`
#### divID должен быть уникален
```
<html>
  <body>
    ...
    <div id="block1"></div>
    ...
    <div id="block2"></div>
    ...
    <div id="block3"></div>
    ...
    <script src="//starmetrics.ru/widget/mmStarNewsWidget_VERSIA.js"></script>
    <script>
      const Widget1 = new mmStarWidget({
          divID: 'block1'
      });
      const Widget2 = new mmStarWidget({
          divID: 'block2'
      });
      const Widget3 = new mmStarWidget({
          divID: 'block3'
      });
    </script>
  </body>
</html>
```

# Финальный вид виджета
<img width="851" alt="Снимок экрана 2022-02-09 в 12 39 47" src="https://user-images.githubusercontent.com/10125278/153143882-ce869ed2-0a55-47a3-a4d4-68aac8ae1d9e.png">

