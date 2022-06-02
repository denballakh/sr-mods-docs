Про интерфейс
=============

Интерфейс полностью задается разделом `ML` мейна. Интерфейс имеет иерархическую структуру.
Каждый блок в `ML.` - это форма [кастомные формы тут же?]. Форма содержит в себе множество различных блоков, вложенных друг в друга.

[см. про строки и числа]

Параметры, общие для нескольких типов элементов:
- `Name` - название элемента, по этому названию к элементу можно обращаться из скрипта

- `Pos` - позиция элемента относительно родительского
    `X,Y[,Z]`
- `Size` - размер элемента
    `X,Y`
- `AlignX` - выравнивание элемента по горизонтали
    `Center|Left|Right`
- `AlignY` - выравнивание элемента по вертикали
    `CenterEx|Top|Bottom`
- `PosZ` - Z-координата элемента
    `Z`
- `Active` - активен ли элемент при начале игры
    `True|False`
- `PosAutoCorrection` - корректировка позиции при разных разрешениях
    `True|False`
- `PosAutoCorrectionXCoef` - коррекция координаты при больших размерах экрана. Дополнительный сдвиг вычисляется по формуле: `([горизонтальное разрешение] - 1024) * PosAutoCorrectionXCoef`
- `PosAutoCorrectionYCoef` - `([вертикальное разрешение] - 768) * PosAutoCorrectionYCoef`
    число

- `Font` - шрифт
    путь к шрифту
- `Style` - стиль
    путь к стилю
- `TextColor` - цвет текста
    `R,G,B`

- `Help` - путь к разделу ланга, где лежит текст подсказки
    `Help.LabelMoney` (пример)
- `MVUpdate`
    `True|False`
- `MouseBlocking` - блокировка взаимодействия с элементами под этим элементом
    `True|False`
- `MoveWorld`
    `True|False`
- `Sme`
    `X,Y`



Названия элементов и список их параметров:
Все разделы с кастомными именами
- `Border` - аналог Pos и Size
    `X1,Y1,X2,Y2`


`Panel` - может содержать другие элементы
- `Name`
- `Pos`
- `Size`
- `Active`
- `MVUpdate`
- `MouseBlocking`
- `MoveWorld`


`Image` - изображение
- `Name`
- `Pos`
- `Size`
- `Active`
- `Help`
- `PosZ`
- `Sme`

- `Auto`
    `Pos,Size | Size`
- `KindX` - выравнивание по горизонтали
    `Center|Left|Right|LeftFill|RightFill`
- `KindY` - выравнивание по вертикали
    `Center|Top|Bottom|TopFill`
- `Image` - изображение
    `GI,<путь к параметру в кешдате>`


`GraphButton` - кнопка
- `Name`
- `Pos`
- `Size`
- `Font`
- `Help`
- `MouseBlocking`
- `Style`

- `MouseBlockingTest`
    `True|False`
- `OnPressCode` - код, исполняемый при левом щелчке мышью по объекту
- `OnMouseRightClick` - код, исполняемый при правом щелчке мышью по объекту
- `OnMouseEnterCode` - код, исполняемый при наведении наведении курсора на объект
- `OnMouseLeaveCode` - код, исполняемый при уводе курсора с объекта
- `Caption` - путь к тексту кнопки (или сам текст?)
- `CaptionColorDisable` - цвет текста
- `CaptionColorDisableA` - цвет текста
- `CaptionColorDown` - цвет текста
- `CaptionColorNormal` - цвет текста
- `CaptionColorNormalA` - цвет текста
    `R,G,B`
- `CaptionSme`
    `X1,Y1,X2,Y2`
- `ImageDisable` - выключенная кнопка
- `ImageDown` - нажатая кнопка
- `ImageNormal` - обычная кнопка
- `ImageNormalA` - обычная кнопка при наведенном курсоре
    `GI,<путь к параметру в кешдате>`
- `Kind`
    `Normal|Disable|FixDisable`
- `KindHit`
    `Rect|Graph`
- `UpOnlyDown`
    `True|False`


`Label` - текст
- `Name`
- `Pos`
- `Size`
- `AlignX`
- `AlignY`
- `Font`
- `Style`
- `TextColor`

- `Text` - текст или путь к тексту
- `TextBorder` - толщина обводки текста
- `TextShadow` - толщина тени текста
    число
- `TextBorderColor` - цвет обводки текста
- `TextShadowColor` - цвет тени текста
    `R,G,B`
- `WordWrap` - перенос по словам
    `True|False`


`Edit` - поле ввода
- `Name`
- `Pos`
- `Size`
- `AlignX`
- `Font`
- `Help`
- `TextColor`

- `MaxLen` - максимальная длина строки
    число
- `ReturnFocusLeave` - сбрасывает фокус при нажатии Enter
    `True|False`
