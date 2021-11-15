# Java-Newbie

- Eclipse
New - Class - Name (class 이름 생성) - public static void main (클릭 시 자동생성)
sout 작성 후  Ctrl + Space = System.out.println 단축키


<p align="center"> Java의 동작원리 </p>

1.
![1](https://user-images.githubusercontent.com/91706338/141711934-566ccd70-c833-400f-9b68-c309671fd689.PNG)

2.
![2](https://user-images.githubusercontent.com/91706338/141711941-9574f1ce-b50c-496a-85e4-b90a1900754c.PNG)


Computer > Java Virtual Machine  >  Java Source code .java (Source code는 사람이 이해할 수 있고, 기계는 직접 이해할 수 없음)  
>  (그러므로 기계가 이해할 수 있도록 전환하는 작업을 해야함)  Compile >  
(Source code 작성 후 저장 버튼을 눌렀을 때 자동으로 .class 확장자가 만들어지는데 이것이) Java Application .class   >  
Eclipse에서 RUN 버튼을 클릭 시 Eclipse는 Java Virtual Machine에서 실행 >  Java Virtual Machine은 확장자 class file을읽고 computer로 동작 시키게 됨

<p align="center"> 데이터와 연산 </p>

숫자를 표현하는 source code example

```
public class Datatype {
  public static void main(String[] args) {
    System.out.println(6); // Number
    System.out.println("six"); // String
    System.out.println("6"); // String 6

    // 사람이 보기엔 숫자 6으로 보이지만 큰 따옴표 수식을 넣어줌으로써 컴퓨터는 문자열로 판단함

    System.out.println(6 + 6); // 12 숫자+숫자
    System.out.println("6" + "6"); // 66 더하기가 아닌 결합연산자라고 하는 문자열 연산

    System.out.println(6 * 6); // 36
//    System.out.println("6"*"6"); // 문자열 Data type은 곱하기 연산을 할 수 없음

    System.out.println("1111".length()); // 4
    System.out.println(1111.length()); // 숫자는 길이를 알려주는 연산이 없음
  }
}
```

<p align="center"> 숫자와 연산 </p>

Math. class method = 여러가지 수식 명령을 나타냄

```
public class Number {
  public static void main(String[] args) {
    // Operator
    System.out.println(6 + 2); //8
    System.out.println(6 - 2); //4
    System.out.println(6 * 2); //12
    System.out.println(6 / 2); //3
    
    System.out.println(Math.PI); //3.141592653589793
    System.out.println(Math.floor(Math.PI)); //3.0 소수점 제외
    System.out.println(Math.ceil(Math.PI)); //4.0 ceil = 올림
  }
}
```

<p align="center"> 문자열 다루기 </p>

class 생성 시 String 의 이름은 충돌 날 수 있기 때문에 뒤에 app을 붙여 StringApp으로 생성

```
public class StringApp {
  public static void main(String[] args) {
  
    System.out.println("Hello World"); // String. Character가 모인 것이 String(문자열)
    System.out.println('H'); // Java에서 작은 따옴표는 특수한 Data type, Character(문자) = 한 글자를 표현하는 Data type 
    System.out.println("H"); // String
    
    System.out.println("Hello "
        + "World"); // Java에서 문자열 내리기 Enter
    
    // \n = new line
    System.out.println("Hello \nWorld"); // Java 줄바꿈
    
    // escape 
    System.out.println("Hello \"World\""); // Hello "World"
  }
}
```

```
public class StringOperation {
  public static void main(String[] args) {
    
    System.out.println("Hello World".length()); // 문자열 길이 메소드
    System.out.println("Hello, [[[name]]] ... bye. ".replace("[[[name]]]", "jefi")); // 문자열 치환
    
  }
}
```
<p align="center"> 변수 </p>

- 변수의 효용
```
public class Variable {
  public static void main(String[] args) {
  
  int a = 1; // Number -> integer ... -2, -1, 0, 1, 2 ...
  System.out.println(a);
  
  double b = 1.1; // real number -> double ... -2.0, -1.0, 0, 1.0, 2.0 ...
  System.out.println(b);
  
  String c = "Hello Wolrd";
  System.out.println(c);
  }
}
```

- 변수의 정의
