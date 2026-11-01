# README.md
Онлайн тренер
я натан 

## Плагины и инструменты

| # | Название | Что делает | Репозиторий |
|---|----------|------------|-------------|
| 1 | **Free LLM API** | Каталог сервисов с бесплатным доступом к LLM API или пробными кредитами (OpenRouter, Google AI Studio, Groq, Mistral, Cerebras и др.) | [cheahjs/free-llm-api-resources](https://github.com/cheahjs/free-llm-api-resources) |
| 2 | **Strix** | Открытые автономные AI-агенты для тестирования безопасности приложений (пентест с proof-of-concept) | [usestrix/strix](https://github.com/usestrix/strix) |
| 3 | **Claude-mem** | Плагин для Claude Code: постоянная память между сессиями (сжатие и подстановка контекста) | [thedotmack/claude-mem](https://github.com/thedotmack/claude-mem) |
| 4 | **Agent-Reach** | CLI, дающий AI-агентам доступ к Twitter/X, Reddit, YouTube, GitHub и др. без платных API | [Panniantong/Agent-Reach](https://github.com/Panniantong/Agent-Reach) |
| 5 | **Claude Code setup** | Официальный плагин Anthropic: анализирует проект и советует автоматизации Claude Code (хуки, скиллы, MCP-серверы, субагенты) | [anthropics/claude-plugins-official](https://github.com/anthropics/claude-plugins-official) |

### Установка

**1. Free LLM API** — это список, устанавливать ничего не нужно. Выберите провайдера в README репозитория и получите у него ключ.

**2. Strix** (нужны Python 3.12+, Docker и ключ LLM-провайдера):
```bash
pipx install strix-agent
strix --target ./app-directory
```
> Тестируйте только свои приложения или те, на которые у вас есть разрешение.

**3. Claude-mem** — в Claude Code:
```
/plugin marketplace add thedotmack/claude-mem
/plugin install claude-mem
```
Затем перезапустите Claude Code.

**4. Agent-Reach**:
```bash
pip install https://github.com/Panniantong/Agent-Reach/archive/main.zip
agent-reach install
agent-reach doctor   # проверить, какие каналы работают
```

**5. Claude Code setup** — в Claude Code:
```
/plugin install claude-code-setup@claude-plugins-official
```
