# Создание нового лендинга

1. Создать [Landing Brief](../templates/landing-brief.md), указав его стабильную identity/version.
2. Собрать Product Facts и материалы из `marketing-context`; разделить факты, гипотезы, решения и неизвестное.
3. Получить точное approval цели и позиционирования.
4. Подготовить структуру и copy; сверить каждый claim со статусом и доказательством; получить approval copy.
5. Подготовить visual spec/design; получить approval дизайна.
6. Реализовать только утверждённую версию в отдельной ветке.
7. Создать preview и evidence ключевых состояний/CTA.
8. Передать фиксированные base/head независимому reviewer через [review handoff](../templates/review-handoff.md); исправления требуют нового head и re-review.
9. Получить отдельное точное approval публикации. До этого merge запрещён.
10. Перепроверить механизм публикации, выполнить отдельно разрешённый merge/deploy и post-check; сохранить результат и rollback point.

Product-change handoff или новая функция сами по себе этот процесс не запускают.
