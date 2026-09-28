<div align="center">

<img src="icon.png" width="64" height="64" alt="Voice Helper for Claude">

# Voice Helper for Claude

**Управляйте Claude голосом — без клавиатуры и мыши.**
Скажите «Клод», продиктуйте задачу — помощник сам включит диктовку, отправит сообщение и выключит микрофон.

[![Последняя версия](https://img.shields.io/github/v/release/vladkharitonov87/claude-voice-helper-releases?label=%D0%B2%D0%B5%D1%80%D1%81%D0%B8%D1%8F&color=D97757)](https://github.com/vladkharitonov87/claude-voice-helper-releases/releases/latest)
[![Дата выхода](https://img.shields.io/github/release-date/vladkharitonov87/claude-voice-helper-releases?label=%D0%B2%D1%8B%D1%88%D0%BB%D0%B0)](https://github.com/vladkharitonov87/claude-voice-helper-releases/releases/latest)
[![Загрузки](https://img.shields.io/github/downloads/vladkharitonov87/claude-voice-helper-releases/total?label=%D0%B7%D0%B0%D0%B3%D1%80%D1%83%D0%B7%D0%BA%D0%B8)](https://github.com/vladkharitonov87/claude-voice-helper-releases/releases)
![Windows 10 | 11](https://img.shields.io/badge/Windows-10%20%7C%2011-0078D4?logo=windows)

<br>

[![Скачать для Windows](https://img.shields.io/badge/%D0%A1%D0%BA%D0%B0%D1%87%D0%B0%D1%82%D1%8C_%D0%B4%D0%BB%D1%8F_Windows-D97757?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/vladkharitonov87/claude-voice-helper-releases/releases/latest)

<sub>Файл <code>voice-helper-for-claude-&lt;версия&gt;-setup.exe</code> в разделе <b>Assets</b> ·
<a href="https://github.com/vladkharitonov87/claude-voice-helper-releases/releases">История версий</a></sub>

</div>

---

## Что умеет

- 🎙️ **Слушает имя-активатор.** Говорите «Клод» — и Claude начинает записывать, руки остаются свободными.
- 📨 **Отправляет сам.** Сообщение уходит после короткой паузы или сразу по команде «Клод, отправь».
- ↩️ **Отменяет и останавливает.** «Отмена» очищает поле ввода, «Стоп» прерывает ответ Claude.
- 🔇 **Выключает микрофон** после каждой команды — Claude не слышит лишнего.
- 🔒 **Распознаёт команды на компьютере**, без интернета: звук никуда не отправляется.
- 🟢 **Показывает состояние** значком в трее: слушаю, запись, нет микрофона, пауза.
- ⚙️ **Настраивается в приложении**: слова команд, задержки, микрофон, звуки, тема оформления.
- 🔄 **Обновляется само**: о новой версии сообщит меню в трее — одно нажатие, и она установлена.

## Голосовые команды

| Скажите | Что произойдёт |
|---|---|
| **«Клод»** (и пауза) или **«Клод, записывай»** | Claude включает диктовку — текст появляется в поле ввода |
| *продиктуйте текст и замолчите на 1,5 с* | Сообщение отправляется само |
| **«Клод, отправь»** | Отправить сразу, не дожидаясь паузы |
| **«Клод, отмена»** | Выбросить надиктованное |
| **«Клод, стоп»** | Остановить ответ, который Claude сейчас пишет |

Во время записи «отправь» и «отмена» работают и без имени. Начать запись и остановить ответ можно,
когда окно Claude активно, — случайная фраза в разговоре не сработает в фоне. Все слова и задержки меняются в
настройках — раздел «Голосовые команды».

## Установка

1. Нажмите **«Скачать для Windows»** выше и в разделе **Assets** скачайте
   `voice-helper-for-claude-<версия>-setup.exe`.
2. Запустите установщик и разрешите изменения — приложение ставится для всех пользователей в
   `C:\Program Files\Voice Helper for Claude`.
3. Если Windows покажет «Windows защитила ваш компьютер» — нажмите **«Подробнее» → «Выполнить в любом
   случае»**. Установщик пока не подписан цифровой подписью, поэтому SmartScreen его не узнаёт.
4. В Claude выберите язык диктовки: **Settings → General → Voice → Language → Russian**.

После установки помощник появится в трее и будет запускаться вместе с Windows (это отключается в
настройках). Настройки открываются щелчком по значку.

> [!TIP]
> Проверить, что файл скачался без искажений, можно по контрольной сумме SHA-256 — она указана рядом
> с файлом на странице релиза:
> `Get-FileHash .\voice-helper-for-claude-<версия>-setup.exe`

## Требования

| | |
|---|---|
| Система | Windows 10 или 11, 64-бит |
| Claude | Приложение Claude для Windows с голосовым вводом |
| Микрофон | Любой: встроенный, гарнитура или USB — выбирается в настройках |
| Язык команд | Русский |

Ничего дополнительно ставить не нужно: распознавание речи и всё необходимое входят в установщик.

## Обновление

Приложение проверяет новые версии само — раз в 6 часов и по пункту **«Проверить обновления»** в меню
трея. Когда выходит новая версия, в меню появляется **«Обновить до X.Y.Z»**: помощник скачает,
установит и перезапустит себя. Можно обновиться и вручную — установить новую версию поверх старой.
Настройки при обновлении сохраняются.

Что изменилось в каждой версии — в [истории версий](https://github.com/vladkharitonov87/claude-voice-helper-releases/releases).

## Приватность

- Команды распознаются локально ([Vosk](https://alphacephei.com/vosk/)) — звук не покидает компьютер.
- Сам текст диктует встроенный голосовой ввод Claude — помощник лишь нажимает его кнопки.
- Единственное обращение в интернет — проверка обновлений на GitHub.
- Журнал работы хранится только на компьютере и не содержит надиктованного текста.

## Удаление

**Параметры Windows → Приложения → Установленные приложения → Voice Helper for Claude → Удалить.**
Настройки остаются в `%AppData%\ClaudeVoiceHelper` — удалите эту папку, если они больше не нужны.

## Вопросы и ошибки

Нашли ошибку или есть идея — [создайте issue](https://github.com/vladkharitonov87/claude-voice-helper-releases/issues).
Приложите, пожалуйста, версию (меню значка в трее) и журнал из `%AppData%\ClaudeVoiceHelper\logs`.

---

<details>
<summary><b>In English</b></summary>

**Voice Helper for Claude** is a Windows tray app for hands-free control of the Claude desktop app:
it listens for a wake word, starts Claude's dictation, sends, cancels or stops by voice and mutes the
microphone after each command. Commands are recognized offline. Voice commands are currently
Russian-only. [Download the latest installer](https://github.com/vladkharitonov87/claude-voice-helper-releases/releases/latest)
(`voice-helper-for-claude-<version>-setup.exe`, Windows 10/11 x64).

</details>

<sub>Voice Helper for Claude — независимый проект, не связанный с Anthropic. Claude — товарный знак Anthropic, PBC.</sub>
