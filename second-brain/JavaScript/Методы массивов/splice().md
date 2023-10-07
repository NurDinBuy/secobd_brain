Метод splice() - изменяет содержимое массива, удаляя существующие элементы и / или добавляя новые.

Один из часто используемых методов в JS




Примеры:

### [Удаляет 0 элементов по индексу 2 и вставляет "drum"](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array/splice#%D1%83%D0%B4%D0%B0%D0%BB%D1%8F%D0%B5%D1%82_0_%D1%8D%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82%D0%BE%D0%B2_%D0%BF%D0%BE_%D0%B8%D0%BD%D0%B4%D0%B5%D0%BA%D1%81%D1%83_2_%D0%B8_%D0%B2%D1%81%D1%82%D0%B0%D0%B2%D0%BB%D1%8F%D0%B5%D1%82_drum "Permalink to Удаляет 0 элементов по индексу 2 и вставляет "drum"")

```
var myFish = ['angel', 'clown', 'mandarin', 'sturgeon'];
var removed = myFish.splice(2, 0, 'drum');

// myFish равен ["angel", "clown", "drum", "mandarin", "sturgeon"]
// removed равен [], ничего не удалено
```


### [Удаляет 1 элемент по индексу 3](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array/splice#%D1%83%D0%B4%D0%B0%D0%BB%D1%8F%D0%B5%D1%82_1_%D1%8D%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82_%D0%BF%D0%BE_%D0%B8%D0%BD%D0%B4%D0%B5%D0%BA%D1%81%D1%83_3 "Permalink to Удаляет 1 элемент по индексу 3")

```
var myFish = ['angel', 'clown', 'drum', 'mandarin', 'sturgeon'];
var removed = myFish.splice(3, 1);

// removed равен ["mandarin"]
// myFish равен ["angel", "clown", "drum", "sturgeon"]
```


### [Удаляет 1 элемент по индексу 2 и вставляет "trumpet"](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array/splice#%D1%83%D0%B4%D0%B0%D0%BB%D1%8F%D0%B5%D1%82_1_%D1%8D%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82_%D0%BF%D0%BE_%D0%B8%D0%BD%D0%B4%D0%B5%D0%BA%D1%81%D1%83_2_%D0%B8_%D0%B2%D1%81%D1%82%D0%B0%D0%B2%D0%BB%D1%8F%D0%B5%D1%82_trumpet "Permalink to Удаляет 1 элемент по индексу 2 и вставляет "trumpet"")

```
var myFish = ['angel', 'clown', 'drum', 'sturgeon'];
var removed = myFish.splice(2, 1, 'trumpet');

// myFish равен ["angel", "clown", "trumpet", "sturgeon"]
// removed равен ["drum"]
```



### [Удаляет 2 элемента начиная с индекса 0 и вставляет "parrot", "anemone" и "blue"](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array/splice#%D1%83%D0%B4%D0%B0%D0%BB%D1%8F%D0%B5%D1%82_2_%D1%8D%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82%D0%B0_%D0%BD%D0%B0%D1%87%D0%B8%D0%BD%D0%B0%D1%8F_%D1%81_%D0%B8%D0%BD%D0%B4%D0%B5%D0%BA%D1%81%D0%B0_0_%D0%B8_%D0%B2%D1%81%D1%82%D0%B0%D0%B2%D0%BB%D1%8F%D0%B5%D1%82_parrot_anemone_%D0%B8_blue "Permalink to Удаляет 2 элемента начиная с индекса 0 и вставляет "parrot", "anemone" и "blue"")

```
var myFish = ['angel', 'clown', 'trumpet', 'sturgeon'];
var removed = myFish.splice(0, 2, 'parrot', 'anemone', 'blue');

// myFish равен ["parrot", "anemone", "blue", "trumpet", "sturgeon"]
// removed равен ["angel", "clown"]
```



### [Удаляет 2 элемента начиная с индекса 2](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array/splice#%D1%83%D0%B4%D0%B0%D0%BB%D1%8F%D0%B5%D1%82_2_%D1%8D%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82%D0%B0_%D0%BD%D0%B0%D1%87%D0%B8%D0%BD%D0%B0%D1%8F_%D1%81_%D0%B8%D0%BD%D0%B4%D0%B5%D0%BA%D1%81%D0%B0_2 "Permalink to Удаляет 2 элемента начиная с индекса 2")

```
var myFish = ['parrot', 'anemone', 'blue', 'trumpet', 'sturgeon'];
var removed = myFish.splice(myFish.length - 3, 2);

// myFish равен ["parrot", "anemone", "sturgeon"]
// removed равен ["blue", "trumpet"]
```



### [Удаляет 1 элемент по индексу -2](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array/splice#%D1%83%D0%B4%D0%B0%D0%BB%D1%8F%D0%B5%D1%82_1_%D1%8D%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82_%D0%BF%D0%BE_%D0%B8%D0%BD%D0%B4%D0%B5%D0%BA%D1%81%D1%83_-2 "Permalink to Удаляет 1 элемент по индексу -2")

```
var myFish = ['angel', 'clown', 'mandarin', 'sturgeon'];
var removed = myFish.splice(-2, 1);

// myFish равен ["angel", "clown", "sturgeon"]
// removed равен s ["mandarin"]
```



### [Удаляет все элементы после индекса 2 (включительно)](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array/splice#%D1%83%D0%B4%D0%B0%D0%BB%D1%8F%D0%B5%D1%82_%D0%B2%D1%81%D0%B5_%D1%8D%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82%D1%8B_%D0%BF%D0%BE%D1%81%D0%BB%D0%B5_%D0%B8%D0%BD%D0%B4%D0%B5%D0%BA%D1%81%D0%B0_2_%D0%B2%D0%BA%D0%BB%D1%8E%D1%87%D0%B8%D1%82%D0%B5%D0%BB%D1%8C%D0%BD%D0%BE "Permalink to Удаляет все элементы после индекса 2 (включительно)")

```
var myFish = ['angel', 'clown', 'mandarin', 'sturgeon'];
var removed = myFish.splice(2);

// myFish равен ["angel", "clown"]
// removed равен ["mandarin", "sturgeon"]
```


[[Методы массивов]] 