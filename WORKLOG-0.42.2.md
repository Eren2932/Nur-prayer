# Передача Nur 0.42.2 (90)

База — полный Nur-prayer_0.42.1.zip из файлов беседы (SHA-256 c490aab5a3936563cb12476adbb82e440c99952cf8005bcb7832632af2a90f4f).

Готово. Использовать полный Nur-prayer_0.42.2.zip из файлов этой беседы, а не собирать версию из патчей. Новый макет: file_00000000957482098bc3d1814737c7c8.png, 841 × 1870 px. Решения по геометрии и цвету, сценарии проверки — в CHANGELOG-0.42.2.md внутри ZIP. Прошли 27 прежних команд плюс проверка контраста, всего 28. Код Android и инструментальные тесты не компилировались и на устройстве не выполнялись. Никаких изменений в GitHub не отправляли.

Сверка ZIP после чтения из файлов беседы: Verified 827 entries; 13 changed; 25578923 bytes; sha256 7d9352add033f78e449ba908df13edadb78c19b52c308e33675454c313d2524b. Для аварийного восстановления: распаковать 0.42.1 и наложить содержимое nur-0.42.2-wip, кроме WORKLOG-0.42.2.md.

Изменённые файлы:
- `CHANGELOG-0.42.2.md`
- `app/build.gradle.kts`
- `app/src/androidTest/java/com/nur/prayer/DeedsUiTest.kt`
- `app/src/androidTest/java/com/nur/prayer/WindowWashTest.kt`
- `app/src/main/java/com/nur/prayer/ui/NurRoot.kt`
- `app/src/main/java/com/nur/prayer/ui/settings/SettingsScreen.kt`
- `app/src/main/java/com/nur/prayer/ui/shell/NavCapsule.kt`
- `app/src/main/java/com/nur/prayer/ui/theme/SystemBarsTone.kt`
- `app/src/main/java/com/nur/prayer/ui/today/DeedMaterial.kt`
- `app/src/main/java/com/nur/prayer/ui/today/TodayScreen.kt`
- `app/src/main/java/com/nur/prayer/ui/wallpaper/DeedsWindowWash.kt`
- `tools/check_window_light.py`
- `tools/package_source.py`
