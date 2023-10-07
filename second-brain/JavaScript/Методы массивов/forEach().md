Один из известных методов для массивов

Она проходится одной и той же функцией по каждому элементу внутри массива


Примеры:

### [Нет операции для неинициализированных значений (разреженные массивы)](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach#sparsearray "Permalink to Нет операции для неинициализированных значений (разреженные массивы)")

```
const arraySparse = [1,3,,7]
let numCallbackRuns = 0

arraySparse.forEach((element) => {
  console.log(element)
  numCallbackRuns++
})

console.log("numCallbackRuns: ", numCallbackRuns)

// 1
// 3
// 7
// numCallbackRuns: 3
// комментарий: как вы видите пропущенное значение между 3 и 7 не вызывало функцию callback.
```

### [Конвертируем цикл for в forEach](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach#%D0%BA%D0%BE%D0%BD%D0%B2%D0%B5%D1%80%D1%82%D0%B8%D1%80%D1%83%D0%B5%D0%BC_%D1%86%D0%B8%D0%BA%D0%BB_for_%D0%B2_foreach "Permalink to Конвертируем цикл for в forEach")

```
const items = ['item1', 'item2', 'item3']
const copy = []

// до
for (let i = 0; i < items.length; i++) {
  copy.push(items[i])
}

// после
items.forEach(function(item){
  copy.push(item)
})
```

[[Методы массивов]] 