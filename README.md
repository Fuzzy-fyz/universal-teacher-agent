# Universal Teacher

An adaptive tutor custom agent for Visual Studio Code and GitHub Copilot. It can teach any subject or skill—not only a predefined set of school or technical topics—while adapting explanations, practice, and feedback to the learner.

## Features

- Explain concepts, diagnose knowledge, and build realistic study plans.
- Teach through examples, practice, hints, and specific feedback.
- Support review, assessments, exam preparation, and project coaching.
- Respond in the learner's language and adapt to the requested level.
- Avoid assuming a learner profile, curriculum, or persistent memory.

## Install in a workspace

1. Copy `.github/agents/teacher.agent.md` into the same path in your project.
2. Open Visual Studio Code Chat and select **Universal Teacher** from the agent picker.
3. Start with a request such as `Explain recursion with an example` or `Help me plan a study path for organic chemistry`.

Custom agents require a version of Visual Studio Code or GitHub Copilot that supports `.agent.md` files.

## Install in your user profile

Copy `teacher.agent.md` to the `agents/` directory in your VS Code prompts folder. This makes the agent available across workspaces. See the [VS Code custom agents documentation](https://code.visualstudio.com/docs/copilot/customization/custom-agents) for current paths and setup details.

## Customize

Edit the agent file to adjust language, teaching style, or safety and academic-integrity requirements. It intentionally does not assume a particular learner, subject, study schedule, or note-taking system.

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
- Без заранее заданного профиля, программы обучения и обещаний постоянной памяти.

## Установка в проект

Скопируйте `.github/agents/teacher.agent.md` в такой же путь своего проекта. Затем откройте чат VS Code, выберите **Universal Teacher** в списке агентов и задайте тему или цель обучения.

Для установки в профиль пользователя скопируйте файл `teacher.agent.md` в папку `agents/` каталога пользовательских промптов VS Code. Актуальные пути и сведения смотрите в [документации VS Code о пользовательских агентах](https://code.visualstudio.com/docs/copilot/customization/custom-agents).

## Лицензия

Лицензия не предоставляется. Репозиторий открыт для просмотра, но повторное использование, изменение и распространение требуют разрешения правообладателя.
