# AD.Caravos

Оживляет NPC в **Fallout: New Vegas** и в **Tale of Two Wastelands** — установщик и менеджер ИИ-диалогов на базе мода **[Numen](https://mod.pub/falloutnv/408-numen-ai-npcs-for-fnv)**.

## Установка

1. Скачайте `AD.Caravos.zip` из раздела **[Releases](https://github.com/Archidexter/AD.Caravos/releases/latest)**.
2. ПКМ по архиву → **Свойства** → внизу поставьте галочку **«Разблокировать»** → **ОК** *(Windows помечает скачанные файлы — это убирает лишние предупреждения системы)*.
3. Распакуйте в любую папку и запустите **`AD.Caravos.exe`**.
4. Дальше — по инструкции внутри лаунчера. Лаунчер обновляется сам.

## Что нужно

**Fallout: New Vegas 1.4.0.525** — Steam или GOG. Epic и Microsoft Store не подойдут: там не работает xNVSE.

**Mod Organizer 2**, **xNVSE** и **4GB-патч** лаунчер ставит сам, рядом с игрой. Оригинальные файлы игры не трогаются. Часть модов приходится скачивать вручную — лаунчер открывает нужные страницы и подхватывает архивы из «Загрузок».

Реплики NPC пишет нейросеть — на выбор облачная или своя. Для облачной нужен ключ к любому OpenAI-совместимому провайдеру, он вводится в самом лаунчере. Своя работает на этом же компьютере через Ollama: ни ключа, ни интернета.

## Обе игры одним персонажем

Лаунчер собирает **Tale of Two Wastelands** — Fallout 3 на движке New Vegas, обе игры одним персонажем. Он проверяет, что обе игры и все их дополнения на месте и на английском языке, готовит папку, показывает, что вписать в окна сборщика, дожидается конца работы и подключает готовую сборку как обычную. ИИ-диалоги встают в неё так же, как в чистый Нью-Вегас.

Ни сами игры, ни сборщик лаунчер не раздаёт: нужны ваши лицензионные копии, а сборщик скачивается со страницы его авторов.

## Голоса

**Ответы нейросети** озвучиваются на вашем компьютере, без ключей и без интернета: клонирование — снимает собственный голос каждого NPC с его же ванильных реплик; **Piper** — русские голоса на процессоре; **OmniTTS** и **XTTS** — локальные серверы на видеокарте. Облачные голоса (Inworld, ElevenLabs) тоже поддерживаются — там нужен ключ.

**Обычные реплики игры** — те, что записаны актёрами, — включаются по-русски переключателем «Озвучка NPC». В Tale of Two Wastelands русской может быть одна половина мира из двух: обе озвучки кладут голоса в одни и те же папки.

**Микрофон**: говорить с NPC можно вслух, русская и английская модели распознавания ставятся вместе с остальными компонентами.

## Русская версия игры

Работает. Fallout хранит текст в кодовой странице Windows-1251 — лаунчер поднимает у себя мост, который перекодирует запросы и ответы, поэтому **во время игры лаунчер должен быть открыт**.

**Писать NPC можно по-русски.** Движок читает клавиатуру напрямую через DirectInput и раскладку Windows не видит — поэтому раскладку в поле ввода даёт плагин, который лаунчер ставит в игру. Ответы NPC тоже приходят по-русски.

## Лицензия

© 2026 Archidexter. Все права защищены. Программа распространяется автором на Boosty — по подписке или при покупке поста. Передача другим людям, публикация, продажа, выдача за своё и изменённые версии — только с письменного разрешения автора. Полные условия — в файле [LICENSE.txt](LICENSE.txt). Моды и модели, которые лаунчер скачивает (Numen, Tale of Two Wastelands, xNVSE, JIP LN NVSE, голоса и модели распознавания речи и прочее), не входят в программу и остаются под собственными лицензиями.

Автор и единственный правообладатель — **Archidexter**.

---

> Brings the NPCs in **Fallout: New Vegas** and **Tale of Two Wastelands** to life — an installer and manager for the [Numen](https://mod.pub/falloutnv/408-numen-ai-npcs-for-fnv) AI-dialogue mod. Needs Fallout: New Vegas 1.4.0.525 (Steam or GOG); Mod Organizer 2, xNVSE and the 4GB patch are set up for you. NPC lines are written either by a cloud provider (any OpenAI-compatible key, entered in the launcher) or by a model on your own PC through Ollama — no key, no internet. Voices are local too: cloning of each NPC's own vanilla voice, Piper, OmniTTS, XTTS.
>
> It also builds **Tale of Two Wastelands** — Fallout 3 on the New Vegas engine, both games with one character — from your own licensed copies and the authors' own installer, then connects the result as an ordinary build.
>
> Download `AD.Caravos.zip` from Releases, right-click → Properties → **Unblock**, unzip, run `AD.Caravos.exe`. Self-updating.
>
> © 2026 Archidexter, all rights reserved. Distributed by the author on Boosty; see [LICENSE.txt](LICENSE.txt).
