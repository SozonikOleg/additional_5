# Brackets

## Task

Implement function `check(str, bracketsConfig)`, that for given brackets sequence will return `true` if it is correct and `false` otherwise

реализовать функцию проверки '(ул. bracketsconfig), которая для заданной последовательности скобок возвращает 'true', если это правильно и false в противном случае

In the second param there is `bracketsConfig` - the array of pairs open-closed brackets. Each subarray includes only 2 elements - opening and closing bracket

во втором парам есть 'bracketsconfig' - массив из пары открытые-закрытые скобки. каждый подмассив содержит только 2 элемента - Открытие и закрытие кронштейна

```js
check('()', [['(', ')']]) // -> true
check('((()))()', [['(', ')']]) // -> true
check('())(', [['(', ')']]) // -> false
check('([{}])', [['(', ')'], ['[', ']'], ['{', '}']]) // -> true
check('[(])', [['(', ')'], ['[', ']']]) // -> false
check('[]()', [['(', ')'], ['[', ']']]) // -> true
check('[]()(', [['(', ')'], ['[', ']']]) // -> false

// special case: opening and closing bracket can be the same :)

check('||', [['|', '|']]) // -> true
check('|()|', [['(', ')'], ['|', '|']]) // -> true
check('|(|)', [['(', ')'], ['|', '|']]) // -> false
check('|()|(||)||', [['(', ')'], ['|', '|']]) // -> true
```

Write your code in `src/index.js`
