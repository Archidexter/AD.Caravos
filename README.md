# AD.Caravos

Оживляет NPC в **Fallout: New Vegas** — установщик и менеджер ИИ-диалогов на базе мода **[Numen](https://mod.pub/falloutnv/408-numen-ai-npcs-for-fnv)**.

## Установка

1. Скачайте `AD.Caravos.zip` из раздела **[Releases](https://github.com/Archidexter/AD.Caravos/releases/latest)**.
2. ПКМ по архиву → **Свойства** → внизу поставьте галочку **«Разблокировать»** → **ОК** *(Windows помечает скачанные файлы — это убирает лишние предупреждения системы)*.
3. Распакуйте в любую папку и запустите **`AD.Caravos.exe`**.
4. Дальше — по инструкции внутри лаунчера. Лаунчер обновляется сам.

## Что нужно

**Fallout: New Vegas 1.4.0.525** — Steam или GOG. Epic и Microsoft Store не подойдут: там не работает xNVSE.

**Mod Organizer 2**, **xNVSE** и **4GB-патч** лаунчер ставит сам, рядом с игрой. Оригинальные файлы игры не трогаются. Часть модов приходится скачивать вручную — лаунчер открывает нужные страницы и подхватывает архивы из «Загрузок».

Нужен ключ к любому OpenAI-совместимому провайдеру: это модель, которая пишет реплики NPC. Ключ вводится в самом лаунчере.

## Русская версия игры

Работает. Fallout хранит текст в кодовой странице Windows-1251 — лаунчер поднимает у себя мост, который перекодирует запросы и ответы, поэтому **во время игры лаунчер должен быть открыт**.

Печатать в игре можно только латиницей: движок читает клавиатуру напрямую через DirectInput и раскладку Windows не видит — переключать её в игре нечем. Зато можно **говорить**: лаунчер ставит русскую модель распознавания речи одной кнопкой.

## Лицензия

© 2026 Archidexter. Все права защищены. Программа распространяется автором на Boosty — по подписке или при покупке поста. Передача другим людям, публикация, продажа, выдача за своё и изменённые версии — только с письменного разрешения автора. Полные условия — в файле [LICENSE.txt](LICENSE.txt). Моды, которые лаунчер скачивает (Numen, xNVSE, JIP LN NVSE и прочие), не входят в программу и остаются под собственными лицензиями.

Автор и единственный правообладатель — **Archidexter**.

---

> Brings the NPCs in Fallout: New Vegas to life — an installer and manager for the [Numen](https://mod.pub/falloutnv/408-numen-ai-npcs-for-fnv) AI-dialogue mod. Needs Fallout: New Vegas 1.4.0.525 (Steam or GOG) and a key for any OpenAI-compatible provider; Mod Organizer 2, xNVSE and the 4GB patch are set up for you.
>
> Download `AD.Caravos.zip` from Releases, right-click → Properties → **Unblock**, unzip, run `AD.Caravos.exe`. Self-updating.
>
> © 2026 Archidexter, all rights reserved. Distributed by the author on Boosty; see [LICENSE.txt](LICENSE.txt).
