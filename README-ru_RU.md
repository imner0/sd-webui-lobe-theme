<a name="readme-top"></a>

<div align="center">

<img height="160" src="https://registry.npmmirror.com/@lobehub/assets-logo/1.0.0/files/assets/logo-3d.webp">

<h1 align="center">Lobe Theme</h1>

Современная тема для стабильной диффузии webui

Ранее известная как Kitchen theme

[English ](./README.md)· [简体中文](./README-zh_CN.md) · Russian · [Changelog](./CHANGELOG.md) · [Report Bug][github-issues-link] · [Request Feature][github-issues-link]

<!-- SHIELD GROUP -->

[![][github-release-shield]][github-release-link]
[![][discord-shield]][discord-link]
[![][github-releasedate-shield]][github-releasedate-link]
[![][github-action-test-shield]][github-action-test-link]
[![][github-action-release-shield]][github-action-release-link]<br/>
[![][github-contributors-shield]][github-contributors-link]
[![][github-forks-shield]][github-forks-link]
[![][github-stars-shield]][github-stars-link]
[![][github-issues-shield]][github-issues-link]
[![][github-license-shield]][github-license-link]

</div>

![][cover]

> **Warning**\
> `Lobe Theme v3` is compatible with `SD WebUI v1.6` and is not backwards compatible. Versions below `< 1.6` should be moved to the branch [legacy-sd-webui-1.5](https://github.com/lobehub/sd-webui-lobe-theme/tree/legacy-sd-webui-1.5)

<details>
<summary><kbd>Table of contents</kbd></summary>

#### TOC

- [✨ Дополнения](#-дополнения)

- [📦 Установка](#-установка)

- [🤯 Использование](#-использование)

- [🖥 Поддерживаемые браузеры](#-поддерживаемые-браузеры)

- [⌨️ Локальная разработка](#️-локальная-разработка)

- [🤝 Содействие](#-содействие)

- [🔗 Ссылки](#-ссылки)

  - [Больше продуктов](#больше-продуктов)
  - [Благодарности](#благодарности)

####

</details>

## ✨ Дополнения

- [x] 🌗 Поддержка светлой и темной темы, с возможностью быстрого переключения на панели навигации
- [x] 🌈 Поддержка кастомных пользовательских и нейтральных цветов с возможностью настройки логотипа
- [x] 🪄 Поддержка форматирования подсказки одним щелчком мыши с помощью простого редактора тегов
- [x] 🎛️ Высоконастраиваемая боковая панель, с боковой панелью быстрых настроек слева и боковой панелью моделей справа
- [x] 🖼️ Регулируемое соотношение холста, благодаря чему генерируемые изображения всегда отображаются сверху
- [x] 📱 Mobile-friendly, с частичной оптимизацией под мобильные экраны
- [x] 🌍 Поддержка i18n(Поддержка разных языков) и приветствуются [PR](https://github.com/lobehub/sd-webui-lobe-theme/tree/main/locales)
- [x] 📝 Подсветка синтаксиса в поле ввода промта
- [x] 📦 Поддержка [PWA](https://support.google.com/chrome/answer/9658361)

<div align="right">

[![][back-to-top]](#readme-top)

</div>

## 📦 Установка

#### Метод 1

Найдите `Lobe Theme` или `Kitchen Theme` в поисковике плагинов SD WebUI и установите их.

> **Note**\
> **Версия 2.0.0** была переименована в **Lobe Theme**.

#### Метод 2

В качестве расширения (рекомендуется) клонировать репозиторий в папку расширений:

```shell
git clone "https://github.com/lobehub/sd-webui-lobe-theme" extensions/lobe-theme
```

> **Important**\
> Минимальные требования `gradio-3.41.2` & `sd-webui 1.6`

#### Обновления

Добавьте проект в избранное, и вы будете получать все уведомления о релизах непосредственно с GitHub \~ ⭐️

<details><summary><kbd>Star History</kbd></summary>
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=lobehub%2Fsd-webui-lobe-theme&theme=dark&type=Date">
    <img src="https://api.star-history.com/svg?repos=lobehub%2Fsd-webui-lobe-theme&type=Date">
  </picture>
</details>

<div align="right">

[![][back-to-top]](#readme-top)

</div>

## 🤯 Использование

![][feat-thememode]

#### Светлая и темная темы

> **Note**\
> В правом верхнем углу панели навигации можно быстро переключаться между светлой и темной темами.

Текущая тема поддерживает как светлые, так и темные темы. Если вы хотите принудительно включить темный режим, используйте аргумент `--theme=dark` для запуска WebUI. Например, под Windows ваш `webui-user.bat` должен содержать:

```shell
set COMMANDLINE_ARGS= --theme=dark
```

Кроме того, переключение можно осуществлять непосредственно через URL:

```shell
http://localhost:7860/?__theme=light
http://localhost:7860/?__theme=dark
```

<div align="right">

[![][back-to-top]](#readme-top)

</div>

![][feat-theme-modify]

#### Кастомизация темы

> **Note**\
> Щелкните на значке `⚙` в правом верхнем углу, чтобы открыть панель настроек. В настоящее время доступны следующие настройки:

- Тема
  - Основной цвет: в настоящее время предлагается 13 цветовых комбинаций тем.
  - Нейтральный цвет: в настоящее время предлагается 6 различных комбинаций оттенков серого.
  - Тип логотипа: `Lobe`, `Kitchen`, `Custom`
    - Пользовательский логотип: `Поддерживаются ссылки`, `base64`, и `emoji`. При вводе одного смайлика он будет автоматически заменен на 3D Fluent Emoji.
    - Пользовательский заголовок: Настраиваемое название сайта/темы.

<div align="right">

[![][back-to-top]](#readme-top)

</div>

![][feat-highlight]

#### Подсветка синтаксиса подсказок

Автоматически подсвечивать промт в соответствии с правилами синтаксиса Stable Diffusion.

<div align="right">

[![][back-to-top]](#readme-top)

</div>

![][feat-sidebar]

#### Настройка боковой панели

> **Note**\
> нажмите значок `⚙` в правом верхнем углу, чтобы открыть панель настроек. Текущие доступные настройки следующие:

- **Текстовое поле промта**
  - Режим отображения: `Фиксированная высота и скрол в поле ввода` | `Увеличение от вводимого текста`
- **Боковая панель**
  - По умолчанию развернуть: `true`
  - Режим отображения: `Фиксированный` | `Плавающий`
  - Ширина по умолчанию: `280`
- **Панель с дом. сетями**
  - Включено: `true`
  - По умолчанию развернуть: `true`
  - Режим отображения: `Фиксированный` | `Плавающий`
  - Ширина по умолчанию: `340`
  - Размер превью по умолчанию: `86`

<details>
<summary><kbd>Recommended System Settings</kbd></summary>

#### Доп. Сети

- Превью
- Ширина: 86
- высота: 128

<br/>

#### Быстрые настройки (изменяются в настройках SD)

```txt
sd_model_checkpoint, sd_vae, CLIP_stop_at_last_layers, img2img_background_color, img2img_color_correction, samples_save, samples_format, grid_save, return_grid,  n_rows, live_previews_enable, show_progress_every_n_steps, live_preview_refresh_period
```

</details>

<div align="right">

[![][back-to-top]](#readme-top)

</div>

![][feat-mobile-friendly]

#### Адаптированно под мобильные устройства

Выполнена частичная адаптация удобства работы с мобильными устройствами, включая откидную панель навигации, адаптацию боковой панели и т.д. Однако из-за высокой сложности и фиксированных значений стабильного диффузного интерфейса трудно обеспечить такое же удобство работы, как и в настольной версии. Приветствуется обратная связь для поиска новых идей.

<div align="right">

[![][back-to-top]](#readme-top)

</div>

![][feat-pwa]

#### Progress Web App

Вы можете использовать Progressive Web Apps [PWA](https://support.google.com/chrome/answer/9658361) для быстрого стабильного запуска на компьютере или мобильном устройстве.

- На компьютере откройте браузер Chrome.
- Перейдите на стабильный сайт диффузии, который вы хотите установить
- В правом верхнем углу адресной строки нажмите кнопку `Установить`
- Follow the onscreen instructions to install the PWA

<div align="right">

[![][back-to-top]](#readme-top)

</div>

#### Форматирование подсказок

Нажмите кнопку <kbd>🪄</kbd> под строкой Prompt, чтобы отформатировать слова подсказки одним щелчком мыши.

> **Note**\
> Преобразует полноразмерные знаки препинания в полуразмерные, уберет лишние пробелы, добавит недостающие запятые и перенесёт в конец Extra-Networks (Дополнительные) модели.

Перед форматированием:

```text
photorealistic   photo of a handsome male (wizard  :1.2）， <lora:LuisapHotlineStyle:0.5> <lora:ElegantHanfuRuqunStyle:0.2>    short beard, white wizard  shirt, (with golden    trim:0.8),
```

После форматирования:

```text
photorealistic photo of a handsome male, (wizard:1.2), short beard, white wizard shirt, (with golden trim:0.8), <lora:LuisapHotlineStyle:0.5>, <lora:ElegantHanfuRuqunStyle:0.2>
```

<div align="right">

[![][back-to-top]](#readme-top)

</div>

## 🖥 Поддерживаемые браузеры

| [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/chrome/chrome_48x48.png" alt="Chrome" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)<br>Chrome | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/edge/edge_48x48.png" alt="Edge" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)<br>Edge | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/safari/safari_48x48.png" alt="Safari" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)<br>Safari |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| last 2 versions                                                                                                                                                                                              | last 2 versions                                                                                                                                                                                      | last 2 versions                                                                                                                                                                                              |

> **Warning**\`
> В настоящее время известна проблема совместимости со стилями в браузере Firefox.

<div align="right">

[![][back-to-top]](#readme-top)

</div>

## ⌨️ Локальная разработка

Вы можете использовать Github Codespaces для разработки в режиме онлайн:

[![][codespaces-shield]][codespaces-link]

В качестве альтернативы можно клонировать его для локальной разработки. Для включения режима горячей загрузки необходимо предварительно запустить Stable-Diffusion на порту `7860`.

[![][bun-shield]][bun-link]

```bash
$ git clone https://github.com/lobehub/sd-webui-lobe-theme.git
$ cd sd-webui-lobe-theme
$ bun install
$ bun dev
```

<div align="right">

[![][back-to-top]](#readme-top)

</div>

## 🤝 Содействие

Любые виды вкладов приветствуются, если вас интересует внесение кода, не стесняйтесь просмотреть наши проблемы на GitHub [Issues][github-issues-link], чтобы показать нам, из чего вы сделаны.

[![][pr-welcome-shield]][pr-welcome-link]

[![][contributors-contrib]][contributors-link]

<div align="right">

[![][back-to-top]](#readme-top)

</div>

## 🔗 Ссылки

### Больше продуктов

- **[🤖 Lobe Chat][lobe-chat] :** Это открытая, расширяемая (с вызовом функций) высокопроизводительная рамка для чат-ботов. Она поддерживает однокликовую бесплатную развертывание вашего частного веб-приложения ChatGPT/LLM.
- **[🌏 Lobe i18n][lobe-i18n] :** Lobe i18n - это автоматизированный инструмент для процесса перевода i18n (интернационализация), работающий на основе ChatGPT. Он поддерживает такие функции, как автоматическое разделение больших файлов, инкрементные обновления и настраиваемые параметры для модели OpenAI, API прокси и температуры.
- **[💌 Lobe Commit][lobe-commit] :** Lobe Commit - это инструмент CLI, который использует Langchain/ChatGPT для создания сообщений о коммитах на основе Gitmoji.

### Благодарности

- stable-diffusion-webui：<https://github.com/AUTOMATIC1111/stable-diffusion-webui>
- gradio-theme-gallery: <https://huggingface.co/spaces/gradio/theme-gallery>
- cozy-nest: <https://github.com/Nevysha/Cozy-Nest>
- _before `1.0.0` version_
  - sd-web-ui-quickcs: <https://github.com/Gerschel/sd-web-ui-quickcss/>
  - Dark-Themes-SD-WebUI-Automatic1111: <https://github.com/Nacurutu/Dark-Themes-SD-WebUI-Automatic1111>

<div align="right">

[![][back-to-top]](#readme-top)

</div>

---

<details><summary><h4>📝 License</h4></summary>

[![][fossa-license-shield]][fossa-license-link]

</details>

Copyright © 2023 [CanisMinor][profile-link]. <br />
This project is [AGPL3](./LICENSE) licensed.

<!-- LINK GROUP -->

[back-to-top]: https://img.shields.io/badge/-BACK_TO_TOP-151515?style=flat-square
[bun-link]: https://bun.sh
[bun-shield]: https://img.shields.io/badge/-speedup%20with%20bun-black?logo=bun&style=for-the-badge
[codespaces-link]: https://codespaces.new/lobehub/sd-webui-lobe-theme
[codespaces-shield]: https://github.com/codespaces/badge.svg
[contributors-contrib]: https://contrib.rocks/image?repo=lobehub/sd-webui-lobe-theme
[contributors-link]: https://github.com/lobehub/sd-webui-lobe-theme/graphs/contributors
[cover]: https://gw.alipayobjects.com/zos/kitchen/8Ab%24hLJ5ur/cover.webp
[discord-link]: https://discord.gg/AYFPHvv2jT
[discord-shield]: https://img.shields.io/discord/1127171173982154893?color=5865F2&label=discord&labelColor=black&logo=discord&logoColor=white&style=flat-square
[feat-highlight]: https://gw.alipayobjects.com/zos/kitchen/iD%24W4U2y3Y/feat_highlight.webp
[feat-mobile-friendly]: https://gw.alipayobjects.com/zos/kitchen/WpWe6Hw8UT/feat_mobile_friendly.webp
[feat-pwa]: https://gw.alipayobjects.com/zos/kitchen/az49akOKJT/feat_pwa.webp
[feat-sidebar]: https://gw.alipayobjects.com/zos/kitchen/Olum2IjxCW/feat_sidebar.webp
[feat-theme-modify]: https://gw.alipayobjects.com/zos/kitchen/CbhlynwJYg/feat_theme_modify.webp
[feat-thememode]: https://gw.alipayobjects.com/zos/kitchen/nSFtJidWUR/feat_thememode.webp
[fossa-license-link]: https://app.fossa.com/projects/git%2Bgithub.com%2Flobehub%2Fsd-webui-lobe-theme
[fossa-license-shield]: https://app.fossa.com/api/projects/git%2Bgithub.com%2Flobehub%2Fsd-webui-lobe-theme.svg?type=large
[github-action-release-link]: https://github.com/actions/workflows/lobehub/sd-webui-lobe-theme/release.yml
[github-action-release-shield]: https://img.shields.io/github/actions/workflow/status/lobehub/sd-webui-lobe-theme/release.yml?label=release&labelColor=black&logo=githubactions&logoColor=white&style=flat-square
[github-action-test-link]: https://github.com/actions/workflows/lobehub/sd-webui-lobe-theme/test.yml
[github-action-test-shield]: https://img.shields.io/github/actions/workflow/status/lobehub/sd-webui-lobe-theme/test.yml?label=test&labelColor=black&logo=githubactions&logoColor=white&style=flat-square
[github-contributors-link]: https://github.com/lobehub/sd-webui-lobe-theme/graphs/contributors
[github-contributors-shield]: https://img.shields.io/github/contributors/lobehub/sd-webui-lobe-theme?color=c4f042&labelColor=black&style=flat-square
[github-forks-link]: https://github.com/lobehub/sd-webui-lobe-theme/network/members
[github-forks-shield]: https://img.shields.io/github/forks/lobehub/sd-webui-lobe-theme?color=8ae8ff&labelColor=black&style=flat-square
[github-issues-link]: https://github.com/lobehub/sd-webui-lobe-theme/issues
[github-issues-shield]: https://img.shields.io/github/issues/lobehub/sd-webui-lobe-theme?color=ff80eb&labelColor=black&style=flat-square
[github-license-link]: https://github.com/lobehub/sd-webui-lobe-theme/blob/main/LICENSE
[github-license-shield]: https://img.shields.io/github/license/lobehub/sd-webui-lobe-theme?color=white&labelColor=black&style=flat-square
[github-release-link]: https://github.com/lobehub/sd-webui-lobe-theme/releases
[github-release-shield]: https://img.shields.io/github/v/release/lobehub/sd-webui-lobe-theme?color=369eff&labelColor=black&logo=github&style=flat-square
[github-releasedate-link]: https://github.com/lobehub/sd-webui-lobe-theme/releases
[github-releasedate-shield]: https://img.shields.io/github/release-date/lobehub/sd-webui-lobe-theme?labelColor=black&style=flat-square
[github-stars-link]: https://github.com/lobehub/sd-webui-lobe-theme/network/stargazers
[github-stars-shield]: https://img.shields.io/github/stars/lobehub/sd-webui-lobe-theme?color=ffcb47&labelColor=black&style=flat-square
[lobe-chat]: https://github.com/lobehub/lobe-chat
[lobe-commit]: https://github.com/lobehub/lobe-commit/tree/master/packages/lobe-commit
[lobe-i18n]: https://github.com/lobehub/lobe-commit/tree/master/packages/lobe-i18n
[pr-welcome-link]: https://github.com/lobehub/lobe-chat/pulls
[pr-welcome-shield]: https://img.shields.io/badge/🤯_pr_welcome-%E2%86%92-ffcb47?labelColor=black&style=for-the-badge
[profile-link]: https://github.com/canisminor1990
