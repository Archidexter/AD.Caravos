# AD.Caravos

Оживляет NPC в **Fallout: New Vegas**, **Tale of Two Wastelands** и **Fallout 4** — установщик и менеджер ИИ-диалогов. Для New Vegas и Tale of Two Wastelands — на базе мода **[Numen](https://mod.pub/falloutnv/408-numen-ai-npcs-for-fnv)**, для Fallout 4 — на базе **Mantella** в нашей сборке из открытых исходников.

## Установка

1. Скачайте `AD.Caravos.zip` из раздела **[Releases](https://github.com/Archidexter/AD.Caravos/releases/latest)**.
2. ПКМ по архиву → **Свойства** → внизу поставьте галочку **«Разблокировать»** → **ОК** *(Windows помечает скачанные файлы — это убирает лишние предупреждения системы)*.
3. Распакуйте в любую папку и запустите **`AD.Caravos.exe`**.
4. Дальше — по инструкции внутри лаунчера. Лаунчер обновляется сам.

## Что нужно

**Fallout: New Vegas 1.4.0.525** — Steam или GOG. Epic и Microsoft Store не подойдут: там не работает xNVSE.

**Fallout 4** — Steam или GOG. Игра новее 1.10.163 откатывается первым шагом установки: заплатку отката вы скачиваете со страницы её авторов, лаунчер открывает её сам и подхватывает файл из «Загрузок».

**Mod Organizer 2**, расширитель скриптов (xNVSE или F4SE) и 4GB-патч для New Vegas лаунчер ставит сам, рядом с игрой. Оригинальные файлы игры не трогаются. Часть модов приходится скачивать вручную — лаунчер открывает нужные страницы и подхватывает архивы из «Загрузок».

Реплики NPC пишет нейросеть — на выбор облачная или своя. Для облачной нужен ключ к любому OpenAI-совместимому провайдеру, он вводится в самом лаунчере. Своя работает на этом же компьютере через Ollama: ни ключа, ни интернета.

## Обе игры одним персонажем

Лаунчер собирает **Tale of Two Wastelands** — Fallout 3 на движке New Vegas, обе игры одним персонажем. Он проверяет, что обе игры и все их дополнения на месте и на английском языке, готовит папку, показывает, что вписать в окна сборщика, дожидается конца работы и подключает готовую сборку как обычную. ИИ-диалоги встают в неё так же, как в чистый Нью-Вегас.

Ни сами игры, ни сборщик лаунчер не раздаёт: нужны ваши лицензионные копии, а сборщик скачивается со страницы его авторов.

## Голоса

**Ответы нейросети** озвучиваются на вашем компьютере, без ключей и без интернета: **Piper** — русские голоса на процессоре, в обеих играх; **OmniTTS** и **XTTS** — локальные серверы на видеокарте; в New Vegas есть ещё клонирование — оно снимает собственный голос каждого NPC с его же ванильных реплик. Облачный голос Inworld тоже поддерживается — там нужен ключ.

**Обычные реплики игры** — те, что записаны актёрами, — включаются по-русски переключателем «Озвучка NPC» в каждой игре: русскую озвучку лаунчер скачивает по ссылкам её авторов. В Tale of Two Wastelands русской может быть одна половина мира из двух: обе озвучки кладут голоса в одни и те же папки.

**Микрофон**: говорить с NPC можно вслух. В New Vegas русская и английская модели распознавания ставятся вместе с остальными компонентами; в Fallout 4 речь распознаёт сама программа нейромода — свободно или пока удерживаете клавишу.

## Русская версия игры

Работает. New Vegas хранит текст в кодовой странице Windows-1251 — лаунчер поднимает у себя мост, который перекодирует запросы и ответы, поэтому **во время игры лаунчер должен быть открыт**. В Fallout 4 нейромод говорит по-русски сам; русский текст мода и русские имена персонажей ставит лаунчер, а открытым его держит только озвучка: все движки, кроме Piper, звучат через него.

**Писать NPC можно по-русски.** Движок New Vegas читает клавиатуру напрямую через DirectInput и раскладку Windows не видит — поэтому раскладку в поле ввода даёт плагин, который лаунчер ставит в игру. Ответы NPC в обеих играх приходят по-русски.

## Лицензия

© 2026 Archidexter. Все права защищены. Программа распространяется автором на Boosty — по подписке или при покупке поста. Передача другим людям, публикация, продажа, выдача за своё и изменённые версии — только с письменного разрешения автора. Полные условия — в файле [LICENSE.txt](LICENSE.txt). Моды и модели, которые лаунчер скачивает (Numen, Mantella, Tale of Two Wastelands, xNVSE, F4SE, JIP LN NVSE, озвучки, голоса и модели распознавания речи и прочее), не входят в программу и остаются под собственными лицензиями.

Автор и единственный правообладатель — **Archidexter**.

---

> Brings the NPCs in **Fallout: New Vegas**, **Tale of Two Wastelands** and **Fallout 4** to life — an installer and manager for AI dialogue: the [Numen](https://mod.pub/falloutnv/408-numen-ai-npcs-for-fnv) mod on New Vegas and Tale of Two Wastelands, our own build of Mantella on Fallout 4. Needs Fallout: New Vegas 1.4.0.525 (Steam or GOG) and/or Fallout 4 (Steam or GOG; a newer game is rolled back to 1.10.163 as the first install step). Mod Organizer 2, the script extender and the 4GB patch (New Vegas) are set up for you. NPC lines are written either by a cloud provider (any OpenAI-compatible key, entered in the launcher) or by a model on your own PC through Ollama — no key, no internet. Voices are local too: Piper, OmniTTS, XTTS, and on New Vegas the cloning of each NPC's own vanilla voice.
>
> It also builds **Tale of Two Wastelands** — Fallout 3 on the New Vegas engine, both games with one character — from your own licensed copies and the authors' own installer, then connects the result as an ordinary build.
>
> Download `AD.Caravos.zip` from Releases, right-click → Properties → **Unblock**, unzip, run `AD.Caravos.exe`. Self-updating.
>
> © 2026 Archidexter, all rights reserved. Distributed by the author on Boosty; see [LICENSE.txt](LICENSE.txt).
