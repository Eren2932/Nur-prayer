# Передача Nur 0.42.0 (versionCode 88)

Готовый исходный архив: `Nur-prayer_0.42.0.zip`, 25,570,199 байт, 821 файлов. SHA-256: `a5eab48ebf12479578b81062ada9ab9fdfffd83ee9d33d1cbb71f6486e9ec16c`.

Для продолжения в этой беседе достаточно распаковать **этот ZIP** и открыть вложенную папку `Nur-prayer`. Это уже полный проект с правками; накладывать WIP повторно не нужно. Если нужен новый диалог, перенесите туда ZIP либо загрузите его в репозиторий. В GitHub из этой беседы ничего не публиковалось.

Резервный путь: `Nur-prayer_0.41.1.zip` → поверх папки `Nur-prayer` скопировать содержимое `nur-0.42.0-wip` (кроме самого журнала). Содержимое исходного ZIP сверено с Git blob 9ca07f438e3a316f79ec7e1f3a85f2c591f605f9 в дереве cbdfb065154c3da20c1b8ee66d0686a4ccf77d13. Все 37 изменённых или добавленных файлов проверены побайтно между финальным ZIP, рабочим деревом и сохранённым WIP. Файлы предыдущей версии не удалялись.

**Сделано:** сетка по референсу 852 × 1846; общее матовое покрытие и согласованные скругления; имена без содержимого, вирд и два независимых входа в азкары; личный прогресс салавата; история дня; перекрашенный, но не растянутый таймер; общий нижний ряд с выходом и неактивным многоточием. Подробности в `CHANGELOG-0.42.0.md` внутри архива.

**Проверки:** все 27 команд `tools/package_source.py` прошли. Финальный ZIP повторно прочитан из файлов беседы, CRC проверен. Шесть векторных ресурсов разобраны как XML, новые подписи проверены в каталогах четырёх дополнительных языков. Не запускались компиляция Android, lint, JVM-тесты и эмулятор; визуальное совпадение на телефоне не подтверждено. Следующий шаг — штатный CI и проверка по чек-листу в changelog.

## Файлы поверх базы

- `CHANGELOG-0.42.0.md`
- `app/build.gradle.kts`
- `app/src/androidTest/java/com/nur/prayer/DeedsUiTest.kt`
- `app/src/main/assets/i18n/ar.tsv`
- `app/src/main/assets/i18n/en.tsv`
- `app/src/main/assets/i18n/tr.tsv`
- `app/src/main/assets/i18n/uz.tsv`
- `app/src/main/java/com/nur/prayer/ui/NurNavigator.kt`
- `app/src/main/java/com/nur/prayer/ui/NurRoot.kt`
- `app/src/main/java/com/nur/prayer/ui/components/ExitButton.kt`
- `app/src/main/java/com/nur/prayer/ui/daily/DailyScreens.kt`
- `app/src/main/java/com/nur/prayer/ui/home/PrayerSheet.kt`
- `app/src/main/java/com/nur/prayer/ui/learn/LessonScreen.kt`
- `app/src/main/java/com/nur/prayer/ui/schedule/DaySheet.kt`
- `app/src/main/java/com/nur/prayer/ui/schedule/ScheduleScreen.kt`
- `app/src/main/java/com/nur/prayer/ui/settings/CityPickerScreen.kt`
- `app/src/main/java/com/nur/prayer/ui/settings/SettingsScreen.kt`
- `app/src/main/java/com/nur/prayer/ui/shell/Frost.kt`
- `app/src/main/java/com/nur/prayer/ui/shell/NavCapsule.kt`
- `app/src/main/java/com/nur/prayer/ui/shell/ShellRoutes.kt`
- `app/src/main/java/com/nur/prayer/ui/today/DeedMaterial.kt`
- `app/src/main/java/com/nur/prayer/ui/today/SalawatGoal.kt`
- `app/src/main/java/com/nur/prayer/ui/today/TodayScreen.kt`
- `app/src/main/java/com/nur/prayer/ui/wallpaper/WallpaperGallery.kt`
- `app/src/main/java/com/nur/prayer/ui/wallpaper/WallpaperImages.kt`
- `app/src/main/res/drawable/deed_allah.xml`
- `app/src/main/res/drawable/deed_bars.xml`
- `app/src/main/res/drawable/deed_clock.xml`
- `app/src/main/res/drawable/deed_moon.xml`
- `app/src/main/res/drawable/deed_star.xml`
- `app/src/main/res/drawable/deed_sun.xml`
- `app/src/test/java/com/nur/prayer/DeedsTest.kt`
- `app/src/test/java/com/nur/prayer/ShellMathTest.kt`
- `tools/i18n_src/ar.json`
- `tools/i18n_src/en.json`
- `tools/i18n_src/tr.json`
- `tools/i18n_src/uz.json`
