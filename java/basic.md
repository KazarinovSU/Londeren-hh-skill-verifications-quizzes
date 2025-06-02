## Java — Базовый уровень

#### Содержание
* Основы синтаксиса
* Циклы
* Типы данных

🏆 Правильных ответов: 11 из 11.

#### Q1 Какое из объявлений метода main является корректным?
- [x] static public void main(String[] args)
- [ ] public void main(String[] args)
- [ ] public static int main(String[] args)
- [ ] public static void main(String args)
- [ ] public static void main()

#### Q2 Какое значение будет выведено в результате выполнения следующего кода?
```java
int x = 5;
int y = x++;
System.out.println(y);
```
```console
5
```
`x++` — это **постфиксный инкремент**. Значит, сначала возвращается текущее значение `x`, а потом `x` увеличивается на 1. Переменная `y` получает **значение** `x` **ДО увеличения**. После этого `x` станет 6, но `y` уже присвоено старое значение.

#### Q3 Какой из вариантов корректно объявляет и инициализирует символьную переменную?
- [ ] char letter = '65';
- [ ] char letter = 65L;
- [ ] char letter = "A";
- [ ] char letter = A;
- [x] char letter = 'A';

#### Q4 Какое ключевое слово используется для выхода из switch expression и возврата значения?
```java
String msg = switch(grade) {
    case “A” -> {
        System.out.println(“excellent grade”);
        // вернуть “Отличная оценка”
    }
    default -> { ... }
}
```
- [ ] goto
- [ ] break
- [x] yield
- [ ] return
- [ ] default

#### Q5 Выберите НЕсуществующий тип циклов в Java.
- [ ] for each
- [ ] while
- [x] until
- [ ] for
- [ ] do while

#### Q6 xто выведет на экран программа?
```java
for(int i = 1; i <= 3; i++) {
    for(int j = 1; j <= i; j++) {
        System.out.print("*");
    }
    System.out.print(“ “);
}
```
- [ ] *****
- [ ] * *** *****
- [x] * ** ***
- [ ] *** ** *
- [ ] * * *

#### Q7 Какие из способов обращения к статическому методу из другого класса являются корректными?
```java
class Test {
    public static void staticCall() {
        System.out.println(“static call”);
    }
}
public class Main {
    public static void main(String[] args) {
        Test t = new Test();
        t.staticCall();    // 1
        new Test().staticCall();    // 2
        Test.staticCall();      // 3
    }
}
```
- [ ] Только 3
- [ ] Только 2
- [ ] 1 и 2
- [ ] Только 1
- [x] Все верные

#### Q8 Какой из вариантов НЕКОРРЕКТНО инициализирует массив из трех элементов нулями?

- [ ] int [] a = new int[3];
- [ ] int [] a = new int[] {0, 0, 0};
- [ ] Все инициализации корректные
- [x] int [] a = new int[3] {0, 0, 0};
- [ ] int [] a = {0, 0, 0};

#### Q9 Где должен располагаться .java-файл, если класс находится в пакете my.love.is.coding?
- [ ] my.love.is.coding
- [x] my/love/is/coding
- [ ] my/love/is
- [ ] my-love-is-codeing
- [ ] my.love.is
```swift
my/love/is/coding/MyClass.java
```
#### Q10 Выберите правильное утверждение о конструкции try-catch-finally в контексте Java.
- [ ] В конструкции может быть несколько как `try`, так и `catch` блоков
- [ ] Внутри блока `try` обязательно должен быть код, потенциально выбрасывающий проверяемое исключение
- [ ] В конструкции обязательно должен быть `finally` блок
- [ ] В конструкции может быть несколько `try` блоков, но только один `catch` блок
- [x] В конструкции может быть несколько `catch` блоков, но только один `try` блок

#### Q11 Какой класс предназначен для чтения текстовых файлов?
- [ ] `InputStreamReader`
- [x] `FileReader`
- [ ] `BufferedWriter`
- [ ] `OutputStreamWriter`
- [ ] `FileWriter`
