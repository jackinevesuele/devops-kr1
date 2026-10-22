# Контрольная работа 1

Босарев Евгений, ЭФБО-11-24. Инструменты DevOps.

Проект импортирован из шаблона преподавателя:
https://gitverse.ru/dgimatdinov/devops-kr-template

Реализованы validate_email, validate_phone и validate_snils.
В tests/test_validator.py исправлены отсутствующие импорты шаблона.
Для номера 001-001-999 верное контрольное число СНИЛС равно 65, а не 32.

## Проверка

```bash
python -m pip install pytest
python -m pytest -q
```

История feature-ветки очищена командой git rebase -i HEAD~4:
коммиты тестов и исправления опечатки объединены с основной функцией,
заготовка validate_inn исключена через drop.
Конфликт с feature/instructor-change разрешён с сохранением трёх валидаторов.

Основной репозиторий: https://github.com/jackinevesuele/devops-kr1
Зеркало: https://github.com/jackinevesuele/devops-kr1-mirror
