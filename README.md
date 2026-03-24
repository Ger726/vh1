// 1. Базовый вызов
function sayHello() {
    console.log("Hello, JS!");
}
sayHello();

// 2. Параметры
function greet(name) {
    console.log(`Hello, ${name}`);
}
greet("Arthur");

// 3. Приветствие с проверкой
function greet(name) {
    return name ? `Hello, ${name}` : "Hello, stranger";
}
console.log(greet("Arthur"));
console.log(greet());

// 4. Возведение в квадрат
function square(x) {
    return x * x;
}
console.log(square(5)); // 25

// 5. Сумма массива
function sumArray(arr) {
    let sum = 0;
    for (let num of arr) sum += num;
    return sum;
}
console.log(sumArray([1, 2, 3, 4])); // 10

// ============================================
// УСЛОВИЯ И ЦИКЛЫ - 5 задач (для оценки 3)
// ============================================

// 1. Проверка числа
let n = -5;
if (n > 0) console.log("positive");
else if (n < 0) console.log("negative");
else console.log("zero"); // negative

// 2. Минимум из двух
let a = 12, b = 7;
console.log(a < b ? a : b); // 7

// 3. Делится ли на 3
n = 15;
console.log(n % 3 === 0 ? "yes" : "no"); // yes

// 4. Сумма от 1 до N
let N = 7, sum = 0;
for (let i = 1; i <= N; i++) sum += i;
console.log(sum); // 28

// 5. Нечётные числа
for (let i = 1; i <= 15; i += 2) {
    console.log(i);
}

// ============================================
// СТРОКИ - 5 задач (для оценки 3)
// ============================================

// 1. Базовый срез
console.log("JavaScript".slice(4)); // "Script"

// 2. Проверка начала/конца
let str = "report.pdf";
console.log(str.startsWith("rep")); // true

// 3. Замена
str = "I like cats";
console.log(str.replace("cats", "dogs"));

// 4. Подсчёт слов
str = "apple,banana,orange,apple";
let count = 0;
str.split(",").forEach(word => {
    if (word === "apple") count++;
});
console.log(count); // 2

// 5. Только числа
str = "My phone number is 12345 and my code is 67890";
console.log(str.match(/\d+/g)); // ["12345", "67890"]

// ============================================
// МАССИВЫ - 10 задач (для оценки 3)
// ============================================

// 1. Добавить
let arr = [1, 2];
arr.push(3);
console.log(arr); // [1, 2, 3]

// 2. Удалить
arr = ["a", "b", "c"];
let last = arr.pop();
console.log(last); // "c"

// 3. Есть ли 100
console.log([10, 20, 30, 40].includes(100)); // false

// 4. Подмассив
console.log([5, 10, 15, 20, 25].slice(1, 4)); // [10, 15, 20]

// 5. Замена splice
arr = [1, 2, 3, 4];
arr.splice(1, 2, "X", "Y");
console.log(arr); // [1, "X", "Y", 4]

// 6. Умножение
console.log([2, 4, 6].map(x => x * 10)); // [20, 40, 60]

// 7. Чётные
console.log([1, 2, 3, 4, 5, 6].filter(x => x % 2 === 0)); // [2, 4, 6]

// 8. Сумма reduce
console.log([10, 20, 30, 40].reduce((a, b) => a + b)); // 100

// 9. Найти объект
let users = [
    {id: 1, name: "Anna"},
    {id: 2, name: "Ivan"},
    {id: 3, name: "Olga"}
];
console.log(users.find(u => u.name === "Ivan")); 

// 10. Сортировка
console.log([100, 5, 20, 15].sort((a, b) => a - b));

// ============================================
// ОБЪЕКТЫ - 10 задач (для оценки 3)
// ============================================

// 1. Объект book
let book = {title: "JS", author: "Arthur", year: 2026};
console.log(book.title);

// 2. Добавить pages
book.pages = 300;
console.log(book.pages);

// 3. Удалить year
delete book.year;
console.log(book);

// 4. Поле с пробелом
let student = {"full name": "Ivan Ivanov"};
console.log(student["full name"]);

// 5. Увеличить возраст
let person = {name: "Ivan", age: 30};
person.age++;
console.log(person.age); // 31

// 6. Вложенный объект
let car = {engine: {power: 150, type: "diesel"}};
console.log(car.engine.type);

// 7. Безопасная проверка
console.log(car?.owner?.name ?? "Нет");

// 8. Перебор свойств
let user = {id: 1, login: "root", isAdmin: true};
for (let key in user) {
    console.log(key + ": " + user[key]);
}

// 9. Цена ноутбука
let orders = {
    id1: {product: "Phone", price: 500},
    id2: {product: "Laptop", price: 1500}
};
console.log(orders.id2


price);

// 10. Значение по ключу
function getValue(obj, key) {
return obj[key];
}
console.log(getValue({name: "Ann"}, "name"));.
    return obj[key];
}
console.log(getValue({name: "Ann"}, "name"));.
