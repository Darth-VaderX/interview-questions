# Lexical Environment (лексическое окружение)
____

Лексическое окружение - это объект спецификации, который существует только в спецификации языка, для описания того, как все работает.

## Лексическое окружение состоит из двух частей:

1. **Environment Record (Запись окружения)**: Это объект, в котором как свойства хранятся все локальные переменные (а также некоторая другая информация, такая как значение `this`).

2. **Ссылка на внешнее лексическое окружение**: Это ссылка на лексическое окружение, которое соответствует коду снаружи текущих фигурных скобок.

## Два типа лексического окружения:

1. **Глобальное окружение (глобальный контекст выполнения)** — это лексическое окружение, у которого нет внешнего окружения. Ссылка глобального окружения на внешнее окружение представлена значением `null`. В глобальном окружении (в записи окружения) доступны встроенные сущности языка (такие, как `Object`, `Array`, и так далее), которые связаны с глобальным объектом, там же находятся и глобальные переменные, определённые пользователем. Значение `this` в этом окружении указывает на глобальный объект.

2. **Окружение функции** — в записи окружения, хранятся переменные, объявленные пользователем. Ссылка на внешнее окружение может указывать как на глобальный объект, так и на внешнюю по отношении к рассматриваемой функции функцию.

[Вопросы к собеседованию](../../README.md)<br>
[Как определить контекст this](this.md)<br>
[Variable Environment](./variableEnvironment.md)<br>
[Execution Context](./executionContext.md)