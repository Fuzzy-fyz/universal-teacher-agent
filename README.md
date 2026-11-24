# Universal Teacher

An adaptive tutor custom agent for Visual Studio Code and GitHub Copilot. It can teach any subject or skill—not only a predefined set of school or technical topics—while adapting explanations, practice, and feedback to the learner.

## Features

- Finds an approach that fits the learner's goal, prior experience, constraints, and feedback.
- Explains, diagnoses prerequisites, plans a learning path, and teaches through examples and practice.
- Tracks evidence-based mastery from not-yet-assessed to transfer into unfamiliar contexts.
- Analyzes errors, supports tests and exam prep, and recommends spaced review.
- Uses an explicit source hierarchy and clearly distinguishes verified sources from general model knowledge.
- Coaches projects while respecting learner authorship and course rules.
- Responds in the learner's language without assuming a fixed student profile, subject, or memory shared across workspaces.
- Offers conversational shortcuts such as `/plan`, `/learn`, `/practice`, `/test`, `/review`, `/progress`, and `/project`.

## Study memory

During substantive learning sessions, the agent reads and maintains a `study/` folder at the root of the active workspace. It records session outcomes, demonstrated progress, recurring errors, learning goals, and suggested review topics so later sessions in that same workspace can continue from the notes.

The agent preserves session and error history, distinguishes self-reports from demonstrated results, and follows more specific file and privacy rules in the host project. Learning records are not copied to this public repository. Memory is limited to the workspace files available to the agent: it is not shared across workspaces, cannot work when those files are inaccessible, and does not guarantee perfect recall. Review dates are suggestions, not scheduled reminders.

## Sources and factual accuracy

The agent prioritizes learner-provided course materials and requirements, then primary or authoritative sources, followed by reputable textbooks and reviews. For current, specialized, disputed, high-stakes, or explicitly sourced questions, it checks available tools and workspace materials, cites only what it actually inspected, and distinguishes those findings from its general model knowledge. It does not invent citations or claim that a source was checked when browsing or file access was unavailable.

If a reference is likely to be useful again, the agent may record its bibliographic details, topic, and last-checked date in `study/SOURCES.md`. A saved reference is not automatically re-verified for a later answer. The agent cannot browse the web unless the host environment provides a suitable search or browser tool.

## Install in a workspace

1. Copy `.github/agents/teacher.agent.md` into the same path in your project.
2. Open Visual Studio Code Chat and select **Universal Teacher** from the agent picker.
3. Start with a request such as `Explain recursion with an example` or `Help me plan a study path for organic chemistry`.

Custom agents require a version of Visual Studio Code or GitHub Copilot that supports `.agent.md` files.

## Install in your user profile

Copy `teacher.agent.md` to the `agents/` directory in your VS Code prompts folder. This makes the agent available across workspaces. See the [VS Code custom agents documentation](https://code.visualstudio.com/docs/copilot/customization/custom-agents) for current paths and setup details.

## Customize

Edit the agent file to adjust language, teaching style, or safety and academic-integrity requirements. Keep any learner profile opt-in and clearly separate reported information from demonstrated results.

## License

No license is granted. The repository is public for viewing, but reuse, modification, and redistribution are not permitted without the copyright holder's permission.

---

# Универсальный учитель

Адаптивный агент-преподаватель для Visual Studio Code и GitHub Copilot. Помогает осваивать любые предметы и навыки, подстраивая объяснения, практику и обратную связь под ученика.

## Возможности

- Объяснение понятий, диагностика знаний и составление реалистичных планов.
- Обучение через примеры, практику, подсказки и конкретную обратную связь.
- Повторение, проверка знаний, подготовка к экзаменам и сопровождение проектов.
- Работа на языке ученика и адаптация к запрошенному уровню.
- Без заранее заданного профиля или программы обучения; учебная память хранится только в доступных файлах текущего рабочего пространства.

## Установка в проект

Скопируйте `.github/agents/teacher.agent.md` в такой же путь своего проекта. Затем откройте чат VS Code, выберите **Universal Teacher** в списке агентов и задайте тему или цель обучения.

Для установки в профиль пользователя скопируйте файл `teacher.agent.md` в папку `agents/` каталога пользовательских промптов VS Code. Актуальные пути и сведения смотрите в [документации VS Code о пользовательских агентах](https://code.visualstudio.com/docs/copilot/customization/custom-agents).

Агент подстраивает обучение под цель, исходный уровень и ограничения ученика; оценивает освоение по наблюдаемым результатам, разбирает ошибки и предлагает интервалы повторения. Команды `/plan`, `/learn`, `/practice`, `/test`, `/review`, `/progress` и `/project` работают как текстовые сокращения, если их не перехватывает сам интерфейс.

Во время содержательных занятий агент читает и поддерживает папку `study/` в корне текущего рабочего пространства: записывает итоги занятий, подтверждённый прогресс, повторяющиеся ошибки, цели обучения и темы для повторения. Эти записи остаются в рабочем пространстве и не копируются в публичный репозиторий агента. Память доступна только пока агенту доступны эти файлы; между разными рабочими пространствами она не переносится. Интервалы повторения — рекомендации, а не назначенные напоминания.

При ответах он отдаёт приоритет материалам ученика и первичным или авторитетным источникам. Для актуальных, специальных, спорных или важных утверждений он проверяет доступные источники и ссылается только на реально просмотренные материалы; общие знания модели не выдаёт за внешнюю проверку. Список полезных ссылок с датой проверки при необходимости хранится в `study/SOURCES.md`. Веб-поиск возможен только при наличии соответствующего инструмента в среде Copilot.

## Лицензия

Лицензия не предоставляется. Репозиторий открыт для просмотра, но повторное использование, изменение и распространение требуют разрешения правообладателя.
