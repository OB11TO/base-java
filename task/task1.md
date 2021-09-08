##TASK 1
- Реализуйте методы `save, get, delete, clear, getAll, size` в классе `ru.ob11to.basejava.storage.ArrayStorage`, организовав хранение резюме в массиве 
- Храните все резюме в начале `ru.ob11to.basejava.storage` (без пустот в виде `null`), чтобы не перебирать каждый раз все 10_000 элементов
- При реализации метода `delete` учитывайте, что после удаления резюме между оставшимися резюме не должно быть пустых ячеек, заполненных null
```
Схема хранения резюме в массиве ru.ob11to.basejava.storage (в элементах от 0 до size-1 отсутствуют null):

r1, r2, r3,..., rn, null, null,..., null
<----- size ----->
<------- ru.ob11to.basejava.storage.length (10000) ------->
```
- Проверьте вашу реализацию с помощью классов `ru.ob11to.basejava.MainArray.main()` и `ru.ob11to.basejava.MainTestArrayStorage.main()`

### Замечания
1. Все резюме в хранилище имеют уникальный `uuid`, что исключает повторы.  Сортировка по `uuid` не требуется
1. Давайте осмысленные комментарии коммитам
1. Перед каждым коммитом не забывайте пользоваться сочетанием клавиш `Ctrl + Alt + L` (автоматическое форматирование кода)
1. Удаляйте в классах неиспользуемые импорты (`Ctrl + Alt + O`)
1. Не игнорируй подсказки IDEA (подсвечивает)
1. В методе `clear()` обнуление массива предполагает обнуление (null) ячеек, где хранятся ru.ob11to.basejava.model.Resume, а не создание нового или присваивание ему null
1. При реализации методов не используйте коллекции
1. Не меняйте сигнатуры методов в `ru.ob11to.basejava.storage.ArrayStorage`
1. Не добавляйте в `ru.ob11to.basejava.model.Resume` новые поля
1. ru.ob11to.basejava.model.Resume r — давайте переменным осмысленные имена, например resume. r допустимо в коротких циклах и лямбда-выражениях
