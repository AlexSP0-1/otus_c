# Комментарий
В проекте использована система сборки Make
- `make` - сборка программы вресии debug
- `make BUILDTYPE=release` - сборка версии release, таким же образом можно модифицировать последующие команды

Артефакты хранятся в папке __bin/debug__ или __bin/release__   

# Задание
Написать программу, подсчитывающую контрольную сумму CRC32 (не Adler32) для файлов, превышающих
по объёму оперативную память без многократного вызова read. Сторонние библиотеки не использовать.

