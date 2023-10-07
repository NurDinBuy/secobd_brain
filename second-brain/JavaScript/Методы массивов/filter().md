Метод **создаёт новый массив со всеми элементами**, прошедшими проверку, задаваемую в передаваемой функции.

```
const words = ['spray', 'limit', 'elite', 'exuberant', 'destruction', 'present'];

const result = words.filter(word => word.length > 6);

console.log(result);
```

[[Методы массивов]]