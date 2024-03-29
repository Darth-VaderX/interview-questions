# Hoisting
____

**Подъем JavaScript** — это процесс, при котором интерпретатор перемещает объявления функций, переменных, классов или импортируемых объектов в начало их области действия перед выполнением кода.

**Подъём переменных:**
При использовании ключевого слова `var` переменные поднимаются вверх и получают значение `undefined` до того, как код начнет выполняться. Это позволяет использовать переменные до их фактического объявления.
Переменные, объявленные с использованием `let` и `const`, также поднимаются, но остаются в "временной мертвой зоне" [Temporal Dead Zone (TDZ)](./TDZ.md) до момента их фактического объявления. В этом состоянии попытка обращения к ним вызовет ошибку. 

**Подъём функций:**
Функция, объявленная с помощью синтаксиса [Function Declaration](), а также классы поднимаются вверх и могут быть вызваны до объявления в коде, но [Arrow Function]() и [Function Expression]()  могут быть использованы только после того, как они были инициализированы.

- [Вопросы к собеседованию](../../README.md)
- [Разница между var, let, const](./difference.md)
- [Временная мёртвая зона(TDZ)](./TDZ.md)
- [Области видимости](./scope.md)