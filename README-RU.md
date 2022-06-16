# hoi4geoparser

Используется для создания отдельных карт местности на основе данных hoi4. Первоначально написано malashin.

### Языки:
- [English](https://github.com/ICodeMaster/hoi4geoparser/blob/master/README.md)
- [Русский](https://github.com/ICodeMaster/hoi4geoparser/blob/master/README-RU.md)

### Установка и использование hoi4geoparser
- Скачать готовые билды со [страницы GitHub релизов](https://github.com/ICodeMaster/hoi4geoparser/releases)
- Запустите Geoparser один раз, чтобы сгенерировать конфигурационный файл.
- Отредактируйте файл конфигурации (указать путь к моду или игре, и т.д настройки)
- Запустите hoi4geoparser и введите данные карты для создания при появлении запроса.

### Добавление сгенерированных файлов для пользовательских режимов карты в вашем моде:
- Скопируйте файлы из мода в свой мод
- Перетащите папки внутри mod_path (найденные в каталоге инструмента) в свой путь к моду. Вот и все!

### Информация
`global.states` -> Все регионы в функции карты.
`find_color_graph = yes` -> Создает цвета страны, чтобы ни у кого из соседей не было общего цвета.
`set_state_flag = mapmode_state_hashed_visible` -> Состояние имеет хэшированную текстуру.
`set_state_flag = mapmode_state_visible` -> Состояние имеет видимую нормальную текстуру.
`state_frame_number_hashed` -> Рамка (Цвет) для текстуры хэшированного состояния.
`state_frame_number` -> Рамка (Цвет) для текстуры нормального состояния.
`calculate_country_center_point_quick_all = yes` -> Найти приблизительную центральную точку каждой страны.
`set_country_flag = mapmode_shield_visible` -> Отобразить щит для каждой страны.
`set_country_flag = mapmode_shield_use_capital` -> Использовать для отображения щита регион, где располагается столица страны вместо центральной точки.
`set_state_flag = info_text_visible` -> Показать информационный текст.

____
Переведено [sepera_okeq](https://github.com/Sepera-okeq).

Проект распространяется под лицензией MIT, подробнее читайте в файле [ЛИЦЕНЗИЯ](https://github.com/ICodeMaster/hoi4geoparser/blob/master/LICENSE)
