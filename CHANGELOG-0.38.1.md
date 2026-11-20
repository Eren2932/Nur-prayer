# Нур 0.38.1

versionCode 82. Исправление сборки 0.38.0 (упала на `:app:compileDebugAndroidTestKotlin`). Функциональность и вид не менялись.

## Что упало

`ObservatoryScreenTest.theMiddleButtonIsAtTheCentreAndTheOthersStandEvenlyFromIt` читал `DpRect.width` / `DpRect.height`
(результат `getBoundsInRoot()`). Это не члены класса, а extension-свойства `androidx.compose.ui.unit`, и без их импорта
компилятор отвечает `Unresolved reference 'width'` / `'height'` (5 ошибок, строки 201–207). `compileDebugKotlin`,
`compileReleaseKotlin` и `compileDebugUnitTestKotlin` в том прогоне прошли.

## Что сделано

- `ObservatoryScreenTest`: ширина и высота считаются как `right - left` и `bottom - top` (`DpRect` импортирован), без extension-свойств.
- `ShellBarTest`: допуск проверки альфы блика равен 1/255. sRGB-цвет хранит альфу в 8 битах, 0.75 возвращается как 0.7490 (раньше запас был ~2·10⁻⁵).
- `tools/check_extension_imports.py`: новое правило. Файл, который читает `DpRect` / `getBoundsInRoot()`, и обращается к `.width` / `.height`
  без импорта, не проходит проверку (проверено на файле из 0.38.0: ловит обе ошибки).
- Версия 0.38.1, versionCode 82: по versionCode CI однозначно берёт именно этот архив, а не 0.38.0.

Android-компиляция, юнит-тесты, lint и эмуляторные тесты по-прежнему запускаются только в CI.
