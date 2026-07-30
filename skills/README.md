# Claude Code Skills

Публичная коллекция скиллов для Claude Code — устанавливаются в Агента по запросу.

## Структура

```
global/     — универсальные скиллы (дизайн, UI, презентации)
custom/     — специализированные скиллы (код, исследования, контент)
```

## Global (7 скиллов)

| Скилл | Назначение |
|---|---|
| banner-design | Баннеры для соцсетей и рекламы |
| brand | Голос бренда, стайлгайды, айдентика |
| design | Логотипы, корпоративная айдентика, иконки |
| design-system | Дизайн-токены, компоненты |
| slides | HTML-презентации с Chart.js |
| ui-styling | Стилизация через Tailwind/shadcn |
| ui-ux-pro-max | UI/UX для веб и мобайл, 50+ стилей |

## Custom (9 скиллов)

| Скилл | Назначение |
|---|---|
| code-review | Анализ кода |
| competitor-research | Исследование трендов и анализ ЦА |
| instagram-stories | Instagram Stories с текстом на фото |
| media-download | Скачивание медиа |
| monitor-knowledge | Мониторинг и база знаний |
| server-management | Управление сервером |
| system | Системные операции |
| video-transcript | Транскрипция видео |
| web-scraping | Парсинг веб-страниц |

> `discovery-interview`, `content-creator`, `fullstack-developer`, `frontend-design` — уже предустановлены в `.claude/skills/` вместе с архитектурой, отдельно ставить не нужно (это те же файлы).

## Установка одного скилла

Скажи своему Агенту:

```
Установи скилл <имя> из https://github.com/likebosssssssssss/mars-agent-template
```

Агент скачает файлы из папки `skills/global/<имя>/` или `skills/custom/<имя>/` и положит в `~/.claude/skills/<имя>/`. После `/reset` скилл активен.

## Установка всех скиллов

```bash
git clone https://github.com/likebosssssssssss/mars-agent-template ~/mars-agent-template
cp -r ~/mars-agent-template/skills/global/* ~/.claude/skills/
cp -r ~/mars-agent-template/skills/custom/* ~/.claude/skills/
```

## Лицензия

Скиллы предоставляются «как есть» для использования с Claude Code.
