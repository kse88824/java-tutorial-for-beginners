# Java Tutorial For Beginners
 
**"Learning Java In 150 Steps"** 책에 오신것을 환영합니다.

저는 **Ranga Karanam** 이고, 20년 이상의 프로그래밍 경력을 가지고 있습니다.

저는 프로그래밍을 사랑합니다. ```in28minutes``` 를 시작할 때 저의 목표 중 하나는 프로그래밍을 쉽게 배울 수 있도록 하는 것이었습니다. 저희가 놀라운 강의를 만들 수 있도록 도와주신 전 세계 30만명의 학습자분들께 감사합니다.

**In28Minutes** 에서는, 저희는 매일 "어떻게 하면 멋진 학습 경험을 만들 수 있을까?"하고 스스로에게 묻습니다. 

이 책에서는, 여러분은 Java와 함께 **객체** **지향적** 코드를 배우게 될 것이며, 많은 예제들,실습들, 팁들을 접하게 될 것입니다. 저희는 Java 사용자들을 위해 많은 예시를 들며 코드를 쓰는 방법을 알아보려고 노력할 것입니다.

본 가이드를 개선하는데 도움을 주시려면 - **Fork, Pull Requests, Shares and Likes 를 추천드립니다**!

## Table of Contents

* [Chapter 01 - 프로그래밍 소개와 Print-Multiplication-Table](#프로그래밍-소개와-print-multiplication-table)
* [Chapter 02 - 메소드 이해](#메소드-이해)
* [Chapter 03 - 자바 플랫폼의 이해](#자바-플랫폼의-이해)
* [Chapter 04 - Eclipse](#Eclipse)
* [Chapter 05 - 객체 지향 프로그래밍 (OOP)](#객체-지향-프로그래밍-oop)
* [Chapter 06 - 기본형 타입](#기본형-타입)
* [Chapter 07 - 조건문 소개 - if, switch and more](#조건문-소개---if-switch-and-more)
* [Chapter 08 - 반복문](#반복문)
* [Chapter 09 - 참조형 타입](#참조형-타입)
* [Chapter 10 - Array와 ArrayList](#array와-arraylist)
* [Chapter 11 - 객체 지향 프로그래밍 (*OOP*) - 복습](#객체-지향-프로그래밍-oop---복습)
* [Chapter 12 - 컬렉션의 이해](#컬렉션의-이해)
* [Chapter 13 - 제네릭의 이해](#제네릭의-이해)
* [Chapter 14 - Introduction to Functional Programming](#introduction-to-functional-programming)
* [Chapter 15 - 스레드와 동시 실행](#스레드와-동시-실행)
* [Chapter 16 - 예외처리의 이해](#예외처리의-이해)
* [Chapter 17 - 파일 입출력](#파일-입출력)
* [Chapter 18 - 동시 실행 : 더 나아가기](#동시-실행--더-나아가기)

## 우리의 접근법

왜 학생들이 프로그래밍 공부를 포기할까요?

가장 흔한 대답은

> '첫 프로그램 짜기가 어려워서' 입니다

초보자의 입장에서 이 전형적인 예제를 한번 보세요.

'''Java Hello World Example'''

```java
package com.in28minutes.firstjavaproject; 
public class HelloWorld 
{   
     public static void main(String[] args) {           
            System.out.println("Hello World");   
     } 
}
```

프로그래밍 초보자는 이것에 압도당할 것입니다. 저는 거의 20년전에 이것을 봤을 때 어떤 기분이었는지 기억합니다. 망연자실했죠.

왜냐구요?
- 패키지, public, 클래스, static, void, String[] 등 이보다 더 다양한 키워드와 개념들이 있었습니다.
- 프로그래머가 오타를 낸다면? 고칠 수 있을까요?

**우리는 프로그래밍을 배우기 더 좋은 방법이 있다고 믿습니다.**

- 왜 프로그래밍을 단계별로 배우지 않을까요?
- 왜 재미가 없을까요?
- 많은 예제들을 풀어보면서 프로그래밍을 배운다면?
이것이 본 가이드를 작성하고 Java와 Python을 위한 프로그래밍 입문 과정을 개발하기 위해 저희가 취한 접근법입니다.
> 처음 3시간 강의 이용 가능 [링크](https://courses.in28minutes.com/p/java-tutorial-for-beginner-in-250-steps).


## 프로그래밍 소개와 Print-Multiplication-Table

### Step 01: 첫번째 도전 : Print-Multiplication-Table (*PMT-도전*)
프로그래밍을 배우는 것은 자전거 타는 법을 배우는 것과 비슷합니다. 처음 몇 걸음이 가장 어렵죠.
이러한 순차적 접근법으로 문제를 몇번 풀어보면 습관이 될 거예요.
이 책에서 처음에는, 간단한 문제들과 함께 자바 프로그래밍을 소개할 것입니다.
> 과정이 재밌는 것이 저희의 목표입니다.
_여러분, 첫번째 도전을 시작할 준비가 되셨나요? **그렇다구요?** 시작해봅시다!_
저희의 첫번째 *프로그래밍 도전*은 모든 아이들이 수학시간에 하는 것과 같습니다. 바로 곱셈표 읽기입니다.
####  *PMT-도전*

1. ```1``` 부터 ```10```까지 ```5```단 구구단을 계산하시오
2. 출력하시오.

```
5 * 1  =  5
5 * 2  = 10
5 * 3  = 15
5 * 4  = 20
5 * 5  = 25
5 * 6  = 30
5 * 7  = 35
5 * 8  = 40
5 * 9  = 45
5 * 10 = 50
```

구구단 문제를 해결하려면 다음과 같은 개념들에 대한 소개가 필요합니다.:
* **JShell**
* **문장(Statements)**
* **수식(Expressions)**
* **변수**
* **리터럴(Literal)**
* **조건문**
* **반복문**
* **함수** 

#### 요약

이 단계에서, 우리는:
* 첫번째 도전인 *PMT-Challenge*에 대해 설명하고,
* 이 과제를 해결하기 위해 배울 자바의 기본 개념을 파악할 것입니다.
### Step 02:  ```JShell``` 소개
- - - 

```JShell``` 은 프로그래밍 도구로, Java SE 9에서 소개되었습니다. JShelldms **_REPL_** 인터페이스입니다. **REPL** 의 의미는 다음과 같습니다.
* **_'R'_**  **R**ead(읽기)의 R; 입력된 자바 코드 *읽기* 
* **_'E'_**  **E**val(평가)의 E; 소스코드 *평가* 
* **_'P'_**  **P**rint(출력)의 P; 결과값 *출력* 
* **_'L'_**  **L**oop(반복문)의 L; *반복*하며 다음 입력을 기다림

자바를 시작해보니 어떤가요? 계속 해볼까요?
##### Snippet-1: 자바 개발 환경 확인하기

첫 25단계의 코드를 실행시키기 위해 [https://tryjshell.org/](https://tryjshell.org/) 혹은 [Install Java 12+](https://github.com/in28minutes/java-a-course-for-beginners/blob/master/00-02-java-eclipse-installation.md#installing-java) 를 사용할 수 있습니다.
문제가 생겼을 때는 다음 페이지를 확인해 주세요. [troubleshooting section](https://github.com/in28minutes/java-a-course-for-beginners/blob/master/00-02-java-eclipse-installation.md#troubleshooting)


명령 프롬프트나 터미널을 설치하세요

터미널에 ```java -version``` 를 입력하고 엔터를 누르세요.

```

	in28minutes$>java -version
	java version "x.0.1"
	Java(TM) SE Runtime Environment (build x.0.1+11)
	Java HotSpot(TM) 64-bit Server VM (build x.0.1+11, mixed mode)
	in28minutes$>

```

성공적으로 실행하면 시스템에 설치된 Java 버전이 표시됩니다. 이 책을 읽으려면 최소한 자바 9가 필요합니다.
##### Snippet-2: JShell 설치

터미널에 ```jshell``` 을 검색해서 설치 할 수 있습니다. 

```java

	in28minutes$>jshell

	|  Welcome to JShell version x.0.1
 	|  For an introduction type: /help intro
	jshell>
	
```

실행 시, 이 명령은 설치된 ```JShell```에 대한 기본적인 정보를 표시합니다. 그리고 당신의 입력을 기다리는 ```jshell``` 프롬프트가 나타납니다.
##### Snippet-3: 내장 명령어를 이용한 JShell 입력 예시

```intro```라는 매개 변수를 가진 ```JSHell```의 명령 ```/help``` 는 이 도구를 사용하는 방법에 대한 기본적인 지침을 제공합니다.

```java

	jshell> /help intro

	|
	| intro
	| The jshell tool allows you to execute Java code, getting immediate results.
	| You can enter a Java definition (variable, method, class, etc), like: int x =8
	| or a Java expression, like: x + x
	| or a Java statement or import.
	| These little chunks of Java code are called 'snippets'.
	| There are also jshell commands that allow you to understand and
	| control what you are doing, like: /list
	|
	| For a list of commands: /help
	
	jshell>

```


##### Snippet-4: 수식(Expression) 평가

JShell 프롬프트에 ```3+4``` 를 입력하세요

```java

	jshell> 3 + 4
	$1 ==> 7
	jshell>

```

이것이 여러분의 진짜 첫번째 **REPL** 사이클입니다! ```3 + 4```를 입력했을 때, JShell은 그것을 계산하고 결과를 출력합니다.
> Entity ```$1``` 는 결과에 실제로 부여된 변수 이름입니다. 이것은 나중에 알아보도록 합시다. 

##### Snippet-5: JShell에서 빠져나오기

 ```/exit``` 명령어를 입력하면 ```JShell``` 프로그램을 종료하고 터미널 프롬프트로 돌아갑니다.


```java

	jshell> /exit
	|  Goodbye
	
	in28minutes$>

```


##### Snippet-6: 다시 JShell에 들어가고 빠져나와 봅시다!

이제 손쉽게 시작하고, 코드를 작성하고 , ```JShell```을 탈출할 수 있습니다.

```java

	in28minutes$> jshell
	
	|  Welcome to JShell version 9.0.1
	|  For an introduction type: /help intro
	jshell> /exit
	|  Goodbye
	
	in28minutes$>

```

#### 요약

이번 단계에서 우리가 배운 것들은 다음과 같습니다:

* ```JShell``` 설치하고 명령어 몇가지 실행하기
* ```JShell``` 프롬프트에서 자바 코드 실행하기

### Step 03: 문제를 풀어봅시다.

 *PMT-Challenge* 문제를 해결해봅시다.

```
5 * 1  =  5
5 * 2  = 10
5 * 3  = 15
5 * 4  = 20
5 * 5  = 25
5 * 6  = 30
5 * 7  = 35
5 * 8  = 40
5 * 9  = 45
5 * 10 = 50
```


우리의 초안은 다음과 같습니다.
* ```5 * 3``` 를 계산하고 결과 ```15```를 출력한다.
* ```5 * 3 = 15``` 출력한다.(```15```는 이전 연산의 결과물)
* 각 테이블에 대한 연산을 열번 수행한다.( ```1``` 부터 ```10``` 까지)

#### 요약

이 단계에서

* *PMT-Challenge* 문제를 sub -problem으로 분해

### Step 04: 수식(Expressions) 소개

우리의 *PMT-Challenge*를 해결하는 첫 번째 부분은 ``5"와 ``3"이라는 또 다른 숫자를 계산하는 것이다.
jshell을 시작하고 ```5 X 3```을 입력해보자.

```java

	in28minutes$> jshell

	|  Welcome to JShell version x.0.1
	|  For an introduction type: /help intro
	jshell> 5 X 3
	| Error:
	| ';' expected
	| 5 X 3
	|  ^
	| Error:
	| not a statement
	| 5 X 3
	|   ^
	| Error:
	| ';' expected
	| 5 X 3
	|    ^
	| Error:
	| missing return statement
	| 5 X 3
	| ^---^
```
여러분은 학교에서 배운 것을 생각하면서 부호 'X'를 곱하기 처럼 보고 있을 것이다.
자바는 곱셈 연산자로 '```X```'를 사용하지 않는다! 자바는 곱셈을 지원하지만, *미리 약속된* ```*``` 연산자 만을 사용해야 한다.
아래에 표시된 코드를 입력해봅시다:

```java
	jshell> 5 * 3
	$1 ==> 15
	jshell>

```

성공!

몇가지 용어들을 살펴보자
- ```5 * 3 ``` 는 수식이다.
- ```5``` 와 ```3``` 은 피연산자이다. **리터럴** 혹은 상수로도 불린다.
- ```*``` 는 연산자이다.

자바는 숫자를 다루는 작업을 처리하기 위한 내장 연산자를 더 많이 가지고 있습니다.
* 덧셈: ```+``` 
* 뺄셈: ```-```
* 나눗셈: ```/```
* 모듈러 연산: ```%``` 

다음 예제는 연산자들을 어떻게 사용하는지 그 예를 보여줍니다. 

```java

	jshell> 5 * 10
	$2 ==> 50
	jshell> 5 + 10
	$3 ==> 15
	jshell> 5 - 10
	$4 ==> -5
	jshell> 10 / 2
	$5 ==> 5
	jshell>

```

여러분들은 학교에서 배운 수학을 아직 잘 기억하고 있고,  ```+```, ```-``` 와 ```/``` 는 아주 기본적인 것들이니까요.
```%``` 는 모듈러 연산으로, 정수의 나눗셈을 수행한 나머지를 결과로 보여줍니다.

```java

	jshell> 9 % 2
	$6 ==> 1
	jshell> 8 % 2
	$7 ==> 0
	jshell>

```

##### Snippet: 복잡한 수식(Exprssion), 도전해볼까요?

자바에서는 수식에서 한 개 이상의 연산자를 사용할 수 있습니다.
다중 연산자를 이용한 예를 살펴봅시다.

```java
 
	jshell> 5 + 5 + 5
	$8 ==> 15
	jshell> 5 + 10 - 15
	$9 ==> 0
	jshell> 5 * 5 + 5
	$10 ==> 30
	jshell> 5 * 15 / 3
	$11 ==> 25

```

위의 각 수식에는 두 개의 연산자와 세 개의 피연산자가 있습니다.

#### 요약

이번 단계에서는
* 숫자 수식을 구성하는 방법을 알아보았습니다.
* 연산자가 미리 정의된 기호임을 알아보았습니다.
* 여러 연산자를 결합하여 더 긴 표현식 구성해보았습니다.

### Step 05: 프로그래밍 실습 PE-1 (솔루션 포함)

이 단계에서, 당신의 미소는 당신이 자바 수식을 평가하는 것을 즐긴다는 것을 말해줄 것입니다. 

여기 두 개의 프로그래밍 실습 예제가 있습니다.

1. 하루가 몇 분인지 계산하는 식을 작성하시오.
2. 하루가 몇 초인지 계산하는 식을 작성하시오.

####  솔루션 1

60 (한 시간은 60분) 과 24를 곱한다  (하루는 24시간)

```java

	jshell> 60 * 24
	$1 ==> 1440
```

#### 솔루션 2

60 (1분은 60초)과 60 (한 시간은 60분) 그리고 24를 곱한다. (하루는 24시간)

```java
$jshell>60 * 60 * 24

$1 ==> 86400
```

### Step 06: 연산자

연산자를 이해하기 위해 몇 가지 예제들을 더 살펴봅시다.

#### 유효하지 않은 연산자

 JShell에 ```5 ** 6```에 이어 ```5 $ 6```를 입력해봅시다.
 
```java
	jshell> 5 ** 6
	| Error:
	| Illegal start of expression
	| 5 ** 6
	|     ^

	jshell> 5 $ 6 
	| Error:
	| ';' expected
	| 5 $ 6
	|  ^
	| Error:
	| not a statement
	| 5 $ 6
	|   ^
	| Error:
	| ';' expected
	| 5 $ 6
	|    ^

	jshell> 5 */ 6
	| Error:
	| Illegal start of expression
	| 5 */ 6
	|     ^
	
```

```JShell``` 은 우리의 노력에 전혀 응답하지 않았다!

자바에는 **syntax**라고 불리는 일련의 문법 규칙이 있습니다. 이 규칙을 따르지 않는 코드는 오류를 발생시킵니다. 컴파일러는 오류를 나열하여 알려주고, 오류를 수정할 수 있는 방법에 대한 힌트도 제공합니다. 

그럼, 오류는 왜 발생하는가?

자바에 있는 연산자는 모두 사전에 정의되어 있으며, 수가 제한되어 있다. ``*"는 유효한 연산자인 반면 ``**"와 ``$"는 오류 메시지와 함께 거부당했다.

#### 혼합형 수식의 결과 이해

또 다른 코드를 살펴봅시다.

```java

	jshell> 5 / 2
	$1 ==> 2
	jshell>

```

놀랍게도 ```JShell```은  ``` 5 / 2 ```를  ```2.5```가 아닌 ``` 2 ```로 계산했다! 어디서 잘못된 걸까?

다음 내용을 자세히 살펴보자

**평가된 수식의 결과는 연산자의 실행 문맥에 따라 달라진다**. 여기서 문맥은 그것에 전달된 피연산자에 의해 결정된다.
프로그래밍에 일반적으로 사용되는 숫자의 종류는 정수 (1,2,3,...)나 부동 소수점 (1.1,2.3,56.7889 등)이다.
이러한 값들은 자바에서 서로 다른 **타입**으로 표현됩니다. 정수는 흔히 ```int```형이고, 부동 소수점은 기본적으로 ```double```형입니다.
수식 ```5/2```에서 ```5```와 ```2```는 ```int```형이기 때문에 결과 또한 ```int```형으로 표현됩니다.

부동 소수점 숫자를 사용해보자.

```java

	jshell> 5.0 / 2.0
	$2 ==> 2.5
```
```5.0``` 와 ```2.0``` 모두 ```double```형이기 때문에, 결과  또한 ```double```형이다. 그렇다면 우리는 ```2.5```를 얻을 수 있을 것 같다.

부동 소수점과 정수를 혼합하여 연산을 해보자.

```java
	jshell> 5.0 / 2
	$3 ==> 2.5
	jshell>

```

```int```형과 ```double```형 중에서, ```double```형이 더 *넓은 타입*으로 간주됩니다. 두가지 타입 간에 연산을 수행할 때는 더 넓은 타입으로 결과를 표시합니다. 



#### 연산자 우선 순위 이해

두 개 이상의 연산자가 있는 수식의 복잡한 예를 몇 가지 살펴보자.

```java

	jshell> 5 + 5 * 6
	$1 ==> 35
	jshell> 5 - 2 * 2
	$2 ==> 1
	jshell> 5 - 2 / 2
	$3 ==> 4
	jshell>

```

결과를 보고 놀랐습니까?  여러분은 아마 5 + 5 * 6 에서  10 * 6 을 계산하는 것. 즉, 60을 예상했을 것이다. 그러나 ```35```가 나왔다! 

> 우리는 영어 왼쪽에서 오른쪽으로 쓰고, 이 습관을 계산에도 적용합니다.

_여러 연산자 식에서 하위수식의 평가 순서는 **연산자 우선 순위**에 따라 달라진다._

연산자 우선 순위에 대한 기본 규칙은 사실 매우 간단합니다.(조금 후에 다른 규칙을 살펴보자).

 {```*```, ```/```, ```%```} 이 연산자 모음은 {```+```, ```-```} 연산자 모음보다 높은 우선 순위를 가지고 있습니다 .

``5 + 5 * 6"이라는 수식에서 5*6을 먼저 계산합니다. 따라서 5 + 5 * 6은 5 + 30이 된다. 즉, 결과는 35이다.

``5 - 2 * 2"와 ``5 - 2 / 2"는 같은 규칙을 따라 계산합니다.

#### 명확한 코드를 위해 괄호 사용하기

자바는 수식의 일부를 묶기 위해 **괄호**라고 불리는 ```(```와 ```)```를 제공합니다. 

```java

	jshell> (5 - 2) * 2
	$4 ==> 6
	jshell> 5 - (2 * 2)
	$5 ==> 1
	jshell>

```

괄호 안에 식을 넣으면 해당 식이 먼저 계산됩니다.  (5 - 2) * 2 => 3 * 2 => 6.
 
괄호는 혼동을 줄이고 오류를 방지하므로 가독성을 향상시킵니다

옛 속담 ***제때의 바늘 한번이 아홉 바느질을 던다 (호미로 막을 것을 가래로 막는다)*** 를 잘 기억해야 합니다. 사소한 경우에도 코드를 쉽게 읽을 수 있도록 괄호를 사용합시다.

#### 요약

이 단계에서는

* 연산자는 모두 사전에 정의되었다는 것을 확인했습니다.
* 연산 결과는 피연산자의 타입에 따라 결정된다는 것을 알게 되었습니다.
* 연산자 우선 순위의 의미 이해했습니다.
* 표현식의 일부를 그룹화하는 데 괄호 사용했습니다.
 
### Step 07: 콘솔 출력 소개

우리는 이전 단계에서 두개의 리터럴(```5 * 3```)의 산출물을 계산했습니다.

다음 단계는 이 결과를 ```5 * 3 = 15```라는 맞춤형 형식으로 출력할 것입니다.

어떻게 할까요?

JShell에 다음과 같이 입력해봅시다.

```java
jshell> 5 * 3 = 15
|  Error:
|  unexpected type
|    required: variable
|    found:    value
|  5 * 3 = 15
|  ^---^
```

음.. 에러가 발생했네요.

텍스트를 출력하려면 어떻게 해야 할까요?

자바에는 콘솔에 텍스트를 표시하는 ```System.out.println()```이라는 유틸리티 방식이 내장되어 있습니다.

```java
jshell> System.out.println(3*4)
12
```

우리는 ```3*4```라는 표현을 만들어  ```System.out.println()```에게 넘겨주었는데, 이것을 자바에 내장된 **메소드**라고 한다.
```System.out.println(3*4)``` 는 **문장(statement)**의 예시이다. 이것을 **메소드 호출**이라고 부른다.

메소드 호출에 대한 구문 규칙은 상당히 엄격하며, 그 모든 부분은 의무적이다.

```java
jshell> System.out.println3*4)
| Error:
| ';' expected
| System.out.println3*4)
|___________________^
| Error:
| cannot find symbol
|       symbol: variable println3
| System.out.println3*4)
| ^---------------------^

jshell> System.out.println 3*4
|  Error:
|  ';' expected
|  System.out.println 3*4
|                    ^
|  Error:
|  cannot find symbol
|    symbol:   variable println
|  System.out.println 3*4
|  ^----------------^

```

*PMT-Challenge*에 대한 솔루션의 일부로 곱셈표 항목을 출력하려면 어떻게 할 것인가? 즉, 콘솔에 있는 ``5 * 2 = 10"이라는 정확한 문자를 어떻게 출력할 것인가?

```java

	jshell> System.out.println(5 * 2 = 10)
	| Error:
	| unexpected type
	| required:  variable
	| found:     value
	| System.out.println(5 * 2 = 10)
	|____________________^--------^

```

여러분은 콘솔에 ```5 * 2 = 10```를 출력하고 싶다. 하지만, 우리는  ```System.out.println()``` 로 ```5 * 2 = 10``` 를 넘길 수 없다.

```5 * 2 = 10```는 하나의 값이 아니다. 그것은  ```*``` and ```=```라는 문자들로 이루어져있다. 

자바에서는 ```String```을 사용하여 문자를 표기한다. ```String literal```은 일련의 문자들로 **큰 따옴표**: ```"```와 ```"```로 둘러싸여 있다.

```java
	jshell> System.out.println("5 * 2 = 10")
	| 5 * 2 = 10
```

축하합니다! 여러분은 이제 콘솔에 숫자뿐만 아니라 문자도 표시하는 방법을 알아냈답니다!

#### 요약

이번 단계에서는

* 콘솔 출력을 위한 ```System.out.println()``` 메소드 사용방법을 알아보았다.
* 이 유틸리티를 하나의 *PMT-Challenge* 테이블 항목 출력하는데 사용할 수 있다.


### Step 08: 프로그래밍 실습 PE-02

다음 실습을 수행해보시오:

1. 콘솔에 ```Hello World``` 출력한다.

2. ```5 * 3```을 그대로 출력한다.

3.   5 * 3의 계산 결과를 출력한다.

4. ```System.out.println```메소드를 사용하여 하루는 몇 초인지 출력하시오.

5.위의 각 실습에 대해 작성하는 코드에 대한 구문 수정을 수행하십시오. 코드에서 다음 요소를 식별하십시오.
* 숫자 및 문자열 리터럴
* 수식
* 연산자
* 피연산자
* 메소드 호출

### Step 09:  PE-02의 솔루션

#### Solution 1

```java

	jshell> System.out.println("Hello World")
	Hello World

```

#### Solution 2

```java

	jshell> System.out.println("5 * 3")
	5 * 3
	jshell>
```

#### Solution 3

```java

	jshell> System.out.println(5 * 3)
	15

```

#### Solution 4

```java

	jshell> System.out.println(60 * 60 * 24)
	86400

```

### Step 10: White Space: 대소문자 구분 및 공백 문자
*공백(White space)*은 연속 공백, 탭 또는 줄 바꿈 문자의 순서를 가리킨다.

#### 공백

공백의 몇 가지 예를 보자.

공백 문자열 리터럴 사용 시 출력에 영향을 미친다.

```java
jshell> System.out.println("Hello World")
Hello World
jshell> System.out.println("Hello      World")
Hello      World
jshell> System.out.println("HelloWorld")
HelloWorld
```


컴파일러는 숫자 수식에 사용된 공백은 무시한다.

```java

	jshell> System.out.println(24 * 60 * 60)
	86400
	jshell> System.out.println(24    *    60    *    60)
	86400
	jshell>

```

#### 대소문자 구분

자바는 대소문자를 구분한다.

```System.out.println()```는 사전에 정의된 자바 요소들을 포함한다 : ```System```은 **클래스** 이름이고,  ```out```은 **변수** 이름이며, ```println```은 **메소드** 이름이다.이들은 모두 *대소문자를 구분*한다. 이 이름에서 어느 하나라도 다른 대소문자가 사용되면 오류가 발생한다.

```java

	jshell> system.out.println("Hello World")
	| Error:
	| package system does not exist
	| system.out.println("Hello World")
	| ^-------^

	jshell> System.Out.println("Hello World")
	| Error:
	| cannot find symbol
	| symbol: variable Out
	| System.Out.println("Hello World")
	| ^------------^

	jshell> System.out.Println("Hello World")
	| Error:
	| cannot find symbol
	| symbol: method Println(java.lang.string)
	| System.out.Println("Hello World")
	| ^---------------------^

	jshell>

```

문자열 리터럴 안에서 문자의 경우는 오류를 일으키지 않는다. 문자 그대로 받아 출력할 것이다

```java
jshell> System.out.println("hello world")
hello world
jshell> System.out.println("HELLO WORLD")
HELLO WORLD
```

#### 특수문자 리터럴
**특수문자 리터럴**은 다른 정규 기호와 함께 사용되는 특수 기호(이스케이프 시퀀스)이다. 자바에서는 ```\```(*백슬래시*)가 탈출 문자 역할을 한다. 이 이스케이프 시퀀스는 기호의 원래 용도를 바꾼다.

If you want to print the string **delimiter**, the ```"``` character, you need to escape it with a ```\```. Without it, a ```"``` character within a string literal causes an error!
문자열을 분리할 때 사용되는 기준 문자인 **구분 문자**(delimiter)를 출력하려면 ```\```와 함께 사용해야 한다. 백슬래시가 없으면  ```"```문자가 있는 문자열이 오류를 일으킨다!

```java

	jshell> System.out.println("Hello "World")
	| Error:
	| ')' expected
	| System.out.println("Hello "World")
	|                            ^

	jshell> System.out.println("Hello \"World")
	Hello "World
	jshell>

```

이스케이프 시퀀스 ```\n```은 *새로운 줄*을 삽입한다.

```java

jshell> System. out.println("Hello \n World")
Hello
 World
jshell> System.out.println("Hello n World")
Hello n World
jshell> System.out.println("Hello\nWorld")
Hello 
World
jshell>

```

이스케이프 시퀀스 ```\t```은 *탭*을 삽입한다.

```java

	jshell> System.out.println("Hello \t World")
	Hello    World
	jshell> System.out.println("Hello t World")
	Hello t World
	jshell> System.out.println("Hello\tWorld")
	Hello    World
	jshell>

```

```\```는 어떻게 출력하는가?

```
jshell> System.out.println("Hello \ World")
|  Error:
|  illegal escape character
|  System.out.println("Hello \ World")
```

또 다른 ```\```와 함께 입력해야 한다. ```\\```를 입력하면 기호 ```\```가 콘솔창에 출력된다.

```java

	jshell> System.out.println("Hello \\ World")
	Hello \ World
	jshell> System.out.println("Hello \\\\ World")
	Hello \\ World

```


#### 요약

이번 단계에서는

* ```System.out.println()```과 함께 메소드 호출 구문을 알아보앗다.
* 공백 문자의 사용법 발견하였다
* Java 이스케이프 시퀀스에 대해 알아보았다

### Step 11: 메소드 호출 더 알아보기

Let's look at method calls with a few more examples.
메소드 호출에 대한 몇가지 예시를 더 살펴보자.

You know how to invoke a method with a single argument, courtesy  Other scenarios do exist, such as 
* Calling a method without any arguments
* Calling a method with several arguments
당신은 ```System.out.println(3*4)```이라는 단 하나의 구문으로 어떻게 메소드를 호출할 수 있는지 알고 있다. 다음과 같은 다른 시나리오가 존재한다.
* 인수 없이 메소드 호출
* 여러 인수를 사용하여 메소드 호출

자바 ```Math``` 클래스에 내장된 방법을 사용하여 그들을 살펴보자.


#### 매개 변수가 없는 메소드

메소드를 호출할 때, 괄호는 구문에서 꼭 필요하다. 잊지말자!

```Math.random()``` 는 호출할 때마다 ```[0 , 1]``` 범위 내에서 임의의 숫자 하나를 출력한다. 

```java

	jshell> Math.random
	| Error:
	| cannot find symbol
	|    symbol: Math.random
	| Math.random
	| ^------------- ^
	jshell> Math.random()
	$1 ==> 0.0424279106074651_
	jshell> Math.random()
	$2 ==> 0.8696879746593543 
	jshell> Math.random()
	$3 ==> 0.8913591586787125
```


#### 여러 개의 매개 변수를 가진 메소드

```23```과 ```45```라는 두개의 매개 변수를 가지고 어떻게 ```Math.min```을 호출할 것인가? 

```java

	jshell> Math.min 23 45
	| Error
	| cannot find symbol
	| symbol: variable min
	| Math.min 23 45
	| ^---------^
	jshell> Math.min(23 45)
	| Error
	| ')' expected
	| Math.min 23 45
	| ---------------^
```

메소드를 호출할 때, 프로그래머가 반드시 지켜야 할 것들이 있다.
* 모든 매개 변수는 반드시 괄호 안에 작성해야 한다.
* 목록 내에서 각각의 파라미터들은 ```,```로 구분한다.

```java
	jshell> Math.min(23, 45)
	$4 ==> 23
	jshell> Math.min(23, 2)
	$5 ==> 2
	jshell> Math.max(23, 45)
	$6 ==> 45
	jshell> Math.max(23, 2)
	$7 ==> 2
	jshell>

```

```Math.min()```은 주어진 두 개의 숫자 중 최솟값을 반환한다. ```Math.max()```는 주어진 두개의 숫자 중 최댓값을 반환한다.

#### 요약

이번 단계에서는
* 메소드를 호출할 때, 매개 변수가 0개 혹은 여러개의 매개 변수가 전달되는 방법을 이해했다.

### Step 12: 출력 형식 더 알아보기

```System.out.println()```는 최대 한 개의 값을 인자로 받아들일 수 있다. 

계산된 값으로 ``5"의 곱셈표를 표시하려면 숫자와 문자열을 모두 출력하는 방법이 필요하다.
이를 위해서는 또 다른 내장 메소드 ```System.out.printf()```를 사용할 수 있다.

.
```System.out.printf()```는 *단일* 문자열 인수와 함께 호출될 때, 읽을 수 없는 정보를 출력한다. 현재로서는 이 정보가 내장형 ```java.io.PrintStream```에 관한 정보라는 것만 알면 된다.


```java
	jshell> System.out.printf("5 * 2 = 10")
	5 * 2 = 10$1 ==> java.io.PrintStream@4e1d422d
	jshell>

```

다행인 것은 우리가 ```println()"을 호출하면 읽기 어려운 것들이 사라진다는 점이다.

```java

	jshell> System.out.printf("5 * 2 = 10").println()
	5 * 2 = 10
```

```System.out.printf()```라는 메소드는 다음과 같은 다양한 인수들 수용한다.

* 첫 번째 인수는 출력 형식을 지정한다. 이는 문자열 리터럴이며, **형식 지정자**가 0개 이상 있다. 형식 지정자는 특정 유형의 데이터("%d" 와 같은)를 포맷하는 사전 정의된 문자("%d" 형식 데이터(""int" 형식)이다.
형식 지정자는 ```%d```가 데이터 타입을 ```int```로 지정하는 것과 같이 특정 유형의 데이터를 포맷하는 리터럴이며, 이 또한 사전에 정의되어 있다.
* 뒤에 있는 인수는 수식이며,

이론이 너무 많은가? 하나씩 알아보자. 예시를 살펴보자

```java
	jshell> System.out.printf("5 * 2 = %d", 5*2).println()
	5 * 2 = 10
	jshell>

```
```System.out.printf("5 * 2 = %d", 5*2).println()``` 는 ```5 * 2 = 10```를 출력한다.  ```%d``` 는```5*2```의 연산 결과의 자리를 대신한다.

```printf```에 대해 조금만 더 알아보자

```java

	jshell> System.out.printf("%d %d %d", 5, 7, 5).println()
	5 7 5
```

연산 결과를 표시해보자. 예시에서 ```5*7```은 ```35```로 계산되었다.

```java
	jshell> System.out.printf("%d %d %d", 5, 7, 5*7).println()
	5 7 35
```

이를 통해 곱셈표에 사용할 형식으로 내용을 출력해 봅시다.

```java
	jshell> System.out.printf("%d * %d = %d", 5, 7, 5*7).println()
	5 * 7 = 35
```

축하합니다! 우리는 ```5*7```을 계산하고 ```5 * 7 = 35```를 성공적으로 출력할 수 있게 되었다!

#### 실습

1. Print the following output on the console: ```5 + 6 + 7 = 18```. Use three literals ```5```, ```6```, ```7```. Calculate 18 as ```5 + 6 + 7```.
1. 콘솔에 다음의 결과물을 출력력하시오: 
 ```5 + 6 + 7 = 18```.
 ```5```,```6```,```7``` 세 리터럴을 사용하시오.
 18을 ```5 + 6 + 7```로 계산하시오

#### 솔루션

```java

	jshell> System.out.printf("%d + %d + %d = %d", 5, 6, 7, 5 + 6 + 7).println()
	5 + 6 + 7 = 18
	jshell>

```

####  ```System.out.printf()``` 사용해보기

아래의 예시에서는 네 개의 형식 지정자(```%d```)가 있으며 인자는 ```5, 6, 7```세 개이다.

```java

	jshell> System.out.printf("%d + %d + %d = %d", 5, 6, 7).println()
	5 + 6 + 7 = | java.util.MissingFormatArgumentException thrown: Format specifier '%d'
	| at Formatter.format (Formatter.java:2580)
	| at PrintStream.format (PrintStream.java:974)
	| at PrintStream.printf (PrintStream.java:870)
	| at (#52:1)
```

```System.out.printf()```를 호출할 때, 형식 지정자의 수가 뒤에 있는 인자의 수를 초과하면 자바 런타임은 *예외*를 던진다.

형식 지정자의 수가 인자의 수보다 적으면, 컴파일러는 초과된 인수만 무시한다.

```java

	jshell> System.out.printf("%d + %d + %d", 5, 6, 7, 8).println()
	5 + 6 + 7
	jshell>

```

#### 형식 지정자 더 알아보기

문자열은 ```System.out.printf()```를 사용해서 출력할 수 있고, 형식 지정자는 ```%s```를 사용한다.

```java

	jshell> System.out.printf("Print %s", "Testing").println()
	Print Testing

```

앞서, 우리는 %d를 이용해 ```int```값을 출력했다. 하지만  %d로는 부동 소수점을 표시할 수 없다.

```java
	jshell> System.out.printf("%d + %d + %d", 5.5, 6.5, 7.5).println()
	| java.util.IllegalFormatConversionException thrown: d != java.lang.Double
	| at Formatter$FormatSpecifier.failedConversion(Formatter.java:4331)
	| at Formatter$FormatSpecifier.printInteger(Formatter.java:2846)
	| at Formatter$FormatSpecifier.print(Formatter.java:2800)
	| at Formatter.format(Formatter.java:2581)
	| at PrintStream.format(PrintStream.java:974)
	| at PrintStream.print(PrintStream.java:870)
	| at #(57:1)

```

부동 소수점 리터럴(혹은 수식)은 ```%f```를 사용하여 형식을 지정할 수 있다.

```java

	jshell> System.out.printf("%f + %f + %f", 5.5, 6.5, 7.5).println()
	5.500000 + 6.500000 + 7.500000
	jshell>

```

#### 요약

이번 단계에서는

* ```System.out.printf()```를 사용하여 형식이 지정된 출력을 표기하는 방법을 알아보았다.
* 형식을 지정하기 위해서는 인자의 수와 순서가 중요하다. 
* 기본형 타입을 위해 내장된 형식 지정자에 대해 알아보았다.

### Step 13: 변수에 대한 소개

이전 단계에서는, 곱셈표의 일부로 계산된 값을 어떻게 출력하는지 알아보았다.

```java
	jshell> System.out.printf("%d * %d = %d", 5, 1, 5 * 1).println()
	5 * 1 = 5
```

**전제 곱셈표는 어떻게 출력할까?**

다음과 같이 해볼 수 있다.

```java
	jshell> System.out.printf("%d * %d = %d", 5, 1, 5 * 1).println()
	5 * 1 = 5
	jshell> System.out.printf("%d * %d = %d", 5, 2, 5 * 2).println()
	5 * 2 = 10
	jshell> System.out.printf("%d * %d = %d", 5, 3, 5 * 3).println()
	5 * 3 = 15
	jshell> System.out.printf("%d * %d = %d", 5, 4, 5 * 4).println()
	5 * 4 = 20
	jshell>

```

Too much work. Isn't it?
일이 너무 많지 않은가?

코드를 유심히 살펴보면, 구문들이 비슷하다는 것을 알 수 있다.
***무엇이 다른가?*** 매개 변수의 세 번째와 네 번째 숫자가 1부터 4로 변경된다. 
이렇게 값이 변하는 것을 다르게 표현하면 더 좋지 않을까?

***변수에 대해 알아보자***

```java

	jshell> int number = 10
	number ==> 10
	jshell>

```

#### 용어 및 배경지식

 ```int number = 10```라는 구문에서,  
* ```number```은 **변수** 이다. 
* 리터럴인 ```number``` 는 변수의 **이름**이다.
* 자바의 *키워드*인 ```int``` 는  ```number```의 **타입**을 지정한다.
* 리터럴 ```10``` 은 ```number```의 **초깃 값**을 제공한다. 
* 이 구문은  **변수 선언**이다.

이 변수 선언이 미치는 영향은 다음과 같다:
* 컴퓨터 메모리의 특정 위치는 ```number```로 지정되었다.
* 이 위치는 이제 ```int```형 타입의 데이터가 저장될 수 있다.
* ```10```이라는 값은 이곳에 저장된다.

숫자 변수의 값을 변경할 수 있다:

```java

	jshell> number = 11
	number ==> 11
```

위와 같은 구문을 변수**할당**이라고 한다. 

할당으로 인해 메모리의 해당 위치에 저장된 값이 변경된다. 이 경우에는, ```10```은 ```11```로 대체된다.

number 변수의 값을 확인해보자.

```java
	jshell> number
	number ==> 11
```

변수의 값을 여러 번 변경할 수 있다.

```
	jshell> number = 12
	number ==> 12
	jshell> number
	number ==> 12

```

또 다른 변수를 생성해보자.
	
```java

	jshell> int number2 = 100
	number2 ==> 100
	jshell> number2 = 101
	number2 ==> 101
	jshell> number2
	number2 ==> 101
	jshell>

```

```int number2 = 100```이라는 구문은 변수```number2```를 *명확히* 정의하고 있다.

*** 어떻게 하면 변수를 사용해 *PMT-Challenge*를 더 간단하게 개선시킬 수 있을까?*** 
어디 한번 보자

```java

	jshell> System.out.printf("%d * %d = %d", 5, 4, 5*4).println()
	5 * 4 = 20
```

변수 ```i```를 정의하고 이 값을 ```1```로 초기화한다.

```java
	jshell>int i = 1
	i ==> 1
	jshell> i
	i ==> 1
	jshell> 5*i
	$1 ==> 5
```

곱셈표를 출력할 때, 변수 i를 사용하도록 개선해보자.

```java
	jshell> System.out.printf("%d * %d = %d", 5, i, 5*i).println()
	5 * 1 = 5
```

***```5 * 2 = 10```는 어떻게 출력할 것인가?***

```i```를 ```2```로 업데이트하고 이전과 같은 코드를 실행해본다.

```java

	jshell> i = 2
	i ==> 2
	jshell> 5*i
	$2 ==> 10
	jshell> System.out.printf("%d * %d = %d", 5, i, 5*i).println()
	5 * 2 = 10
	jshell>

```


```i```를 어떤 숫자로도 업데이트할 수 있다.

이전 구문은 배수를 5로 하여 출력할 것이다.


```java

	jshell> i = 3
	i ==> 3
	jshell> System.out.printf("%d * %d = %d", 5, i, 5*i).println()
	5 * 3 = 15
	jshell> i = 10
	i ==> 10_
	jshell> System.out.printf("%d * %d = %d", 5, i, 5*i).println()
	5 * 10 = 50
	jshell>

```

```i```값을 다양화해서, 우리는 같은 구문으로 5의 서로 다른 곱들을 출력할 수 있다.
변수라는 중대한 발견을 한 것을 축하한다! 

#### 요약

이번 단계에서는


* 변수의 필요성에 대해 이해했다.
* 변수 선언의 각 부분이 무엇을 의미하는지 살펴보았다.
* 변수가 선언될 때, 뒷부분에서는 무슨 일이 일어나는지 알아보았다.

### Step 14: 프로그래밍 실습 PE-03 (솔루션 포함)


1. ```a```, ```b```, ```c```라는 세 개의 정수형 변수를 생성한다.
	* 이 세 개의 변수들의 합을 출력하는 구문을 작성하시오.
	* ```a```의 값을 변경한 후, 이들의 합을 출력하시오.
	* 다시 ```b```의 값을 변경한 후, 이들의 합을 출력하시오.

#### PE-03 솔루션

```java 

	jshell>int a = 5
	a ==> 5
	jshell>int b = 7
	b ==> 7
	jshell>int c = 11
	c ==> 11
	jshell>System.out.printf("a + b + c = %d", a+b+c).println()
	a + b + c = 23
	jshell>a = 2
	a ==> 2
	jshell>System.out.printf("a + b + c = %d", a+b+c).println()
	a + b + c = 20
	jshell>b = 9
	b ==> 9
	jshell>System.out.printf("a + b + c = %d", a+b+c).println()
	a + b + c = 22
	jshell>
	
```

### Step 15: 변수의 사용

변수는 사용되기 전에 선언되어야 한다.

```java

	jshell>newVariable
	| Error:
	| cannot find symbol
	| symbol: newVariable
	| newVariable
	  ^------------^
```

Java is a **strongly typed** programming language. This means two things:
자바는 **강력한 형식**(strongly typed)언어이다. 이는 두가지를 의미한다:

* 프로그램 내의 모든 변수들은 타입과 함께 선언되어야 한다.
* 변수에 할당된 값은 다음과 같아야 한다:
	* 변수의 타입과 같은 타입이거나
	* **호환이 가능한** 변수 타입이어야 한다.


```java

	jshell> int number = 5.5
	| Error:
	| incompatible types: possible lossy conversion from double to int
	| int number = 5.5
	|_____________^---^
	jshell>

```

변수 ```number```는 정수이고 수학적으로 '숫자'이다. 상수 ```5.5```또한 마찬가지이다.
그런데 왜 결과에 에러가 발생할까?
	
```5.5``` is a floating-point number of type ```double```. We are trying to store a ```double``` inside a memory slot meant for ```int```.
```5.5```는 부동 소수점으로 ```double```타입이다. 우리가 ```int```형을 가지는 메모리 공간에 ```double```형을 저장하려고 했기 때문이다.
또 다른 예시를 살펴보자:

```java

	jshell> int number = "Hello World"
	| Error:
	| incompatible types: java.lang.String cannot be converted to int
	| int number = "Hello World"
	|_____________^--------------^
	jshell>

```
```number``은 ```int```형 변수이고, ```String```변수인 ```"Hello World"```를 저장해보려 했다. ***실패했다.***

#### 요약

이번 단계에서는

* 변수를 선언하는 방법이 중요하다는 것을 알았다.
* 기본 자바 자료형의 호환성 규칙에 대해 이해했다. 

### Step 16: 변수: Behind-The-Scenes

변수의 선언 중에 변수에 값을 부여하는 것을 초기화라고 한다.

```java

	jshell> int number = 5
	number ==> 5
	jshell>

```

```int number = 5```는 ```number```에 대한 선언과 초기화가 결합되어 있다.
다음 구문 ```int number2 = number```은 약간 다르다.

```java

	jshell> int number2 = number
	number2 ==> 5
	jshell> number2
	number2 ==> 5
	jshell>

```

```number2```의 초기 값은 또 다른 변수로, 이전에 정의했던 ```number```이다.

```int nubmer2 =number```의 이면에 무슨 일이 일어나는지 알아보자:
* ```int```형 크기를 가진 메모리 공간 ```number2```가 할당된다.
* ```number```의 공간에 저장된 값을 ```number2```의 공간으로 복사된다.


예를 들면  ```a = 100```, ```c = a + b```, ``` a = c``` 를 ```할당```이라고 한다.

```java

	jshell> int a = 5
	a ==> 5
	jshell> int b = 10
	b ==> 10
	jshell> a = 100
	a ==> 100
	jshell> int c
	c ==> 0
	jshell> c = a + b
	c ==> 110
	jshell> a = c
	a ==> 110
	jshell> int d = b + c
	d ==> 120
	jshell>

```


변수 **할당**은 여러 가지 방법으로 발생할 수 있다:
* 리터럴 값에서 변수에 이르기까지, 호환되는 타입이 있다. ```a = c```가 그 예시이다.
* 변수 식에서 변수로. 이 수식은 호환되는 타입의 변수 및 리터럴로 구성할 수 있으며, 할당 전에 평가된다. "c = a + b"가 그 예다.

상수 리터럴에 대한 할당은 **허용되지 않는다.**

```java

	jshell> 20 = var
	| Error:
	| unexpected type
	| required : variable
	| found : value
	| 20 = var
	| ^^

	jshell>

```
 
#### 요약

이 단계에서는, 초기 값을 갖는 변수를 제공하는 방법과 할당의 기본 사항에 대해 논의하였다.

### Step 17: 변수 이름 짓기

변수 정의에 대한 구문 규칙은 상당히 엄격하다. 변수 이름을 붙이는 방식이 자유로운가? 대답은 어느 정도 '그렇다'이다.

### 변수 명명 규칙

변수 이름에 대한 Java 규칙은 간단히 설명하자면 다음과 같다:

변수의 이름은 다음 세 가지를 어떤 순서로도 쓸 수 있다.
* 글자 [```A-Z, a-z```]
* 숫자 [```0-9```]
* 특수 기호 '```$```' ("dollar") 와 '```_```' ("underscore")

다음과 같은 예외 사항:
* 이름은 숫자 [```0-9```]로 시작할 수 없다.
* 이름은 사전에 정의된 자바 **키워드**와 같을 수 없다.

이제 이러한 명명 규칙을 위반할 경우 컴파일러가 어떤 오류를 발생시키는지 봅시다.

***Error : Using a invalid character ```-```***

```java

	jshell> int test-test
	| Error:
	| ';' expected
	| int test-test
	|         ^

```

***Error : Starting name of a variable with a number***

```java

	jshell> int 2test
	| Error:
	| '.class' expected 
	| int 2test
	|     ^
	| Error:
	| not a statement
	| int 2test
	|      ^--^
	| Error:
	| unexpected type
	| required: value
	| found: class
	| int 2test
	| ^--^
	| Error:
	| missing return statement
	| int 2test
	| ^-------^

	jshell>

```

***Error : Using a keyword as the name of variable***

자바에서는 몇몇 특정한 단어를 ```키워드```라고 부른다. 예를 들어 우리가 살펴본 데이터 타입 중 일부인 ```int```와 ```double```이다. 이들 ```키워드```는 변수 이름으로 사용할 수 없다.

```java

	jshell> int int
	   ...> ;	
	| Error:
	| '.class' expected
	| int int
	|     ^
	| Error:
	| unexpected type
	| required: value
	| found: class
	| int int
	| ^--^
	| Error:
	| missing return statement
	| int int
	| ^------...

```

### 변수 이름 지정 규칙

훌륭한 프로그래머들은 읽기 쉬운 코드를 쓴다. 변수에 적절한 이름을 지정하면 코드를 쉽게 읽을 수 있다.

예를 들어, 축구 스코어 카드 어플리케이션에 ```s```를 점수를 뜻하는 변수로 사용하는 것은 모호하다. ```score```처럼 조금 더 많은 의미를 내포하는 것이 좋다.

```java

	jshell> int s
	s ==> 0
	jshell> int score
	score ==> 0
	jshell>

```


> 풍부한 경험을 가진 자바 커뮤니티는 프로그래머들이 **이름 지정 규칙**을 따를 것을 *제안한다*. 위의 예는 이것들 중 하나이다. 이러한 규칙을 위반해도 컴파일이 발생하지 않는다.

자바에서 또 다른 규칙은, 변수 이름에 여러 개의 단어가 들어갈 때 **카멜 케이스(CamelCase)**를 사용하는 것이다. 

```java 
 
	jshell> int noOfGoals
	noOfGoals ==> 0

```

```noOfGoals``` 이 ```noofgoals```보다 읽기 쉽다.

 ```noOfGoals``` 와 ```NoOfGoals``` 둘 다 읽기 쉽다. 

그러나 자바에서는 변수 이름은 소문자로 시작하는 것이 규칙이다. 따라서 변수의 이름은 ```noOfGoals```가 좋다.

*** 권장되지 않음*** 
```
	jshell> int NoOfGoals
	NoOfGoals ==> 0
```

변수의 이름을 매우 길게도 지을 수 있다.

```java

	jshell> int iThinkThisIsQuiteALongName
	iThinkThisIsQuiteALongName ==> 0
	jshell> int iThinkThisIsSuchALongNameThatIMightNeverUseSuchALongNameAgain
	iThinkThisIsSuchALongNameThatIMightNeverUseSuchALongNameAgain ==> 0

```

그러나, 변수 이름을 너무 길게 짓지는 말자.
***변수에 가능한 가장 짧고, 의미 있고, 읽기 쉬운 이름을 사용하자***

#### 요약

이번 단계에서는

* 자바의 변수 이름 규칙에 대해 알아보았다.
* 우리를 안내하는 규칙이 있다는 것을 이해했다.
* 널리 사용되는 변수 이름 규칙을 살펴보았다.

### Step 18: 기본형 타입 소개

The table below lists the **primitive types** in Java.
아래의 표는 자바의 **기본형 타입**이 나열되어 있다.


| 값의 타입 | Java의 기본형 타입 | 크기 (in bits) | 범위 | 예시 |
| :---: | :---: |:---: |:---: |:---:|
| 정수 |byte|8|```-128``` ~ ```127```|```byte b = 5;```|
| 정수 |short|16|```-32,768``` ~ ```32,767```|```short s = 128;```|
| 정수 |int|32|```-2,147,483,648``` ~ ```2,147,483,647```|```int i = 40000;```|
| 정수 |long|64|```-9,223,372,036,854,775,808``` ~ ```9,223,372,036,854,775,807```|```long l = 2222222222;```|
| 부동 소수점 | float| 32 | 대략 ±3.40282347E+38F. 정확하지 않음(재정/과학 수학은 피하기 위해)||```float f = 4.0f;```|
| 부동 소수점 |double|64| 대략  ±1.79769313486231570E+308. 정확하지 않음(재정/과학 수학은 피하기 위해)||```double d = 67.0;```|
| 문자 |char|16|```'\u0000``` ~ ```'\uffff```|```char c = 'A';```|
|부울형| boolean|1| ```true``` ~ ```false```|```boolean isTrue = false;```|

이제 이러한 타입의 데이터를 어떻게 생성하여 메모리에 저장하는지 살펴봅시다.


다음을 기반으로 데이터 타입을 선택하십시오:
* 저장할 데이터 타입
* 저장할 값의 범위


> 참고: 위의 예시에서, 우리는 문자의 끝에 세미콜른 ```;```을 사용했다. 이것은 자바의 *구문 구분 기호* 이며, 단일 문장에 대해서는 '''JShell'''에서 필수 사항이 아니다.

#### 정수 타입

정수 타입들의 유일한 차이점은 저장 용량이다.

```java

	jshell> byte b = 5
	b ==> 5
	jshell> short s = 128
	s ==> 128
	jshell> int i = 40000
	i ==> 40000
	jshell> long l = 2222222222
	l ==> 2222222222
	jshell>

```

#### 부동 소수점 타입

```double```은 64 비트 크기의 부동 소수점 기본 타입이다.

```
	jshell> double d = 67.0
	d ==> 67.0
```

```float``` occupies 32 bits. ```float``` literals need to have a suffix '```f```' (as in ```4.0f```).
```float```는 32비트를 차지한다. ```float```리터럴은 '```f```'라는 접미사가 필요하다 (예를 들어 ```4.0f```).

```

	jshell> float f = 4.0f
	f ==> 4.0
```

이 접미사 ```f```를 생략하면, 부동 소수점 숫자는 ```double```로 가정한다. 32비트에는 64비트의 값을 저장할 수 없다.

```java
	jshell> float f2 = 4.0
	| Error:
	| incompatible types: possible lossy conversion from double to float
	| float f2 = 4.0
	|            ^-^

```

```float```값을 ```double```로 저장할 수 있다. 두 타입 모두 비슷한 값을 저장하지만 ```float```의 크기는 32비트이고 ```double```은 64비트임을 기억하자.

```
	jshell> double d2 = 67.0f
	d2 ==> 67.0
```

#### 문자 타입

문자 타입 ```char```은 단일 문자 기호를 저장할 수 있다. 이 기호는 한 쌍의 작은 따옴표, ```'```와 ```'```로 묶여야 한다.

```java

	jshell> char c = 'A'
	c ==> 'A'
```

다음은 몇 가지 char 선언 오류이다: 작은 따옴표를 사용하지 않고 여러 문자를 저장하려고 시도함.

```
	jshell> char ch = A
	| Error:
	| cannot find symbol
	| symbol: variable A
	| char ch = A
	|           ^

	jshell> char cab = 'AB'
	| Error:
	| unclosed character literal
	| char cab = 'AB'
	|            ^

```

#### 부울 타입


```boolean```타입의 개념은 수학적 논리에 근간을 두고 있다. 이 데이터 타입은 ```true```나 ```false```라는 두 개의 값을 저장 가능하다. 둘 다 대소문자를 구분하는 레이블이지만 따옴표로 묶지 않는다.


```java

	jshell> boolean isTrue = false
	isTrue ==> false
	jshell> isTrue = true
	isTrue ==> true
	jshell> boolean isFalse = True
	| Error:
	| cannot find symbol
	| symbol: variable True
	| boolean isFalse = True
	|                   ^--^

	jshell> isFalse = False
	| Error:
	| cannot find symbol
	| symbol: variable False
	| isFalse = False
	|           ^---^

```

```boolean```데이터는 코드의 논리적인 조건을 형성하는 데 사용되는 수식에 주로 사용된다. 자바의 조건문에 대해 더 많이 이야기 할 때 더 알아보자.


#### 요약

이번 단계에서는


* 자바에서 제공하는 기본형 데이터 타입을 알아보았다.
* 타입들이 분류되는 범주를 이해하였다.
* 각 기본형 타입별로 저장할 수 있는 데이터의 종류에 대해 알아보았다.

### Step 19: 데이터 타입 선택

변수에 대한 데이터 타입을 선택하는 방법의 몇 가지 예를 보자.

#### Example 1 : 축구 경기의 골


축구 점수를 추적하는 프로그램을 쓰는 스포츠 방송사를 생각해보자. 축구 경기에서 두 팀이 경기하고 있다. 경기는 일반적으로 90분이며, 추가 시간은 최대 120분 이다. 사실, 최종 점수는 그렇게 크지 않다. 현실적인 관점에서 볼 때 한 경기에서 득점한 골 수는 결코 7200개(120분의 초 수)를 넘지 않는다. 조금 더 신중하게 생각해보면, ```short```타입이면 각 팀의 점수를 저장하기에 충분할 것이다.(한```byte```여도 충분하긴 하지만)

```java

	jshell> short numTeamAGoals = 0
	numTeamAGoals ==> 0
	jshell> short numTeamBGoals = 0
	numTeamBGoals ==> 0
	jshell>

```

#### Example 2 : 세계 인구를 어떻게 저장하지?

우리는 현재 전 세계 인간의 수가 70억 명을 훨씬 넘어섰다는 것을 알고 있기 때문에 이를 저장할 수 있는 정수 데이터 타입은 ```long```뿐이다.

```java

	jshell> long globalPopulation = 7500000000;
	globalPopulation ==> 7500000000
	jshell>

```

#### Example 3 : 한 달 평균 강우량을 어떻게 저장할까?

강우량은 보통 밀리미터로 측정된다.(*mm*), 평균 30일 이상 계산하면 부동 소수점이 될 가능성이 높다는 걸 알 수 있다. 따라서, ```float```를 사용하거나, 정확성을 높이기 위해 ```double```을 사용할 수도 있다.

```java

	jshell> float avgJanRainfall = 31.77f;
	avgJanRainfall ==> 31.77
	jshell> double averageJanRainfall = 31.77
	averageJanRainfall ==> 31.77
	jshell>

```
#### Example 4 : 학생의 성적

고등학교의 성적은 일반적으로 A, B, C , ...이다.
성적표를 작성하는 프로그램이라면 ```char``` 타입이 최선의 선택이 될 것이다.

```java

	jshell> char gradeA = 'A'
	gradeA ==> 'A'
	jshell> char gradeB = 'B'
	gradeB ==> 'B'
	jshell> char gradeC = 'C'
	gradeC ==> 'C'
	jshell> char gradeD = 'D'
	gradeD ==> 'D'
	jshell> char gradeF = 'F'
	gradeF ==> 'F'
	jshell>

```

#### Example 5 : 숫자가 홀수인가 짝수인가?

'boolean isNumEven'은 기본 초기 값이 'false'인 좋은 베팅이다. 짝수로 판명되면 'true'로 바꿀 수 있다.

```java

	jshell> boolean isNumEven
	isNumEven ==> false
	jshell> isNumEven = true
	isNumEven ==> true
	jshell>

```

#### 요약

이번 단계에서는


* 데이터 타입을 선택하면서 사고하는 방법 이해했다
* 정수, 부동 소수점, 문자 및 부울 데이터에 대한 사례 탐색했다.

### Step 20: 할당 연산자 ```=```


우리는 변수 할당을 알아보던 중 할당 연산자를 접했다.

```c = a + b```와 같은 코드를 사용하여 수식을 사용하여 변수에 값을 할당할 수 있다.

할당을 수행할 수 있는 몇 가지 추가적인 방법을 살펴봅시다.

```java

	jshell> int i = 10
	i ==> 10
	jshell> int j = 15
	j ==> 15
	jshell> i = j
	i ==> 15
	jshell>

```

다음 예제를 살펴봅시다:

```java
	jshell> i = i * 2
	i ==> 30
	jshell>

```

똑같은 변수 ```i```가 우측(*RHS*)과 좌측(*LHS*)에 모두 나타난다. 이게 가능한가?
먼저, *RHS*에 있는 수식이 *독립적으로* 평가된다. 그렇게 얻은 값은 *LHS*변수의 메모리 공간에 복사된다.
위의 논리를 이용하여, ```i = i * 2```라는 할당은 실제로 ```i```(초기에는 ```15```) 의 값을 ```30```(두 배로 증가)으로 갱신한다
자바 역시 ```i = i + i```라는 헷갈리는 구문과 마주쳤을 때 옳은 일을 한다, 여기서 ```i```가 사방에 널려 있다! 코드는 ```i```의 값을 두 배로 하고, 이는 ```JShell```에서의 출력에 반영한다.

```java

	jshell> i = i + i
	i ==> 60
```

다음의 예는 자명하다.

```
	jshell> i = i - i
	i ==> 0
```

#### 변수의 증가와 감소

우리는 이미 할당에 따른 증가를 보았다.

```java

	jshell> int i = 0
	i ==> 0
	jshell> i = i + 1
	i ==> 1
	jshell> i = i + 1
	i ==> 2
	jshell> i = i + 1
	i ==> 3
	jshell>

```

반대로 ```i = i - 1```은 변수의 **감소**라고 한다. 이 또한 반복해서 수행될 수 있으며, ```i```의 값은 매번 변한다.


```java

	jshell> i = i - 1
	i ==> 2
	jshell> i = i - 1
	i ==> 1
	jshell> i = i - 1
	i ==> 0
	jshell>
	
```

#### 요약 

이번 단계에서는

* Looked at the assignment operator ```=``` in a more formal way
* Looked at heavily used scenarios for assignment, such as increment and decrement

### Step 21: 할당 Puzzle과  *PMT-Challenge* 복습


이제 우리는 표현에서 변수를 정의하고 할당하고 사용하는 방법을 이해했으므로, 이제는 조금 더 밀어붙일 때가 되었다. 다음 예들은 우리가 코드에서 변수를 가지고 놀 수 있는 방법을 탐구한다.

##### Snippet-1 : 사전 및 사후의 증분과 감소

증분을 하기 위한 두 가지 약칭이 있다. ```number++```는 *사후-증분*을 의미한다. 반대로, ```++number```은 **사전-증분**을 의미한다.
연산자 ```++```은  ```byte```, ```short```, ```int``` 그리고 ```long```과 같은 정수형 타입 변수에 적용될 수 있다.

```number++``` 은 ```number = number + 1```구문과 같은 의미이다.

```java

	jshell> int number = 5
	number ==> 5
	jshell> number++
	$1 ==> 5
	jshell> number
	number ==> 6
	jshell> ++number
	$2 ==> 7
	jshell> number
	number ==> 7
	jshell>

```

```number--``` 은 *사후-감소*를, 반면에 ```--number``` 는 **사전-감소**를 의미한다.

```java

	jshell> number--
	$3 ==> 7
	jshell> number
	number ==> 6
	jshell> --number
	$4 ==> 5
	jshell> number
	number ==> 5
	jshell>

```

***사전과 사후의 차이점은 무엇인가?***

사전 수정 버전과 사후 수정 버전 모두 위의 예에서 동일한  결과를 얻지만 약간의 차이가 있다. 이는 나중에 알아볼 것이다.

##### Snippet-2 : 복합적인 할당 연산자들

복합적인 할당 연산자는 ```=```과 숫자 연산자가 결합한 것이다.

```i += 2``` : ```i```의 최신 값에 ```2```를 더하라.

```java

	jshell> int i = 1
	i ==> 1
	jshell> i = i + 2
	i ==> 3
	jshell> i += 2
	$1 ==> 5
	jshell>

```


```i -= 1``` :  ```i```의 최신 값에서 ```1```를 빼라.

```java

	jshell> i
	i ==> 5
	jshell> i -= 1
	$2 ==> 4
	jshell> i
	i ==> 4
	jshell>

```


```i *= 4``` :  ```i```와 ```4```를 곱하고 그 결과를 다시 ```i```에 저장하라.

```java

	jshell> i *= 4
	$3 ==> 20
	jshell> i
	i ==> 20
	jshell>

```

```i /= 4``` :  ```i``` 를 ```4```로 나누고 그 결과를 다시 ```i```에 저장하라.

```java

	jshell> i /= 4
	$4 ==> 5
	jshell> i
	i ==> 5
	jshell>

```

```i %= 2``` :  ```i```를 ```2```로 나누고 **나머지**를 다시 ```i```에 저장하라.

```java

	jshell> i %= 2
	$5 ==> 1
	jshell> i
	i ==> 1
	jshell>

```
#### 요약

이번 단계에서는

* 내장된 Java 증분 및 감소 연산자 살펴보았다.
* 이러한 운영자의 사전 및 사후 수정 버전의 부작용에 대해 살펴보았다.
* 복합 할당의 이점 확인하였다.

### Step 22: ```JShell``` 사용 팁

* 단축키
	1. 현재 프롬프트의 시작/끝 이동.
		* '```Ctrl+a```' : 줄의 시작부터
		* '```Ctrl+e```' : 줄의 마지막부터
	2. 완료된 프롬프트 입력의 기록 위/아래 이동
		* *위쪽 화살표* key : 시간을 거슬러 올라감
		* *아래 화살표* key : 시간을 앞당김
	3. 역키워드 검색
		* JShell 프롬프트 입력 히스토리의 역순으로 용어 검색 :  '```Ctrl+r```' 입력
		* 일치 항목 내에서 스크롤(히스토리의 역순으로):  '```Ctrl+r```' 반복 입력
* ```/exit``` :JShell 세션을 재설정 및 종료하고 저장된 변수 값을 모두 삭제한다.
* JShell 내부 변수 : ```$1```, ```$2``` 등
	* When expressions involving literals and/or previously declared variables are entered as-is, without assignment, those expressions are still evaluated. The result is stored in such an internal variable, and is available for use until the JShell session is reset.
	* 리터럴,또는 이전에 선언된 변수를 포함하는 수식을 할당 없이 그대로 입력해도 해당 수식은 여전히 연산 가능하다. 결과는 그러한 내부 변수에 저장되며, JShell 세션이 재설정될 때까지 사용할 수 있다.
* 변수 선언 규칙 완화
	1. 단일 자바 구문을 구분 기호 '```;```'로 종료할 필요는 없음.
	2. 프롬프트에서 한 줄에 여러 개의 구문을 입력할 때, 연속된 문장은 ';'로 구분해야 한다. 그러나 후행 ';'는 여전히 생략할 수 있다.

#### 요약

이번 단계에서는

* Explored some useful keyboard shortcuts for ```JShell``` 명령어의 유용한 단축키를 몇 가지 알아보았다.
* ```JShell``` 내부 변수 이면을 이해했다.
* ```JShell```은 일부 코딩 규칙을 완화해, 코드 작성의 수고를 던다.

### Step 23: 조건문 ```if``` 소개


*PMT-Challenge*는 총 10개의 테이블 항목을 출력해야 한다. ```for```문은 이 작업을 수행하기 위한 적절한 반복 메커니즘이다. *loop*라는 단어는 영어 사전이 말하는 그대로를 의미한다.

* ```i``` 는```1``` 부터 ```10``` 다양하기 때문에, ```i```와 관련된 일을 수행한다.*

*PMT-Challenge*에서 무언가를 하는 것은 ```System.out.printf()```를 호출할 수 있다.

```for``` 문의 구조는 다음과 같다:

```java

	for(initialization; condition; update) {
		statement1;
		statement2;
	}

```

위 코드의 동작 방법:
1.  ```초기문``` 을 실행한다. 
2.  ```조건식``` 평가 결과 참이면, ```작업문```을 수행한다. 그렇지 않으면 루프를 벗어난다.
3. ```반복 후 작업문```을 실행한다.
4. 2번과 3번을 반복한다.

***복잡해 보이는가?*** 쪼개서 살펴보자.

우선 ```조건식```에 대해 전부 이해해보자.

#### 논리 연산자

```조건식``` 은 논리 결과를 나타난다.( ```참``` 혹은 ```거짓```). 

자바는 **논리 수식**을 피연산자로 사용하는 **논리 연산자**가 있고, 이는 ```boolean```값을 평가한다.
아마 여러분은 학교에서 ```=```기호를 숫자를 비교하기 위해 사용했을 것이다.

***자바의 세계에서는 조금 다르다.***  ```=```는 할당 연산자이다. ```==``` 가 비교 연산자이다.

```java

	jshell> int i = 10
	i ==> 10
	jshell> i == 10
	$1 ==> true
	jshell> i == 11
	$2 ==> false

```

 ```<``` 와 ```>``` 등 다른 비교 연산자도 있다. 
 
```java

	jshell> i < 5
	$3 ==> false
	jshell> i > 5
	$4 ==> true

```

```<=```와 ```>=```는 단순한 확장이다.

```java

	jshell> i <= 5
	$4 ==> false
	jshell> i <= 10
	$5 ==> true
	jshell> i >= 10
	$6 ==> true
	jshell>

```

#### 조건문: "if"문 

우리는 조건이 참일 때만 특정한 코드 라인을 실행하기를 원할 것이다.

```if``` 문을 보자.

하나의 ```if``` 은 다음과 같이 구성된다:

```java

	if (조건식) {
	      작업문;
	}

```

```작업문```은 ```조건식```이 ```참```인 경우만 실행된다.


일반적으로 우리가 쓰는 모든 코드는 항상 실행된다.

아래 예시의 ```i is less than 5```도 항상 출력된다.

```java

	jshell> int i = 10
	i ==> 10
	jshell> System.out.println("i is less than 5")
	i is less than 5
```

```if```문을 사용하면, ```System.out.println("i is less than 5");```의 실행을 제어할 수 있다.

```java

	jshell> if (i < 5)
	   ...> System.out.println("i is less than 5");
	jshell> 
```

 ```i```의 값이 ```10```이기 때문에 조건문 ```i < 5```이 ```거짓```이 되어 콘솔 창에 아무것도 출력되지 않는다.


```if``` 문을 실행하기 위해```i``` 를 ```4```로 바꿔보자.

```java

	jshell> i = 4
	i ==> 4
	jshell> if (i < 5)
	   ...> System.out.println("i is less than 5");
	i is less than 5
	jshell>

```

```i is less than 5```는 콘솔 창에 출력된다.

저장된 변수 ```i```값을 조절하여```System.out.println("i is less than 5");``` 구문의 실제 실행 여부를 제어할 수 있다.

***만세! 이제 우리는 *조건문 수행*을 달성했다!***


변수를 리터럴과 비교할 수 있듯이 두 변수의 값을 비교할 수도 있다. 동일한 집합의 비교 연산자, 즉 ```==```, ```<```, ```>```, ```<=``` 그리고 ```>=``` 도 사용될 수 있다.

```java

	jshell> int number1 = 5
	number1 ==> 5
	jshell> int number2 = 7
	number2 ==> 7
	jshell> if (number2 > number1)
	   ...> System.out.println("number2 is greater than number1");
	number2 is greater than number1

	jshell> number2 = 3
	number2 ==> 3
	jshell> if (number2 > number1)
	   ...> System.out.println("number2 is greater than number1");

	jshell>

```

#### 요약

이번 단계에서는,

* 조건문의 필요성에 대해 이해했다.
* 논리적 표현식 및 조건부 연산자의 개념을 도입하였다.
* 자바에서의 ```if```문의 사용을 알아보았다.

### Step 24: 프로그래밍 실습 PE-04 
- - - 


1. ```a```, ```b```, ```c``` 그리고 ````d````라는 네 개의 정수형 변수를 생성한 후, ```a```와 ```b```의 합을 ```c```와 ```d```의 합보다 큰 경우에만 출력하는 ```if문```을 작성하시오.

2. 삼각형의 각도를 저장하는 세 개의 정수형 변수 ```angle1```, ```angle2``` 그리고 ```angle3```을 저장하여라. 세 각도가 삼각형을 그릴 수 있는지 여부를 나타내는 ```if문```을 작성하시오.
	_힌트: 삼각형은 세 개의 각도로 이루어져있고, 그 합은 정확히 ```180도```이어야만 한다._
	
3. 변수가 하나의 정수를 저장하도록 하여라. 해당 변수가 짝수인지 알아내는 ```if문``` 작성하시오.
	
	_힌트: ```%``` 연산자를 사용하자._

### Step 25:  PE-04 솔루션

#### Solution 1

```java

	jshell> int a = 5
	a ==> 5
	jshell> int b = 7
	b ==> 7
	jshell> int c = 4
	c ==> 4
	jshell> int d = 3
	d ==> 3
	jshell> if (a + b > c + d)
	   ...> System.out.println("a and b together tower above c plus d");
	a and b together tower above c plus d

	jshell>

```

#### Solution 2

```java

	jshell> int angleOne = 55
	angleOne ==> 55
	jshell> int angleTwo = 65
	angleOne ==> 55
	jshell> int angleThree = 60
	angleOne ==> 55
	jshell> if (angleOne + angleTwo + angleThree == 180)
	   ...> System.out.println("The three angles together form a triangle");
	The three angles together form a triangle

	jshell> angleThree = 75
	angleOne ==> 55
	jshell> if (angleOne + angleTwo + angleThree == 180)
	   ...> System.out.println("The three angles together form a triangle");

	jshell>

```

#### Solution 3

```java

	jshell> int num = 10
	num ==> 10
	jshell> if (num % 2 == 0)
	   ...> System.out.println("The number is even");
	The number is even

	jshell> num++
	num ==> 11
	jshell> if (num % 2 == 0)
	   ...> System.out.println("The number is even");

	jshell>
```

### Step 26:  ```if문``` 더 알아보기

if문의 몇 가지 예를 더 살펴보자.

##### Snippet-1 

여기 조건부 실행의 기본적인 예가 있다.

```java

	jshell> int i = 5
	i ==> 5
	jshell> if (i == 5)
	   ...> System.out.println("i is odd");
	i is odd
```

두 번째 라인에 두 개의 구문을 추가해보자.

```java
	jshell> if (i == 5)
	   ...> System.out.println("i is odd"); System.out.println("i is prime");
	i is odd
	i is prime

	jshell>

``` 
두 문자 메시지 모두 출력되었다.

```i```의 값을 ```6```으로 바꾸고 다시 실행해보자.

```java

	jshell> i = 6
	i ==> 6
	jshell> if (i == 5)
	   ...> System.out.println("i is odd"); System.out.println("i is prime");
	i is prime

	jshell>

```

```i is prime```이 콘솔 창에 출력되었다. 왜일까?

왜 조건문이 ```false```인데도 실행되었을까?

기본적으로 ```if문```은 바로 다음에 오는 문장에만 구속력을 가진다.

그렇기 때문에 무조건적으로 실행되는 ```System.out.println("i is prime");```를 제어하지 않는다.

두 개 구문을 조건부 실행할 수 있는 방법이 있을까? 두 개보다 더 많다면?

##### Snippet-2 : 블록으로 묶은 ```if문``` 

마치 마술과 같은 묘안이 있다! 이 마술은 '```{```' 와 '```}```'라는 *braces*의 한 쌍에 있다.  

이들은 일련의 구문을 **블록**으로 그룹화하는 데 사용된다. 조건문의 결과 (```참``` 또는 ```거짓```)에 따라서 이 블록의 모든 구문이 실행되거나 아예 실행되지 않는다.

```java

	jshell> int i = 5
	i ==> 5
	jshell> if (i == 5) {
	   ...> System.out.println("i is odd");
	   ...> System.out.println("i is prime");
	   ...> }
	i is odd
	i is prime

	jshell> i = 6
	i ==> 6
	jshell> if (i == 5) {
	   ...> System.out.println("i is odd");
	   ...> System.out.println("i is prime");
	   ...> }

	jshell>

```

```if문```에서 *항상* 블록을 사용하는 것은 좋은 프로그래밍 습관이다. 여기 예시가 있다:

```java

	if (i == 5) {
		System.out.println("i is odd");
	}

```
	
블록은 또한 하나의 구문으로도 구성될 수 있다! 이는 코드의 가독성을 향상시킨다.

#### 요약

이번 단계에서는

* ```if문```에서 블록을 사용의 중요성을 알아보았다.
* 제어 흐름을 보다 쉽게 읽을 수 있는 방법 이해했다.


### Step 27: 반복문 소개:  ```for문``` 

 *PMT-Challenge*는 총 10개의 테이블 항목을 출력해야 한다. ```for``` **loop**은 이 작업을 수행하기 적절한 반복 메커니즘이다.
 
*loop*이라는 단어는 영어 사전이 말하는 그대로를 의미한다.

* ```i``` 는```1``` 부터 ```10``` 다양하기 때문에, ```i```와 관련된 일을 수행한다.*

```for문```은 다음과 같이 구성된다:

```java

	for(initialization; condition; update) {
		statement1;
		statement1;
	}

```

***위 코드 실행 방법:***
1. ```초기문```을 실행한다. 
2. ```조건식``` 평가 결과 참이면, ```작업문```을 수행한다. 그렇지 않으면 루프를 벗어난다.
3. ```반복 후 작업문```을 실행한다.
4. 2번과 3번을 반복한다.

이러한 구성 요소를 분리해보자:

* _초기문_ : ```int i = 1```
* _조건식_ : ```i <= 10```
* _반복 후 작업문_ : ```i++```

이제 더 큰 그림을 그리기 위해 그들을 함께 모읍시다. 다음과 같이 보일 수 있다:

```java

	for (int i = 1; i <= 10; i++) {
		System.out.println("Hello World");
	}

```

이 반복문은 실행될 때, 각 줄에 "Hello World"라는 메시지를 총 ```10번```출력한다.

##### Snippet-1 : *PMT-Challenge* 솔루션

우리는 "Hello World" 메시지를 테이블 항목을 콘솔에 출력하는 것으로 바꿔야 한다. 이 출력은 ```1```부터 ```10```의 값을 가지는 ```i```에 의해 제어된다.

```java

	jshell> int i
	i ==> 0
	jshell> for (i=0; i<=10; i++) {
	   ...> System.out.printf("%d * %d = %d", 5, i, 5*i).println();
	   ...> }
	5 * 1 = 5
	5 * 2 = 10
	5 * 3 = 15
	5 * 4 = 20
	5 * 5 = 2
	5 * 6 = 30
	5 * 7 = 35
	5 * 8 = 40
	5 * 9 = 45
	5 * 10 = 50

```

##### Snippet-1 설명

1. 첫 단계는 초기문이다: ```i = 1```. 
2. 이 후, ```System.out.printf("%d * %d = %d", 5, i, 5*i).println();``` 라는 구문이 한번 실행된다.
3. 그러면 반복 후 작업이 실행된다: ```i++```.
4. 그 후 바로 조건식  ```i<=10```이 평가된다. ```참```값을 반환한다. 진전을 보인다. ```for문```이기 때문에 작업문이 한번 더 반복된다.
5. 이 후, 연속적인 반복 후 작업으로 ```i```값이 ```11```이 될 때 까지 이 시퀀스가 실행된다.
6. ```i```값이 ```11```이 되는 순간, 조건식은 ```거짓```이 된다. ```for문```내의 루프는 종료된다.
이제, ```1```부터 ```10```에 대한 5의 곱셈표가 표시되었다!

자, 진짜 멋지지 않은가? 대단하다!
이 정도의 단계까지 왔다고 스스로를 토닥여주자. 이 멋지고 강력하기까지 한 기술 (*반복문*)은 거의 모든 자바 프로그램을 작성할 때 사용된다.

#### 요약

이번 단계에서는

* ```for문```과 같은 반복문이 왜 필요한지 알아보았다.
* ```for문```의 메커니즘에 대해 이해했다.
* 반복을 위해 ```for문```을 사용하여  *PMT-Challenge*를 해결하였다.


### Step 28: 프로그래밍 실습 PE-05

1. 이제 ```7```이라는 숫자에 대한 곱셈표 출력을 위해 전과정을 반복해 보아라. 기존 세션을 사용하고 있다면 새로운 ```JShell```세션으로 시작하시오.
2. ```6```과 ```10```에 대한 곱셈표를 출력하기 위해 마지막 솔루션을 사용하시오.
3. ```1```부터 ```10```까지의 정수를 출력하시오.
4. ```10```부터 ```1```까지의 정수를 출력하시오.
5. ```1```부터 ```10```까지의 정수의 제곱을 출력하시오.
6. 첫 짝수 ```10```개의 제곱을 출력하시오
7. 첫 홀수 ```10```개의 제곱을 출력하시오

### Step 29:  PE-05 솔루션

#### Solution 2

```java

	jshell> int i
	i ==> 0
	jshell> for (i=0; i<=10; i++) {
	   ...> System.out.printf("%d * %d = %d", 6, i, 6*i).println();
	   ...> }
	6 * 1 = 6
	6 * 2 = 12
	6 * 3 = 18
	6 * 4 = 24
	6 * 5 = 30
	6 * 6 = 36
	6 * 7 = 42
	6 * 8 = 48
	6 * 9 = 54
	6 * 10 = 60

	jshell> i = 0
	i ==> 0
	jshell> for (i=0; i<=10; i++) {
	   ...> System.out.printf("%d * %d = %d", 10, i, 10*i).println();
	   ...> }
	10 * 1 = 10
	10 * 2 = 20
	10 * 3 = 30
	10 * 4 = 40
	10 * 5 = 50
	10 * 6 = 60
	10 * 7 = 70
	10 * 8 = 80
	10 * 9 = 90
	10 * 10 = 100

```

#### Solution 3

```java

	jshell> for (int i=1; i<=10; i++) {
	   ...> System.out.printf(i).println();
	   ...> }
	1
	2
	3
	4
	5
	6
	7
	8
	9
	10

```

#### Solution 4


```i--```의 첫 번째 사용이다. 흥미롭지 않은가?

```java

	jshell> for (int i=10; i>0; i--) {
	   ...> System.out.printf(i).println();
	   ...> }
	10
	9
	8
	7
	6
	5
	4
	3
	2
	1

```

#### Solution 5

```java

	jshell> for (int i=1; i<=10; i++) {
	   ...> System.out.printf(i*i).println();
	   ...> }
	1
	4
	9
	16
	25
	36
	49
	64
	81
	100

```

#### Solution 6

for문의 ```반복 후 작업```으로 여러 가지 일을 할 수 있다. 여기서 우리는 ```i += 2```를 사용했다.


```java

	jshell> for (int i=2; i<20; i += 2) 
	   ...> System.out.printf(i*i).println();
	   ...> }
	4
	16
	36
	64
	100
	144
	196
	256
	324
	400

```

#### Solution 7

```java

	jshell> for (int i=1; i<=19; i += 2) {
	   ...> System.out.printf(i*i).println();
	   ...> }
	1
	9
	25
	49
	81
	121
	169
	225
	289
	361

```

### Step 30: 어려운  ```for문``` 살펴보기

```for문```의 개념적 구조는 다음과 같다:

```java

	for (initialization; condition; updation) {
		statement;
		statement;
		//...
		statement;
	}

```
  

*초기문(initialization)*, *조건(condition)*, *반복 후 작업(updation)* 이 **선택적**인 것을 보고 놀랄 것이다. 그것들은 모두 개별적으로, 조합으로, 아니면 전부 다 제외될 수 있다!! 몇 가지 흥미로운 사례들을 코드로 살펴보자. 

1.  비어있는 초기문과 작업문

조건이 거짓으로 평가될 때까지 연속적으로 제어 변수를 증가시킨다.

```java

	jshell> int i = 1
	i ==> 1
	jshell> for (; i<=10; i++);
	jshell> i
	i ==> 11
	jshell>

```

2.  여러 개의 초기문과 비어있는 작업문

```초기문```과 ```작업 후 반복문```은 ```,```로 분리해서 여러 개를 사용할 수 있다.

```java

	jshell> int j
	i ==> 11
	jshell> for (i=1, j=2; i<=10; i++, j++);
	jshell> i
	i ==> 11
	jshell> j
	j ==> 12
	jshell>

```


아래의 예시에서, i는 증가하고 j는 감소한다.

```java

	jshell> for (i=1, j=2; i<=10; i++, j--);
	jshell> i
	i ==> 11
	jshell> j
	j ==> -8
	jshell>

```

3. 무한 반복


무한 반복이란 *조건*이 비어있는 상태를 말한다. 조건이 비어있으면 항상 ```참```으로 평가 된다. ```for문```은 조건이 ```거짓```인 경우에만 종료되기 때문에, 그러한 루프는 절대 종료되지 않는다.

이는 예외적으로 ``CTRL + c``` 키를 사용하여 종료 시킬 수 있다.

```java

	jshell> for (;;);

	^C
	jshell>

```


4. for문에서의 블록


```if문```에서 처럼, ```for문```도 구문에 블록을 가질 수 있다. 이전처럼, 괄호 '```{```'와 '```}```'의 사이에 있는 구문들을 묶을 수 있다. 이 구문들은 블록에 나타나는 순서와 같이 반복적으로 실행된다. 

```java

	jshell> for (i=1; i<=5; i++) {
	   ...> System.out.println("No 1");
	   ...> System.out.println("No 2");
	   ...> }
	No 1
	No 2
	No 1
	No 2
	No 1
	No 2
	No 1
	No 2
	No 1
	No 2

```


#### 요약

이번 단계에서는, 우리는 ```for문```의 구성요소들이 선택적이란는 것을 알았습니다:
* *초기문*
* *조건*
* *반복 후 작업*
* *작업문*


### Step 31: 기본 개념 복습

더 나아가기 전에, 우리가 여기서 무엇을 배웠는지 빠르게 생각해보자!


**컴퓨터**는 우리를 위한 작업을 하는 *기계*이다. 그것은 우리가 복잡하고, 시간이 많이 걸리거나 심지어 지루하다고 생각하는 작업들을 실행시키는 데 사용될 수 있다! 예를 들면 랩탑 컴퓨터는 CD안의 음악, 웹의 동영상을 재생하거나 인쇄 작업을 시작할 수 있다.

우리는 우리 주위에 작은 버전의 컴퓨터인 휴대폰을 가지고 있다. 그리고 혈당 측정기에서 일기예보 시스템 등 다른 것들도 있다. 우리가 가는 곳마다 컴퓨터가 우리를 에워싸고 있다!

모든 컴퓨터는 두 개의 기본 계층으로 구성된다:

* **하드웨어**: *전자 회로*를 포함한 컴퓨터의 모든 *전자* 및 *기계* 부품으로 구성된다.
* **소프트웨어**: *하드웨어*에서 실행되고 저장되는 *명령*을 기술한다.


만일 인체가 컴퓨터라면,
* *하드웨어*는 여러가지 장기로 이루어져 있을 것이다.(사지, 혈액, 심장 등)
* *소프트웨어*는 신경계로부터의 신호일 것이며, 이는 이 장기를 움직이는 것이다.



.
**컴퓨터 프로그래밍***은 컴퓨터에서 작업을 실행하기 위한 소프트웨어 명령을 작성하는 것을 포함한다. 이러한 명령을 제공하는 사용자를 **프로그래머**라고 한다. 종종, 컴퓨터 프로그래밍은 도전적이고 매우 흥미로운 문제들을 해결하는 것을 포함한다.

앞의 단계에서는 자바 언어의 기본 개념과 구성을 소개하였다.
우리는 기본적인 자바 구조를 사용하여 *PMT-Challenge*라는 프로그래밍 과제를 해결했다.

JShell REPL을 사용하여 다음과 같은 개념들을 차근차근 배웠다:
* 수식, 연산자 ,구문
* 변수와 출력 형식
* 조건문과 반복문

각 단계마다 *PMT-Challenge*에 새로운 지식을 적용하여 솔루션을 강화하였따.

지금까지의 여정이 마음에 들었기를 바란다. 다음 섹션에서는 동일한 Step by-step 접근 방식을 사용하여 Java 기능에 대해 자세히 알아볼 것이다. 우리가 또 한번 따라잡을 수 있기를 바란다!


## 메소드 이해

지금까지 배운 것들이 마음에 드는가? *PMT-Challenge*를 위한 우아하면서도 강력한 솔루션을 개발하여 다음과 같은 이점을 얻었다:

* 연산자, 변수, 수식
* 내장되어 있는 출력 형식
* 흐름 제어 조건
* 루프를 통한 반복문
 

그리고 우리가 결국 무엇으로 끝났는지 알아맞춰봐라. 바로 곱셈표 출력! 주변 사람들이 그걸 보고 싶어하고, 사용하고, 그리고 아마 친구들과 공유하고 싶어할지도 모른다.

그러나 일부에서는 ```8```도 ```7```도 아닌 ```5```에만 적용되는 것에 불만을 가질 수도 있다. 그러면 그들은 그 코드들을 다시 입력해야 할 것이다. 이것은 그들을 실망시킬 수 있다.
확실히 더 우아한 해결책이 존재하는데, 그것은 스스로 풀기를 기다리는 패턴이다.

자바에는 이를 위해 **메소드**를 사용하는 메커니즘이 존재한다. ```메소드```란 일련의 구문들을 그룹화하여 이름을 붙일 수 있는 기능이다. 이 이름은 해당 집합의 *기능*을 나타내며, 필요할 때 다시 사용할 수 있다. 


메소드는 본질적으로 특정 작업을 수행하는 *루틴*이며, 요청된 횟수만큼 수행할 수 있다. 또한 수행하는 작업에 대한 결과를 반환할 수도 있다. ***메소드 정의*** 구문은 다음과 같다:

```
반환형   메소드 이름 () {
  메소드 바디
}

```

 

* ```메소드 이름``` 은 루틴의 이름이다.
* ```메소드 바디``` 는 구문의 집합이다.
* 한 쌍의 ```{``` 와 ```}``` 괄호는 ```메소드 바디```를 하나로 묶는다.
* ```반환형```은 ```메소드 이름```의 반환 값의 타입이다.


#### 요약

이번 단계에서는

* 라벨링 코드의 필요성 및 재사용 여부를 조사했다
* Java 메서드가 성능에 적합하다는 것을 알게 되었다.
* 메소드 정의가 어떻게 구성되어 있는지 개념적으로 확인했다.

### Step 01 : 간단한 메소드 정의

"```Hello World```"를 화면에 두 번 출력하는 간단한 메소드를 작성해보자.

```java

	jshell> void sayHelloWorldTwice() {
	   ...> System.out.println("Hello World");
	   ...> System.out.println("Hello World");
	   ...> }
	| created method sayHelloWorldTwice()

```


약간의 이론은 다음과 같다:
* 위와 같은 메소드를 위한 코드를 **메소드 정의**라고 한다.
* ```void```는 해당 메소드가 연산 결과를 반환하지 않음을 의미한다. 메소드의 반환 값에 대해서는 조금 후에 알아보자.

***코드가 실행 되었을 때, 우리를 두번이나 반겨주지는 않았지?*** 우리가 받은 것은 ```created method sayHelloWorldTwice()```를 중얼거리는 지루한 메시지 뿐이다.

이는 메소드를 정의하는 것이 메소드 바디를 실행하는 것이 ***아니기 때문이다.***

메소드 바디가 더 이상 독립적인 구문이 아니기 때문에, 이는 기능적으로 **호출**되어야 한다. 이는 **메소드 호출**을 통해 이루어진다.

**메소드 호출**에 대해서 몇 가지 예시를 살펴보자.

```java

	jshell> sayHelloWorldTwice
	| Error:
	| cannot find symbol
	| symbol: variable sayHelloWorldTwice
	| sayHelloWorldTwice
	| ^----------------^

	jshell> sayHelloWorldTwice()
	Hello World
	Hello World
	
``` 

All that we had to do was to add parantheses to name of the metho
메소드 이름 뒤에 괄호만 추가하면 된다.

> 뒤에있는 '```;```'는 ```JShell```에서는 생략될 수 있다. 이는 구문 규칙을 완화하는 또 다른 예시이다.

> 메소드 이름은 변수 이름을 지을 때와 같은 규칙을 따른다.



#### 요약

이번 단계에서는

* 직접 첫 번째 메소드를 코딩해 보았다.
* 메소드의 정의와 호출이 서로 다른 단계임을 배웠다.


### Step 02: PE-01 실습

이제 몇 가지 실습을 해봄으로써 방법에 대한 기본적인 이해를 강화합시다.

#### Exercise Set -5

1. ```Hello World```를 세 번 출력하는 ```sayHelloWorld``` 메소드를 작성하시오.
2. 아래 네 개의 구문을 출력하는 메소드를 작성하시오.
	
	```I've created my first variable```

	```I've created my first loop```
	
	```I've created my first method```
	
	```I'm excited to learn Java```	

#### PE-01 솔루션

#### 솔루션 -1

```java

	jshell> void sayHelloWorldThrice() {
	   ...> System.out.println("Hello World");
	   ...> System.out.println("Hello World");
	   ...> System.out.println("Hello World");
	   ...> }
	| created method sayHelloWorldThrice()

	jshell> sayHelloWorldThrice()
	Hello World
	Hello World
	Hello World

```
 
#### 솔루션 -2

```java
 
	jshell> void sayFourThings() {
	   ...> System.out.println("I've created my first variable");
	   ...> System.out.println("I've created my first loop");
	   ...> System.out.println("I've created my first method");
	   ...> System.out.println("I'm excited to learn Java");
	   ...> }
	| created method sayFourThings()

	jshell> sayFourThings()
	I've created my first variable
	I've created my first loop
	I've created my first method
	I'm excited to learn Java

```

### Step 03: 메소드 정의 수정하기 (```Jshell``` Tips)

##### Snippet-01: sayHelloWorldTwice() 수정

```java

	jshell> void sayHelloWorldTwice() {
	   ...> System.out.println("Hello World");
	   ...> System.out.println("Hello World");
	   ...> }
	| created method sayHelloWorldTwice()
```

```/methods``` 명령어는 현재 세션에 정의된 메소드를 나열한다.
 
```
	jshell> /methods
	| void sayHelloWorldTwice()
	jshell>

```

 ```/list```명령어는 지정된 메소드의 코드를 나열한다.

```java

	jshell> /list sayHelloWorldTwice
	59 : void sayHelloWorldTwice() {
	System.out.println("HELLO WORLD");
	System.out.println("HELLO WORLD");
	}
	jshell>

```


```/edit``` 명령어를 사용하면 별도의 편집기 창에서 메소드 정의를 수정할 수 있다.

```java

	jshell> /edit sayHelloWorldTwice
	| modified method sayHelloWorldTwice
	jshell> sayHelloWorldTwice()
	HELLO WORLD
	HELLO WORLD
	jshell>

```

 ```/save``` 메소드는 파일 이름을 매개 변수로 사용한다. 실행 시 세션 메소드 정의를 파일에 저장한다.

```java
	
	jshell> /save backup.txt
	jshell> /exit
	| Goodbye

in28minutes$>

```

#### 요약

이번 단계에서는, 메소드를 정의할 때 더 편리하게 해주는 ```JShell```팁을 몇 가지 알아보았다.


### Step 04: 인수가 있는 메소드

우리는 ```Hello World```를 두 번 출력하기 위해 ```sayHelloWorldTwice```메소드를 작성하였다. 프로그래밍 실습에서는,  ```Hello World```를 세 번 출력하기 위해 ```sayHelloWorldThrice```라는 새로운 메소드를 작성하였다.

여러분이 Java 수업에 있다고 상상해 보십시오. 그 교실에서 선생님은 다음과 같이 말하면서 Java 사용 능력을 시험하고 싶어합니다:
_"***```Hello World```***를 임의의 횟수만큼 출력하고 싶다면 어떻게 해야 할까요?"_.

자, 그러면 여러분의 인내심을 시험해 볼 수 있을 거다!

```Hello World```를 임의의 횟수만큼 출력하는 메소드를 어떻게 작성할까?



주목해야 할 것은 "임의"라는 단어인데, 이것은 메소드의 본체가 아무런 실마리도 갖지 말아야 한다는 것을 의미한다! 이 숫자는 메소드 호출이 있어야만 가능한 메소드 외부에서 나와야 한다.

메소드에 대한 외부의 입력은 **인수** 혹은 *매개변수*로 주어진다.

호출 중에 인수를 지원하려면 메소드의 개념을 다음과 같이 수정해야 한다.

```java

	ReturnType methodName(ArgType argName) {

		method-body

	}

``` 

메소드 개념에 유일하게 추가된 것은 다음 구절이다:

```ArgType argName``` 

괄호 안의 ```argName```은 인수를 나타내고, ```ArgType```은 인수의 타입이다. 다음 예제가 이해를 도울 것이다.

##### Snippet-01: 인수가 있는 메소드: 정의

 ```numOfTimes```라는 인수를 사용하는 메소드 정의를 보자.

```java

	jshell> void sayHelloWorld(int numOfTimes) {
	   ...> }
	| created method sayHelloWorld(int)
```

메소드를 호출해보자.

```java
	jshell> sayHelloWorld()
	| Error:
	| method sayHelloWorld in class cannot be applied to given types;
	| required : int
	| found : no arguments
	| reason : actual and formal argument lists differ in length
	| sayHelloWorld(
	|^-----------------^
	jshell> sayHelloWorld(1)
	jshell>

```

메소드 호출은 정의된 것과 동일한 수의 인수와 타입을 포함해야 한다.  ```sayHelloWorld```가 한 개의 매개변수를 가지는 것으로 정의되었기 때문에 ```sayHelloWorld()```는 에러가 발생하고 ```sayHelloWorld(1)```는 동작한다.

그러나 이 메소드는 아무 것도 하지 않는다. 슬프지 않은가?

##### Snippet-02 : 매개변수 전달 및 접근

다음 예제는 본문 코드가 호출 중에 전달된 인수에 접근하는 방법을 보여 준다. 뿐만 아니라, 인수 값은 계산 중에 사용할 수 있다.

```java

void sayHelloWorld(int numOfTimes) {
	System.out.println(numOfTimes);
}

```

`System.out.println(numOfTimes)` 은 전달된 인수의 값을 출력한다.

하나의 메소드는 프로그램 내에서 여러 번 호출 될 수 있고, 매 번 다른 값을 전달 받을 수도 있다. 다음 예제가 이 사실을 보여준다.

```java

	jshell> sayHelloWorld(1)
	1
	jshell> sayHelloWorld(2)
	2
	jshell> sayHelloWorld(4)
	4
	jshell> /edit sayHelloWorld
	| modified method sayHelloWorld(int)
	jshell>

```

##### Snippet-03: 더 복잡한 메소드

메소드 내의 코드는 어디든 유효한 Java 코드가 될 수 있다! 예를 들어 ```for문```과 같은 반복문 코드를 작성할 수 있다.

다음 예시를 보자:

```java

	void sayHelloWorld(int numOfTimes) {
		for (int i=1; i<=numOfTimes; i++) {
			System.out.println(numOfTimes);
		}
	}

```

 위의 예시에서, 우리는 각 메소드가 호출 될 때마다  ```numOfTimes```만큼 출력했다.

```2```를 두 번, ```4```를 네 번 출력한다.

```java

	jshell> sayHelloWorld(2)
	2
	2
	jshell> sayHelloWorld(4)
	4
	4
	4
	4
	jshell>

```

##### Snippet-4 : Saying "Hello World", Again and again...

우리는 "Hello World"를 여러 번 출력하고 싶었다. 메소드를 다음과 같이 수정해보자:

```java
	void sayHelloWorld(int numOfTimes) {
		for (int i=1; i<=numOfTimes; i++) {
			System.out.println("Hello World");
		}
	}
```

멋지지 않은가?

```java
	jshell> sayHelloWorld(1)
	Hello World
	jshell> sayHelloWorld(2)
	Hello World
	Hello World
	jshell> sayHelloWorld(4)
	Hello World
	Hello World
	Hello World
	Hello World
	jshell>

```

이제 이 코드를 Java 강사에게 자랑스럽게 증명할 수 있다. 여러분의 프로그램은 임의의 횟수만큼 "Hello World"를 출력할 수 있다!

What started off giving you a headache, will probably keep you in her good books, for the rest of your course!

이렇게 자신감 강화로 무장한 여러분이 자바에서 저지르는 실수를 살펴봅시다.
.
  
##### Snippet-5 : 매개변수 타입 불일치


자바 언어는 형식 호환성을 위해 규정된 엄격한 규칙을 가진 강력한 형식의 언어다. 우리는 변수를 가지고, 그리고 그들의 수식과 할당을 어떻게 다루는지를 보았다. 메소드 호출의 인수를 메소드 정의와 일치시켜야 할 때 컴파일러에 의해 동일한 유형의 호환성 규칙이 적용된다

```java

	jshell> sayHelloWorld("value")
	| Error:
	| incompatible types: java.lang.String cannot be converted to int
	| sayHelloWorld("value")
	|               ^-----^
	jshell> sayHelloWorld(4.5)
	| Error:
	| incompatible types: possibly lossy conversion from double to int
	| sayHelloWorld(4.5)
	|               ^-^
	jshell>

```

#### 요약

이번 단계에서는:


* Java가 메소드의 인수를 지원하는 이유와 이를 사용하는 방법을 이해했다
* 메소드의 인수가 편리성과 재사용으로 이어지는 방법을 관찰했다
* 실제 인수에 대한 형식 호환성을 준수하기로 결정했다.

### Step 05:  PE-02 실습 모음 (솔루션 포함)

#### 실습

1. ```1``` 부터 ```n```에 이르는 모든 연속된 정수를 출력하는 ```printNumbers(int n)``` 메소드를 작성하시오.
2. ```1``` 부터 ```n```까지 모든 연속된 정수의 제곱을 출력하는  ```printSquaresOfNumbers(int n)``` 메소드를 작성하시오.

#### 솔루션-01

```java

	jshell> void printNumbers(int n) {
	   ...> for(int i=0; i< n; i++) {
	   ...> System.out.println(i);
	   ...> }
	   ...> }
	| created method printNumbers(int)
	
```

**jshell>**

#### 솔루션 2

```java

	jshell> void printSquaresOfNumbers(int n) {
	   ...> for(int i=0; i< n; i++) {
	   ...> System.out.println(i*i);
	   ...> }
	   ...> }
	| created method printSquaresOfNumbers(int)
	jshell>

```

### Step 07: *PMT-Challenge* 복습 (그리고 복잡한 것들..)

메소드는 그 자체로 코드 블록의 이름을 지정하고 재사용할 수 있는 우아한 방법을 제공한다. 게다가, 그것의 수행은 매개변수로 제어될 수 있다.

*PMT-Challenge*의 기존 솔루션을 더욱 우아하게 보충할 수 있을까? 그래, 지금 우리가 말하는 건:
1. 5의 곱셈표 인쇄 방법 작성
2. 이 메소드를 사용하여 임의의 숫자에 대한 곱셈표를 출력한다.

한번 볼래? 바로 시작해보자.

우리가 앞서 한 일은 다음과 같다:

```java

	jshell> for (int i=1; i<=10; i++) {
	   ...> System.out.printf("%d * %d = %d", 5, i, 5*i).println();
	   ...> }
	5 * 1 = 5
	5 * 2 = 10
	5 * 3 = 15
	5 * 4 = 20
	5 * 5 = 25
	5 * 6 = 30
	5 * 7 = 35
	5 * 8 = 40
	5 * 9 = 45
	5 * 10 = 50

```


이 문제를 하나의 메소드로 포장해보자.

```java

	void printMultiplicationTable() {
		for (int i=1; i<=10; i++) {
		System.out.printf("%d * %d = %d", 5, i, 5*i).println();
		}
	}

```

여러분은 5의 곱셈표를 출력하기 위해 이를 호출하기만 하면 된다.

```java

	jshell> printMultiplicationTable()
	5 * 1 = 5
	5 * 2 = 10
	5 * 3 = 15
	5 * 4 = 20
	5 * 5 = 25
	5 * 6 = 30
	5 * 7 = 35
	5 * 8 = 40
	5 * 9 = 45
	5 * 10 = 50
	jshell>
	
```

#### 요약

이번 단계에서는

* 앞서 본  *PMT-Challenge* 솔루션을 다시 살펴보았다.
*  ```printMultiplicationTable()```의 메소드 정의에 이 논리를 적용하였다.
* 아직 이 힘을 충분히 탐구하지 못했다!

### Step 08: 인수가 있는 메소드와 오버로딩(Overloading)

```printMultiplicationTable()```와 같은 정의의 진정한 힘은 이를 인수로 무장했을 때 나온다. 그냥 인수가 아니라 진짜 "값" 말이다!

우리는 ```printMultiplicationTable()```를 수정해 보다 더 유연하게 매개변수를 받아들이도록 할 것이다.

```java
	void printMultiplicationTable(int number) {
		for (int i=1; i<=10; i++) {
			System.out.printf("%d * %d = %d", number, i, number*i).println();
		}
	}
```

우리는 이제 ```printMultiplicationTable(number)```메소드를 호출함으로써 어떤 숫자든 곱셈표를 출력할 수 있다.

```java

	jshell> printMultiplicationTable(6)
	6 * 1 = 6
	6 * 2 = 12
	6 * 3 = 18
	6 * 4 = 24
	6 * 5 = 30
	6 * 6 = 36
	6 * 7 = 42
	6 * 8 = 48
	6 * 9 = 54
	6 * 10 = 60
	jshell>
	
```

여기서 새롭게 설명한 것은 없다. 우리는 그저 이미 배웠던 것들을 조합했을 뿐인데 기존 코드에 메소드의 멋짐을 더했다.

여러분, 이 프로그램의 힘, 단순함, 우아함에 흠뻑 빠져보십시오!


#### 오버로딩된 메소드

`printMultiplicationTable()` and `printMultiplicationTable(5)` 라는 두 가지 버전의 메소드를 호출할 수 있음을 알았다. 

```java

	jshell> printMultiplicationTable()
	5 * 1 = 5
	5 * 2 = 10
	5 * 3 = 15
	5 * 4 = 20
	5 * 5 = 25
	5 * 6 = 30
	5 * 7 = 35
	5 * 8 = 40
	5 * 9 = 45
	5 * 10 = 50
	jshell>

```

 그리고 

```java

	jshell> printMultiplicationTable(5)
	5 * 1 = 5
	5 * 2 = 10
	5 * 3 = 15
	5 * 4 = 20
	5 * 5 = 25
	5 * 6 = 30
	5 * 7 = 35
	5 * 8 = 40
	5 * 9 = 45
	5 * 10 = 50
	jshell>

```

이름은 같지만 매개 변수 수는 다른 여러 메소드를 가질 수 있다. 이것을 ***메소드 오버로딩***이라고 한다.


#### 요약

이번 단계에서는 

* 인수를 전달함으로써 ```printMultiplicationTable()```의 논리를 강화시켰다.
* Added flexibility to the *PMT-Challenge* 솔루션에 유연성을 더했다.
* 메소드 오버로딩 개념을 소개했다.

### Step 09:  여러 개의 인수를 가진 메소드

한 개 이상의 인수를 갖는 메소드를 정의하는 것은 가능하고 꽤 유용하다.
우리는 이미 각각 두 개의 인수를 갖는 자바의 내장 메소드 ```Math.max``` 와 ```Math.min```를 어떻게 호출하는지 알아보았다.
이제 우리 스스로도 그러한 메소드을 하나 써보면서 우리의 이해를 증진시킬 시간이다.

 ```void sum(int, int)```두 정수의 합을 계산하고 결과를 출력하는 메소드이다.

```java 

	jshell> void sum(int firstNum, int secondNum) {
	   ...> int sum = firstNum + secondNum;
	   ...> System.out.println(sum);
	   ...> }
	| created method sum(int, int)
	jshell> sum(5, 10)
	15
	jshell>

```

 ```void sum(int, int, int)``` 는 세 정수의 합을 계산하고 결과를 출력하는 메소드이다.

```java

	jshell> void sum(int firstNum, int secondNum, int thirdNum) {
	   ...> int sum = firstNum + secondNum + thirdNum;
	   ...> System.out.println(sum);
	   ...> }
	| created method sum(int,int,int)
	jshell> sum(5, 10, 15)
	30
```

```sum```이라는 이름은 같고 인수의 수는 다르다. 이를 오버로딩된 메소드라고 한다.

#### 요약

이번 단계에서는

* 메소드 오버로딩에 대한 이해를 활용하여 자체적으로 메소드를 정의했다.


### Step 10: 메소드로부터의 반환

메소드는 계산 결과를 반환하도록 코딩될 수도 있다. 이러한 결과를 **반환 값**이라고 한다.

많은 자바 내장 메소드들은 반환 값을 가지고 있다. 우리가 가장 주목할 만한 것은  ```Math.min()``` 과 ```Math.max()```이다. 

```java
	jshell> Math.max(15, 25)
	$1 ==> 25
	jshell> $1
	$1 ==> 25

```

```Math.max()``` 는  ```JShell```의 변수 ```$1```에 저장된 값을 반환한다.

반환 메커니즘은 다음과 같은 유연성을 제공하기 때문에 매우 중요하다.
* 계산된 결과를 다른 코드 및 메소드와 공유
* 문제 해결을 위해 하위 문제로 분할

다음 예시에서는 메소드의 반환 값을 수집하는 방법을 설명한다.

```java
	jshell> int max = Math.max(15, 25)
	max ==> 25
	jshell> max
	max ==> 25
	jshell>

```

변수 ```int max```에 반환 값을 저장한다.

우리는 비슷한 방식으로 값을 반환하는 메소드를 직접 작성할 수 있다. 위의  ```sumOfTwoNumbers```메소드에서 ```sum```을 보여주지 않고 호출한 코드로 ```반환```한다.

```java

	jshell> int sumOfTwoNumbers(int firstNum, int secondNum) {
	   ...> int sum = firstNum + secondNum;
	   ...> return sum;
	   ...> }
	| created method sumOfTwoNumbers(int,int)
	jshell> sumOfTwoNumbers(1, 10)
	$2 => 11
```

```return sum;```이라는 구문은 **반환문**이라고 한다.

```sum = sumOfTwoNumbers(1, 10)``` 코드가 실행될 때, ```sum```은 ```sumOfTwoNumbers()```에서 반환된 결과를 취합한다. 이제 콘솔에 ```sum```을 출력하거나, 다른 변수에 저장하거나, 
심지어 다른 메소드를 호출할 때 이를 인자로 넘겨줄 수도 있다!


```
	jshell> sum = sumOfTwoNumbers(1, 10)
	sum => 11_
	jshell> sum = sumOfTwoNumbers(15, 15)
	sum => 30
	jshell>
```

#### 요약

이번 단계에서는

* 메소드를 이용한 반환 메커니즘의 필요성을 이해했다.
* 반환문을 알아보았다
* 반환 값을 가지는 ```sumOfTwoNumbers()```메소드를 직접 작성하고 어떻게 하면 더 유연해지는지 알아보았다.


### Step 11: 실습 모음 PE-04 (솔루션 포함)

이제 반환 값을 가지는 메소드에 대해 몇 가지 실습을 해보자

#### 실습

1. 세 개의 정수의 합을 반환하는 메소드를 작성하시오.
2. 삼각형의 두 각도를 의미하는 두 정수를 입력받는 메소드를 작성하고, 세 번째 각도를 계산한다.
*힌트: 삼각형의 세 각의 합은 180도이다.*


#### 솔루션-01

```java

	jshell> int sumOfThreeNumbers(int firstNum, int secondNum, int thirdNum) {
	   ...> int sum = firstNum + secondNum + thirdNum;
	   ...> return sum;
	   ...> }
	| created method sumOfThreeNumbers(int,int, int)
	jshell>

```

#### 솔루션-02

```java

	jshell> int getThirdAngle(int firstAngle, int secondAngle) {
	   ...> int sumOfTwo = firstAngle + secondAngle;
	   ...> return 180 - sum;
	   ...> }
	| created method getThirdAngle(int,int)
	jshell>
	
```

### Step 12: 자바 메소드 복습
In this section, we introduced you to the concept of methods in Java.
이번 섹션에서는 자바의 메소드의 개념에 대해 소개했다.
* 우리는 메소드가 계산 단위 하나를 수행하는 루틴이라는 것을 이해했다. 이들은 일련의 구문을 하나의 블록으로 그룹화하며, 메소드 호출을 통해 호출되어 실행되어야 한다.
* 인수가 없거나 한 개 이거나, 여러 개인 메소드를 정의할 수 있다.
* 메소드는 내부의 연산 결과를 반환하도록 정의할 수도 있다. 이는 프로그램을 더 유연하게 만들어준다.


## 자바 플랫폼의 이해

JShell은 자바 프로그래밍의 기초부터 시작한다는 점이 놀랍ㄴ다. 이는 자바 코드의 작성, 컴파일, 실행 뒤에 숨겨진 모든 복잡성을 추상화한다.

화면 뒤에서는 무슨 일이 일어날까? 지금부터 알아보자.

### Step 01: 자바 플랫폼 - 소개


컴퓨터는 비트라고 불리는 ```0```과 ```1```의 연속적인 이진 코드만 이해한다. 모든 명령은 실행 전에 ```0```과 ```1```들로 전환되어야 한다.
***JShell에서 코드를 작성할때, 이를 어떻게 이진코드로 전환하는가?***

우리는 학습, 기억, 유지관리가 용이하기 때문에 자바와 같은 고급 언어로 프로그램을 작성한다.
누가 이것을 이진 코드로 변환하는가?

일반적으로 **Compiler**는 프로그래밍 언어의 구문을 이해하고 이진 코드로 변환하는 프로그램이다.
자바 디자이너들은 그것이 플랫폼에 독립적이기를 원했다. 코드를 한 번 컴파일하여 아무 곳에서나 실행하십시오.
그러나 운영 체제마다 명령 모음이 다르다. 즉, 이진 코드가 다르다.

자바는 다음과 같은 흥미로운 솔루션을 제공한다:
\- 모든 자바 컴파일러는 소스 코드를 **바이트 코드**라고 불리는 **중간 표현**으로 번역한다.
- 자바 프로그램(**바이트 코드**)을 실행시키기 위해서는 ***JVM***(자바 가상 기계)가 필요하다
	- ***JVM***은 **바이트 코드**를 이해하고 실행시킨다.
	- 운영체제마다 서로 다른 JVM이 존재한다. 윈도우 JVM은 **바이트 코드**를 윈도우에서 실행 가능한 명령어로 변환한다. 리눅스 JVM은 **바이트 코드**를 리눅스에서 실행 가능한 명령어로 변환한다.
\

자바 컴파일러는 자바 소스 코드를 **바이트 코드**로 번역하고, 이는 컴퓨터의 **.class**파일로 저장된다.

#### 요약

이번 단계에서는

* 소스 코드 변환 시, 자바 컴파일러의 역할에 대해 이해했다.
* 바이트 코드와 같은 중간 표현(IR)의 필요성에 대해 인지했다.
* (컴파일러 + 자바 가상 기계 + 운영체제) 조합이 소스 코드 이식성을 보장하는 방법 이해했다.


### Step 02: 자바의 ```클래스``` 작성

먼저, `클래스`의 개념에 대해 이해해보자.

다음 예시를 살펴보아라:

**국가**는 *개념*이다. **인도**, **미국**, 그리고 **네덜란드** 는 **국가**의 *예시* 혹은 *인스턴스(사례)*이다.

마찬가지로, `클래스`는 하나의 템플릿이다. `객체`는 `클래스`의 `인스턴스`이다. 

객체 지향 프로그래밍에 관한 섹션에서 `클래스`와 `객체`에 대해 더 많이 논의해 볼 것이다.

클래스를 만드는 구문과 클래스의 객체는 매우 간단하다.


```java

	jshell> class Country {
	   ...> }
	created class Country
```

클래스의 인스턴스를 생성해보자:


```java
	jshell> Country india = new Country();
	india ==> Country@6e06451e
```

구문은 간단하다 - `ClassName objectName = new ClassName()`.

```india``` 는 ```Country```타입의 객체이며, ```6e06451e``` 로 표시된 메모리 공간에 저장된다. 


클래스의 객체를 몇 개 더 생성해보자:

```java
	jshell> Country usa = new Country();
	usa ==> Country@6e1567f1
	jshell> Country netherlands = new Country();
	netherlands ==> Country@5f134e67
	jshell>

```

 ```india```, ```usa``` 와 ```netherlands``` 는 ```Country```타입의 서로 다른 객체들이다. 

우리는 아직 ```클래스```와 ```Country```의 내용은 살펴보지 않았다.

```클래스```는 모든 데이터 (멤버 변수)와 메소드 정의를 포함하기도 한다. 이에 대해서는 적절한 시기에 알아보자.

또 다른 예시가 있다:

```java

	jshell> class Planet {
	   ...>}
	created class Planet
	jshell> Planet planet = new Planet();
	planet ==> Planet@56ef9176
	jshell> Planet earth = new Planet();
	earth ==> Planet@1ed4004b
	jshell> Planet planet = new Planet();
	venus ==> Planet@25bbe1b6

```

우리는 ```Planet```이라는 ```클래스```를 위한 또 다른 개념을 만들었다.

```Planet```은 또 다른 템플릿이다. ```planet```, ```earth``` 그리고 ```venus```는 `Planet`클래스의 객체이다.


#### 요약

이번 단계에서는

* ```클래스```의 창조가 어떻게 새로운 타입을 만들어내는지 확인했다.
* 클래스의 인스턴스 (객체) 생성 방법에 대해 이해했다.

### Step 03: ```클래스``` 에 메소드 추가하기

```클래스```내에 정의한 메소드는 ```클래스```객체에 대해 수행할 수 있는 것보다  더 많은 동작을 의미한다.

```Planet``` 메소드 안에 ```revolve()```를 정의해보자!

```java

		jshell> class Planet {
	   ...> void revolve() {
	   ...> System.out.println("Revolve");
	   ...> }
	   ...> }
	replaced class Planet
	update replaced variable planet, reset to null
	update replaced variable earth, reset to null
	update replaced variable venus, reset to null
```
`revolve()` 구문은 이전에 우리가 만들어 보았던 다른 메소드들과 비슷하다. 

> 새로운 메소드를 추가한 결과, ```클래스``` 템플릿이 업데이트 되었다.
> 이전 사례인 ```planet```,```earth``` 그리고 ```venus```는 ```이전 템플릿을 기반으로 하기 때문에 ```null```로 재설정되었다.

\

몇몇 객체를 다시 생각해보자.


```java
	jshell> Planet earth = new Planet();
	earth ==> Planet@192b07fd
	jshell> Planet planet = new Planet();
	venus ==> Planet@64bfbc86
	jshell>

```

 ```revolve``` 메소드를 어떻게 호출하는가?

```java

	jshell> Planet.revolve();
	| Error:
	| non-static method revolve() cannot be referenced from a static context
	| Planet.revolve();
	|^-----------------^
	jshell> earth.revolve();
	Revolve
	jshell> venus.revolve();
	Revolve
	jshell>

```

```revolve()```가 정적 메소드가 아니기 때문에 이를 수행하기 위한 우리의 시도는 ```Planet.revolve()``` 구문에서는 통하지 않았다. (뒷부분에 더 자세히 설명)
```earth.revolve()```를 통해 ```revolve()```를 호출하는 시도는 성공했다. ```earth```가 ```Planet```타입의 객체이기 때문이다. 

#### 요약

이번 단계에서는

* 기존 ```클래스```에 메소드를 추가하는 방법을 배웠다.
* ```클래스```의 객체에서 이를 어떻게 호출하는지 발견했다.


### Step 04: 별도의 소스 파일에서 Java 코드 쓰기 및 실행

지금까지 우리는 친근한 이웃인 ```JShell```과 함께 클래스를 만들고 그 안에서 메소드를 정의하는 것을 즐겼다.

```JSHell```은 일부 자바 구문 규칙을 완화시키고 우리를 대신하여 컴파일러를 호출하며 룸서비스처럼 코드를 실행함으로써 우리 아이들을 버릇없게 했다.

개구리 왕자들이 속담에 나오는 우물에서 벗어날 때가 왔다. 그래, 네 말이 맞아! 적절한 코드 편집기에서 코드를 쓰기 시작하고, 더 넓은 세상으로 나아갈 시간이다.

먼저 새 소스 코드 파일 'Planet.java'를 만드는 것으로 시작합시다. 하드 디스크의 폴더를 선택하고 아래와 같은 파일을 만드십시오:

_**Planet.java**_

```java

	class Planet {
		void revolve() {
			System.out.println("Revolve");
		}
	}

```

>  ```/list Planet```이라는 명령어를 실행하고 복사하면 JShell에서 이미 작성한 ```Planet```코드를 얻을 수 있다.
> 지금은 원하는 텍스트 편집기를 아무거나 사용할 수 있다.

소스 파일의 이름은 가지고 있는 ```클래스```이름과 일치해야 한다. 여기서는 우리는 파일 이름을 `Planet.java`로 지어야 한다.

다음 단계는 이 코드를 컴파일 하는 것이다. (2단계). 이를 위해 ```JShell```을 종료하고 시스템 터미널 또는 명령 프롬프트를 다시 실행하십시오. 자, 이제, 어떤 효과가 있는지 봅시다!


```java

	jshell> /exit
	|  Goodbye
```

 `Planet.java` 파일을 만든 폴더에 ```cd```하여라.

```
	in28minutes$> cd in28Minutes/git/JavaForBeginners/
	command-prompt> ls
	Planet.java
```

자바 버전을 클릭하여라.

```
	command-prompt> java -version
	java version "x.0.1"
	Java(TM) SE Runtime Environment (build x.0.1+11)
	Java HotSpot(TM) 64-bit Server VM (build x.0.1+11, mixed mode)
```

```javac Planet.java```를 사용해서 자바 코드를 컴파일 할 수 있다. 이제 `바이트 코드`를 포함하고 있는 `Planet.class`라는 이름으로 만들어진 새로운 파일을 볼 수 있다. 

```
	command-prompt> javac Planet.java
	command-prompt> ls
	Planet.class         Planet.java_
```

`java Planet` 명령어를 사용해 클래스를 실행할 수 있다..

```java
	command-prompt> java Planet
	Error: Main method not found inside class Planet, please define the main method as
	public static void main(String[] args)
	or a JavaFX application class must extend javax.application.Application
	command-prompt>	
```

왜 에러가 발생하는가? 다음 단계에서 논의해보자.

#### 요약

이번 단계에서는

* 'JShell'에서 미개척 영역으로 과감하게 전환하여 소스 코드 작성해보았다.
* 터미널에서 컴파일러를 호출하여 소스 파일을 컴파일하는 방법 알아보았다.


### Step 05: ```main()```소개와 바이트 코드 실행

이전 단계에서, 우리는 **_Planet.java_** 를 컴파일했다. 이번 단계에서는, **_Planet.class_** 내에 있는 바이트 코드를 실행해 봅시다.

##### Snippet-01: ```Planet``` 실행

**_콘솔 명령어_**

```java

	command-prompt> ls
	Planet.class         Planet.java
	command-prompt> java Planet
	Error: Main method not found inside class Planet, please define the main method as
	public static void main(String[] args)
	or a JavaFX application class must extend javax.application.Application
	command-prompt>

```

The code may have compiled without any errors, but what's the use if we cannot run the program to see what stuff it's got!
코드는 아무 오류 없이 컴파일했을지 모르지만, 프로그램을 실행하지 못하면 무슨 소용이 있겠는가!
**_The ```main()``` 메소드는 어떠한 ```클래스```내에서 정의된 코드를 컴파일하는 데에 필수적이다._**

```main()```의 정의는 다음과 같은 정확한 구문을 가져야한다.

`public static void main(String[] args) {  /* <일부 코드가 여기에 포함됨> */ }`

A few details:
* `void` is its return type
* `main` is its name
* `args` is its formal argument. Here, it's an **array** of ```String```.
* `public``` and ```static``` are reserved Java keywords. More on these later sections.

몇 가지 세부 사항:
* 반환형은 'void' 입니다.
* `main`은 그 이름이다.
* `aggs`는 공식적인 인수이다. 여기에서는 ```String```의 **배열**이다.
* ```public```과 ```static```은 자바의 키워드다. 이후의 섹션에 대해 자세히 알아보자.


```Plnet``` 코드 안에 그러한 정의를 하나 더 추가하자. 텍스트 편집기를 열고 아래와 같은 ```main``` 메소드를 추가하라.

**_Planet.java_**

```java

	class Planet {
		void revolve() {
			System.out.println("Revolve");
		}
		public static void main(String[] args) {

		}
	}

```

이제 실행해보자:

```java

	command-prompt> java Planet
	Error: Main method not found inside class Planet, please define the main method as
	public static void main(String[] args)
	or a JavaFX application class must extend javax.application.Application
```

왜 결과에는 변화가 없는 것일까?

Java 소스 파일을 변경한 후 코드를 다시 컴파일하여 새 클래스 파일을 만드십시오.

```
	command-prompt> javac Planet.java
	command-prompt> ls
	Planet.class         Planet.java_
```

다시 시도해보자.

```
	command-prompt> java Planet
	command-prompt>

```
터미널이 텅 비었다. 왜?

우리는 ```main``` 메소드 안에 무엇을 작성했는가? 아무 것도 없다.


```java
		public static void main(String[] args) {

		}

```

고치자. **_Planet.java_** 를 다시 한 번 수정해야 한다!

**_Planet.java_**

```java

	class Planet {
		void revolve() {
			System.out.println("Revolve");
		}
		public static void main(String[] args) {
			Planet earth = new Planet();
			earth.revolve();
		}
	}

```

**_콘솔 명령어_**

```java

	command-prompt> javac Planet.java
	command-prompt> ls
	Planet.class         Planet.java
	command-prompt> java Planet
	Revolve
	command-prompt>

```

빙고! 드디어 우리가 보고 싶은 걸 얻었어!

#### 요약

이번 단계에서는

* 자바 프로개름을 실행하기 위해서는 ```main()``` 메소드가 필요함을 배웠다.
* 모든 코드를 업데이트할 때 마다, 소스 파일을 컴파일 해야 한다는 것을 발견했다.

### Step 06:  ```Planet```에 대한 더 복잡한 것들

이 단계에서는 ```Planet```의 소스 코드를 가지고 놀아보자. 시행착오를 겪으면서 에러의 희극에 대비하라!
아래는 잘 작동하는 ```Planet```코드이다:

**_Planet.java_**

```java

	class Planet {
		void revolve() {
			System.out.println("Revolve");
		}
		
		public static void main(String[] args) {
			Planet earth = new Planet();
			earth.revolve();
		}
	}

```

미친 짓을 한 번 해보자.

##### Snippet-01: Messing-up ```main()``` - v1

메소드 이름을 `main` 에서 `main1`로 변경하여라. 



**_Planet.java_**

```java

	class Planet {
		void revolve() {
			System.out.println("Revolve");
		}

		public static void main1(String[] args) {
			Planet earth = new Planet();
			earth.revolve();
		}
	}

```

**_콘솔 명령어_**

```java

	command-prompt> javac Planet.java
	command-prompt> java Planet
	Error: Main method not found inside class Planet, please define the main method as
	public static void main(String[] args)
	or a JavaFX application class must extend javax.application.Application
	command-prompt>

```

 ```main()```의 메소드의 이름을 함부로 건드리지 마라.

다른 부분들도 다음과 같이 동일하게 유지될 필요가 있다:
* 반환형: ```void```
* 인수 타입: ```String[]```
* 키워드 ```public``` and ```static```.

##### Snippet-02: Messing-up ```main()``` - v2

`Planet earth = new Planet()`구문과 `earth.revolve()` 구문 뒤의  세미콜론을 삭제하여라.

**_Planet.java_**

```java

	class Planet {
		void revolve() {
			System.out.println("Revolve");
		}

		public static void main(String[] args) {
			Planet earth = new Planet()
			earth.revolve()
		}
	}

```

**_콘솔 명령어_**

```java

	command-prompt> javac Planet.java
	Planet.java:6: error: ';' expected
	Planet earth =  new Planet()
	|_______________________^
	Planet.java:7: error: ';' expected
	earth.revolve()
	|_____________^
	2 errors
	command-prompt>

```

 ```;``` 기호는 자바의 구문 구분자로 의무화 되어있다.

JShell에서는 필요하지 않지만 별도의 Java 소스 파일을 작성할 때는 필수 사항이다.


##### Snippet-03: Messing-up  ```main()``` - v3

`Planet earth = new Plane();`라는 오타를 만들어보자.

**_Planet.java_**

```java

	class Planet {
		
		void revolve() {
			System.out.println("Revolve");
		}

		public static void main(String[] args) {
			Planet earth = new Plane();
			earth.revolve();
		}
	}

```

**_콘솔 명령어_**

```java

	command-prompt> javac Planet.java
	Planet.java:6: error: cannot find symbol
	Planet earth =  new Plane();
	|________________^
	symbol: class Plane
	location: class Planet
	1 error
	command-prompt>

```

```Planet``` 의 철자를 **```Plane```** 로 잘못 표기했고 컴파일러가 이 오류를 잡아냈다. 그것은 우리에게 우리의 실수를 바로잡는 데 도움이 되는 메시지가 담긴 붉은 표시를 보여준다.

##### Snippet-04: Messing-up ```main()``` - v4

존재하지 않는 메소드 `earth.revolve1();`를 호출해보자.

**_Planet.java_**

```java

	class Planet {
		void revolve() {
			System.out.println("Revolve");
		}

		public static void main(String[] args) {
			Planet earth = new Planet();
			earth.revolve1();
		}
	}

```

**_콘솔 명령어_**

```java

	command-prompt> javac Planet.java
	Planet.java:7: error: cannot find symbol
	earth.revolve1();
	|_____^
	symbol: method revolve1()
	location: variable earth of type Planet
	1 error
	command-prompt>

```

```revolve()```메소드의 철자를 **```revolve1()```** 로 잘못 표기하였다. 맞아, 컴파일러가 에러 메시지를 출력한다.

#### 요약


이번 단계에서는:
* 언어 기능에 대해 배우는 가장 좋은 방법은 작업 코드를 가지고 노는 것이라는 것을 알게 되었다.
* ```JShell```은 일부 구문 규칙을 완화하면서 코딩을 단순화한다는 것을 관찰하였다.
* 코드 편집기에서 Java 코드를 개발하는 것이 힘을 얻는 느낌이라는 결론을 내렸다!

### Step 07: JVM, JRE 그리고 JDK

*JVM*, *JRE* 그리고 *JDK* 란 무엇일까? 

모든 것이 '*J*'로 시작한다는 사실과는 별개로, 그들이 무엇을 포함하는지, 무엇을 하는지에 중요한 차이가 있다.

다음 목록은 이들을 조감해 준다.

**JVM**은 프로그램의 바이트 코드를 실행시킨다.

**JRE** = **JVM** + **라이브러리들** + **기타 구성 요소**

* *라이브러리들* 은 사용자가 생성하는 모든 프로그램 내에서 사용할 수 있으며, 자바에서 기본으로 제공하는 유틸리티이다.  ```System.out.println()``` 는 그러한 유틸리티 중 하나인```java.lang``` 라이브러리 내의 메소드이다.
* *기타 구성 요소* 는 디버깅 및 코드 프로파일링 도구 포함한다.(메모리 관리 및 성능용)


**JDK** = **JRE** + **컴파일러** + **디버거**

* *JDK* 는 **Java Development Kit**를 의미한다. 이것은 당신의 Java 프로그램을 컴파일러로 컴파일하고 실행(*JRE* 사용)하는데 필요한 묶음의 머리글자이다.

이 구조를 기억하는 흥미로운 방법은 다음과 같다.:

* **JDK** 는 자바 프로그램의 **컴파일과 실행**에 필요.

* **JRE** 는 자바 프로그램의 **실행**에 필요.

* **JVM**는 자바 프로그램으로부터 생성되는 **바이트 코드 실행**에 필요

몇 가지 시나리오를 확인하여 이해도를 테스트해 봅시다.

**Scenario 1**: 다른 운영체제를 사용하는 친구에게 *Planet.class*파일을 주었다. 그가 그 파일을 실행하려면 무엇이 필요한가?
먼저 운영 체제에 **JRE**를 설치하여라. 터미널에서 *java Planet*을 사용하여 실행해보자. 그는 이미 바이트코드를 가지고 있기 때문에 *javac*는 실행할 필요가 없다.

**Scenario 2**: 친구에게 *Planet.java*의 소스 파일을 주었다. 그가 그 파일을 실행하려면 무엇이 필요한가?
호환되는 버전의 *JDK*를 설치하십시오. *javac Planet.java*를 사용하여 코드를 컴파일하십시오. 터미널에서 *java Planet*을 실행하십시오.

요약하면

* **응용 프로그램 개발자** _가 필요한 것_ **==> JDK**

* **응용 프로그램 사용자** _가 필요한 것_ **==> JRE**

#### 요약

이번 단계에서는

* JVM, JRE 그리고 JDK에서 수행되는 작업의 범위와 그 차이를 이해했다.
* 각 명령어가 *javac* 및 *java*와 같은 서로 다른 터미널 명령에 의해 호출될 수 있는 방법을 실현했다.

## Eclipse

TODO - 수정 필요 

### TODO - Need Revision 

### Eclipse를 사용한 자바 소프트웨어 개발 소개

*  Eclipse IDE(통합 개발 환경)의 특징
	* 설치 및 구성
	* 작업영역 작성 및 구성
	* 프로젝트 생성 및 조직
		* JRE 버전 선택 및 포함된 라이브러리
		* Eclipse Java Perspectives
		* 소스 파일을 폴더 내에 구성
		* 패키지?
	* IDE 사용자 인터페이스 설명
		* Perspective
		* Views
		* 콘솔 콘텐츠 및 디스플레이 옵션

* Eclipse에서 새로운 자바 ```class```(와 관련 소스 파일) 생성하기 
	* 패키지 이름
		* 문제 해결을 위한 Java 솔루션은 여러 응용 프로그램의 구성요소로 구성될 수 있다. 각 구별되는 구성요소에 대한 클래스를 식별하는 것은 좋은 프로그래밍 요소로 간주된다. 패키지는 소스 코드로 클래스를 구성하는 자바 방식이다.
		* 비유: 냉장고에 있는 식기류(냉장고, 냉각선, 야채선, 보틀랙)
	* Public 메소드 stub : 기본 ```public static void main(String[] args)```를 만드는 데 사용할 수 있다.
	* (스냅샷 포함)
		* 선택한 옵션이 있는 클래스 만들기 팝업
		* 편집기 창에서 기본 생성된 소스 코드
		
	* 생성된 소스 코드를 필요에 맞게 사용자 정의
		* 구문 강조 표시
			* 키워드
			* 기본형 타입
			* 상수 리터럴: 숫자, 문자열
		* 코드 입력 시 자동 제안 기능

	* "Run as --> Java Application" 는 소스 코드를 컴파일하고 실행하기 위한 옵션
		* 옵션은 main() 메소드를 가진 클래스에 한하여 사용 가능.


#### 디버그 모드에서 Eclipse 사용

곱셈표 프로그램 실행은 단계별로 할 수 있다. 즉, 전체 응용 프로그램이 한 번에 실행되지 않고 최종 출력을 콘솔에 인쇄하는 것이다. 우리는 Eclipse IDE를 이용하여 그것의 실행을 제어함으로써 그것의 흐름을 몇 단계로 지연시킬 수 있다. 이것은 **디버그 모드**라고 불리는 Eclipse의 특별한 모드에서 가능하다.

이 과정을 **디버깅**이라고 하는데, 이 모드는 단순히 무슨 일이 일어나는지 보는 재미뿐만 아니라 소프트웨어 **버그**를 탐지하고 수정하는 데도 많이 사용되기 때문이다. 버그는 작성 중인 프로그램의 결함으로 인해 잘못된 실행으로 이어진다. 버그를 제거하는 과정을 디버깅이라고 한다. 인간은 인간이기 때문에 프로그래밍 오류는 자연스러운 것이며, IDE의 디버그 모드는 프로그래머에게 황금과 같은 가치가 있다. Eclipse가 Java 애플리케이션의 디버깅을 촉진하는 방법은 다음과 같다.

* 응용 프로그램을 디버깅하기 전에 **중단점**을 몇 개 설정해야 한다. 중단점은 디버그 모드에서 실행이 일시 중단되고 제어권이 프로그래머에게 전달되기 전에 프로그램의 출처에 있는 문장이다.
* 일시 중단된 프로그램에 있는 데이터의 전반적인 상태는 특정 중단점에서 프로그래머가 이용할 수 있다. 프로그램에 하나 이상의 중단점을 명시하게 되며, 실행이 중단되었을 때 다음과 같은 가능한 조치 목록을 수행할 수 있다:
	* 데이터 변수 읽기 및 수정
	* 프로그램 실행 재개
	* 현재 구문 재실행
	* 다음 중단점까지 모든 구문 건너뛰기

	기타 등등.
.	

* Eclipse IDE는 디버그 모드(디버그 모드 실행의 다양한 단계에서 IDE의 스냅샷 제공)에서 프로그램 실행을 제어하기 위해 프로그래머에게 매우 사용자 친화적이고 직관적인 인터페이스를 제공한다.
	
	* 중단점 설정 및 제거(토글링)
	* 메소드 호출이나 메소드 본체 내부/외부를 넘어 다님.(메소드를 호출하는 동안)
		* ```int print()``` 와 ```int print(int)``` 그리고 ```int print(int,int,int)``` 를 넘나드는 것은 흥미롭지만, ```System.out.printf```에 들어가는 것은 여러분을 놀라게 할 수 있다! 그래서, 당신은 그것을 넘어서는 것이 좋을지도 모른다.
	* For nested method calls, examine the method call **Stack Trace** (Call child, call parent relationship)
	* 중첩된 메소드를 호출하는 경우, **스택 추적(Stack Trace)*** 메소드를 검사하십시오(부모,자식 관계를 호출)
		* 예시 :  ```class MultiplicationTable```에서의 ```int print()```, ```int print(int)``` 와 ```int print(int,int,int)``` 메소드의 콜 체인.
	* 중단점에서 데이터 변수의 현재 상태 보기 및 수정
	* 소스 코드에서 한 구문에서 다른 구문으로 이동
		* 단계를 진행하면서 데이터 변수 값의 변화를 표시하는 뷰를 관찰하십시오.
		* 예를 들어 ```for문```의 제어 변수 ```i```가 ```class MultiplicationTable```의  ```int print(int,int,int)``` 메소드 내에 있을 때
		*  ```i<=10```이라는 조건이 더 이상 ```참```이 아닐 때 ```for문```에서 빠져나가는 것을 관찰하시오.
	* 해당 라인의 코드를 재실행
	* 다음 중단점까지 모든 코드 건너뛰기
	* 나머지 중단점 무시, 완료될 때까지 코드 실행 재개
	
### Eclipse IDE 키보드 바로가기

* 코드 텍스트 편집기 바로 가기
* 새 프로젝트/클래스 작성 바로 가기
* 클래스 검색

### JShell과 IDE의 차이점
 
방금 선언되었지만 초기화 없이 사용된 변수는 IDE에서 컴파일 오류를 플래그로 표시할 것이다! 그러나 JShell에서는 그렇지 않다. 일반 소프트웨어에서는 선언 시점에서의 변수 초기화(이미 알고 있는 바와 같이 "정의"라고 함)가 필수적이다

##### Snippet-1 : JShell은 언제든지 변수를 재정의 한다. 

```java

	jshell> int i = 2
	$1 ==> 2
	jshell> int i = 4
	$2 ==> 4
	jshell> long i = 1000
	$3 ==> 1000
	jshell>

```


다음 코드(JShell에 제공된 코드와 유사)를 수동으로 컴파일하거나 Eclipse와 같은 IDE에 의해 컴파일하면 오류가 플래그 표시됨!

```java

	package com.in28minutes.firstjavaproject;
	
	public class RedefineTestRunner {
		public static void main(String[] args) {
			int i = 2;
			int i = 4;
			long i = 1000;
			System.out.println(i);
		}
	}

```

그것은 자바 소스 코드가 엄격한 **범위 규칙(Scope Rule)** 에 의해 관리되기 때문이다.



*PMT-Challenge* 문제에 대한 솔루션을 통해 어떤 결과를 얻었는지 다시 한 번 살펴봅시다. 이제 코드 배열을 바꿔보자.

##### Snippet-01: 복습 - The *PMT-Challenge*

**_MultiplicationTable.java_**

```java

	package com.in28minutes.firstjavaproject;
	public class MultiplicationTable {
		public static void print() {
			for(int i=1; i<=10;i++) {
				System.out.printf("%d * %d = %d", 5, i, 5*i).println();
			}
		}
	}

```

**_MultiplicationRunner.java_**

```java

	package com.in28minutes.firstjavaproject;

	public class MultiplicationRunner {
		public static void main(String[] args) {
			MultiplicationTable table = new MultiplicationTable();
			table.print();	
	}	
}

```

**_Console Output_**

_5 * 1 = 5_

_5 * 2 = 10_

_5 * 3 = 15_

_5 * 4 = 20_

_5 * 5 = 25_

_5 * 6 = 30_

_5 * 7 = 35_

_5 * 8 = 40_

_5 * 9 = 45_

_5 * 10 = 50_

##### Snippet-01 Explained

* 이제 코드를 두 개의 소스 파일로 나누었다: 
	* **_MultiplicationTable.java_**: ```MultiplicationTable``` ```class```  정의에 필요한 몇 가지 메소드가 포함되어 있다.
	* **_MultiplicationRunner.java_**: ```MultiplicationTable``` ```class```의 기능을 호출하기 위한 클라이언트로써 동작하며, ```MultiplicationTable```의 객체를 인스턴스화 하고, ```print()``` 메소드를 호출하는 ```main()```메소드를 정의하고 있다.
* 이 코드가 재배열된 후에도 여전히 작동하게 되었다!

#### Print-Multiplication-Table: 강화

* 이제 우리는 먼 길을 왔음에도 불구하고 이 도전에 대한 현재의 해결책을 개선하고자 한다. **"한번 성공의 냄새를 맡게 되면, 하늘이 한계다!"**. 필요한 변화는 다음과 같다.:
	* 표를 출력해야 하는 숫자를 인수로 전달하시오.
	* 표에서 인덱스 항목이 출력될 (연속) 범위의 숫자를 전달하십시오. (예를 들어, ```15```에서 ```30``` 사이의 인덱스 항목이 ```6```의 표로 인쇄된다.)

이 모든 것을 이루기 위한 한 가지 방법은 ```print()``` 메소드에 오버로드를 호출할 것이다. 다음 예는 그러한 시도 중 하나이다

##### Snippet-02: 오버로딩된 print() 

```print()````를 오버로딩하는 것은 우리에게 효과가 있으며, 이제 우리는 어떤 테이블도 표시할 수 있는 세 가지 방법을 지원한다.

```java

		public static void print() {
			for(int i=1; i<=10;i++) {
				System.out.printf("%d * %d = %d", 5, i, 5*i).println();
			}
		}

```	

**_콘솔창 출력_**

_5 * 1 = 5_

_5 * 2 = 10_

_5 * 3 = 15_

_5 * 4 = 20_

_5 * 5 = 25_

_5 * 6 = 30_

_5 * 7 = 35_

_5 * 8 = 40_

_5 * 9 = 45_

_5 * 10 = 50_

```1```부터 ```10```까지 항목이 고정되어 있는 ```5```의 기본 표이다.

```java

		public static void print(int number) {
			for(int i=1; i<=10;i++) {
				System.out.printf("%d * %d = %d", number, i, number*i).println();
			}
		}

```

**_콘솔창 출력_**

_8 * 1 = 8_

_8 * 2 = 16_

_8 * 3 = 24_

_8 * 4 = 32_

_8 * 5 = 40_

_8 * 6 = 48_

_8 * 7 = 56_

_8 * 8 = 64_

_8 * 9 = 72_

_8 * 10 = 80_

아무 숫자의 표를 출력하지만 ```1```과 ``10``` 사이에 기입이 고정되어 있다.

```java

		public static void print(int number, int from, int to) {
			for(int i=from; i<=to;i++) {
				System.out.printf("%d * %d = %d", number, i, number*i).println();
			}
		}

```

**_Console Output_**

_6 * 11 = 66_

_6 * 12 = 72_

_6 * 13 = 78_

_6 * 14 = 84_

_6 * 15 = 90_

_6 * 16 = 96_

_6 * 17 = 102_

_6 * 18 = 108_

_6 * 19 = 114_

_6 * 20 = 120_

임의의 숫자에 대한 표 표시한다(모든 범위에 대한 항목 포함)

전체 코드:

**_MultiplicationTable.java_**

```java

	package com.in28minutes.firstjavaproject;
	
	public class MultiplicationTable {
		public static void print() {
			for(int i=1; i<=10;i++) {
				System.out.printf("%d * %d = %d", 5, i, 5*i).println();
			}
		}	
	
		public static void print(int number) {
			for(int i=1; i<=10;i++) {
				System.out.printf("%d * %d = %d", number, i, number*i).println();
			}
		}

		public static void print(int number, int from, int to) {
			for(int i=from; i<=to;i++) {
				System.out.printf("%d * %d = %d", number, i, number*i).println();
			}
		}
	}

```


**_MultiplicationRunner.java_**

```java

	package com.in28minutes.firstjavaproject;

	public class MultiplicationRunner {
		public static void main(String[] args) {
			MultiplicationTable table = new MultiplicationTable();
			table.print();
			table.print(8);
			table.print(6, 11, 20);
		}
	}

```

#### Issue: Code Duplication In Print-Multiplication-Table

```class MultiplicationTable``` 코드에 문제가 하나 있다. 최종 출력 형식에서 곱셈 기호 '```*```'를 '```X```'로 대체하여 학교 아이들이 더 좋아하게 하면 어떨까? ```print()``` 의 각 버전에 세 번의  ```System.out.printf()```호출이 있기 때문에, 우리는 세 번의 변경이 필요하다.

##### Snippet-3: 코드 중복

**_MultiplicationTable.java_**

```java

	package com.in28minutes.firstjavaproject;

	public class MultiplicationTable {
		public static void print() {
			for(int i=1; i<=10;i++) {
				System.out.printf("%d X %d = %d", 5, i, 5*i).println();
			}
		}

		public static void print(int number) {
			for(int i=1; i<=10;i++) {
				System.out.printf("%d * %d = %d", number, i, number*i).println();
			}
		}

		public static void print(int number, int from, int to) {
			for(int i=from; i<=to;i++) {
				System.out.printf("%d X %d = %d", number, i, number*i).println();
			}
		}
	}

```

**_콘솔창 출력_**

_5 X 1 = 5_

_5 X 2 = 10_

_5 X 3 = 15_

_5 X 4 = 20_

_5 X 5 = 25_

_5 X 6 = 30_

_5 X 7 = 35_

_5 X 8 = 40_

_5 X 9 = 45_

_5 X 10 = 50_

_8 * 1 = 8_

_8 * 2 = 16_

_8 * 3 = 24_

_8 * 4 = 32_

_8 * 5 = 40_

_8 * 6 = 48_

_8 * 7 = 56_

_8 * 8 = 64_

_8 * 9 = 72_

_8 * 10 = 80_

_6 X 11 = 66_

_6 X 12 = 72_

_6 X 13 = 78_

_6 X 14 = 84_

_6 X 15 = 90_

_6 X 16 = 96_

_6 X 17 = 102_

_6 X 18 = 108_

_6 X 19 = 114_

_6 X 20 = 120_

##### Snippet-3 설명

* 인간은 실수를 한다. 프로그래머가  ```void print(int, int)```코드의 형식 기호를 변경하는 것을 놓쳤지만, 우리는 처벌을 권하지 않는다. 그는 피곤했을 수도 있고, 몇 년 전에 다른 사람이 쓴 코드를 혼자 유지하고 있었을 수도 있다!! 요점은 인간의 결함을 탓하는 것이 아니라(많다) 코드 중복이 어떻게 오류를 일으키는지 보여주는 것이다. 이 문제는 오버로딩된 메소드에서 자주 발생한다.

* 인간의 본성을 바꾸려고 하는 대신에, 우리는 소프트웨어를 바꿀 수 있을까? ```print()```을 자세히 살펴보자:
	* ```void print()``` 메소드는 기본 범위 ```1```부터```10```까지의  ```5```의 곱셈표를 출력한다.
	* ```void print(int)``` 메소드는 어떤 숫자로도 곱셈표를 출력하지만 ```1```에서 ```10```까지의 일정한 범위에서만 산출된다.
	* ```void print(int,int,int)``` 메소드는 어떤 숫자로든, 모든 범위에서 곱셈표를 출력한다.
	
#### A Solution: 코드 재사용

앞의 예시에서 우리가 관찰할 수 있는 것이 있다. ```print()```의 모든 오버로딩된 버전은 거의 동일한 코드를 가지고 있다!

* ```print(int)``` 는 ```print()```보다 사용 잠재력이 넓다. 후자는 특별한 경우로 ```5```만을 출력하고 있다. 우리는 ```print(int)```에 ```5```라는 **고정된**매개변수 값을 전달하여 ```print()```가 하는 일을 수행할 수 있다. 간단한 예를 보자: ```5```를 전달하여 ```print()```내에 ```print(int)```를 호출해보자.
*  주목해야 할 점은 **좀 더 전문화된 기능이 보다 일반적인 기능의 범위 내에서 구현될 수 있다는 것이다**.

이제 코드의 이 부분을 재구성해 봅시다.

##### Snippet-4: 코드 재사용

**_MultiplicationTable.java_**

```java

	public static void print() {
		print(5);
	}

	public static void print(int number) {
		for(int i=1; i<=10;i++) {
			System.out.printf("%d * %d = %d", number, i, number*i).println();
		}
	}

```

**_MultiplicationRunner.java_**

```java

	package com.in28minutes.firstjavaproject;

	public class MultiplicationRunner {
		public static void main(String[] args) {
			MultiplicationTable table = new MultiplicationTable();
			table.print();
			table.print(8);
		}
	}

```

**_콘솔창 출력_**

_5 * 1 = 5_

_5 * 2 = 10_

_5 * 3 = 15_

_5 * 4 = 20_

_5 * 5 = 25_

_5 * 6 = 30_

_5 * 7 = 35_

_5 * 8 = 40_

_5 * 9 = 45_

_5 * 10 = 50_

_8 * 1 = 8_

_8 * 2 = 16_

_8 * 3 = 24_

_8 * 4 = 32_

_8 * 5 = 40_

_8 * 6 = 48_

_8 * 7 = 56_

_8 * 8 = 64_

_8 * 9 = 72_

_8 * 10 = 80_

##### Snippet-4 설명

우리가 다른 내부에서 어떤 메소드를 호출할 때, 해당 메소드 호출 구문은 본체로 대체된다.(실제 인자로 형식 인자도 대체함). ```int print()```의 새로운 정의에서, 호출 중 실행되는 코드는 다음과 같다: 

```java

	for(int i=1; i<=10;i++) {
		System.out.printf("%d * %d = %d", 5, i, 5*i).println();
	}

```

#### 코드 재사용 확장

* ```int print(int,int,int)``` 메소드는 ```int print(int)```보다 일반적인 버전이다. 우리는 전자에 대한 인수로 ```1```부터 ```10```까지의 일련의 **고정된** 인덱스를 전달함으로써 후자의 계산을 달성할 수 있었다. 다음의 코드를 살펴보자.

##### Snippet-5 : 코드 재사용 확장

**_MultiplicationTable.java_**

```java

	public static void print(int number) {
		print(number, 1, 10);		
	}	

	public static void print(int number, int from, int to) {
		for(int i=from; i<=to;i++) {
			System.out.printf("%d X %d = %d", number, i, number*i).println();
		}
	}

```

**_MultiplicationRunner.java_**

```java

	package com.in28minutes.firstjavaproject;

	public class MultiplicationRunner {
		public static void main(String[] args) {
			MultiplicationTable table = new MultiplicationTable();
			table.print(8);
			table.print(6, 11, 20);
		}
	}

```

**_콘솔창 출력_**

_8 * 1 = 8_

_8 * 2 = 16_

_8 * 3 = 24_

_8 * 4 = 32_

_8 * 5 = 40_

_8 * 6 = 48_

_8 * 7 = 56_

_8 * 8 = 64_

_8 * 9 = 72_

_8 * 10 = 80_

_6 * 11 = 66_

_6 * 12 = 72_

_6 * 13 = 78_

_6 * 14 = 84_

_6 * 15 = 90_

_6 * 16 = 96_

_6 * 17 = 102_

_6 * 18 = 108_

_6 * 19 = 114_

_6 * 20 = 120_

##### Snippet-5 설명

* 이 예시는 이전 단계에서 수행한 작업을 확장했을 뿐이다. 이제 우리는 다음 단계까지 나아갈 것이다! 그래, 우리는 ```print(int,int,int)```안에서 ```print()``` 를 구현할 것이다.

##### Snippet-6 : 코드 재사용 확장 (contd.)

**_MultiplicationTable.java_**

```java

	public static void print() {
		print(5, 1, 10);
	}

	public static void print(int number, int from, int to) {
		for(int i=from; i<=to;i++) {
			System.out.printf("%d X %d = %d", number, i, number*i).println();
		}
	}

```


**_MultiplicationRunner.java_**

```java

	package com.in28minutes.firstjavaproject;

	public class MultiplicationRunner {
		public static void main(String[] args) {
			MultiplicationTable table = new MultiplicationTable();
			table.print();
			table.print(6, 11, 20);
		}
	}

```


**_콘솔창 출력_**

_5 * 1 = 5_

_5 * 2 = 10_

_5 * 3 = 15_

_5 * 4 = 20_

_5 * 5 = 25_

_5 * 6 = 30_

_5 * 7 = 35_

_5 * 8 = 40_

_5 * 9 = 45_

_5 * 10 = 50_

_6 * 11 = 66_

_6 * 12 = 72_

_6 * 13 = 78_

_6 * 14 = 84_

_6 * 15 = 90_

_6 * 16 = 96_

_6 * 17 = 102_

_6 * 18 = 108_

_6 * 19 = 114_

_6 * 20 = 120_

##### Snippet-6 설명

*  코드 재사용의 동일한 논리를 확장함으로써,  ```int print(int,int,int)``` 메소드는 ```int print()```의 논리를 구현하는데 사용될 수 있다. 그저 매개변수인 숫자```5```와 고정된 범위 매변수 ```1```과 ```10```을 전자를 호출할 때 전달하십시오. 따라서 ```int print()``` 는 ```int print(int,int,int)```에 **구현된다**.

* 우리의 새로운 버전의```class MultiplicationTable```는 다음과 같다:

##### Snippet-7: 코드 재사용 확장 (Contd.)

**_MultiplicationTable.java_**

```java

	package com.in28minutes.firstjavaproject;

	public class MultiplicationTable {
		public static void print() {
			print(5, 1, 10);
		}

		public static void print(int number) {
			print(number, 1, 10);
		}

		public static void print(int number, int from, int to) {
			for(int i=from; i<=to;i++) {
				System.out.printf("%d X %d = %d", number, i, number*i).println();
			}	
		}
	}

```

* ```class MutliplicationRunner``` 의 논리는 전혀 변하지 않는다:

**_MultiplicationRunner.java:_**

```java

	package com.in28minutes.firstjavaproject;
	
	public class MultiplicationRunner {
		public static void main(String[] args) {
			MultiplicationTable table = new MultiplicationTable();
			table.print();
			table.print(8);
			table.print(6, 11, 20);
		}
	}

```

**_콘솔창 출력_**

_5 * 1 = 5_

_5 * 2 = 10_

_5 * 3 = 15_

_5 * 4 = 20_

_5 * 5 = 25_

_5 * 6 = 30_

_5 * 7 = 35_

_5 * 8 = 40_

_5 * 9 = 45_

_5 * 10 = 50_

_8 * 1 = 8_

_8 * 2 = 16_

_8 * 3 = 24_

_8 * 4 = 32_

_8 * 5 = 40_

_8 * 6 = 48_

_8 * 7 = 56_

_8 * 8 = 64_

_8 * 9 = 72_

_8 * 10 = 80_

_6 * 11 = 66_

_6 * 12 = 72_

_6 * 13 = 78_

_6 * 14 = 84_

_6 * 15 = 90_

_6 * 16 = 96_

_6 * 17 = 102_

_6 * 18 = 108_

_6 * 19 = 114_

_6 * 20 = 120_

##### Snippet-7 설명

깔끔하지? 우리 프로그램 학교 아이들을 친근하게 만들려면 코드에서 한 글자만 바꾸면 돼, 아래를 살짝 들여다보자.

##### Snippet-8 : 코드 재사용 확장 (Contd.)

**_MultiplicationTable.java:_**

```java

	package com.in28minutes.firstjavaproject;

	public class MultiplicationTable {
		public static void print() {
			print(5, 1, 10);		
		}

		public static void print(int number) {
			print(number, 1, 10);
		}

		public static void print(int number, int from, int to) {
			for(int i=from; i<=to;i++) {
				System.out.printf("%d X %d = %d", number, i, number*i).println();
			}
		}
	}

```

**_콘솔창 출력_**

_5 X 1 = 5_

_5 X 2 = 10_

_5 X 3 = 15_

_5 X 4 = 20_

_5 X 5 = 25_

_5 X 6 = 30_

_5 X 7 = 35_

_5 X 8 = 40_

_5 X 9 = 45_

_5 X 10 = 50_

_8 X 1 = 8_

_8 X 2 = 16_

_8 X 3 = 24_

_8 X 4 = 32_

_8 X 5 = 40_

_8 X 6 = 48_

_8 X 7 = 56_

_8 X 8 = 64_

_8 X 9 = 72_

_8 X 10 = 80_

_6 X 11 = 66_

_6 X 12 = 72_

_6 X 13 = 78_

_6 X 14 = 84_

_6 X 15 = 90_

_6 X 16 = 96_

_6 X 17 = 102_

_6 X 18 = 108_

_6 X 19 = 114_

_6 X 20 = 120_

##### Snippet-8 설명

소프트웨어 개발은 반복적인 과정이다. 우리가 쓰고 싶은 최고의 코드는 단번에 만들어지지 않는다. 그것은 일정 수준에서 시작되며, 항상 개선될 수 있다. 더 중요한 것은 이러한 개선사항을 기억해야 하며, 동일한 프로그램의 서로 다른 지점에서 그리고 프로그램 간에 다시 적용되어야 한다. 이 과정을 **코드 리팩토링**이라고 한다. 계속해서 살펴보자.

#### 요약

이번 단계에서는

* *PMT-Challenge*의 코드를 ```클래스```로 재편하는 방법에 대해 알아보았다.
* 오버로딩이 ```클래스``` 메소드와 동일한 메소드로 작용한다는 것을 이해했다.
* 오버로딩된 버전의 ```클래스```메소드에서 코드 재사용이 가능하다는 점에 주목했다.

## 객체 지향 프로그래밍 (OOP)

훌륭한 객체 지향 프로그램은 어떻게 설계할까?

알아보자.

권장 비디오:
- Object Oriented Progamming - Part 1 - https://www.youtube.com/watch?v=NOD802rMMCw
- Object Oriented Progamming - Part 2 - https://www.youtube.com/watch?v=i6EztA-F8UI

### Step 01: 객체 지향 프로그래밍 (OOP) - 기본 용어

객체 지향 프로그래밍에 대해 알아보기 전에 몇 가지 예를 들어보자.

인간은 점진적인 과정을 생각한다.

내가 런던에서 뉴욕으로 가는 비행기를 타야 한다고 가정해 보자. 내 생각은 이렇다.

- 런던 공항으로 가는 택시 타기
- 체크인
- 보안 검색대 통과
- 비행기 탑승
- 승무원 만남
- 이륙
- 비행
- 착륙
- 비행기에서 내리기
- 택시를 타고 ..

절차적 프로그래밍은 이러한 사고 과정을 반영하는 것에 불과하다. 위의 프로세스에 대한 절차적 프로그램은 다음과 같이 보일 것이다.

```java
takeACabToLondonAirport();
checkIn();
passSecurity();
boardPlane();
wishHostess();
takeOff();
cruiseMode();
land();
getOffPlane();
//...
```

객체 지향 프로그래밍(OOP)은 이것을 중심으로 새로운 사고 과정을 가져온다.

다른 배우들의 관점에서 생각해보는 건 어때? 각 배우와 관련된 데이터를 바로 옆에 저장하는 것은 어떨까? 그들에게 책임을 주고 그들 자신의 행동을 하게 하는 것은 어떨까?

서로 다른 배우의 관점에서 생각하고 데이터와 책임을 줄 때 우리의 프로그램이 어떤 모습일지 소개한다.

```java

    Person
    	name
    	boardFlight(Plane flight), wishHostess (Hostess hostess), getOffFlight(Plane flight)

    AirPlane
    	altitude, pilot, speed, flightMode
		takeOff(), cruiseMode(), land()

    Hostess
    	welcome()
```

구현 세부 정보에 대해 걱정하지 마십시오. 접근 방식의 차이에 초점을 맞추십시오.

이러한 독립체들에 **캡슐화된** 데이터와 메소드를 가지고 있으며, 이제 이것을 **객체**라고 부른다. 우리는 객체의 경계와 그것이 할 수 있는 것(그리고 할 수 없는 것)을 정의했다.

하나의 객체는
* **상태** : 데이터
* **행동** : 연산
을 가지고 있다.

```Airplane```의 ```position```은 시간이 지나면서 바뀔 수 있다. ```Airplane```에서 할 수 있는 연산으로는 ```takeOff()```,```land()```,그리고 ```cruiseMode()```를 포함한다.
이러한 행동 하나하나가 ```position```을 바꿀 수 있다. 그러므로, 어떤 객체의 행동은 그 객체의 상태에 영향을 미친다.

이제 향후 논의를 더 쉽게 할 수 있는 핵심적인 **OOP** 용어들을 소개할 때 입니다.

#### OOP 용어

몇 절 전에 썼던 ```Planet```예제를 강화시켜보자. 이번에는 개념도 같이 살펴보자.

**_Planet_**

```java

	class Planet
		name, location, distanceFromSun // data / state / fields
		rotate(), revolve() // actions / behavior / methods

	earth : new Planet
	venus : new Planet

```

몇 가지 **OOP** 용어 예시가 있다.

* **class** 는 하나의 템플릿이다. **object**는 클래스의 인스턴스이다. 위의 예제에서, `Planet`은 클래스이고 `earth`와 `venus` 는 객체이다.
* ```name```, ```location``` 과```distanceFromSun```는 객체의 상태를 구성한다.
* ```rotate()```와 ```revolve()``` 객체의 행동을 정의한다.

**필드**는 객체 상태를 구성하는 요소들이다. 객체 동작은 **메소드**를 통해 구현된다.

각 planet이 가진 상태는 다음과 같다:
* ```name```: "Earth", "Venus"
* ```location``` : 각자 자기 궤도를 가짐
* ```distanceFromSun``` : sun으로부터 서로 다른 유일무이한 거리상에 있음.

각각은 고유한 행동을 가지고 있다
* ```rotate()``` : 그들은 다른 속도로 회전한다 (사실, 다른 방향!)
* ```revolve()``` : 그들은 다른 궤도로, 다른 속도로 태양 주위를 돈다.

#### 요약

이번 단계에서는

* OOP가 절차적 프로그래밍과 어떻게 다른지 이해했다.
* 몇 가지 기본적인 OOP 용어에 대해 알아보았다.

### Step 02: 프로그래밍 실습 PE-01

#### 실습

다음 각 시스템에서 관련된 기본 실체를 식별하고 객체 지향 용어를 사용하여 구성한다.

1. Online Shopping System
2. Person

#### Solution-1: Online Shopping System
	
```java

	Customer
		name, address
		login(), logout(), selectProduct(Product)

```

```java

	ShoppingCart
		items
		addItem(), removeItem()

```

```java

	Product
		name, price, quantityAvailable
		order(), changePrice()

```

#### Solution-2: Person

```java

	Person
		name, address, hobbies, work
		walk(), run(), sleep(), eat(), drink()

```

### Step 03: ```MotorBike``` ```class``` 생성

이 일련의 예에서 우리는 당신의 운송수단인 오토바이를 모형화하고자 한다. 우리는 오토바이 객체를 만들어 가지고 놀고 싶다.
자바 파일 두 개로 시작하겠다: 
* **_MotorBike.java_**, ```MotorBike``` ```class``` 정의를 포함하고 있다. 이 ```class``` 가 우리 오토바이의 상태와 행동을 캡슐화할 것이다. 
* **_MotorBikeRunner.java_**, ```class MotorBikeRunner```에서 프로그램의 시작점인 ```main``` 메소드를 포함하고 있음.

##### Snippet-1: MotorBike Class

**_MotorBike.java_**

```java

	package com.in28minutes.oops;
		public class MotorBike {
		//behavior
		void start() {
			System.out.println("Bike started!");
		}
}

```

**_MotorBikeRunner.java_**

```java

	package com.in28minutes.oops;

	public class MotorBikeRunner {
		public static void main(String[] args) {
			MotorBike ducati = new MotorBike();
			MotorBike honda = new MotorBike();
			ducati.start();
			honda.start();
		}
	}

```

**_콘솔창 출력_**

_Bike started!_

_Bike started!_

##### Snippet-1 설명

우리는 `start`메소드로 간단한 `MotorBike` 클래스를 만들기 시작했다. 우리는 몇 가지 객체를  만들어 그들에게 `start`메소드를 부여했다.

우리는 `Separation of Concern`을 위해 두 클래스를 만들었다:
- `MotorBike`클래스는 그의 모든 데이터와 행동을 책임진다.
- `MotorBikeRunner`클래스는 오토바이 예제들의 실행을 담당한다.

#### 요약

이번 단계에서는

* 다음 단계에서 *OOP* 개념을 추가 탐색할 수 있도록 ```MotorBike``` ```class```를 정의했다.

### Step 04:  프로그래밍 실습 OO-PE-02

#### 실습

1. 작은 자바 프로그램을 작성하여 ```Book``` ```class```를 만든 후, 책 제목을 대표할 객체들을 다음과 같이 만드시오:
	* "The Art Of Computer Programming"
	* "Effective Java"
	* "Clean Code"

#### 솔루션

**_Book.java_**

```java

	public class Book {
		private String title;

		public void setTitle(String bookTitle) {
			title = bookTitle;
		}

		public String getTitle() {
			return title;
		}
	}

```

**_BookRunner.java_**

```java

	public class BookRunner {
		public static void main(String[] args) {
			Book taocp = new Book();
			taocp.setTitle("The Art Of Computer Programming");
			Book ej = new Book();
			ej.setTitle("Effective Java");
			Book cc = new Book();
			cc.setTitle("Clean Code");
			System.out.println(taocp.getTitle());
			System.out.println(ej.getTitle());
			System.out.println(cc.getTitle());
		}
	}

```

**_콘솔창 출력_**

_The Art Of Computer Programming_

_Effective Java_
	
_Clean Code_

### Step 05: ```MotorBike``` -  상태 표시

An object encapsulates both *state* and *behavior*. 
하나의 객체는 *상태*와 *행동*이 둘 다 캡슐화되어 있다.

*상태*는 "특정 시간에 객체의 상태"를 정의하고, *행동*은 **멤버 변수**로 표시된다.

```MotorBike```의 예시에서, 각 ```MotorBike```에 대해 ```speed```속성이 필요하다면, 여기 포함시켜보자.

##### Snippet-1 : 상태 변수 speed를 포함한 MotorBike

**_MotorBike.java_**

```java

	package com.in28minutes.oops;

	public class MotorBike {
		int speed;
		void start() {
			System.out.println("Bike started!");
		}
	}
	

```

**_MotorBikeRunner.java_**

```java

	package com.in28minutes.oops;

	public class MotorBikeRunner {
		public static void main(String[] args) {
			MotorBike ducati = new MotorBike();
			MotorBike honda = new MotorBike();
			ducati.start();
			honda.start();

			ducati.speed = 100;
			honda.speed = 80;
			ducati.speed = 20;
			honda.speed = 0;
		}
	}

```

**_콘솔창 출력_**

_Bike started!_

_Bike started!_

##### Snippet-4 설명

```MotorBike```내의 ```int speed;```는 멤버 변수를 정의한다.

```ducati```와 ```honda```와 같이 객체 내의 이름으로 접근할 수도 있다.

```
ducati.speed = 100;
honda.speed = 80;

```

```ducati``` 는```speed```라는 고유한 값을 가지고 있고, ```honda```도 마찬가지이다. 이 값들은 각각 독립적이다. 하나를 변경한다고 나머지 다른 하나에 영향을 주지 않는다.

#### Classroom Exercise CE-OO-01

1. 이전에 만든 ```Book``` ```Class```를 업데이트하여 ```noOfCopies```라는 멤버 변수를 포함시키고, 앞에서 지정한 세 개의 제목에 대해 어떻게 독립적으로 설정 및 업데이트할 수 있는지 보이시오.

#### 솔루션

TODO

### Step 07: ```MotorBike``` - get() , set() 메소드

이전 단계에서, 우리는 즐겁게 ```ducati```와 ```honda```객체 내에 있는 ```speed```속성과 ```main()```프로그램 내에서 직접 수정하고 있었다.

```java
	public class MotorBikeRunner {
		public static void main(String[] args) {
			//... Other code
			ducati.speed = 100;
			honda.speed = 0;
		}
	}
```

이것은 잘 작동했지만, **OOP** 캡슐화의 기본 원리를 깨트린다.

*"한 객체의 메소드는 다른 객체의 상태에 직접 접근하도록 허용해서는 안 된다. 그렇게 하는 것은 오직 대상 객체에서만 메소드를 호출할 수 있도록 허용되어야 한다"

즉, 멤버 변수는 ```class```의 외부에 선언된 메소드에는 직접 접근할 수 없어야 한다.

##### Snippet-3 : private 속성을 가진 MotorBike

**_MotorBike.java_**

```java

	package com.in28minutes.oops;
	
	public class MotorBike {
		private int speed;
		
		void start() {
			System.out.println("Bike started!");
		}

		void setSpeed(int speed) {
			this.speed = speed;
		}
	}

```

**_MotorBikeRunner.java_**

```java

	package com.in28minutes.oops;

	public class MotorBikeRunner {
		public static void main(String[] args) {
			MotorBike ducati = new MotorBike();
			MotorBike honda = new MotorBike();
			ducati.start();
			honda.start();
		
			ducati.setSpeed(100);
			honda.setSpeed(80);
	
			ducati.setSpeed(20);
			honda.setSpeed(0);
		}
	}

```

**_콘솔창 출력_**

_Bike started!_

_Bike started!_

##### Snippet-3 설명

```speed```를 ```private```으로 선언하여, ```MotorBike```에 **접근 제어**라는 것을 제공하고 있다. Java keywords such as ```public``` and ```private``` 와 같은 자바 키워드는**접근 지정자**라고 불린다. 이들은 외부의 객체가 대상이 되는 객체에 접근하는 것을 통제한다.

```setSpeed()```메소드 내의  ```this.speed = speed;``` 를 보자:
* 멤버 변수는 항상 특정한 ```class```의 인스턴스에 속한다.
* 메소드의 인수는 해당 메소드 내의 지역 변수처럼 동작한다.
* 이 둘을 구분하기 위해, ```this```를 사용한다.```this.speed```라는 표현은 ```MotorBike```객체의 ```speed```라는 멤버 변수를 가리킨다. 바로 이를 위해 ```setSpeed()```가 호출된다.

일찍이 ```MotorBikeRunner```에 쓰여진 ```ducati.speed = 100;````이라는 표현은 이제 오류를 발생시킬 것이다! ```speed```에 접근하고 이를 수정하는 올바른 방법은 ```MotorBike```객체에 ```setSpeed()```와 같은 적절한 메소드를 동원하는 것이다.

#### Classroom Exercise CE-OO-02

1. ```class``` ```Book``` 이 더 이상 캡슐화 원칙을 어기지 않도록 업데이트한다.

#### 솔루션

TODO

#### 요약

이번 단계에서는:
* 캡슐화를 구현하기 위해 접근 제어의 필요성에 대해 알아보았다.
* Java가 이러한 통제를 위해 접근 지정자(```public```,```private```같은)를 제공하는 것을 관찰했다.
* 객체의 데이터에 접근하기 위한 ```get()```과 ```set()```메소드의 필요성에 대해 이해했다.

- - - 
### Step 08: 객체 상태에 접근
 
캡슐화는 다른 객체의 직접적인 접근으로부터 객체의 상태를 보호하기 위해 필요하다. 우리는 ```speed```를 ```private```으로 선언하여 ```MotorBike```의 객체를 보호할 수 있었다. ```private```의 ```speed```선언으로, *get*조차 접근하지 못하게 된 경직된 상황이 되었다. 이 문제를 어떻게 해결해야 할까? 이번에도 답은 ```speed```를 읽을 수 있는 메소드를 제공하는 것에 있다.

##### Snippet-4 : ```MotorBike```의  ```getSpeed()```

**_MotorBike.java_**

```java

	package com.in28minutes.oops;

	public class MotorBike {
		//Same as before

		int getSpeed() {
			return this.speed;
		}
	}

```

**_MotorBikeRunner.java_**

```java

	package com.in28minutes.oops;

	public class MotorBikeRunner {
		public static void main(String[] args) {
			MotorBike ducati = new MotorBike();
			MotorBike honda = new MotorBike();
			ducati.start();
			honda.start();

			ducati.setSpeed(100);
			honda.setSpeed(80);
			System.out.printf("Current Ducati Speed is : %d", ducati.getSpeed()).println();
			System.out.printf("Current Honda Speed is : %d", honda.getSpeed()).println();
		}
	}

```

**_콘솔창 출력_**

_Bike started!_

_Bike started!_

_Current Ducati Speed is : 100_

_Current Honda Speed is : 80_

##### Snippet-4 설명

```getSpeed()```와 같은 메소드를 정의하여 하나의 ```MotorBike``` 객체의 ```speed```에 접근하는 것을 허용한다.

```
		int getSpeed() {
			return this.speed;
		}
```



> 이클립스는 매우 편리한 기능을 가지고 있다. 클래스의 상태 요소(멤버 변수)가 정의되면 각 클래스에 대해 기본 get(), set()메솓를 생성하고 설정할 수 있다. 시간 절약과 타이핑 노력을 줄이기 위해 정기적으로 이것을 사용하고 싶을 것이다.`class 우클릭 > Generate Source > Generate Getters and Setters`

#### 요약

이번 단계에서는:

* 접근 제어가 어떻게 우리에게 ```get()```메소드를 제공하도록 하는지 이해했다.
* 각 ```class```속성에 대한 ```get()```과 ```set()```버전을 만들기 위한 몇 가지 Eclipse 팁을 살펴보았다.

### Step 10: 기본 객체 내 상태

객체 내부의 데이터 요소가 값으로 초기화되지 않으면 어떤 일이 일어나는가?

##### Snippet-5 : 객체 내 상태의 기본 초기화

**_MotorBike.java_**

```java
//Same as before
```

**_MotorBikeRunner.java_**

```java

	package com.in28minutes.oops;

	public class MotorBikeRunner {
		public static void main(String[] args) {
			MotorBike honda = new MotorBike();			
			System.out.printf("Current Honda Speed is : %d", honda.getSpeed()).println();
		}
	}

```

**_콘솔창 출력_**

**_Current Honda Speed is : 0_**

##### Snippet-6 설명

우리가 객체를 인스턴스화할 때, 객체의 모든 상태 요소는 항상 그 타입의 기본값으로 초기화된다. ```MotorBike```내부에서는 ```speed```가 ```int```로 선언되어 ```0```으로 초기화된다. 이는 심지어 ```start()```를 비롯한 ```MotorBike```의 어떤 메소드도 호출하기도 전에 일어난다.

우리가 명시적으로 초기화하지 않았는데도 `honda.getspeed()`가 0으로 출력된 것을 볼 수 있다.


#### 요약

이번 단계에서는
* 객체의 멤버 변수에는 기본 값이 할당된 다는 것을 배웠다.

### Step 10: 캡슐화: 이점

캡슐화의 중심에는 객체의 상태를 보호할 필요가 있다. 누구한테서? 다른 객체로부터.

캡슐화를 더 잘 이해하기 위한 예를 보자.

##### Snippet-7 : 캡슐화의 이점

**_MotorBike.java_**

```java

	package com.in28minutes.oops;

	public class MotorBike {
		private int speed;

		public void start() {
			System.out.println("Bike started!");
		}

		public void setSpeed(int speed) {
			this.speed = speed;
		}

		public int getSpeed() {
			return this.speed;
		}
	}

```

**_MotorBikeRunner.java_**

```java

	package com.in28minutes.oops;

	public class MotorBikeRunner {

		public static void main(String[] args) {
			MotorBike ducati = new MotorBike();
			ducati.start();
			ducati.setSpeed(-100);
			System.out.printf("Current Ducati Speed is : %d", ducati.getSpeed()).println();
		}
	}

```

**_콘솔창 출력_**

_Bike started!_

**_Current Ducati Speed is : -100_**

##### Snippet-01 Explained

오토바이에 ```-100```은 잘못된 속도일 수 있다. 현재 우리는 어떠한 검증도 받지 않았다. ```setSpeed```라는 메소드를 갖게 되면 우리는 타당성 검증을 추가할 있게된다.
Let's see how to do that.
어떻게 하는지 보자.

##### Snippet-02 : 속도의 타당성 검사

**_MotorBike.java_**

```java

	package com.in28minutes.oops;

	public class MotorBike {

		//Other code as is

		public void setSpeed(int speed) {
			if(speed > 0)
				this.speed = speed;
		}

	}

```

**_MotorBikeRunner.java_**

```java
//Same as before
```

snippet의 출력은 다음과 같다:

_Bike started!_

**_Current Ducati Speed is : 0_**

##### Snippet-8 설명

```setSpeed()```는 if(speed > 0)을 체크하고 음의 값으로 속도를 업데이트하지 않는다.

> `setSpeed`메소드의 호출자가 성공했다고 가정하기 떄문에 완벽한 해결책은 아니다. 이상적으로 검증 오류를 나타내는 예외를 적용해야 한다. 예외에 대해서는 나중에 이야기하겠다.
> This is not perfect solution because the caller of the `setSpeed` method assumes that he was successful. Ideally, we should throw an Exception indicating validation error. We will talk about Exceptions later.


#### 요약

이번 단계에서는
* 캡슐화의 첫 번째 이점에 대해 알아보았다. - 데이터 검증을 추가하기 위한 공급
* ```MotorBike``` 예제를 사용하여 그러한 검증이 어떻게 이루어질 수 있는지 강조하였다.


### Step 11: 캡슐화 - 이점 (코드 재사용)

우리는 *OOP*의 캡슐화에 대해 꽤 많은 것을 이해했다.

```100 mph```이라고 말하는 혼다와 두카티 오토바이의 속도를 모두 일정한 양만큼 높이고 싶다고 가정해보자. 논리는 간단하겠지? 각 오토바이의 현행 ```speed```를 ```100```만큼 끌어올린 다음 새로운 값을 그 오토바이의 ```speed```로 다시 설정한다. 다음의 예는 이 논리를 실행에 옮긴다.


##### Snippet-1 : Bulky Speed Increment code 

**_MotorBike.java_**

```java
// No Change
```

**_MotorBikeRunner.java_**

```java

	package com.in28minutes.oops;

	public class MotorBikeRunner {
		public static void main(String[] args) {
			MotorBike ducati = new MotorBike();
			MotorBike honda = new MotorBike();
			ducati.start();		
			honda.start();
			ducati.setSpeed(100);
			
			System.out.printf("Earlier Ducati Speed is : %d", ducati.getSpeed()).println();
			System.out.printf("Earlier Honda Speed is : %d", honda.getSpeed()).println();
		
			int ducatiSpeed = ducati.getSpeed();
			ducatiSpeed = ducatiSpeed + 100;
			ducati.setSpeed(ducatiSpeed);
			
			int hondaSpeed = honda.getSpeed();
			hondaSpeed = hondaSpeed + 100;
			honda.setSpeed(hondaSpeed);
			
			System.out.printf("Later Ducati Speed is : %d", ducati.getSpeed()).println();
			System.out.printf("Later Honda Speed is : %d", honda.getSpeed()).println();
		}
	}

```

The output of this snippet is:

_Bike started!_

_Bike started!_

_Earlier Ducati Speed is : 100_

_Earlier Honda Speed is : 0_

**_Later Ducati Speed is : 200_**

**_Later Honda Speed is : 100_**

##### Snippet-1 설명

```MotorBikeRunner```의 반복된 코드를 주목해보겠는가? ```ducati```의 ```speed```를 갱신하는 코드는 ```honda```의 코드와 거의 같다. 이 책의 첫머리에서 우리는 다음과 같은 말을 한 것을 기억하라:

*"모든 컴퓨터 프로그램의 목표는 프로그래머를 위해 작업을 더 쉽고, 덜 번거롭고, 더 우아하게 만드는 것이다."*

*OOP*는 캡슐화를 통해 모든 것을 달성한다! 그 아이디어는 메소드 내에서 반복된 논리를 *캡슐화*하고, 그것에 객체별 정보를 인수로 전달하는 것이다. 다음 예는 그것을 하는 한 가지 방법을 보여준다.


##### Snippet-2 : 코드 캡슐화를 통한 속도 증가


**_MotorBike.java_**

```java

	package com.in28minutes.oops;

	public class MotorBike {
		//Other code same as before
		public void increaseSpeed(int howMuch) {
			this.speed = this.speed + howMuch;
		}
	}

```

**_MotorBikeRunner.java_**

```java

	package com.in28minutes.oops;

	public class MotorBikeRunner {
		public static void main(String[] args) {
			
			MotorBike duati = new MotorBike();
			MotorBike honda = new MotorBike();
			ducati.start();
			honda.start();

			ducati.setSpeed(100);

			System.out.printf("Earlier Ducati Speed is : %d", ducati.getSpeed()).println();
			System.out.printf("Earlier Honda Speed is : %d", honda.getSpeed()).println();

			ducati.increaseSpeed(100);
			honda.increaseSpeed(100);

			System.out.printf("Later Ducati Speed is : %d", ducati.getSpeed()).println();
			System.out.printf("Later Honda Speed is : %d", honda.getSpeed()).println();
		}
	}

```

The output of this snippet is:

_Bike started!_

_Bike started!_

_Earlier Ducati Speed is : 100_

_Earlier Honda Speed is : 0_

**_Later Ducati Speed is : 200_**

**_Later Honda Speed is : 100_**

##### Snippet-2 설명

```MotorBike```에 ```increaseSpeed()```메소드가 추가되었다. 그것은 ```ducati```와 ```honda```에서 호출될 수 있다.

이제 ```MotorBike```의 속도를 줄일 수 있는 부분을 추가해보자.

##### Snippet-3 : 코드 캡슐화를 통한 속도 증가 및 감소

**_MotorBike.java_**

```java

	package com.in28minutes.oops;

	public class MotorBike {
		// Other methods same as before
		public void decreaseSpeed(int howMuch) {
			this.speed = this.speed - howMuch;
		}
	}

```

**_MotorBikeRunner.java_**

```java

	package com.in28minutes.oops;

	public class MotorBikeRunner {
		public static void main(String[] args) {
			MotorBike ducati = new MotorBike();
			MotorBike honda = new MotorBike();
			ducati.start();
			honda.start();
	
			ducati.setSpeed(100);
			System.out.printf("Earlier Ducati Speed is : %d", ducati.getSpeed()).println();
			System.out.printf("Earlier Honda Speed is : %d", honda.getSpeed()).println();

			ducati.increaseSpeed(100);
			honda.increaseSpeed(100);
			ducati.decreaseSpeed(50);
			honda.decreaseSpeed(50);

			System.out.printf("Later Ducati Speed is : %d", ducati.getSpeed()).println();
			System.out.printf("Later Honda Speed is : %d", honda.getSpeed()).println();
			
			ducati.decreaseSpeed(200);
			honda.decreaseSpeed(200);

			System.out.printf("Final Ducati Speed is : %d", ducati.getSpeed()).println();
			System.out.printf("Final Honda Speed is : %d", honda.getSpeed()).println();
		}
	}

```

The output of this snippet is:

_Bike started!_

_Bike started!_

_Earlier Ducati Speed is : 100_

_Earlier Honda Speed is : 0_

**_Later Ducati Speed is : 150_**

**_Later Honda Speed is : 50_**

**_Final Ducati Speed is : -50_**

**_Final Honda Speed is : -150_**

##### Snippet-3 설명

```MotorBike```에 ```decreaseSpeed()```메소드가 추가되었다. 그것은 ```MotorBike```의 ```main()```메소드 안에 있는 ```ducati```와 ```honda``` 객체에서 호출될 수 있다.

여러분이 다시 관찰할 수 있는 것 중 하나는 *** 음수 속도 값**이다. 우리의 검증은 개선되어야 한다.

##### Snippet-4 : 여러 메소드에 걸친 검증, 반복!


**_MotorBike.java_**

```java

	package com.in28minutes.oops;

	public class MotorBike {

		//Same as before

		public void increaseSpeed(int howMuch) {
			if(this.speed + howMuch > 0)
			   this.speed = this.speed + howMuch;
		}

		public void decreaseSpeed(int howMuch) {
			if(this.speed - howMuch > 0)
			   this.speed = this.speed - howMuch;
		}
	}

```

**_MotorBikeRunner.java_**

```java
	//Same as before
```

The output of this snippet is:

_Bike started!_

_Bike started!_

_Earlier Ducati Speed is : 100_

_Earlier Honda Speed is : 0_

_Later Ducati Speed is : 150_

_Later Honda Speed is : 50_

**_Final Ducati Speed is : 150_**

**_Final Honda Speed is : 50_**

##### Snippet-4 설명

우리는 ```ducati```와 ```honda```의 ```speed```를 ```0```이하로 낮추려는 시도가 지금은 무시되고 있기 때문에 유효성 검증에 성공했다.

그러나 이것은 *코드 비대화*라는 대가를 치렀다.

코드의 중복을 어떻게 줄일 것인가?

##### Snippet-5: 코드 재사용을 통한 유효성 검증

**_MotorBike.java_**

```java

	package com.in28minutes.oops;

	public class MotorBike {
		//Other methods same as before


		public void setSpeed(int speed) {
			if(speed > 0)
				this.speed = speed;
		}

		public void increaseSpeed(int howMuch) {
			setSpeed(this.speed + howMuch);
		}

		public void decreaseSpeed(int howMuch) {
			setSpeed(this.speed - howMuch);
		}
	}

```

**_MotorBikeRunner.java_**

```java
	//Same as before

```

The output of this snippet is:

_Bike started!_

_Bike started!_

_Earlier Ducati Speed is : 100_

_Earlier Honda Speed is : 0_

_Later Ducati Speed is : 150_

_Later Honda Speed is : 50_

**_Final Ducati Speed is : 150_**

**_Final Honda Speed is : 50_**

##### Snippet-5 설명

이 해결책의 이면에 있는 생각은 *업데이트*가 ```set()```의 연산과 같다는 것이다. ```setSpeed()```는 이미 유효성을 검사했기 때문에 ```increaseSpeed()```와 ```decreaseSpeed()``` 둘 다 적절한 매개변수를 가지고 내부에서 호출할 수 있다.

이러한 방식으로 거증 논리는 메소드를 업데이트하는 방법으로 재사용될 것이다.

> 항상 조심하라. 논리의 중복은 여러분의 코드를 유지하기 어렵게 만든다.


#### 요약

이번 단계에서는

* 캡슐화의 두 번째 이점인 코드 재사용을 살펴보기 시작했다.
* 이러한 이해를 ```MotorBike```의 사례에 연관지어 유효성 검증에 대해 알아보았다.

### Step 12: 프로그래밍 실습 PE-OO-03

#### 실습

1. 캡슐화 기법을 사용하여 ```Book``` ```class```를 위한 메소드를 작성하시오.
	* 도서의 수 증가
	* 도서의 수 감소

#### 솔루션

**_BookRunner.java_**

```java

	public class BookRunner {
		public static void main(String[] args) {
			Book taocp = new Book();
			taocp.setTitle("The Art Of Computer Programming");
			Book ej = new Book();
			ej.setTitle("Effective Java");
			Book cc = new Book();
			cc.setTitle("Clean Code");
			
			System.out.println(taocp.getTitle());
			System.out.println(ej.getTitle());
			System.out.println(cc.getTitle());

			taocp.increaseCopies(10);
			ej.increaseCopies(15);
			cc.increaseCopies(20);
			taocp.decreaseCopies(5);
			ej.decreaseCopies(10);
			cc.decreaseCopies(15);

			System.out.println(taocp.getNumberOfCopies());
			System.out.println(ej.getNumberOfCopies());
			System.out.println(cc.getNumberOfCopies());
		}
	}

```

**_Book.java_**

```java

	public class Book {
		private String title;
		private int numberOfCopies;

		public void setTitle(String bookTitle) {
			title = bookTitle;
		}

		public String getTitle() {
			return title;
		}

		public void setNumberOfCopies(int numberOfCopies) {	
			if(numberOfCopies > 0) {
				this.numberOfCopies = numberOfCopies;
			}
		}

		public int getNumberOfCopies() {
			return numberOfCopies;
		}

		public void increaseCopies(int howMuch) {
			setNumberOfCopies(numberOfCopies + howMuch);
		}

		public void decreaseCopies(int howMuch) {
			setNumberOfCopies(numberOfCopies - howMuch);
		}
	}

```

**_콘솔창 출력_**

_The Art Of Computer Programming_

_Effective Java_
	
_Clean Code_

_5_

_5_

_5_

### Step 13: 생성자 소개

우리가 두카티와 혼다 모터바이크를 만들 때, 우리는 그들을 약간의 시작 속도가 있는 것으로 구성하기를 원할지도 모른다.

우리의 변덕이 두카티 오토바이는 100mph로 시작하고 혼다는 200mph로 출발한다고 가정해보자.


##### Snippet-1: MotorBike 생성자

**_MotorBike.java_**

```java

	package com.in28minutes.oops;

	public class MotorBike {
		private int speed;

		
		MotorBike(int speed) {
			if(speed > 0)
				this.speed = speed;
		}

		//Same as before

	}

```

**_MotorBikeRunner.java_**

```java

	package com.in28minutes.oops;

	public class MotorBikeRunner {
		public static void main(String[] args) {
			MotorBike ducati = new MotorBike(100);
			MotorBike honda = new MotorBike(200);
			ducati.start();
			honda.start();
			System.out.printf("Earlier Ducati Speed is : %d", ducati.getSpeed()).println();
			System.out.printf("Earlier Honda Speed is : %d", honda.getSpeed()).println();
		}
	}

```

The output of this snippet is:

_Bike started!_

_Bike started!_

_Earlier Ducati Speed is : 100_

_Earlier Honda Speed is : 200_

##### Snippet-1 설명

우리는 ```MotorBike```에 인자가 하나인 생성자를 정의했는데, 그 정의는 다음과 같다.

```public MotorBike(int speed){ /* 생성자 코드는 여기에 작성  */ }```

생성자는 ```class```와 이름이 같은 메소드이다. 메소드에 대한 모든 Java 규칙은 생성자에게도 적용된다. 생성자를 직접 호출할 수는 없다.

생성자는 ```새로운```키워드를 사용하여 ```class```객체가 생성될 때, 항상 호출된다. ```class```를 위한 생성자는 0개 혹은 하나 이상의 인자를 받아들일 수 있다. 다음에는 ```MotorBike```생성자를 위한 완전한 코드를 써보자.


#### 요약

이번 단계에서는, ```class```생성자라는 개념을 알게 되었다.

### Programming Exercise PE-OO-04, 생성자 더 알아보기

#### 실습

1. ```Book``` ```class```의 솔루션을 생성자를 사용하여 재작성 하십시오. 이 생성자는 최초 발행 부스를 명시하는 정수 인수를 받는다:
	* "The Art Of Computer Programming" : 100부
	* "Effective Java" : 75부
	* "Clean Code" : 60부

####  PE-OO-04 솔루션

**_BookRunner.java_**

```java

	public class BookRunner {
		public static void main(String[] args) {
			Book taocp = new Book(100);
			taocp.setTitle("The Art Of Computer Programming");
			
			Book ej = new Book(75);
			ej.setTitle("Effective Java");
			
			Book cc = new Book(60);
			cc.setTitle("Clean Code");

			System.out.println(taocp.getTitle());
			System.out.println(taocp.getNumberOfCopies());

			System.out.println(ej.getTitle());`
			System.out.println(ej.getNumberOfCopies());

			System.out.println(cc.getTitle());
			System.out.println(cc.getNumberOfCopies());
		}
	}

```

**_Book.java_**

```java

	public class Book {
		private String title;
		private int numberOfCopies;
		
		public Book(int numberOfCopies) {
			this.numberOfCopies = numberOfCopies;
		}

		public void setTitle(String bookTitle) {
			title = bookTitle;
		}

		public String getTitle() {
			return title;
		}

		public int getNumberOfCopies() {
			return numberOfCopies;
		}
	}

```

**_콘솔창 출력_**

_The Art Of Computer Programming_

_100_

_Effective Java_

_75_
	
_Clean Code_

_60_

#### 생성자에 대한 더 많은 정보

우리는 ```MotorBike``` ```class```를 정의하고 ```ducati```와 ```honda```라는 그 인스턴스의 행동을 확인했다.

처음 시작했을 때, 우리는 다음과 같이 ```MotorBike```의 클래스의 인스턴스를 만들었다:

```MotorBike ducati = new MotorBike();```

뭔가 낯익은 것을 눈치챘나? ```new MotorBike()```라는 수식은 생성자 호출처럼 보이지 않는가?

알고보니 ```MotorBike```에 대한 생성자 호출이다!

우리가 자바에서 ```class```(비어 있는것 처럼 보이는)를 정의하면, 이면에서는 마술이 일어난다. 그런 ```class``` ```Cart```를 생각해보자:


```java

	class Cart {

	};

```

이 ```class```는 상태도 행동도 없다. 우리가 이러한 "비어있는" ```class```의 인스턴스를 만들려고 할 때:

```java

	class CartRunner {
		public static void main(String[] args) {
			Cart cart = new Cart();
		}
	}

```

이 코드는 꽤 순조롭게 컴파일, 실행, 초기화 되는 것 같다! 결국 컴파일러가 ```Cart```를 위한 ```기본 생성자```를 조용히 만들어 낸다는 것이다.

기본 생성자는 어떤 인수도 허용하지 않는 생성자이다. 마치 ```Cart``` ```class```를 이렇게 정의한 것과 같다.


```java

	class Cart {
		public Cart() {
		}
	};

```

생성자도 오버로딩된 정의를 가질 수 있다.

이제 ```Cart```와 마찬가지로 기본 초기화로 ```MotorBike```의 인스턴스를 만들어보자.

##### Snippet-2 : MotorBike의 기본 생성자?

**_MotorBike.java_**

```java

	package com.in28minutes.oops;

	public class MotorBike {

		private int speed;

		MotorBike(int speed) {
			if(speed > 0)
				this.speed = speed;
		}
	}

```

**_MotorBikeRunner.java_**

```java

	package com.in28minutes.oops;

	public class MotorBikeRunner {
		public static void main(String[] args) {
			MotorBike ducati = new MotorBike(100);
			MotorBike honda = new MotorBike(200);
			MotorBike yamaha = new MotorBike();
		}
	}

```

**_콘솔창 출력_**

**_컴파일 에러_**

##### Snippet-2 설명

컴파일러는 **_MotorBikeRunner.java_**로 오류를 표시한다! `MotorBike yamaha = new MotorBike();` 는 컴파일에 실패했다. 왜일까?

여기서 기본 생성자가 생성되지 않았다! 클래스에 생성자 정의를 하나라도 제공하면 컴파일러는 기본 생성자를 추가하지 않는다. **다 너를 위한거야. 마음에 안들면 전부 네가 해!**라고 외치는 것이다.

기본 생성자가 필요한 경우 명시적으로 추가할 수 있다.


##### Snippet-3 : 프로그래머가 정의한 기본 생성자

**_MotorBike.java_**

```java

	package com.in28minutes.oops;

	public class MotorBike {
		//state
		private int speed;

		//behavior
		MotorBike() {
			this(5);
		}

		MotorBike(int speed) {
			if(speed > 0)
				this.speed = speed;
		}

	}

```

**_MotorBikeRunner.java_**

```java

	package com.in28minutes.oops;

	public class MotorBikeRunner {
		public static void main(String[] args) {
			MotorBike ducati = new MotorBike(100);
			MotorBike honda = new MotorBike(200);
			MotorBike yamaha = new MotorBike();
			System.out.printf("Earlier Yamaha Speed is : %d", yamaha.getSpeed()).println();
		}
	}

```

The output of this snippet is:

**_Earlier Yamaha Speed is : 5_**

##### Snippet-3 설명

인수가 없는 생성자 ```MotorBike()```를 정의하여 기본 객체 초기화가 가능하도록 했다. 그런데 ```this(5);```라는 구문으로 그 내부에서 우리가 무엇을 하고 있는 것일까?

우리는 ```MotorBike()```내에서 ```this```라는 키워드를 가진 생성자를 ```MotorBike(int)```로 호출했다.


## 기본형 타입

이에 앞서 우리는 기본적인 자바 타입(```int```,```double```,```boolean```등)을 살펴본 후 조금 익숙해졌다.

우리는 리터럴 값, 선언된 변수, 그리고 그것들을 사용하여 수식을 만들었다. 

자바 **기본형 타입** 은 다음과 같은 것들을 포함한다:
* 정수형
	* ```byte```
	* ```short```
	* ```int```
	* ```long```
* 부동 소수점형
	* ```float```
	* ```double```
* 문자형
	* ```char```
* 논리형
	* ```boolean```

이 섹션에서는 이러한 타입들을 더 자세히 파악해 봅시다.


### Step 01: 정수형

정수는 그다지 미스터리는 아니지? 이들은 학창시절부터 우리의 일부였고, 우리는 보통 다른 숫자보다 그들을 더 선호한다.(덜 무섭거든!)

자바는 그들을 쉽게 지원하고, 우리는 이미 그것들을 사용하여 꽤 많은 예시들을 코딩했다.

자바에도 각각에 해당하는 **래퍼 클래스(Wrapper class)**가 잇어 기초 버전이 더욱 다용도로 사용할 수 있다. 우리가 말하는 래퍼 클래스는 다음과 같다:

* ```Byte```: ```byte```용
* ```Short```: ```short```와 일치
* ```Integer``` ```int```에 해당
* ```Long```: ```long```과 같음

우리가 어떻게 그들을 사용할지 한 번 봅시다.

##### Snippet-01 : 정수의 크기

이 작은 클래스들이 여러분을 위해 가지고 있는 모든 정보를 보라! 그들이 말하듯이, **_"예고된 것은 미리 무장되어 있다"_** 프로그램이 다루는 데이터(범위 및 크기)에 따라 사용할 타입을 결정하고 저장할 수 있다.

```java

	jshell> Byte.SIZE
	$1 ==> 8
	jshell> Byte.BYTES
	$2 ==> 1
	jshell> Byte.MAX_VALUE
	$3 ==> 127
	jshell> Byte.MIN_VALUE
	$4 ==> -128
	jshell> Short.BYTES
	$5 ==> 2
	jshell> Integer.BYTES
	$6 ==> 4
	jshell> Long.BYTES
	$7 ==> 8
	jshell> Short.MAX_VALUE
	$8 ==> 32767
	jshell> Integer.MAX_VALUE
	$8 ==> 2147483647
	jshell> int i = 100000;
	i ==> 100000
	jshell> long l = 50000000000;
	| Error:
	| integer number too large: 50000000000
	| long l = 50000000000;
	|_________^
	jshell> long l = 50000000000l;
	l ==> 50000000000
	jshell>

```

#### 정수형 변환

우리가 큰 데이터를 작은 공간에 저장하려고 하면 문제가 발생할 것이다. 컴파일러는 오류를 플래그로 표시하여 프로그래머에게 그러한 문제에 대해 경고한다. 그러나 프로그래머가 위험을 알고 있고 이를 계속 진행하고자 한다면 **명시적 캐스트**는 코드를 밀어넣기 위한 프로그래머의 도구이다.

반대 상황(큰 공간에 작은 데이터 값을 저장)에서의 연산은 컴파일러에게는 아주 쉽다. 이러한 변환을 **묵시적 캐스트**라고 한다.

##### Snippet-02 : 정수형 변환 

```long```의 값을 ```int```변수에 저장하려고 하는 것은 우리에게 컴파일러 오류를 줄 것이다. 그러나 ```i = (int) l;''' 과 같은 명시적 캐스팅을 사용할 수 있다.

```java

	jshell> int i = 100000;
	i ==> 100000
	jshell> long l = 50000000000l;
	l ==> 50000000000
	jshell> i = l;
	| Error :
	| incompatible types: possible lossy conversion from long to int
	| i = l;
	|_____^
	jshell> i = (int) l;
	i ==> -1539607552
	jshell> l = i;
	l ==> -1539607552
	jshell>
	
```

**_컴파일러는 이 문장의 형식 안정성에 대한 책임이 없다. 그 책임은 프로그래머인 나에게 있다._**

잘못된 프로그램 동작 가능성에 대한 이전의 구문을 기억하는가? 보다시피 ```i```에 다른 값이 저장되었다.

#### 요약

이번 단계는

* 기초 정수형 타입에 대해 존재하는 래퍼 클래스를 탐색했다.
* 이러한 타입의 다양한 용량 및 데이터 범위에 대해 이해했다.
* 명시적 및 묵시적 캐스팅 사용 방법에 대해 살펴보았다.

### Step 02: 정수 표현 및 기타 문제

십진법에서 허용된 숫자는 ```0``` 부터 ```9```이다. ```10```이라는 값이 나오면 숫자가 1개씩 늘어나며 "```10```"으로 표현된다.

숫자 체계에 익숙한 사람들을 소수만이 컴퓨터가 이해하는 시스템이 아니라는 것을 알 것이다.

자바 언어가 지원하는 다른 숫자 체계는 **8진법**과 **16진법**이 있다.

8진법 체계에서 허용되는 숫자는 ```0```부터 ```7```까지 이며, ```8```은 "```010```"으로 표현된다. 맨 앞의 ```0```은 ```10```진법과 소수점 형식을 구분하기 위해서 추가된 것이다.

16진법 체계에서 허용되는 숫자는 ```0```부터 ```9```이고 그 다음이 ```a``부터 ```f``` (혹은 ```A```부터 ```F```)이다. ```16```의 값은 "```0x10```"으로 표현된다. 앞의 ```0x```는 컴파일러가 16진법임을 인식하게 하기위해 추가되었다.

자바에서 이 세 가지 숫자 체계를 어떻게 지원하는지 보자.

##### Snippet-01 : 정수형으로 8진법 및 16진법 저장

자바에는 각 숫자 체계별 정수형이 없다! 10진법,8진법,16진법 값을 저장하는 데에는 같은 ```int```형이 사용된다.

유효한 숫자에 대한 숫자 체계 규칙을 준수하고 컴파일러가 주는 힌트를 이해한다면 어려울 것이 없다.

```java

	jshell> int eight = 010;
	eight ==> 8
	jshell> int sixteen = 0x10;
	sixteen ==> 16
	jshell> int fifteen = 0xf;
	fifteen ==> 15
	jshell> int eight = 08;//8 is invalid octal digit
	| Error:
	| integer number too large : 08
	| int eight = 08;
	|___________^
	jshell> int big = 0xbbaacc;
	big ==> 12298956
	jshell>

```

##### Snippet-02 : 정수 타입 캐스팅 더 알아보기

할당에는 두 종류가 있다:
* 리터럴에서 변수 할당: ```short s = 123456;``` 에서 이 데이터는 분명히 범위를 벗어났다.(컴파일 타임에 알 수 있다) 컴파일러가 오류를 표시한다.
* 변수에서 변수 할당: ```sh =in;```에서, ```int in```에 저장된 가치는 ```4567```로, ```short``` 타입의 범위 내에 충분히 있다. 컴파일러는 모험을 하지 않기로 선택하고 오류를 표시한다. 이는 또 `sh = (short) in`으로 명시적으로 캐스팅할 수 있다.

```java

	jshell> byte b = 128;
	| Error:
	| incompatible types: possible lossy conversion from int to byte
	| byte b = 128;
	|_________^--^
	jshell> short s = 123456;
	| Error:
	| incompatible types: possible lossy conversion from int to short
	| short s = 123456;
	|__________^-------^
	jshell> short sh = 3456;
	sh ==> 3456
	jshell> int in = 4567;
	in ==> 3456
	jshell> sh = in;
	| Error:
	| incompatible types: possible lossy conversion from int to short
	| sh = in;
	|______^
	jshell> sh = (short) in;
	sh ==> 4567
	jshell> int num = sh;
	num ==> 4567
	jshell>

```

#### 정수형에 대한 기본형 연산자

우리는 이미 다음과 같은 정수 유형의 산술 연산자를 엿볼 수 있었다:

* ```+```
* ```-```
* ```*```
* ```/```
* ```%```
* ```++``` (사전,사후 증가 둘 다)
* ```--``` (사전,사후 감소 둘 다)

증감 연산자는 실제로 복잡한 구문을 하기에는 부족하기 때문에 때문에 흥미로운 사례다. 우리가 그들의 사전,사후 연산 버전을 사용할 때, 우리는 부작용에 대해 주의해야 한다.

##### Snippet-03 : 증감 연산자

```int j = i++;```와 같은 사후 증가에서는,  할당 *이후* 증가가 이루어진다. ```j```는 증가하기 전에 값을 얻는다.

```java

	jshell> int i = 10;
	i ==> 10
	jshell> int j = i++;
	j ==> 10
	jshell> i
	i ==> 11
```

```int n = ++m;```과 같은 사전 증가는, 증가가 할당 *이전*에 이루어진다. ```n```은 증가 후 값을 얻는다.

```java
	jshell> int m = 10;
	m ==> 10
	jshell> int n = ++m;
	n ==> 11
	jshell> m
	m ==> 11ㄷ
```

```int l = k--;```와 같이 사후 감소는,  할당이 완료된 *이후* 감소한다. ```int q = --p;```와 같이 사전 감소는 할당 *이전*에 수행된다.

```java
	jshell> int k = 10;
	k ==> 10
	jshell> int l = k--;
	l ==> 10
	jshell> k
	k ==> 9
	jshell> int p = 10;
	p ==> 10
	jshell> int q = --p;
	q ==> 9
	jshell> p
	p ==> 9
	jshell>

```

#### 요약:

이번 단계에서는

* 자바에서 지원하는 정수 숫자 체계를 확인했다.
* 사전 및 사후 증감 연산자가 어떻게 작동하는지 조사했다.

- - -	
### Step 03: Classroom Exercise CE-01 (With Solutions)

#### Exercise Set

1. 한 쌍의 정수를 저장하고 다음과 같은 기능을 가진 자바 ```class``` ```BiNumber```를 생성하시오

	* 초기 2 개의 숫자를 전달하여 저장할 수 있음
	* 저장된 정수의 덧셈 및 곱셈 작업을 지원해야함
	* 두 숫자의 값을 두 배로 증가시키는 연산
	* 각 숫자에 개별적으로 접근하기 위한 연산

요컨대 우리는 러너 클래스의 ```main```메소드로 이와 같은 코드를 작성할 수 있어야 한다.
	
```java

	BiNumber numbers = new BiNumber(2, 3);
	System.out.println(numbers.add());
	System.out.println(numbers.multiply());
	numbers.double();
	System.out.println(numbers.getNumber1());
	System.out.println(numbers.getNumber2());

```

#### Solution to CE-01

**_BiNumber.java_**

```java

	package com.in28minutes.primitive.datatypes;
	
	public class BiNumber {
		private int number1;
		private int number2;

		public BiNumber(int number1, int number2) {
			this.number1 = number1;
			this.number2 = number2;
		}

		public int add() {
			return number1 + number2;
		}

		public int multiply() {
			return number1 * number2;
		}

		public void doubleValue() {
			number1 *= 2;
			number2 *= 2;
		}

		public int getNumber1() {`
			return number1;
		}

		public int getNumber2() {
			return number2;
		}

		public void setNumber1(int number1) {
			this.number1 = number1;
		}

		public void setNumber2(int number2) {
			this.number2 = number2;
		}
	}

```

**_BiNumberRunner.java_**

```java

	package com.in28minutes.primitive.datatypes;

	public class BiNumberRunner {
		public static void main(String[] args) {
			BiNumber numbers = new BiNumber(2, 3);
			System.out.println(numbers.add());
			System.out.println(numbers.multiply());
			numbers.doubleValue();
			System.out.println(numbers.getNumber1());
			System.out.println(numbers.getNumber2());
		}
	}

```

**_콘솔창 출력_**

_5_

_6_

_4_

_6_

### Step 05: 부동 소수점형

Java에는 부동 소수점 숫자를 지원하는 두 가지 유형이 있다는 점을 상기할 수 있다:
* ```double```: 8바이트 용량의 부동 소수점 리터럴에 대한 기본 타입.
* ```float```: 4바이트 용량의 부동 소수점 데이터에 대해 더 좁은 표현.(덜 정확함)

Code Snippet 몇 개로 우리가 알고 잇는 것들을 새롭게 해보자.

##### Snippet-01 : double과 float

자바의 기본 부동 소수점 타입은 ```double```이다. ```float```리터럴은 ```f```또는 ```F```가 뒤에 붙어야 한다.


```java

	jshell> float f = 34.5;
	| Error:
	| incomaptible types: possible lossy conversion from double to float
	| float f = 34.5;
	|_________^---^
	jshell> float f = 34.5f;
	f ==> 34.5
	jshell> float fl = 34.5F;
	fl ==> 34.5
	jshell> double d = 34.5678;
	d ==> 34.5678
	jshell> float flo = d;
	| Error:
	| incomaptible types: possible lossy conversion from double to float
	| float flo = d;
	|__________^
	jshell> float flo = (float) d;
	flo ==> 34.567
	jshell>

```

##### Snippet-02 : double형 연산자

double형에서는 `++`,`--`와 `%` 연산자를 사용할 수 있다.

```java

jshell> double dbl = 34.5678;
dbl ==> 34.5678

jshell> dbl++
$3 ==> 34.5678

jshell> dbl
dbl ==> 35.5678

jshell> dbl--
dbl ==> 35.5678
jshell> dbl % 5
dbl ==> 4.567799999999998
```

float형을 정수형으로 변환하려면 `int i = (int)f`와 같은 명시적인 캐스트가 필요하다.

```java
	jshell> float f = 34.5678f;
	f ==> 34.5678
	jshell> int i = f;
	| Error:
	| incomaptible types: possible lossy conversion from float to int
	| int i = f;
	|_______^
	jshell> int i = (int)f;
	i ==> 34
	jshell> float fl = i;
	fl ==> 34.0
	jshell>

```
#### 요약

이번 단계에서는

* 부동 소수점 타입의 변수 및 리터럴을 생성하는 방법을 확인했다.
* ```double```과 ```float```형의 차이점을 이해했다.


### Step 06: Introducing BigDecimal

```double```과 ```float```는 비슷하지만 부동 소수점의 정확한 표현은 아니다.

사실, 그들은 과학적 실험이나 재정적 응용과 같이 높은 정확도를 요구하는 계산에는 사용되지 않는다. 다음 예는 그 이유를 보여준다.


```java

	jshell> 34.56789876 + 34.2234
	$1 ==> 68.79129875999999
```

문자 그대로 ```34.56789876 + 34.2234```는 ```68.79129876```으로 평가해야 한다. 위의 덧셈은 정확하지 않다.

이는 ```double````과 ```float```타입에서 사용되는 부동소수점의 결함 때문이다.

이러한 문제를 해결하기 위해 자바에는 ```BigDecimal``` 클래스가 도입되았다.

```BigDecimal```표현의 정확성은 ```String```의 리터럴을 사용할 때만 유지된다.


```java

	jshell> BigDecimal number1 = new BigDecimal("34.56789876");
	number1 ==> 34.56789876
	jshell> BigDecimal number2 = new BigDecimal("34.2234");
	number2 ==> 34.2234_
```

```BicDecical```타입은 **불가변**객체를 만들 때만 사용될 수 있따. *불가변*객체의 값은 생성 후 변경할 수 없다.

`number1.add(number2)`를 실행할 때 number1의 값이 변경되지 않음을 알 수 있다. 합계의 결과를 얻기 위해서는, 새로운 변수 `sum`을 만든다.

```java
	jshell> number1.add(number2);
	$2 ==> 68.79129876
	jshell> number1
	number1 ==> 34.56789876
	jshell> BigDecimal sum = number1.add(number2);
	sum ==> 68.79129876
```

#### 요약

이번 단계에서는

* ```double```과 ```float```가 매우 정확한 데이터 타입이 아니라는 것을 알게 되었다.
* ```BigDecimal```의 내장 데이터 타입 소개했다.
* ```BigDecimal```은 불변하다는 것을 이해했다.
* 문자열 리터럴을 사용하여 ```BigDecimal```데이터를 구성할 때 정확도가 가장 우수하다는 점을 확인했다.

### Step 06: BigDecimal 연산자

```BigDecimal```클래스에 정의된 몇 가지 다른 연산자들을 살펴보자. 

##### Snippet-01: 산술 연산

모든 BigDecimal 연산자는 BigDecimal 피연산자만 지원한다.

```java

	jshell> BigDecimal number1 = new BigDecimal("11.5");
	number1 ==> 34.56789876
	jshell> BigDecimal number2 = new BigDecimal("23.45678");
	number2 ==> 23.45678
	jshell> number1.add(number2);
	$1 ==> 34.95678
```

```BigDecimal```은 기본형 타입의 데이터와는 잘 어울리지 않는다.

```java
	jshell> int i = 5;
	i ==> 5
	jshell> number1.add(i);
	| Error:
	| incompatible types: int cannot be converted to java.math.BigDecimal
	| number1.add(i);
	|_____________^
```

`BigDecimal` 값을 더하거나, 곱하거나, 나누거나 뺄수도 있다.

```java
	jshell> number1.add(new BigDecimal(i));
	$2 ==> 16.5
	jshell> number1.multiply(new BigDecimal(i));
	$3 ==> 67.5
	jshell> number1.divide(new BigDecimal(100));
	$4 ==> 0.115
	jshell>

```

#### 요약

이번 단계에서는

* 기본적인 산수를 위한 ```BigDecimal``` 메소드 탐구했다
* ```BigDecimal```에 대부분의 기본 자바 숫자 타입을 수용하는 생성자가 있는 것으로 확인되었다.


###Step 07: Classroom Exercise CE-02

#### Exercise-Set

원금 금액에 대해 단순 이자 계산을 수행하는 프로그램을 작성하십시오. 그러한 계산 공식은 다음과 같다:

`총액(TA) = 원금 (PA) + ( PA * 단순 이자(SI) 금리 * 년 단위 기간(N))`

본질적으로 다음과 같은 방법으로 사용할 수 있는 ```SimpleInterestCalculator`` ```class```를 작성하시오.

```java

	SimpleInterestCalculator calculator = new SimpleInterestCalculator("4500.00", "7.5");
	BigDecimal totalValue = calculator.calculateTotalValue(5); //5 year duration
	System.out.println(totalValue);

```

#### Solution To CE-02

**_SimpleInterestCalculatorRunner.java_**

```java

	package com.in28minutes.primitive.datatypes;
	import java.math.BigDecimal;

	public class SimpleInterestCalculatorRunner {
		public static void main(String[] args) {
			SimpleInterestCalculator calculator = new SimpleInterestCalculator("4500.00", 7.5");
			BigDecimal totalValue = calculator.calculateTotalValue(5); //5 year duration
			System.out.println(totalValue);
		}
	}

```

**_SimpleInterestCalculator.java_**

```java

	package com.in28minutes.primitive.datatypes;
	import java.math.BigDecimal;

	public class SimpleInterestCalculatorRunner {
		BigDecimal principal;
		BigDecimal interest;

		public SimpleInterestCalculator(String principal, String interest) {
			this.principal = new BigDecimal(principal);
			this.interest = new BigDecimal(interest).divide(new BigDecimal(100));
		}

		public BigDecimal calculateTotalValue(int noOfYears)
			//Total Value = Principal  + Principal * Interest* Years
			BigDecimal totalValue = prinipal.add(principal.multiply(interest).multiply(new BigDecimal(noOfYears)));
			return totalValue;`
		}	
}

```

**_콘솔창 출력:_**

_6187.50000_

#### Tip: The ```import``` Statement

자바의 ```import(가져오기)``` 구문은 또 다른 ```package```의 ```class```를 사용하는 각 소스 파일에 필요하다. 따라서 **SimpleInteretCalculator.java_**(```class```정의)와 **SimpleInterestCalculatorRunner.java_**(runnber ```class```정의) 모두 ```class``` ```java.math.BigDecimal```을 가져와야 한다.

```package java.lang.*```는 기본적으로 가져오게 된다.

뒤에 붙는 ```.*```는 ```package``` ```java.lang```의 모든 클래스를 가져오는 것을 나타낸다.


#### 요약

이번 단계는

* 독립된 자바 프로그램에서 ```BigDecimal```값 사용했다.
* ```import```구문을 통해 내장된 자바 패키지의 사용 방법을 알아보았다.


### Step 08: ```boolean```, 관계 및 논리적 연산자

자바 ```boolean```의 데이터 타입은 ```참```과 ```거짓```이라는 두 가지 가치 중 하나만을 담고 있는 것이다. 두 라벨 모두 대소문자를 구분한다. 우리는 ```boolean```의 결과를 주기 위해 수식을 평가하는 ```=```,```!=```,```>```와 같은 내장 비교 연산자의 예를 보아왔다. 이들 중 몇 가지를 간단히 재점검해 보자.

##### Snippet-01 : 관계 연산자 : 재점검

관계 연산자는 주로 비교를 위해 사용된다. 이들은 ```boolean```이 아닌 기본형 타입의 피연산자를 받아들여 ```boolean```값을 반환한다.

```java

	jshell> int i = 7;
	i ==> 7
	jshell> i > 7;
	$1 ==> false
	jshell> i >= 7;
	$2 ==> true
	jshell> i < 7;
	$3 ==> false
	jshell> i <= 7;
	$4 ==> true
	jshell> i == 7;
	$5 ==> true
	jshell> i == 8;
	$6 ==> false
	jshell>
	
```

#### 논리 연산자

자바에는 수식에 사용되는 논리 연산자도 있다. 논리 연산자들은 ```boolean```타입의 피연산자를 기대한다. 이와 관련된 표현들은 ```if```,```for```,과 ```while```의 구문을 포함하여 ```boolean```의 코드 조건을 형성하는 데 사용된다. 유명한 논리 연산자는:

* ```&&``` : 논리적 **AND**
* ```||``` : **OR**
* ```!``` : **NOT**

이제 이들을 우리의 코드에 어떻게 사용하는지 알아보자.

##### Snippet-02 : 논리 연산자

우리는 `i`rk `15`와 `25`사이인지 알고싶다. 이는 `i >= 15 && i <= 25`라는 수식을 사용할 수 있다. 자세한 내용은 아래를 참조하십시오.

```java

	jshell> int i = 17;
	i ==> 17
	jshell> i >= 15
	$1 ==> true
	jshell> i <= 25
	$2 ==> true
	jshell> i >= 15 && i <= 25
	$3 ==> true
	jshell> i == 30;
	i ==> 30
	jshell> i >= 15 && i <= 25
	$4 ==> false
	jshell> i == 5;
	i ==> 30
	jshell> i >= 15 && i <= 25
	$5 ==> false
```

```&&```을 사용한 수식은 ```boolean``` 피연산자가 **모두** ```참```으로 평가해야만 ```참```으로 평가된다.

```java
	jshell> true && true
	$6 ==> true
	jshell> true && false
	$7 ==> false
	jshell> false && true
	$8 ==> false
	jshell> false && false
	$9 ==> false
	jshell>

```

##### Snippet-02 설명

다음 예는 유명한 논리 연산자를 위한 진리표를 시각화하는데 도움이 된다.

```java

	jshell> true || true
	$1 ==> true
	jshell> true || false
	$2 ==> true
	jshell> false || true
	$3 ==> true
	jshell> false || false
	$4 ==> false
	jshell> true ^ true
	$5 ==> false
	jshell> true ^ false
	$6 ==> true
	jshell> false ^ true
	$7 ==> true
	jshell> false ^ false
	$8 ==> false
	jshell> !true
	$9 ==> false
	jshell> !false
	$10 ==> true
	jshell> int x = 6;
	x ==> 6
	jshell> !(x > 7)
	$11 ==> true
	jshell>

```

#### 요약

이번 단계에서는

* 우리는 ```boolean```의 기본형 타입을 소개받았다.
* Java 프로그램에서 논리 연산자가 사용되는 위치를 이해했다.
* 일반적으로 사용되는 논리 연산자의 진리표를 탐색했다.

### Step 09: 단락 평가

아래의 코드를 살펴보십시오. ```j > 15 && i++ > 5```라는 표현은 예상대로 ```거짓```으로 평가된다. `j>15`는 `j` 값이 15이기 때문에 거짓이다.

```java

	jshell> int j = 15;
	j ==> 15
	jshell> int i = 10;
	i ==> 10
	jshell> j > 15 && i++ > 5
	$1 ==> false
	jshell> j
	j ==> 15
	jshell> i
	i ==> 10
```

i의 값이 변하지 않고 `10`인 것도 관찰할 수 있다.

왜냐 하면 ```i++ > 5```는 평가조차 받지 않았기 때문이다.

그 이유는 `&&`가 게으르기 때문이다. `j < 5`를 거짓이라고 봤다. 따라서,두 번째 수식의 결과와 상관없이 이 `&&`의 결과는 거짓일 것이다. 그렇기 때문에 두 번째 수식을 평가하지 않는다.

***자세한 설명***

```j > 15 && i++ > 5```라는 수식은 왼쪽에서 오른쪽으로 스캔되었다. ```&&```의 첫 피연산자가 ```거짓```이라고 평가하자, 컴파일러는 게을러졌다. `&&`는 최종 결과에 영향을 주지 않는 수식의 연산은 피한다. 이러한 최적화의 이름은 **Short-Circuit Evaluation**으로 **지연 평가**라고도 한다.
 
 논리 연산자 ```&```는 또 다른 버전의 논리**AND** 연산자로, 지연 평가를 하지 않는다.
 
 ```&```의 두 피연산자는 항상 평가된다.

```java

	jshell> j > 15 & i++ > 5
	$1 ==> false
	jshell> j
	j ==> 15
	jshell> i
	i ==> 11
	jshell>

```

마찬가지로 논리 **OR** 연산자에도 두 가지 버전이 있다:
* 앞서 본 ```||```연산자. 이는 지연 평가를 보여준다.
* 지연 평가가 없는 ```|```연산자.

컴파일러의 지연 평가에 코드가 의존하는 것은 나쁜 프로그래밍 관행이다. 그것은 코드를 읽기 어렵게 만들고, 고치기 어려운 소프트웨어 버그를 숨길 수 있다. 이는 분명히 코드 유지에 부담을 가중시키므로, 하지 않는게 좋다.

#### 요약

이번 단계에서는

* 논리적 연산자를 포함한, 즉 지연 평가가 있는 조건식을 조사했다.
* 지연 평가는 연산자의 진리표에 따라 결정됨.
* 지연 평가기 없는 버전의 연산자를 확인했다.
* 지연 평가에 의존하는 코드는 읽기 어렵다는 것을 알게 됨.


### Step 10: 문자형
 
앞서, 다음과 같은 기본 키보드 문자(일명 **아스키 코드**문자)를 저장할 수 있는 방법을 살펴보았다.
* 대문자 및 소문자(A-Z,a-z)
* 숫자(0-9)
* 문장 부호 미 기타 특수 문자(',','$','{'등)

자바는 **유니코드**라고 하는 훨씬 더 큰 문자 부호화 집합을 지원한다. 모든 유니코드 문자는 코드에 의해 입력,출력 및 이해 처리 될 수 있다.


##### Snippet-01 : 유니코드 문자

모든 유니코드 문자를 키보드에서 입력할 수 있는 것은 아니다. 하지만 자바는 당신이 그들의 형식을 올바르게 처리한다면 당신의 코드에서 그 값을 처리할 수 있게 해준다.

```java 
 
	jshell> char ch = '"';
	ch ==> '"'
	jshell> char c = '\u0022';
	c ==> '"'
```

정수 값은 ```char```변수에 저장할 수 있다. 값이 유의미한 범위 내에 있으면 키보드 문자의 **아스키**값과도 일치한다.

```java
	jshell> char cn = 65;
	cn ==> 'A'
```

정수 산술은 `char`데이터에 대해 수행할 수 있다.

```java
	jshell> cn++
	$1 ==> 'A'
	jshell> cn
	$2 ==> 'B'
	jshell> ++cn
	$3 ==> 'C'
	jshell> cn + 5
	$4 ==> 72
	jshell> cn
	cn ==> 'C'
	jshell> (int)cn
	cn ==> 67
	jshell>

```


#### 요약

이번 단계에서는

* ```char```데이터 타입을 소개했다.
* 유니코드가 문자 집합을 키보드보다 더 많이 갖는다는 사실을 확인했다.
* 아스키 문자는 정수 값으로 부호화된 ```char```값이다.

### Step 11: Programming Exercise PE-02

#### Exercise Set

1.  특별한 ```char```타입인 ```MyChar```클래스를 작성하시오. ```MyChar```타입의 객체는 ```char```입력 데이터 요소를 중심으로 생성되며, 다음과 같은 작업을 수행한다.
	* 입력 문자가 다음과 같은지 확인:
		* 숫자
		* 알파벳 문자
		* 모음(대문자 또는 소문자)
		* 자음(대문자 또는 소문자) 참고: 글자는 모음이 아니면 자음이다.
	* 알파벳을 모두 다음과 같이 출력
		* 대문자
		* 소문자
		
본질적으로 ```MyChar```의 러너인 ```class```의 경우 ```main```메소드가 다음과 유사한 코드를 실행하게 될 것이다.

```java

	MyChar myChar = new MyChar('c');
	System.out.println(myChar.isDigit());
	System.out.println(myChar.isAlphabet());
	System.out.println(myChar.isVowel());
	System.out.println(myChar.isConsonant());
	myChar.printLowerCaseAlphabets();
	myChar.printUpperCaseAlphabets();

```

### Step 12: Solution To PE-02, Part 1 - ```isVowel()```

**_MyCharRunner.java_**

```java

	package com.in28minutes.primitive.datatypes;

	public class MyCharRunner {
		public static void main(String[] args) {
			MyChar myChar = new MyChar('c');
			System.out.println(myChar.isVowel());
		}
	}

```

**_MyChar.java_**

```java

	package com.in28minutes.primitive.datatypes;
	
	public class MyChar {
		private char ch;
		
		public MyChar(char ch) {
			this.ch = ch;
		}

		public boolean isVowel() {
			if(ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u') {
				return true;
			} 
			if(ch == 'A' || ch == 'E' || ch == 'I' || ch == 'O' || ch == 'U') {
				return true;
			}
			return false;
		}
	}

```

**_콘솔창 출력_** :

_false_

### Step 13: Solution To PE-02, Part 2 - ```isDigit()```

**_MyCharRunner.java_**

```java

	package com.in28minutes.primitive.datatypes;

	public class MyCharRunner {
		public static void main(String[] args) {
			MyChar myChar = new MyChar('c');
			System.out.println(myChar.isDigit());
			System.out.println(myChar.isVowel());
		}
	}

```

**_MyChar.java_**

```java

	package com.in28minutes.primitive.datatypes;

	public class MyChar {
		private char ch;

		public MyChar(char ch) {
			this.ch = ch;
		}

		public boolean isVowel() {
			if(ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u') {
				return true;
			} 

			if(ch == 'A' || ch == 'E' || ch == 'I' || ch == 'O' || ch == 'U') {
				return true;
			}
			return false;
		}

		public boolean isDigit() {
			if(ch >= 48 && ch <= 57) {
				return true;
			}
			return false;
		}

}

```

**_콘솔창 출력_** :

_false_

_false_

### Step 14: Solution To PE-02, Part 3 - Other Methods

**_MyCharRunner.java_**

```java

	package com.in28minutes.primitive.datatypes;
	
	public class MyCharRunner {
		public static void main(String[] args) {
			MyChar myChar = new MyChar('c');
			System.out.println(myChar.isDigit());
			System.out.println(myChar.isAlphabet());
			System.out.println(myChar.isVowel());
			System.out.println(myChar.isConsonant());
			myChar.printLowerCaseAlphabets();
			myChar.printUpperCaseAlphabets();
		}
	}

```

**_MyChar.java_**

```java

	package com.in28minutes.primitive.datatypes;

	public class MyChar {
		private char ch;
		
		public MyChar(char ch) {
			this.ch = ch;
		}

		public boolean isVowel() {
			if(ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u') {
				return true;
			} 
			if(ch == 'A' || ch == 'E' || ch == 'I' || ch == 'O' || ch == 'U') {
				return true;
			}
			return false;
		}

		public boolean isConsonant() {
			if(isAlphabet() && !(isVowel())) {
				return true;
			}
			return false;
		}

		public boolean isDigit() {
			if(ch >= 48 && ch <= 57) {
				return true;
			}
			return false;
		}

		public boolean isAlphabet() {
			if(ch >= 97 && ch <= 122) {
				return true;
			}
			if(ch >= 65 && ch <= 90) {
				return true;
			}
			return false;
		}

		public void printLowerCaseAlphabets() {
			for(char ch='a'; ch <= 'z'; ch++) {
				System.out.println(ch);
			}
		}

		public void printUpperCaseAlphabets() {
			for(char ch='A'; ch <= 'Z'; ch++) {
				System.out.println(ch);
			}
		}
	}

```

**_콘솔창 출력_** :

_false_

_true_

_false_

_true_

a

b

c

d

e

f

g

h

i

j

k

l

m

n

o

p

q

r

s

t

u

v

w

x

y

z

A

B

C

D

E

F

G

H

I

J

K

L

M

N

O

P

Q

R

S

T

U

V

W

X

Y

Z

### Step 15: 기본형  타입 -복습

이 절에서는 기본형 자바 타입에 대한 지식을 바탕으로 하였다.

* 우리는 처음에 유용한 타입 정보를 저장하는 정수 타입의 기본 래퍼에 익숙해졌다.
* 정수에서 부동 소수점 타입으로 전환하여 타입 호환성과 컴파일러가 일반적인 에러에 대해 경고하는 방법을 검토했다. 우리는 형 변환을 강제하기 위해 명시적인 캐스팅을 사용했고, 묵시적 형 변환 또한 꽤 흔하다는 것을 배웠다.
* 정밀도와 정확도가 높은 부동 소수점 타입인 ```BigDecimal```클래스로 넘어갔다.
* 그 다음 행은 ```boolean```으로, 우리가 알고 있는 논리적인 표현을 바탕으로 했다. 우리는 논리 연산자에 초점을 맞췄고, 그들의 수식에 대한 단락 평가에 더 집중했다.
* 지연 평가에 의존하는 것이 좋은 프로그래밍 관행이 아니라는 것과 부작용에 대해 알게 되었다.
* 마침내 우리는 ```char```타입에 도달했고, 키보드가 한계가 아니라는 것을 알게 되어 놀랐다.

## 조건문 소개 - if, switch and more

의사결정은 우리의 일상 생활의 일부분이다. 컴퓨터는 인간을 위한 일을 하기 때문에 프로그램도 결정을 내려야 한다. 그들은 ```boolean``` 값으로 평가되는 논리적 조건문을 점검함으로써 다음과 같이 한다.

다음 단계에서는, 다음 **조건문**을 살펴보십시오.

* ```if```
* ```if```-```else```
* ```if```-```else if```-```else```
* ```switch```  

이러한 기본을 숙달하기 위해 프로그래밍 과제를 해결하기 데에 사용하는 것보다 더 좋은 방법은 무엇일까?

자, 갑니다!

#### Programming Challenge : Design A Menu (The *Menu-Challenge*)


* 사용자에게 입력을 요청하는 것:
	* 두 개의 숫자를 입력하십시오.
	* 다음 항목에 대해 수행할 산술을 선택하십시오:
		* 더하기
		* 빼기
		* 곱하기
		* 나누기
* 작업 수행
* 결과 게시

***An example scenario could be:***

Enter First Number

2

Enter Second Number

4

1 - Add

2 - Subtract

3 - Multiply

4 - Divide

Enter your choice of operation

3

The Result Is : 8

#### 요약

이번 단계에서는

* 입력 내용이 프로그램의 제어 흐름에 미치는 영향을 설명했다.
* Java에서 사용할 수 있는 조건문의 목록을 살펴보았다.
* 조건문에 대해 배우는 데 도움이 되는 프로그래밍 과제를 선택했다.

### Step 01: 조건식 ```if``` 와 ```if```-```else```

```if```구문은 프로그램의 제어 흐름을 관리하기 위한 가장 기본적인 방법이다. ```boolean```의 상태를 검사하고 ```참```으로 판명되면 일부 코드가 실행된다. 그렇지 않으면, 그 코드는 실행되지 않는다.

* "**_```조건식```이 ```참```일때 무언가 하라_**"

개념적으로, if구문은 다음과 같다:

```java

	if(condition) {
		<if-body>
	}

```

```if```-```else```구문이 평이한 ```if```에 비해 개선되었다. 이제 우리는 ```조건문```이 무엇을 평가하느냐에 따라 두 가지 코드 중 하나를 실행할 수 있다.

* "**_```조건식```이 ```참```일 때는 뭔가 하고, ```조건식```이 ```거짓```일 때는 또 다른 것을 하라_**"

```if```-```else```구문은 다음과 같은 것으로 요약된다.

```java

	if(condition) {
		<if-body>
	} else {
		<else-body>
	}

```

If ```condition``` is found to be ```true```, the statement block ```<if-body>``` is executed, otherwise ```<else-body>``` is run.
```조건문```이 ```참```으로 판명되면, 구문 블록 ```<if-body>```가 실행되고, 그렇지 않으면 ```<else-body>```가 실행된다.

이제 이러한 조건문을 활용한 예를 살펴보자.

##### Snippet-01 : ```if``` behavior

이 예에서는 다음을 수행하십시오.
* ```boolean```값을 평가하는 ```<=```, ```>=``` 복합 비교 연산자를 사용한다.
* 또한 ```boolean```타입의 가치를 수용하고 반환하는 ```&&```과 ```||```와 같은 논리적 연산자도 사용된다.


```java

	jshell> int i = 3;
	i ==> 3
	jshell> if(i==3) {
	   ..>> System.out.println("True");
	   ..>> }
	True
	jshell> if(i<2) {
	   ..>> System.out.println("True");
	   ..>> }
	
	jshell> if(i<=3 || i >= 35) {
	   ..>> System.out.println("True");
	   ..>> }
	True
	jshell> if(i<=3 && i >= 35) {
	   ..>> System.out.println("True");
	   ..>> }
```

```if```-```else```는 조건식이 `거짓`일 때 실행할 코드를 지정할 수 있다. 

```java
	jshell> if(i==3) {
	   ..>> System.out.println("True");
	   ..>> } else {
	   ..>> System.out.println("i is not 3");
	   ..>> }
	True
	jshell> i = 5;
	i ==> 5
	jshell> if(i==3) {
	   ..>> System.out.println("True");
	   ..>> } else {
	   ..>> System.out.println("i is not 3");
	   ..>> }
	i is not 3
	jshell>

```


##### Snippet-02 : chained ```if```-```else``` - v1

**_IfStatementRunner.java_**

```java

	com.in28minutes.ifstatement.examples;

	public class IfStatementRunner {
		public static void main(String[] args) {
			//int i=25;
			int i=26;
			if(i == 25) {
				System.out.println("i = 25");
			} else {		
				System.out.println("i != 25");
			}
		}
	}

```

**_콘솔창 출력_**

_i != 25_

##### Snippet-03 : chained if-else v2

우리는 세 가지 조건식 즉, `값은 24`, `값은 25` 또는 `값은 24와 25가 아니다`에 대한 수치를 시험하고 싶다. 아래 예에서 나온 코드를 생각해보자.

**_IfStatementRunner.java_**

```java

	com.in28minutes.ifstatement.examples;

	public class IfStatementRunner {
		public static void main(String[] args) {
			// if i is 25, print i = 25
			//if i is 24, print i = 24
			//otherwise, print i != 25 and i != 24
			
			int i=25;
			if(i == 25) {
				System.out.println("i = 25");
			}
			if(i == 24) {
				System.out.println("i = 24"); 
			} else {			
				System.out.println("i != 25 and i != 24");
			}
		}
	}

```

**_콘솔창 출력_**

_i = 25_

_i != 25 and i != 24_

##### Snippet-03 설명

이게 어떻게 된 걸까? 프로그램 내에서 ```i```의 값은 ```25```로 설정되었기 때문에, 앞의 사례처럼 **_i = 25_** 만 출력되었어야 한다.

나머지 출력은 무엇일까?

우리는 세 가지 가능성을 확인하려 한다:
	* ```i```는 ```25```와 같다.
	* ```i```는 ```24```와 같다.
	* 위의 두 가지 모두 해당되지 않음

```if```의 첫 번째 ```i == 25```는 , 뒤에 나오는 ```if```-```else```의 ```i ==24```와는 독립되어 있기 때문에 우리는 출력값을 잘못 알고 있었다.

우리의 결론은 아직 명확하지 않다. 세 가지 이상의 대안을 다루기 위해서는 더 엄격한 조건식이 필요하다. 우리는 다음 단계에서 이 주제를 탐구할 것이다.


#### 요약

이번 단계에서는

* ```if```와 ```if```-```else```조건문에 대해 배웠다.
* 사용법을 알아보기 위해 몇 가지 예제를 시도했다.

### Step 02: The ```if```-```else if```-```else``` Conditional

The ```if```-```else if```-```else``` statement solves the issue we faced, while trying to test more than two conditions.

Let's see an example.

##### Snippet-01 : Matching The ```if``` Clause

**_IfStatementRunner.java_**

```java

	com.in28minutes.ifstatement.examples;

	public class IfStatementRunner {
		public static void main(String[] args) {
			// if i is 25, print i = 25
			//if i is 24, print i = 24
			//otherwise, print i != 25 and i != 24

			int i=25;
			if(i == 25) {
				System.out.println("i = 25");
			} else if(i == 24) {
				System.out.println("i = 24"); 
			} else {
				System.out.println("i != 25 and i != 24");
			}
		}
	}

```

**_Console Output_**

_i = 25_

Let's now try giving ```i``` a different value, say ```24```.

##### Snippet-02: Matching The ```else if``` Clause 

**_IfStatementRunner.java_**

```java

	com.in28minutes.ifstatement.examples;

	public class IfStatementRunner {
		public static void main(String[] args) {
			// if i is 25, print i = 25		
			//if i is 24, print i = 24
			//otherwise, print i != 25 and i != 24
		
			//int i=25;
			int i=24;
			if(i == 25) {
				System.out.println("i = 25");
			} else if(i == 24) {
				System.out.println("i = 24"); 
			} else {
				System.out.println("i != 25 and i != 24");		
			}
		}
	}

```

**_Console Output_**

**_i = 24_**

##### Snippet-02 Explained

* With ```i``` holding ```24```, a different condition (the one coresponding to ```i == 24```) evaluates to ```true```.

Let's now try to get a match with the ```else``` clause, the only one unexplored so far. 

##### Snippet-03: Matching The ```else``` Clause

**_IfStatementRunner.java_**

```java

	com.in28minutes.ifstatement.examples;

	public class IfStatementRunner {
		public static void main(String[] args) {
			// if i is 25, print i = 25
			//if i is 24, print i = 24
			//otherwise, print i != 25 and i != 24
			
			//int i=24;
			int i=26;
			if(i == 25) {
				System.out.println("i = 25");
			} else if(i == 24) {
				System.out.println("i = 24"); 
			} else {
				System.out.println("i != 25 and i != 24");
			}
		}
	}

```

**_Console Output_**

**_i != 25 and i != 24_**

##### Snippet-03 Explained

When ```i``` is given a value of ```26```, the first two conditions are false. Hence, the code in the `else` gets executed. 

_**one, and only one** clause among those present in an  ```if```-```else if```-```else``` statement ever evaluates to ```true```. Also, the code block corresponding to the matched clause will get executed. This is ensured even if conditions are *duplicated*, or *overlap*. In that scenario, only the first such condition, downward from the ```if``` in sequence, will evaluate to ```true```. The remaining possible matches are not even checked._

#### Summary

In this step, we:

* Learned about the ```if```-```else if```-```else``` conditional
* Found out how to test when each different clause gets executed
* Understood the guarantees made by Java regarding the conditional's code execution

### Step 03:  Puzzles on ```if```

Try and guess the outputs of the following puzzles.

#### Programming Puzzle PP-01

```java

	public class puzzleRunner {

		public static void main(String[] args) {
			puzzleOne();
		}

		public static void puzzleOne() {
			int k = 15;
			if(k > 20) {
				System.out.println(1);
			} else if(k > 10) {
				System.out.println(2);
			} else if(k < 20) {
				System.out.println(3);
			} else {
				System.out.println(4);
			}
		}
	}

```

**Answer:**

**_2_**

#### Programming Puzzle PP-02

```java

	public class puzzleRunner {
		public static void main(String[] args) {
			puzzleTwo();
		}

		public static void puzzleTwo() {
			int l = 15;
			if(l < 20)
			System.out.println("l < 20");
			if(l > 20)
			System.out.println("l > 20");
			else
			System.out.println("Who Am I?");
		}
	}

```

**Answer:**

**_l < 20_**

**_Who Am I?_**

#### Programming Puzzle PP-03

```java

	public class puzzleRunner {
		public static void main(String[] args) {
			puzzleThree();
		}
		
		public static void puzzleThree() {
			int m = 15;
			if(m > 20)
			if(m < 20)
			System.out.println("m >  20");	else
			System.out.println("Who Am I?");
		}
	}

```

**Answer:**
 

> Nothing is printed. Because the code is structured this way.

```java
if(m > 20) {
	if(m < 20)
		System.out.println("m >  20");	
	else
		System.out.println("Who Am I?");
}
```

#### Programming Puzzle PP-04

```java

	jshell> int i = 0;
	i ==> 3
	jshell> if(i) {
	   ..>> System.out.println("i");
	   ..>> }
	| Error:
	| incompatible types: int cannot be converted to boolean
	| if(i)
	|____^
	jshell> if(i=1) {
	   ..>> System.out.println("i");
	   ..>> }
	| Error:
	| incompatible types: int cannot be converted to boolean
	| if(i=1)
	|____^-^
	jshell> if(i==1) {
	   ..>> System.out.println("i");
	   ..>> }
	jshell>

```

**Answer:**

_**Compiler Error**_

#### Programming Puzzle PP-05

```java

	public class puzzleRunner {
		public static void main(String[] args) {
			puzzleFive();
		}

		public static void puzzleFive() {
			int number = 5;
			if(number < 0)
			number = number + 10;
			number++;
			System.out.println(number);
		}
	}

```

**Answer : **

**_6_**

> In the absence of explicit blocks, Only the statement next to the if statement is considered to be part of the if statement block.

### Step 04: Reading User Input
- - - 

Look at the statement of *Menu-Challenge* once again:

#### *Menu-Challenge*

* Ask the User for input:
	* Enter two numbers
	* Choose an Arithmetic Operation to perform on them:
		* Add
		* Subtract
		* Multiply
		* Divide
* Perform the Operation
* Publish the Result

We have a good idea about how the ```if```-```else if```-```else``` conditional works.What we don't know, however, is how a such a conditional would behave when fed with random input. To test those scenarios out, the next step would be to learn how to take console input, from within our code.

We will do just that, in our next example.

##### Snippet-01: Reading console input

Java provides a built-in ```class``` named  ```Scanner```, to scan user input from the console. Roping in this utility would require you, the programmer, to do the following:
* ```import``` the ```java.util.Scanner``` ```class``` within your code (here, we were writing code in the Eclipse IDE)
* Create a ```scanner``` object which is of type ```Scanner```. This involves invoking the ```Scanner``` constructor through the ```new``` operator. You also need to pass  ```System.in``` as a constructor parameter, which ties ```scanner``` to the console input.
* To read integer input from the console, call the method ```scanner.nextInt()```. The keyboard's <Enter> key needs to be pressed to complete user input. That number is passed on to your code, where it can be passed around.

**_MenuScanner.java_**

```java

	package com.in28minutes.ifstatement.examples;
	import java.util.Scanner;

	public class MenuRunner {
		public static void main(String[] args) {
			Scanner scanner = new Scanner(System.in);
			System.out.print("Enter Number1: ");
			int number1 = Scanner.nextInt();		
			System.out.println("The number you entered is: " + number1);
		}
	}

```

**_Console Output_**

_Enter Number1: 35_

_The number you entered is: 35_


#### Summary

In this step, we:

* Revisited our *Menu-Challenge* problem statement, and found we needed to read user input
* Explored the basic usage of the ```Scanner``` utility to fulfill this need

### Step 05: *Menu-Challenge* : Reading More Input

The *Menu-Challenge* does not stop at a single user input. It requires a total of three numbers to be typed in at the console. So how do we continue asking for input, and read them when they are given?

##### Snippet-01 : Implementing *Menu-Challenge*

**_MenuScanner.java_**

```java

	package com.in28minutes.ifstatement.examples;
	import java.util.Scanner;

	public class MenuRunner {
		public static void main(String[] args) {
			Scanner scanner = new Scanner(System.in);
			System.out.print("Enter Number1: ");
			int number1 = Scanner.nextInt();
			System.out.print("Enter Number2: ");
			int number2 = Scanner.nextInt();

			System.out.println("Select The Operation Choice");
			System.out.println("1 - Add");
			System.out.println("2 - Subtract");
			System.out.println("3 - Multiply");
			System.out.println("4 - Divide");
			System.out.print("Enter Choice: ");
			int choice = Scanner.nextInt();

			System.out.print("Your Inputs Are:");
			System.out.println("Number1: " + number1);
			System.out.println("Number2: " + number2);
			System.out.println("Choice: " + choice);
		}
	}

```

**_Console Output_**

_Enter Number1: 25_

_Enter Number2: 50_

_Operation Choices Available_

_1 - Add_

_2 - Subtract_

_3 - Multiply_

_4 - Divide_

_Enter Choice: 4_

_Your Inputs Are_

_Number1: 25_

_Number2: 50_

_Choice: 4_

##### Snippet-01 Explained

Repeatedly calling ```scanner.nextInt()``` will keep reading in any number the user may input. Also, the user needs to press the keyboard <Enter> key to send each input.

We were not only able to read in all three values we need, but also wrote them out on the console. The user can now see that we got his data! 

#### Summary

In this step, we:

* Figured out how to read more than one input from the console
* Demonstrated how values read in, can be preserved and used within the program

### Step 06: *Menu-Challenge* - Reading Input, Computing Result, Displaying Output

We don't think that after the previous step, anything can stop you from completing the *Menu-Challenge*. Here is one such way, from head-to-toe. 

##### Snippet-01 : All computations

Our solution above does a very simple thing. It combines the mechanisms we learned for reading input and testing conditions, to solve *Menu-Challenge*. 

The ```if```-```else```-```else if``` statement has a total of ```5``` clauses: 
* To check for ```4``` favorable conditions (The ```choice``` values for the ```4``` supported operations). One ```if``` and three ```else```-```if``` clauses do the stuff for us.
* the last default condition, which corresponds to a ```choice``` value not supported, is handled by an ```else``` clause.

**_MenuScanner.java_**

```java

package com.in28minutes.ifstatement.examples;
import java.util.Scanner;

public class MenuRunner {
	public static void main(String[] args) {
		Scanner scanner = new Scanner(System.in);
		System.out.print("Enter Number1: ");
		int number1 = Scanner.nextInt();
		System.out.print("Enter Number2: ");
		int number2 = Scanner.nextInt();

		System.out.println("Select The Operation Choice");
		System.out.println("1 - Add");
		System.out.println("2 - Subtract");
		System.out.println("3 - Multiply");
		System.out.println("4 - Divide");
		System.out.print("Enter Choice: ");
		int choice = Scanner.nextInt();

		System.out.print("Your Inputs Are:");
		System.out.println("Number1: " + number1);
		System.out.println("Number2: " + number2);			
		System.out.println("Choice: " + choice);

		if(choice == 1) {
			System.out.println("Result = " + (number1 + number2));
		} else if(choice == 2) {
			System.out.println("Result = " + (number1 - number2));
		} else if(choice == 3) {
			System.out.println("Result = " + (number1 * number2));
		} else if(choice == 4) {
			System.out.println("Result = " + (number1 / number2));
		} else {
			System.out.println("Invalid Operation");
		}
	}
}

```

**_Console Output_**

_Enter Number1: 23_

_Enter Number2: 10_

_Operation Choices Available_

_1 - Add_

_2 - Subtract_

_3 - Multiply_

_4 - Divide_

_Enter Choice: 2_

_Your Inputs Are_

_Number1: 23_

_Number2: 10_

_Choice: 2_ 

_Result = 13_

**_Console Output_**

_Enter Number1: 25_

_Enter Number2: 35_

_Operation Choices Available_

_1 - Add_

_2 - Subtract_

_3 - Multiply_

_4 - Divide_

_Enter Choice: 5_

_Your Inputs Are_

_Number1: 23_

_Number2: 10_

_Choice: 5_ 

_Invalid Operation_


#### Summary

In this step, we:

* Combined our knowledge of conditionals, with our recent learning on taking multiple console inputs
* Ultimately solved the *Menu-Challenge* problem

### Step 07: Introducing ```switch```

If you remember, our initial list of conditionals to manage control-flow, also had a ```switch``` statement. A ```switch``` also tests multiple conditions, and just like an ```else``` clause, it can handle the default possibility. Conceptually, a ```switch``` statement looks like the following:

```java

	switch(condition) {	
		case 1:
			//<statements>
			break;
		case 2:
			//<statements>
			break;
		//...
		default:
			//<statements>
			break;
		}
	}

```

```default``` clause is executed when none of the cases match. 

 ```break;``` statement is used to break out of the switch after a successful match.

Let's look at a few examples on how to use ```switch```.   

##### Snippet-01: The ```switch``` statement

Using a ```switch``` leads to code that is quite readable, doesn't it? Compare it with the chained ```if```-```else if```-```else``` statements we used in the previous step.

Leaving out the ```break``` statement from every ```case``` clause is a very common error. It leads to a situation called **switch-fall-through**. Here, even if there is a match with a particular ```case``` clause, all clauses following this one are executed in sequence, until a ```break``` is encountered somewhere!

```java

	jshell> int i = 5;
	i ==> 5
	jshell> switch(i) {
	   ..>> case 1 : System.out.println("1");
	   ..>> case 5 : System.out.println("5");
	   ..>> default : System.out.println("default");
	   ..>> }
	5
	default
	jshell> i = 1;
	i ==> 1
	jshell> switch(i) {
	   ..>> case 1 : System.out.println("1");
	   ..>> case 5 : System.out.println("5");
	   ..>> default : System.out.println("default");
	   ..>> }
	1
	5
	default
```

Adding `break`s ensures that only the matching case is executed. 

```java
	jshell> switch(i) {
	   ..>> case 1 : System.out.println("1"); break;
	   ..>> case 5 : System.out.println("5"); break;
	   ..>> default : System.out.println("default"); break;
	   ..>> }
	1
	jshell>
	
```

##### Snippet-02: refactoring MenuScanner

Let's now refactor the `MenuScanner` example to use `switch` statement.

**_MenuScanner.java_**

```java

package com.in28minutes.ifstatement.examples;
import java.util.Scanner;

public class MenuRunner {
	public static void main(String[] args) {
		Scanner scanner = new Scanner(System.in);
		System.out.print("Enter Number1: ");		
		int number1 = Scanner.nextInt();
		System.out.print("Enter Number2: ");
		int number2 = Scanner.nextInt();

		System.out.println("Select The Operation Choice");
		System.out.println("1 - Add");
		System.out.println("2 - Subtract");
		System.out.println("3 - Multiply");
		System.out.println("4 - Divide");
		System.out.print("Enter Choice: ");
		int choice = Scanner.nextInt();

		System.out.print("Your Inputs Are:");
		System.out.println("Number1: " + number1);
		System.out.println("Number2: " + number2);
		System.out.println("Choice: " + choice);

		//performOperationUsingChainedIfElse(number1, number2, choice);`
		performOperationUsingSwitch(number1, number2, choice);
	}

	public static void performOperationUsingSwitch(int number1, int number2, int choice) {
		switch(choice) {
			case 1 : System.out.println("Result = " + (number1 + number2)); break;
			case 2 : System.out.println("Result = " + (number1 - number2)); break;
			case 3 : System.out.println("Result = " + (number1 * number2)); break;
			case 4 : System.out.println("Result = " + (number1 / number2)); break;
			default : System.out.println("Invalid Operation"); break;
		}
	}

	public static void performOperationUsingChainedIfElse(int number1, int number2, int choice) {
		if(choice == 1) {
			System.out.println("Result = " + (number1 + number2));
		} else if(choice == 2) {
			System.out.println("Result = " + (number1 - number2));
		} else if(choice == 3) {
			System.out.println("Result = " + (number1 * number2));
		} else if(choice == 4) {
			System.out.println("Result = " + (number1 / number2));
		} else {		
			System.out.println("Invalid Operation");
		}
	}
}

```

**_Console Output_**

_Enter Number1: 23_

_Enter Number2: 10_

_Operation Choices Available_

_1 - Add_

_2 - Subtract_

_3 - Multiply_

_4 - Divide_

_Enter Choice: 2_

_Your Inputs Are_

_Number1: 23_

_Number2: 10_

_Choice: 2_ 

_Result = 13_

**_Console Output_**

_Enter Number1: 25_

_Enter Number2: 35_

_Operation Choices Available_

_1 - Add_

_2 - Subtract_

_3 - Multiply_

_4 - Divide_

_Enter Choice: 5_

_Your Inputs Are_

_Number1: 23_

_Number2: 10_

_Choice: 5_ 

_Invalid Operation_

#### Summary

In this step, we:

* Explored the ```switch``` conditional
* Saw how it could implement the same control-flow as the ```if``` family of conditionals
* Learned the importance of coding it correctly, to enjoy Java control-flow guarantees

### Puzzles On ```switch```

Let's now have some fun with the various conditionals. These puzzles will not only ensure you're still wide awake, they will also give you ample food for thought. 

##### Programming Puzzle PP-01

```java

	public class SwitchPuzzleRunner {
		public static void main(String[] args) {
			puzzleOne();
		}

		public static void puzzleOne() {
			int number = 2;
			switch(number) {
				case 1:
					System.out.println(1);			
				case 2:
					System.out.println(2);
				case 3:
					System.out.println(3);
				default:
					System.out.println("default");
			}
		}	
	}

```

**_Answer:_**

_2_

_3_

_default_

#### Programming Puzzle PP-02

```java

	public class SwitchPuzzleRunner {
		public static void main(String[] args) {
			puzzleTwo();
		}

		public static void puzzleTwo() {
			int number = 2;
			switch(number) {
				case 1:
					System.out.println(1);
				case 2:
				case 3:
					System.out.println("Number is 2 or 3");
					break;			
				default:
					System.out.println("default");
					break;
			}
		}
	}

```

**_Answer:_**

_Number is 2 or 3_

##### Programming Puzzle PP-03

```java

	public class SwitchPuzzleRunner {
		public static void main(String[] args) {
			puzzleThree();
		}

		public static void puzzleThree() {
			int number = 10;
			switch(number) {
				case 1:
					System.out.println(1);
					break;
				case 2:
					System.out.println(2);
					break;
				case 3:
					System.out.println(3);
					break;
				default:
					System.out.println("default");
					break;
			}
		}
	}

```

**_Answer:_**

_default_

#### Programming Puzzle PP-04

```java

	public class SwitchPuzzleRunner {
		public static void main(String[] args) {
		puzzleFour();
	}

		public static void puzzleFour() {
			int number = 10;
			switch(number) {
				System.out.println("default");
				break;
				case 1:
					System.out.println(1);
					break;
				case 2:
					System.out.println(2);
					break;
				case 3:
					System.out.println(3);
					break;
				default:	
			}
		}
	}

```

**_Answer:_**

_default_

#### Programming Puzzle PP-05

```java

	public class SwitchPuzzleRunner {
		public static void main(String[] args) {
			puzzleFive();
		}

		public static void puzzleFive() {
			long l = 15;
			switch(l) {
			}
		}
	}

```

**_Answer:_**

**_Compiler Error_**

#### Programming Puzzle PP-06

```java

	public class SwitchPuzzleRunner {
		public static void main(String[] args) {
			puzzleSix();
		}

		public static void puzzleSix() {
			int number = 10;
			int i = number * 2;
			switch(number) {
				case number>5 : System.out.println("number>5");
			}
		}
	}

```

**_Answer:_**

**_Compiler Error_**

### Step 09: Comparing The ```if``` Family, And ```switch```

Let's compare and contrast these two approaches, to gain some experience on how to choose a conditional.

First comes an example using the ```if```-```else if```-```else``` statement.  

##### Snippet-01 : Formatted Output Using ```if```

**_OperatorChoiceRunner.java_**

```java

	package com.in28minutes.ifstatement.examples;

	public class OperatorChoiceRunner {
		public static void main(String[] args) {
			OperatorChoice opChoice = new OperatorChoice(5, 2, 1);
			opChoice.operate();
		}
	}

```

**_OperatorChoice.java_**

```java

	package com.in28minutes.ifstatement.examples;

	public class OperatorChoice {
		private int number1;
		private int number2;
		private int choice;
		
		public OperatorChoice(int number1, int number2, int choice) {
			this.number1 = number1;		
			this.number2= number2;
			this.choice = choice;
		}

		public void operate() {
			System.out.printf("number1 : %d", number1).println();
			System.out.printf("number2 : %d", number2).println();
			System.out.printf("choice : %d", choice).println();
			
			if(choice == 1) {
				System.out.printf("result : %d", number1 + number2).println();
			} else if(choice == 2) {
				System.out.printf("result : %d", number1 - number2).println();
			} else if(choice == 3) {
				System.out.printf("result : %d", number1 * number2).println();
			} else if(choice == 4) {
				System.out.printf("result : %d", number1 / number2).println();
			} else {
				System.out.println("Invalid Operation");
			}
		}
	}

```


**_Console Output_**

_number1 : 5_

_number2 : 2_

_choice : 1_

_result : 7_

Next in line, is an example involving a ```switch```.

##### Snippet-02 : Formatted Output Using ```switch```

**_OperatorChoiceRunner.java_**

```java

	package com.in28minutes.ifstatement.examples;

	public class OperatorChoiceRunner {
		public static void main(String[] args) {
			OperatorChoice opChoice = new OperatorChoice(5, 2, 1);
			opChoice.operateUsingSwitch();
		}
	}

```

**_OperatorChoice.java_**

```java

	package com.in28minutes.ifstatement.examples;

	public class OperatorChoice {
		private int number1;
		private int number2;
		private int choice;

		public OperatorChoice(int number1, int number2, int choice) {
			this.number1 = number1;
			this.number2= number2;
			this.choice = choice;
		}

		public void operateUsingSwitch() {
			System.out.printf("number1 : %d", number1).println();
			System.out.printf("number2 : %d", number2).println();
			System.out.printf("choice : %d", choice).println();

			switch(choice) {
				case 1: System.out.printf("result : %d", number1 + number2).println(); 
					break;
				case 2: System.out.printf("result : %d", number1 - number2).println(); 
					break;
				case 3: System.out.printf("result : %d", number1 * number2).println(); 
					break;				
				case 4: System.out.printf("result : %d", number1 / number2).println(); 
					break;
				default: System.out.printf("result : %d", number1 + number2).println(); 
					break;
			}
		}
	}

```

**_Console Output_**

_number1 : 5_

_number2 : 2_

_choice : 1_

_result : 7_

#### Summary

In this step, we:

* Observed that the same conditional code could be written using an ```if```-family conditional, or the ```switch```.
* Learned that an ```if``` family conditional is difficult to get wrong, as the rules for it are very strict. It can be used to evaluate only ```boolean``` conditions. But it is verbose, and often less readable.
* Came to know that a ```switch``` conditional can be used to check for only integer values. It is very compact, and very readable. However, the relative order of ```case``` clauses and ```default``` are not fixed, and the usage of ```break``` is optional. This can lead to subtle errors in your program. 

### Step 10: Programming Exercise PE-03

1. Write a Java ```class``` which has the following operations within it:
	* Given a number between 0 (Sunday) and 6 (Saturday), return if the day is a Weekday
	* Given a number between 1 (January) and 12 (December), return the corresponding English name for that month
	* Given a number between 1 (January) and 12 (December), return the corresponding English name for that day of the week

#### Solution to PE-03

**_CalendarSwitchRunner.java_**

```java

	package com.in28minutes.ifstatement.examples;

	public class CalendarSwitchRunner {
		public static void main(String[] args) {
			System.out.println(determineNameOfDay(1));
			System.out.println(isWeekDay(1));
			System.out.println(determineMonthOfYear(1));
		}

		public String determineNameOfDay(int dayNumber) {
			switch(dayNumber) {
				case 0 : return "Sunday";
					break;				
				case 1 : return "Monday";
					break;					
				case 2 : return "Tuesday";
					break;
				case 3 : return "Wednesday";
					break;
				case 4 : return "Thursday";
					break;
				case 5 : return "Friday";
					break;
				case 6 : return "Saturday";
					break;
				default : return "Invalid Day";
					break;
			}
		}

		public String determinenameofMonth(int monthNumber) {
			switch(monthNumber) {
				case 1 : return "January";
				case 2 : return "February";
				case 3 : return "March";
				case 4 : return "April";
				case 5 : return "May";
				case 6 : return "June";
				case 7 : return "July";
				case 8 : return "August";
				case 9 : return "September";
				case 10 : return "October";
				case 11 : return "November";
				case 12 : return "December";
				default : return "Invalid Month";
			}
		}

		public boolean isWeekDay(int dayNumber) {
			switch(dayNumber) {
				case 1 : 
				case 2 : 
				case 3 : 	
				case 4 : 
				case 5 : return true;
				case 0 :
				case 6 : 
				default : return false;
			}
		}
	}

```

### Step 12: Introducing ```?:```, The Ternary Operator
- - - 

The ternary operator ```?:``` is a logical operator, that works on three operands. Its functioning is similar to an ```if```-```else``` statement (Checking for just ```2``` conditions). Exactly one  of the two expressions is guaranteed to match.

Conceptually, its syntax is this:

*```result = (condition ? expression-if-condition-true : expression:if-condition-false);```* 

##### Snippet-01 : ternary operator 

`?:` is easy to use. A few examples below:

```java

	jshell> boolean isEven;
	isEven ==> false
	jshell> int i = 6;
	jshell> isEven = ( i%2==0 ? true : false);
	isEven ==> true
	jshell> i = 7;
	i ==> 7
	jshell> isEven = ( i%2==0 ? true : false);
	isEven ==> false
```

You can return non boolean values.
```java
	jshell> String ifEven = ( i%2==0 ? "YES" : "NO");
	ifEven ==> "NO"
	jshell> i = 6;
	i ==> 6
	jshell> ifEven = ( i%2==0 ? "YES" : "NO");
	ifEven ==> "YES"
```

Both the expressions should return value of same type.

```java
	jshell> ifEven = ( i%2==0 ? "YES" : 4 );
	| Error:
	| incompatible types: bad type in conditional expression
	| int cannot be converted to java.lang.String
	| ifEven = ( i%2==0 ? "YES" : 4 );
	|_____________________________^
	jshell> ifEven = ( i%2==0 ? "YES" : true );
	| Error:
	| incompatible types: bad type in conditional expression
	| boolean cannot be converted to java.lang.String
	| ifEven = ( i%2==0 ? "YES" : true );
	|_____________________________^
	jshell>

```


#### Summary

In this step, we:

* Discovered a more compact Java conditional, the ```?:``` operator
* Saw that in most cases it behaves like an ```if```-```else``` construct

## Loops

TODO 

### Revisiting Java loop constructs: ```for``` and ```while```

If you may recall, the structure of a ```for``` loop is:

```for(initialization; condition; update) {```

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;```//<Statements Body>```

```}``` 

The ```<Statements Body>``` inside the loop is executed so long as the ```condition``` is ```true```. Let's look at a few puzzles to explore how we can utilize them.
##### Snippet 1 : First for loop puzzle

**jshell>**```for(int i=0; i <= 10; i++) {```

__**...>>**```System.out.print(i + " ");```

__**...>>**```}```

_0 1 2 3 4 5 6 7 8 9 10_

**jshell>**```for(int i=0; i <= 10; i = i+2) {```

__**...>>**```System.out.print(i + " ");```

__**...>>**```}```

_0 2 4 6 8 10_

**jshell>**```for(int i=1; i <= 10; i = i+2) {```

__**...>>**```System.out.print(i + " ");```

__**...>>**```}```

_1 3 5 7 9_


**jshell>**```for(int i=11; i <= 10; i = i+2) {```

__**...>>**```System.out.print(i + " ");```

__**...>>**```}```


**jshell>**```for(int i=11; i <= 20;) {```

__**...>>**```System.out.print(i + " ");```

__**...>>**```i++;```

__**...>>**```}```

_11 12 13 14 15 16 17 18 19 20_

**jshell>**```int i = 20;```

_i ==> 20_

**jshell>**```for(i <= 30; i++) {```

__**...>>**```System.out.print(i + " ");```

__**...>>**```}```

_21 22 23 24 25 26 27 28 29 30_

**jshell>**

##### Snippet-1 Explained

All the three control components of a ```for``` loop are dispensable

* ```initialziation```
* ```condition```
* ```update```
- - -

## Reference Types

### Step 01: Introducing Reference Types

What happens in the background when we create objects?

```java

	jshell> class Planet {
	..>>}
	| created class Planet
	jshell> Planet jupiter = new Planet();
	jupiter ==> Planet@31a5c39e
```

Where is the object `jupiter` stored?

All Java objects are created on the `Heap` or `Heap Memory`. 

When we create an new instance of `Planet', it is created on the Heap.


```java
	jshell> new Planet()
	$18 ==> Planet@3f49dace
```

`new Planet()` creates an object on the Heap. In above example `Planet@3f49dace`, the object is stored on the Heap at address `3f49dace`.


```java
	jshell> Planet jupiter = new Planet();
	jupiter ==> Planet@31a5c39e
```

`Planet jupiter = new Planet()` does two things.
- Creates an object on the Heap `new Planet()`. In above example, object is created at Heap location `31a5c39e`
- Stores the reference of the object on the Heap in a variable `jupiter`. In above example, `31a5c39e` is the value stored in variable `jupiter`. That's the memory location where the new object was created.

Let's consider another example.

```java
	jshell> class Animal {
	   ..>> int id;
	   ..>> public Animal(int id) {
	   ..>> this.id = id;
	   ..>> }
	   ..>> }
	| created class Animal
	jshell> Animal dog = new Animal(12);
	dog ==> Animal@27c20538
	jshell> Animal cat = new Animal(15);
	cat ==> Animal@6e06451e
	jshell>

```

Two new `Animal` objects are created on the `Heap`. Their memory locations (`references`) are stored in the reference variables - `dog` and `cat`.

In Java, all classes are also called Reference Types. Except for primitive variable instances, all the instances or objects are stored on the Heap. The references to the objects are stored in the reference variables like `jupiter`, `dog` and `cat`.

#### Summary

In this step, we:

* Looked at what references are
* Had a look at what the contents of a reference variable look like

### Step 02: References: Usage And Puzzles

Let's spend some time playing with reference variables.

References that are not initialized by the programmer, are initialized by the Java compiler to ```null```. ```null``` is a special value that stands for an **empty location**. In other words, the ```Animal``` ```nothing``` refers to nothing!

```java

	jshell> class Animal {
	   ..>> int id;
	   ..>> public Animal(int id) {
	   ..>> this.id = id;
	   ..>> }
	   ..>> };
	| created class Animal
	jshell> Animal nothing;
	nothing ==> null

```

Assigning the reference ```cat``` to ```nothing``` does what one would expect: it assigns the address of the object created with ```new Animal(15)``` (stored in ```cat```), to the variable ```nothing```.

```java
	jshell> Animal dog = new Animal(12);
	dog ==> Animal@27c20538
	jshell> Animal cat = new Animal(15);
	cat ==> Animal@6e06451e_

	jshell> nothing = cat;
	nothing ==> 6e06451e
```

`nothing` and `cat` are pointing to the same location on the 'Heap'. When we do `nothing.id = 10` we are changing the `id` of the object pointed to by both `nothing` and `cat`.

```java
	jshell> nothing.id = 10;
	$1 => 10
	jshell> cat.id
	$2 => 10
```

Let's change `nothing` to point to the same object referenced by `dog`.

```java
	jshell> nothing = dog;
	dog ==> 27c20538
	jshell> nothing.id;
	$3 => 12
	jshell>

```

You can `nothing.id` prints the value of the object referenced by `dog` because they are pointing to the same object.

Here are couple of important things to note:

* `nothing = dog` - Assignment between references does not copy the entire referenced object. It only copies the reference. After an assignment, both reference variables point to the same object. 
* `nothing.id = 10` - References can be used to modify the objects they reference.

#### Comparing Reference Variables

Let's look at an example.

With primitive variables, assignment copies values.

```java

	jshell> int i =5;
	i ==> 5
	jshell> int j;
	j ==> 0
	jshell> j = i;
	j ==> 5
	jshell> j = 6;
	j ==> 6
	jshell> i;
	i ==> 5
```
`j = i` copies the value of `i` into `j`. Later, when value of `j` is changed, `i` is not affected.

Comparing primitive variables compares their values.

```java
	jshell> i == j;
	$4 ==> false
	jshell> j = 5;
	j ==> 5
	jshell> i == j;
	$5 ==> true
```


Let's create a few reference variables.

```java
	jshell> Animal dog = new Animal(12);
	dog ==> Animal@4b952a2d
	jshell> Animal cat = new Animal(10);
	cat ==> Animal@3159c4b8
	jshell> Animal ref = cat;
	ref ==> Animal@3159c4b8
	jshell> Animal dog2 = new Animal(12);
	dog ==> Animal@29ca901e_
```

When we compare reference variables, we are still comparing values. But the values are references - the address of memory locations where objects are stored. The values stored inside the referenced objects are not used for comparison.

Both ```cat``` and ```ref``` reference a single ```Animal``` object created using ```new Animal(10)```. `==` returns true
```java
	jshell> cat == dog;
	$6 ==> false
	jshell> cat == ref;
	$7 ==> true
```

The comparison ```dog == dog2``` evaluates to ```false``` since the references i.e. memory locations pointed by these variables are different. They have the same values for ```id``` field (```12```). But, that is not important!

```java
	jshell> dog == dog2;
	$8 ==> false
	jshell>

```



#### Summary

In this step, we:

* Understood the way reference variables behave during initialization and assignment
* Saw the relevance of a ```null``` value for references
* Observed how equality of references, is different from equality of values of primitive types

### Step 03: Introducing ```String```

A sequence of characters, such as ```"Hello"```, ```"qwerty"``` and ```"PDF"``` is very different from other pieces of data. 

In Java, a sequence of characters is typically represented by ```String``` ```class```.

```String``` provides several built-in utility methods. 

Let's look at a few examples.

```java

	jshell> "Test".length()
	$1 ==> 4
```
```"Test"``` is a string literal, so the compiler internally creates an object, gives it the type ```String``` and allocates memory for it. Since ```length()``` is a method of ```String```, it can be invoked on this ```"Test"``` object.



In the example below, ```str``` is a reference to a ```String``` object, containing the value ```"Test"```. Creating a ```String``` object is an exception to how we typically create objects in Java. You don't need to make a ```String``` constructor call. Contrast this with how we would create a ```BigDecimal``` object.
```java
	jshell> String str = "Test";
	str ==> "Test"
	jshell> BigDecimal bd = new BigDecimal("1.0");
	bd ==> 1.0
```

String indexes, like those of arrays, start at ```0```. The ```charAt(int)``` method takes an index value as its argument, and returns the character symbol present at that index.

```java
	jshell> str.charAt(0)
	$2 ==> 'T'
	jshell> str.charAt(2)
	$3 ==> 's'
	jshell> str.charAt(3)
	$4 ==> 't'
```
The ```substring()``` method returns a ```String``` reference, and has overloaded versions:
* The ```substring(int, int)``` method returns the sequence of character symbols starting at the lower index, and ending just before the upper index. 
* The ```substring(int)``` method returns the sequence of character symbols starting from the index to end of string.

```java
	jshell> String biggerString = "This is a lot of text";
	biggerString ==> "This is a lot of text"
	jshell> biggerString.substring(5)
	$5 ==> "is a lot of text"
	jshell> biggerString.substring(5, 13)
	$6 ==> "is a lot"
	jshell> biggerString.charAt(13)
	$7 ==> ' '
	jshell>
	
```


#### Summary

In this step, we:

* Were introduced to the ```String``` class, that represents sequences of characters
* Explored a few utility methods of the ```String``` class

### Step 04: Programming Exercise PE-01, And ```String``` Utilities

#### Exercise

1. Write a method to print the individual characters of a given text string, separately.

#### Solution To PE-01

```java

	jshell> String text = "Equation";
	   ..>> for (int i=0; i < text.length(); i++) {
	   ..>> System.out.println(text.charAt(i));
	   ..>> }
	E
	q
	u
	a
	t
	i
	o
	n
	jshell>
	
```

#### Common ```String``` Utilities

The ```String``` class is part of the built-in ```java.lang``` package. It provides several methods for common text processing. Let's have a peek at some of them, shall we? 

##### Snippet-01: ```String``` Utilities 


Here are a few of the methods used in the examples below:
* ```indexOf()``` : Has two overloaded versions. ```indexOf(char)``` returns the position where a character occurs in a string, the first time. ```indexOf(String)``` returns the starting position where a string occurs within our string, the first time.
* ```lastIndexOf()``` : Similar in function to ```indexOf()```, but replace "*first time*" with "**final time**" in its description.
* ```startsWith()``` : Returns ```true``` if our string starts with the given *prefix*, ```false``` otherwise.
* ```endsWith()``` : Returns ```true``` if our string ends with the given *suffix*, ```false``` otherwise.
* ```isEmpty()``` : Returns ```true``` if our string is empty, ```false``` otherwise.
* ```equals()``` : Returns ```true``` if our string is identical to the argument, ```false``` otherwise.
* ```equalsIgnoreCase()``` : Returns ```true``` if our string is identical to the argument, ignoring the case of its characters. Will return ```false``` otherwise.

```java

	jshell> String someString = "This is a lot of text again";
	someString ==> "This is a lot of text again"
	jshell> someString.indexOf("lot")
	$1 ==> 10
	jshell> someString.charAt(10)
	$2 ==> 'l'
	jshell> someString.indexOf('i')
	$3 ==> 2
	jshell> someString.lastIndexOf('i')
	$4 ==> 25
	jshell> someString.contains("text")
	$5 ==> true
	jshell> someString.startsWith("This")
	$6 ==> true
	jshell> someString.startsWith("jfsdklfj")
	$7 ==> false
	jshell> someString.endsWith("in")
	$7 ==> true
	jshell> someString.endsWith("ain")
	$8 ==> true
	jshell> someString.endsWith("gain")
	$9 ==> true
	jshell> someString.endsWith("againasdf")
	$10 ==> false
	jshell> someString.isEmpty()
	$11 ==> false
	jshell> "".isEmpty()
	$12 ==> true
	jshell> "true".equals("true")
	$13 ==> true
	jshell> String str = "value";
	str ==> "value"
	jshell> str.equals("value")
	$14 ==> true
	jshell> str.equals("VALUE")
	$15 ==> false
	jshell> str.equalsIgnoreCase("VALUE")
	$16 ==> true
	jshell>

```


#### Summary

In this step, we:

* Used our ```String``` programming skills on a small challenge.
* Explored a set of simple, yet useful ```String``` utilities.

### Step 05: ```String``` Immutability

What picture forms in your mind on hearing the word "**immutable**"? Someone whose voice cannot be muted out? Or is it the other way round? 

The word "immutable" is related to the concept of "mutability", or the possibility of "mutating" something. 

"**mutate**" means "**to change**". "Immutable" refers to something that "**cannot be changed**". 

```String``` objects are immutable. You cannot change their value after they are created.

The method ```concat()```joins the contents of two ```String``` objects into one. 

```java

	jshell> String str = "in28Minutes";
	str ==> "in28Minutes"
	jshell> str.concat(" is awesome")
	$1 ==> "in28Minutes is awesome"
```

However, the original value referred by `str` remains unchanged. The `concat` method create a new `String` object.

```
	jshell> str
	str ==> "in28Minutes"
```

Just like ```concat()```, other ```String``` methods such as ```toUpperCase()```, ```toLowerCase()``` and ```trim()``` return new ```String``` objects.

```java

	jshell> String anotherString = str.concat(" is awesome");
	anotherString ==> "in28Minutes is awesome"
	jshell> str
	str ==> "in28Minutes"
	jshell> String string2 = anotherString.concat(".");
	string2 ==> "in28Minutes is awesome."
	jshell> str
	str ==> "in28Minutes"
	jshell> anotherString
	anotherString ==> "in28Minutes is awesome"
	jshell> String s= "in28Minutes is awesome."
	s ==> "in28Minutes is awesome."
	jshell> s.toUpperCase()
	s ==> "IN28MINUTES IS AWESOME."
	jshell> s.toLowerCase()"
	s ==> "in28minutes is awesome."
	jshell> String str2= "  in28Minutes is awesome    "
	str2 ==> "  in28Minutes is awesome    "
	jshell> str2.trim()
	str2 ==> "in28Minutes is awesome"
	jshell>

```

#### Summary

In this step, we:

* We understood that ```String``` objects are immutable
* Observed how common ```String``` utilities return a new String. 

### Step 06:  More ```String``` Utilities

The symbol ```+``` denotes addition, and addition only, right? Any school kid will tell you that, or laugh at you if you disagree. 

Heck, we even saw how to use it with the primitive numeric types, such as ```int```, ```double``` and others related to it.

Java does not strictly follow your arithmetic text book. 

```+``` can also be used as a ```String``` concatenation operator.

Here is how ```+``` works
* if both operands of ```+``` are numeric,  then arithmetic ```+``` (addition) is performed.
* If any one of the operators is a ```String```, then string concatenation is performed.


```java

	jshell> 1 + 2
	$1 ==> 3
	jshell> "1" + "2"
	$2 ==> "12"
	jshell> "1" + 2
	$3 ==> "12"
	jshell> "1" + 23
	$4 ==> "123"
	jshell> 1 + 23
	$5 ==> 24
	jshell> "1" + 2 + 3
	$6 ==> "123"
	jshell> 1 + 2 + "3"
	$7 ==> "33"
```

In the example below, a different value is printed when parentheses are used around `i + 20`.

```java
	jshell> int i = 20;
	i ==> 20
	jshell> System.out.println("Value is " + i);
	Value is 20
	jshell> System.out.println("Value is " + i + 20);
	Value is 2020
	jshell> System.out.println("Value is " + (i + 20));
	Value is 40
```

```join()``` is used to join a set of `String` values.

```java
	jshell> String.join(",", "2", "3", "4");
	$8 ==> "2,3,4"
```

```replace(String, String)```replaces all occurrences of the first sub-string with the second one. It also works with `char` data type.

```java
	jshell> "abcd".replace('a', 'z');
	$9 ==> "zbcd"
	jshell> "abcd".replace("ab", "xyz");
	$10 ==> "xyzcd"
	jshell>

```


#### Summary

In this step, we:

* Learned that the ```+``` operator is overloaded for ```String``` concatenation
* Observed how ```+``` interprets its operands, depending on the context
* Noticed a few more ```String``` utility methods, such as ```join()``` and ```replace()```

### Step 07: Storing mutable text

```StringBuffer``` and ```StringBuilder``` allow you to modify a string literal in-place. 

```java

	jshell> "123" + "123" + "1234" + "12345"
	$1 ==> "123123123412345"
	jshell> StringBuffer sb = new StringBuffer("TEst");
	sb ==> "TEst"
	jshell> sb.append(" 123");
	$2 ==> "TEst 123"
	jshell> sb
	sb ==> "TEst 123"
	jshell> sb.setCharAt(1, 'e');
	sb ==> "Test 123"
	jshell> StringBuilder sbldr = new StringBuffer("TEst");
	sbldr ==> "TEst"
	jshell>

```
How do you choose which one to use?
* `StringBuffer` is thread safe. If you are writing a multi threaded program(more on this in a later section), use ```StringBuffer```.
* Otherwise, use ```StringBuilder```, since it offers better performance in both execution-time and memory usage.

#### Summary

In this step, we:

* Learned about ```StringBuffer``` and ```StringBuilder```

### Step 08: Introducing Wrapper Classes

Each primitive type in Java has a corresponding built-in **wrapper class**. Wrapper classes are also immutable (As well as ```final```, more on this a little later). 

Following is a list of built-in Java wrapper classes and their corresponding primitive types:
* ```byte``` : ```Byte```
* ```short``` : ```Short```
* ```int``` : ```Integer```
* ```long``` : ```Long```
* ```float``` : ```Float```
* ```double``` : ```Double```
* ```char``` : ```Character```
* ```boolean``` : ```Boolean```

The main incentives of using such wrappers in your code, are:
* Accessing type information about the corresponding primitive type
* Auto-Boxing feature, where a primitive data is automatically promoted to an object  reference type
* Moving primitive type data around data structures (called *collections*), using their wrapper-style counterparts

Let's look at these incentives in the next step.

#### Summary

In this step, we:

* Were introduced to the wrapper classes available for the primitive types
* Learned about the advantages of having them around

### Step 09: Creating Wrapper Objects

Now that we know what wrapper classes are, and which ones correspond to each primitive Java type, let's try them out.

Creating instance of Wrapper Classes using `new` is simple. Examples below.

```java

	Integer hundred = new Integer("100");
	Boolean b1 = new Boolean("true"); //true
	Boolean b1 = new Boolean("True"); //true
	Boolean b1 = new Boolean("false"); //false
	Boolean b1 = new Boolean("False"); //false
	Boolean b1 = new Boolean("other arbitrary string"); //false

```

You can also use ```valueOf()``` method within types such as ```Integer``` and ```Float``` to create a wrapper object. 

```java

	Float floatWrapper = Float.valueOf(57.0f);
	int floatToInt = floatWrapper.intValue(); // 57
	Integer seven = Integer.valueOf("111", 2);
	Integer.toString(seven, 2);

```

#### Difference between creating wrapper objects using valueOf and new

The ```Integer.valueOf()``` reuses existing ```Integer``` objects with same value on the heap. If an object with same value is present in the heap, it returns a reference to existing object. Otherwise, it returns a reference of a newly created ```Integer``` object.

Wrapper classes are immutable. Hence, above approach is efficient and accurate.

```java

	jshell> Integer integer1 = new Integer(5);
	integer1 ==> 5
	jshell> Integer integer2 = new Integer(5);
	integer2 ==> 5
	jshell> Integer integer3 = Integer.valueOf(5);
	integer3 ==> 5
	jshell> Integer integer4 = Integer.valueOf(5);
	integer4 ==> 5
	jshell> integer1 == integer2
	$1 ==> true
	jshell> integer3 == integer4
	$2 ==> true
	jshell>

```
#### Summary 

In this step, we:

* Discovered that there are two ways to create a wrapper object for primitive data
* Learned that ```valueOf()``` takes advantage of immutability, to improve efficiency

### Step 10: Auto-Boxing, And Some Wrapper Constants

**Auto-Boxing** is an example of **syntactic sugar** in the Java language. It does not provide new features but makes code more readable. 

Auto-boxing reuses the mechanism provided by ```Integer.valueOf()``` for ```Integer```, ```Float``` and others.



```java

	jshell> Integer seven = Integer.valueOf(7000);
	seven ==> 7000
	jshell> Integer sevenToo = 7000;
	sevenToo ==> 7000
	jshell> Integer sevenAgain = 7000;
	sevenAgain ==> 7000
	jshell> sevenToo == sevenAgain
	$1 ==> true
```

In the above example, 	`Integer sevenToo = 7000` uses auto boxing. We are upgrading a `int` literal to a `Integer` value. This is done implicitly by using `Integer.valueOf` method.

There are constants available on Wrapper classes print the size of their variables and the range of values they can store.

```
	jshell> Integer.MAX_VALUE
	$2 ==> 2147483647
	jshell> Integer.MIN_VALUE
	$3 ==> -2147483648
	jshell> Integer.SIZE
	$4 ==> 32
	jshell> Integer.BYTES
	$5 ==> 4
	jshell>

```


#### Summary

In this step, we:

* Understood the mechanism of auto-boxing, which uses the assignment operator route
* Understood how auto-boxing internally makes use of ```valueOf()``` method

### Step 11: The Java ```Date``` API

No  discussion on the built-in Java primitive and reference types is complete without an exploration of the Date API. 

Before Java SE 8, there were a lot of practical issues regarding the interface and implementation of the ```Date``` class.

From Java 8, Java provided an API for `Date` classes based on the Joda Date Framework. 

The three most significant classes within this framework are : ```LocalDate```, ```LocalTime``` and ```LocalDateTime```. 

##### Snippet-01 : java.time utilities

```java.time.*``` is not imported automatically by Jshell.  Let's import it in. 

The commonly used utilities to access current values of date and time are:
* ```LocalDate.now()``` : Returns the current date value in readable format
* ```LocalTime.now()``` : Returns the current time value in a readable format
* ```LocalDateTime.now()``` : Returns a combination of the current date and time values, in a readable format   

```java

	jshell> import java.time.LocalDate
	jshell> LocalDate now = LocalDate.now()
	now ==> 2018-02-01
	jshell> import java.time.*
	jshell> LocalDateTime now = LocalDateTime.now()
	now ==> 2018-02-01T15:50:48.423164
	jshell> LocalTime now = LocalTime.now()
	now ==> 15:51:09.642001
	jshell>

```

#### Summary

In this step, we:

* Were introduced to the Java Date API, available through the ```java.time``` package
* Saw how to use the ```LocalDate```, ```LocalTime``` and ```LocalDateTime``` types

### Step 12: Playing With ```java.time.LocalDate```

We've been looking at calendars right from childhood, haven't we! How about playing around with a digital calendar? 

`LocalDate` provides a number of methods to retrieve 
* Date information: Day/Month/Year and related attributes
* Date meta-information: Classification-related information, such as whether a leap year, etc.


```java

	jshell> import java.time.*
	jshell> import java.time.*
	jshell> LocalDate today = LocalDate.now()
	today ==> 2018-02-01
	jshell> today.getYear()
	$1 ==> 2018
	jshell> today.getDayOfWeek()
	$2 ==> THURSDAY
	jshell> today.getDayOfMonth()
	$3 ==> 01
	jshell> today.getDayOfYear()
	$4 ==> 32
	jshell> today.getMonth()
	$5 ==> FEBRUARY
	jshell> today.getMonthValue()
	$6 ==> 2
	jshell> today.isLeapYear()
	$7 ==> false
	jshell> today.lengthOfYear()
	$8 ==> 365
	jshell> today.lengthOfMonth()
	$9 ==> 28
```

```LocalDate``` is also immutable. You can use different methods provided to add and subtract days, months and years. Each of these return a new instance of ```LocalDate```.

```java
	jshell> today.plusDays(100)
	$10 ==> 2018-05-12
	jshell> today.plusMonths(100)
	$11 ==> 2026-06-01
	jshell> today.plusYears(100)
	$12 ==> 2118-02-01
	jshell> today.minusYears(100)
	$13 ==> 1918-02-01
	jshell> LocalDate yesteryear = today.minusYears(100)
	yesterYear ==> 1918-02-01
	jshell> today
	today ==> 2018-02-01
	jshell>

```

```LocalDateTime``` extends ```LocalDate``` and provides time component as well. You can access, and perform arithmetic on the hours, minutes, seconds and nanoseconds values.

#### Summary

In this step, we:

* Saw common utilities that the ```LocalDate``` ```class``` provides
* Learned that ```LocalDate```, ```LocalTime``` and ```LocalDateTime``` are all immutable

### Step 13: Comparing ```LocalDate``` Objects

You can take a look at additional utility methods in ```LocalDate``` in examples below:

```java

	jshell> LocalDate today = LocalDate.now()
	today ==> 2018-02-01
	jshell> LocalDate yesterday = LocalDate.of(2018, 01, 31)
	yesterday ==> 2018-01-31
	jshell> today.withYear(2016)
	$1 ==> 2016-02-01
	jshell> today.withDayOfMonth(20)
	$2 ==> 2018-02-20
	jshell> today.withMonth(3)
	$3 ==> 2018-03-01
	jshell> today.withDayOfYear(3)
	$4 ==> 2018-04-30
```

You can also compare dates using the methods shown below:

```java
	jshell> today.isBefore(yesterday)
	$5 ==> false
	jshell> today.isAfter(yesterday)
	$6 ==> true
	jshell>
	
```

These methods are also available with ```LocalTime``` and ```LocalDateTime``` classes as well.

## Arrays and ArrayList

We will use the following exercise to understand heavily used data structures of Java - Arrays and 
`ArrayList`.

We would like to model a student report card in a Java program, which allows the user to do stuff such as:

```java

	Student student - new Student(name, list-of-marks);
	int number = student.getNumberOfmarks();
	int sum = student.getTotalSumOfMarks();
	int maximumMark = student.getMaximumMark();
	int minimumMark = student.getMinimumMark();
	BigDecimal average = student.getAverageMarks();
	student.addMark(35);
	student.removeMarkAtIndex(5);

```

A data structure like array and `ArrayList` allow you to store multiple object of the same kind. These are called **aggregates**. 


### Step 01: The Need For ```Array```

Let's start with understanding the need for arrays.

Consider the example below. We are creating 3 marks and adding them.

```java

	jshell> int mark1;
	mark1 ==> 0
	jshell> mark1 = 100;
	mark1 ==> 10
	jshell> int mark2 = 75;
	mark2 ==> 75
	jshell> int mark3 = 60;
	mark3 ==> 60
	jshell> int sum = mark1 + mark2 + mark3;
	sum ==> 235
	jshell> int mark4 =7 56;
	mark4 ==> 56
	jshell> sum = mark1 + mark2 + mark3 + mark4;
	sum ==> 291
	jshell>

```

If an additional mark component ```mark4``` is added to the existing list of marks ```mark1```, ```mark2``` and ```mark3```, the code for computing ```sum``` needs to change. 

All these marks are similar. How about creating a group of marks and storing it as part of single variable?

Let's create an array - `marks`

```java

	jshell> int[] marks = {75, 60, 56};
	marks ==> int[3]{ 75,60,56 }
```
In above example
* ```marks``` is an ```array```. 
* `marks` stores multiple ```int``` values.
* `marks` array has 3 values

In an array, the index runs from 0 to (length of array - 1). In above example, the index runs from 0 to 2. 

You can use an index to find the specific element from the array. It is done by using the indexing operator, '```[]```'. The expression ```marks[0]``` maps to the first array element stored at index ```0``` of the array ```marks```.


```java
jshell> marks[0]
$20 ==> 75

jshell> marks[1]
$21 ==> 60

jshell> marks[2]
$22 ==> 56
```

How do we write code to sum all values in marks array?

```java

	jshell> int sum = 0;
	sum ==> 0
	jshell> for(int mark:marks) {
	   ..>> sum = sum + mark;
	   ..>> }
	jshell> sum
	sum ==> 191
	jshell>

```

Above construct is called Enhanced ```for``` loop.

```mark``` is the loop control variable. Its type needs to match the type of an array elements, which is ```int```.

Above ```for``` loop can be used irrespective of the number of elements in `marks` array.

### Step 02:  Storing And Accessing Array Values

Let's dig deeper into arrays in this step.

An array can be used to store zero or more number of elements. 

```java

	jshell> int[] marks = {1, 2, 3 };
	marks ==> int[3]{ 1,2,3 }
	jshell> int[] marks = {1, 2, 3, 4, 5};
	marks ==> int[5]{ 1,2,3,4,5 }
	jshell> int[] marks = {1};
	marks ==> int[1]{ 1 }
	jshell> int[] marks = {};
	marks ==> int[0]{  }
```


An array can also be created with ```new``` operator. You've to specify the size of the array.
```java
	jshell> int[] marks2 = new int[5];
	marks2 ==> int[5]{ 0,0,0,0,0 }
```

You can use array index to assign values. 

`marks2[0] = 10` stores `10` as first element in marks array.


```java
	jshell> marks2[0]
	$1 ==> 0
	jshell> marks2[0] = 10;
	$2 ==> 10
	jshell> marks2[0]
	$3 ==> 10
	jshell>

```
  
Snippet below shows more examples.

```java

	jshell> int[] marks2 = new int[5];
	marks2 ==> int[5]{ 0,0,0,0,0 }
	jshell> marks2[0] = 1;
	$1 ==> 1
	jshell> marks2[1] = 2;
	$2 ==> 2
	jshell> marks2[2] = 3;
	$3 ==> 3
	jshell> marks2[3] = 4;
	$4 ==> 4
	jshell> marks2[4] = 5;
	$5 ==> 5
	jshell> marks2
	marks2 ==> int[5]{ 1,2,3,4,5 }
```

`length` can be used to find the number of elements in the array.

```java
	jshell> marks2.length
	$6 ==> 5
	jshell> int marks3 = {};
	marks3 ==> int[0]{  }
	jshell> marks3.length
	$7 ==> 0
	
```
#### Classroom Exercise CE-AA-01

1. Write a program that creates an array ```marks``` to store 	```8``` ```int``` values, and code to iterate through ```marks``` using a ```for``` loop, printing out its values.

Hint: Use the ```marks.length``` property

#### Solution To CE-AA-01

```java

	jshell> int[] marks = {1, 2, 3, 4, 5, 6, 7, 8};
	marks ==> int[8]{ 1,2,3,4,5,6,7,8 }
	jshell> marks.length
	$1 ==> 8
	jshell> for(int i=0; i < marks.length; i++) {
	   ..>> System.out.println(marks[i]);
	   ..>> }
	1
	2
	3
	4
	5
	6
	7
	8
	jshell>

```

### Step 04: Array Initialization, Data Types And Exceptions

Below snippet shows how arrays with different types are initialized.

Summary - int - 0, double - 0.0, boolean - false, Any object - null

```java

	jshell> int[] marks = new int[5];
	marks ==> int[5]{ 0,0,0,0,0 }
	jshell> double[] values = new double[5];
	values ==> double[5]{ 0.0,0.0,0.0,0.0,0.0 }
	jshell> boolean[] tests = new boolean[5];
	tests ==> boolean[5]{ false,false,false,false,false }
	jshell> class Person {
	   ..>>}
	| created class Person
	jshell> Person[] persons = new Person[5];
	persons ==> Person[5]{ null,null,null,null,null }
	jshell>

```

Let's look at a few variations of array declarations.

Important things to Remember
* The declaration part of an array definition must not include the dimension of the array
* The assignment part of an array definition must include the dimension of the array
* All the elements of an array must be of the same, homogeneous type

```java

	jshell> int[5] marks2;
	| Error:
	| ']' expected
	| int[5] marks2;
	|____^
	jshell> int[] marks2 = new int[];
	| Error:
	| array dimension missing
	| int[] marks2 = new int[];
	|____________^========^
	jshell> int[] marks2 = new int[5];
	marks2 ==> int[5]{ 0,0,0,0,0 }
	jshell> marks2[6]
	| java.lang.ArrayIndexOutOfBoundsException thrown : 6
	| at (#54:1)
	jshell> int[] marks3 = {1, 2, 3, 4.0};
	| Error:
	| incompatible types: possible lossy conversion from double to int
	| int[] marks3 = {1, 2, 3, 4.0};
	|__________________________^-^ 
	jshell>

```

The name of an array is a reference variable that stores the address of where the array is created on the heap.
```java

	jshell> int[] marks4 = {1, 2, 3, 4, 5};
	marks4 ==> int[5]{ 1,2,3,4,5 }
	jshell> System.out.println(marks4);
	I@6c49835d
```

The built-in method ```Arrays.toString``` can be used to print out elements of an array.
```java
	jshell> System.out.println(Arrays.toString(marks));
	[1, 2, 3, 4, 5]
	jshell>

```

### Step 05: Array Utilities
- - - 

Let's look at a few examples for
* Iterating through An Array
* Bulk-modification of array elements
* Comparing Arrays
* Sorting Arrays

##### Snippet-01 : Iterating through an array

Using an enhanced ```for``` loop is easy and intutive.

```java

	jshell> int[] marks = {100, 99, 95, 96, 100};
	marks ==> int[5]{ 100,99,95,96,100 }
	jshell> for(int mark:marks) {
	..>> System.out.println(mark);
	..>> }
	100
	99
	95
	96
	100
	jshell> for(int i=0; i < marks.length; i++) {
	..>> System.out.println(marks[i]);
	..>> }
	100
	99
	95
	96
	100
	jshell>

```

##### Snippet-02 : Filling & Comparing Arrays

```Array.fill``` fills the entire array with a specified value.

```java

	jshell> int[] marks = new int[5];
	marks ==> int[5]{ 0,0,0,0,0 }
	jshell> Arrays.fill(marks, 100);
	jshell> marks
	marks ==> int[5]{ 100,100,100,100,100 }
```

```Array.equals``` compares two given arrays, and returns a ```boolean``` value of```true``` only if
* Both arrays are of same length and
* Elements at each corresponding index are equal, for all indexes


```java
	jshell> int[] array1 = {1, 2, 3};
	array1 ==> int[3]{ 1,2,3 }
	jshell> int[] array2 = {1, 2, 3};
	array2 ==> int[3]{ 1,2,3 }

	jshell> Arrays.equals(array1, array2);
	$1 ==> true

	jshell> int[] array3 = {3, 2, 3};
	array3 ==> int[3]{ 3,2,3 }
	jshell> Arrays.equals(array1, array3);
	$2 ==> false

	jshell> int[] array4 = {1, 2};
	array4 ==> int[2]{ 1,2 }
	jshell> Arrays.equals(array1, array4);
	$3 ==> false
```

```Array.sort```: Performs an in-position sorting of elements by comparing pairs of them at a time.
```java
	jshell> Arrays.sort(array3);
	jshell> array3
	array3 ==> int[3]{ 2,3,3 }
	jshell>

```

### Step 06: Classroom Exercise  CE-AA-02

#### Exercise

Armed with the knowledge of Java arrays and their in-built utility methods, let's now solve the challenge we started off with. 

```java

	Student student - new Student(name, list-of-marks);
	int number = student.getNumberOfmarks();
	int sum = student.getTotalSumOfMarks();
	int maximumMark = student.getMaximumMark();
	int minimumMark = student.getMinimumMark();
	BigDecimal average = student.getAverageMarks();

```

We can implement the aggregate ```list-of-marks``` as an array.

#### Solution To CE-AA-02

**_StudentRunner.java_**

```java

	package com.in28minutes.arrays;

	public class StudentRunner {
		public static void main(String[] args) {
			int[] marks = {99, 98, 100};
			Student student = new Student("Ranga", marks);
	
			int number = student.getNumberOfmarks();		
			System.out.println("Number of marks : " + number);	
			int sum = student.getTotalSumOfMarks();
			System.out.println("Sum of marks : " + sum);
	
			int maximumMark = student.getMaximumMark();
			System.out.println("Maximum of marks : " + maximumMark);
			int minimumMark = student.getMinimumMark();
			System.out.println("Minimum of marks : " + minimumMark);
	
			BigDecimal average = student.getAverageMarks();
			System.out.println("Average of marks : " + average);
			student.addMark(35);
			student.removeMarkAtIndex(5);
		}
	}

```

**_Student.java_**

```java

	package com.in28minutes.arrays;
	import java.math.BigDecimal;

	public class Student {
		private String name;
		private int[] marks;

		public Student(String name, int[] marks) {
			this.name = name;
			this.marks = marks;
		}

		public int getNumberOfMarks() {
			return marks.length;
		}

		public int getTotalSumOfMarks() {
			int sum = 0;
			for(int mark:marks) {
				sum += mark;
			}
			return sum;
		}

		public BigDecimal getAverageOfMarks() {
			int sum = getTotalSumOfMarks();
			BigDecimal average = new BigDecimal(sum).divide(new BigDecimal(marks.length), 3, RoundingMode.UP);
		}

		public int getMaximumMark() {
			int max = Integer.MIN_VALUE;
			for(int mark:marks) {
				if(mark > max) {
					max = mark;				
				}
			}
			return max;
		}

		public int getMinimumMark() {	
			int min = Integer.MAX_VALUE;
			for(int mark:marks) {
				if(mark < min) {
					min = mark;
				}
			}
			return min;
		}
	}

```
### Step 08:  Variable Arguments - The Basics

What if you want to create a method which can accept variable number of arguments?

Let's look at an example. The critical part is the parameter `int... values`.

```java

	jshell> class Something {
	   ..>> public void doSomething(int... values) {
	   ..>> System.out.println(Arrays.toString(values));
	   ..>> }
	   ..>> };
	| created class Something
```

A typical parameter would've been `int values`. This allows us to pass one parameter to the method.

What difference does the three dots `...` make in `int... values`?

```java
	jshell> Something thing = new Something();
	thing ==> Something@2e465f6a
	jshell> thing.doSomething(1);
	[1]
	jshell> thing.doSomething(1, 2);
	[1, 2]
	jshell> thing.doSomething(1, 2, 3);
	[1, 2, 3]
	jshell>

```

You can see that `doSomething` can be called with one, two and three parameters. 

Let's look at another example:

```java

	jshell> void sum(int... values) {
	   ..>>   int sum = 0;
	   ..>>   for(value: values) {
	   ..>>     sum += value;
	   ..>>   }
	   ..>>   System.out.println(sum);
	   ..>> }
	| created method sum(int...)
```

We created a `sum` method with a variable argument. Let's look at how to use it.

```java
	jshell> sum(1, 2)
	3
	jshell> sum(1, 2, 3)
	6
	jshell> sum(1, 2, 3, 4)
	1
	jshell> sum(1, 2, 3, 4, 5, 6)
	21
	jshell>

```

In this step, we took our first look at variable arguments. Variable arguments allow us to pass variable number of arguments to a method.

### Step 09: Variable Argument Methods For ```Student``` 

Let's add a few methods to the `Student` class to accept variable arguments.

**_Student.java_**

```java

	package com.in28minutes.arrays;
	import java.math.BigDecimal;

	public class Student {
		private String name;
		private int[] marks;

		public Student(String name, int...  marks) {
			this.name = name;
			this.marks = marks;
		}

		public int getNumberOfMarks() {
			return marks.length;
		}

		public int getTotalSumOfMarks() {
			int sum = 0;
			for(int mark:marks) {
				sum += mark;
			}
			return sum;
		}

		public BigDecimal getAverageOfMarks() {
			int sum = getTotalSumOfMarks();
			BigDecimal average = new BigDecimal(sum).divide(new BigDecimal(marks.length), 3, RoundingMode.UP);
		}

		public int getMaximumMark() {
			int max = Integer.MIN_VALUE;
			for(int mark:marks) {
				if(mark > max) {
					max = mark;
				}
			}
			return max;
		}

		public int getMinimumMark() {
			int min = Integer.MAX_VALUE;
			for(int mark:marks) {
				if(mark < min) {
					min = mark;
				}
			}
			return min;
		}
	}

```

**_StudentRunner.java_**

```java

	package com.in28minutes.arrays;
	public class StudentRunner {
		public static void main(String[] args) {
			//int[] marks = {99, 98, 100};
			Student student = new Student("Ranga", 97, 98, 100);

			int number = student.getNumberOfmarks();
			System.out.println("Number of marks : " + number);
			int sum = student.getTotalSumOfMarks();
			System.out.println("Sum of marks : " + sum);

			int maximumMark = student.getMaximumMark();
			System.out.println("Maximum of marks : " + maximumMark);
			int minimumMark = student.getMinimumMark();
			System.out.println("Minimum of marks : " + minimumMark);
			BigDecimal average = student.getAverageMarks();
			System.out.println("Average of marks : " + average);

			student.addMark(35);
			student.removeMarkAtIndex(5);
		}
	}

```

#### Quick Tip

The variable arguments list must always be at the end of the parameter list passed to a method. The following method definition **will not** be accepted by the Java compiler:

```java

	void process(int... values, String name) {

	}

```

- - - 
### Step 10: Arrays - Some Puzzles And Exercises 

Let's look at a few puzzles and exercises with Arrays.

When creating arrays of objects, the array ends up holding references to the created objects.

```java

	jshell> class Person {
	   ..>> }
	| created class Person
	jshell> Person[] persons = new Person[5];
	persons ==> Person[5]{ null,null,null,null,null }
```

We can assign new `Person` objects to different elements of the array.

```java
	jshell> persons[1] = new Person();
	$1 ==> Person@394e1a0f
	jshell> persons
	persons ==> Person[5]{ null,Person@394e1a0f,null,null,null }
	jshell> persons[0] = new Person();
	$2 ==> Person@1e965684
	jshell> persons
	persons ==> Person[5]{ Person@1e965684,Person@394e1a0f, null,null,null }
```

You can also initialize values when you create an array.

```java
	jshell> Person[] persons2 = {new Person(), new Person()};
	persons2 ==> Person[2]{ Person@3b088d51, Person@1786dec2 }
```

Here's how you can initialize a `String` array.

```java
	jshell> String[] textValues = {"Apple", "Ball", "Cat"};
	textValues ==> String[2]{ "Apple","Ball","Cat" }
	jshell>
	
```

#### Classroom Exercise CE-AA-03 

#### Exercises

1. Create a ```String``` array with the names of days of the week:

```Sunday```, ```Monday```, ```Tuesday```, ```Wednesday```, ```Thursday```, ```Friday```, ```Saturday```
2. Find the day with the most number of letters in it
3. Print days of the week backwards

#### Solutions To CE-AA-03

**_WeekRunner.java_**

```java

package com.in28minutes.arrays;

public class StringRunner {

	public static void main(String[] args) {

		String[] daysOfWeek = { "Sunday", "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday" };

		String dayWithMostCharacters = "";

		for (String day : daysOfWeek) {
			if (day.length() > dayWithMostCharacters.length()) {
				dayWithMostCharacters = day;
			}
		}

		System.out.println("Day with Most number of characters " + dayWithMostCharacters);

		for (int i = daysOfWeek.length - 1; i >= 0; i--) {
			System.out.println(daysOfWeek[i]);
		}

	}

}

```

### Step 11: Problems With Arrays

Let's look at our implementation for our challenge. 

We've implemented most of the features except for ```addMark()``` and ```removeMarkAtIndex()```.

```java

	Student student = new Student(name, <list-of-marks>);
	int number = student.getNumberOfmarks();
	int sum = student.getTotalSumOfMarks();
	int maximumMark = student.getMaximumMark();
	int minimumMark = student.getMinimumMark();
	BigDecimal average = student.getAverageMarks();
	student.addMark(35);	
	student.removeMarkAtIndex(5);

```

We would want to add and remove from an array. Can we do this?

The size of an array is fixed at its compile-time definition. Which means that once we define an array such as:

```String[] textValues = {"Apple", "Ball", "Cat"};```

The size of the `textValues` array is fixed to 3. You an change values inside the array. But the size cannot be changed.

How to add an element to an array?

One of the options is
* Create a fresh array with a few extra element slots to accommodate the additional elements to be inserted
* Copy the existing array elements to the beginning of this new array
* Add the additional elements at the rear end of this array

If elements need to be removed from an array:
* Create a fresh array with correspondingly lesser element slots
* Copy the existing array elements, excluding the ones to be removed, to the beginning of this new array

```java
jshell> int[] marks = {12, 34, 45};
marks ==> int[3] { 12, 34, 45 }

jshell> int[] newMarks = new int[marks.length+1];
newMarks ==> int[4] { 0, 0, 0, 0 }

jshell> System.arraycopy(marks, 0, newMarks, 0, marks.length);

jshell> newMarks
newMarks ==> int[4] { 12, 34, 45, 0 }

jshell> newMarks[3] = 100
$27 ==> 100

jshell> newMarks
newMarks ==> int[4] { 12, 34, 45, 100 }

```

As you can see, this can be very inefficient. How do we solve it?

### Step 12: Introducing ```ArrayList```

`ArrayList` is more dynamic than an array. It provides operations to add and remove elements.

Let's start with creating an `ArrayList` and add a few values.

```java

	jshell> ArrayList arrayList = new ArrayList();
	arrayList ==> []
	jshell> arrayList.add("Apple");
	| Warning:
	| unchecked call to add(E) as a member of the raw type java.util.ArrayList
	| arrayList.add("Apple");
	|_^---------------------^
	$1 ==> true
	jshell> arrayList.add("Ball");
	| Warning:
	| unchecked call to add(E) as a member of the raw type java.util.ArrayList
	| arrayList.add("Ball");
	|_^---------------------^
	$2 ==> true
	jshell> arrayList.add("Cat");
	| Warning:
	| unchecked call to add(E) as a member of the raw type java.util.ArrayList
	| arrayList.add("Cat");
	|_^---------------------^
	$3 ==> true
	jshell> arrayList
	arrayList ==> ["Apple", "Ball", "Cat"]
```
You can remove values using `remove` method.

```java

	jshell> arrayList.remove("Cat");
	$4 ==> true
	jshell> arrayList
	arrayList ==> ["Apple", "Ball"]
```

The ```ArrayList``` instance ```arrayList``` can be used to store objects of pretty much any type, even primitive types. Also, non-homogeneous types! 

> The warning message displayed is a hint to the programmer to discourage this.

```java
	jshell> arrayList.add(1);
	| Warning:
	| unchecked call to add(E) as a member of the raw type java.util.ArrayList
	| arrayList.add(1);
	|_^---------------------^
	$3 ==> true
	jshell> arrayList
	arrayList ==> ["Apple", "Ball", 1]
	jshell>

```

Let's say we want to store only `String` values in an `ArrayList`. How do we do it?

We can specify the type of elements that an `ArrayList` can contain.

```java

	jshell> ArrayList<String> items = new ArrayList<String>();
	items ==> []
```

In above snippet, we are creating an `ArrayList` that can hold `String` values.

You can add `String` value but not numbers.

```java	
	jshell> items.add("Apple");
	$1 ==> true
	jshell> items
	items ==> ["Apple"]
	jshell> items.add(1);
	| Error
	| no suitable method found for add(int)
	|...
	jshell> items.add("Ball");
	$2 ==> true
	jshell> items.add("Cat");
	$3 ==> true
	jshell> items
	items ==> ["Apple", "Ball", "Cat"]
```

Rest of operations are similar to a normal `ArrayList`.
```java
	jshell> items.remove("Cat");
	$4 ==> true
	jshell> items
	items ==> ["Apple", "Ball"]
	jshell> items.remove(0);
	$5 ==> "Apple"
	jshell> items
	items ==> ["Ball"]
	jshell>

```

### Step 13: Refactoring ```Student``` To Use ```ArrayList```

Let's now get to the ```Student``` challenge once again. Let's use an `ArrayList` this time.

```java

	Student student = new Student(name, <list-of-marks>);
	int number = student.getNumberOfmarks();
	int sum = student.getTotalSumOfMarks();
	int maximumMark = student.getMaximumMark();
	int minimumMark = student.getMinimumMark();	
	BigDecimal average = student.getAverageMarks();

```

##### Snippet-01 : Refactoring ```Student```

**_StudentRunner.java_**

```java

	package com.in28minutes.arrays;

	public class StudentRunner {
		public static void main(String[] args) {
			Student student = new Student("Ranga", 97, 98, 100);
			int number = student.getNumberOfmarks();			
			System.out.println("Number of marks : " + number);
			int sum = student.getTotalSumOfMarks();
			System.out.println("Sum of marks : " + sum);

			int maximumMark = student.getMaximumMark();
			System.out.println("Maximum of marks : " + maximumMark);
			int minimumMark = student.getMinimumMark();
			System.out.println("Minimum of marks : " + minimumMark);

			BigDecimal average = student.getAverageMarks();
			System.out.println("Average of marks : " + average);
			System.out.println(student);
		}	
	}

```

**_Student.java_**

```java

	package com.in28minutes.arrays;
	import java.math.BigDecimal;
	import java.math.RoundingMode;
	import java.util.ArrayList;

	public class Student {
		private String name;
		private ArrayList<Integer>  marks = new ArrayList<Integer>();

		public Student(String name, int...  marks) {
			this.name = name;
			for(int mark: marks) {
				this.marks.add(mark);
			}
		}

		public int getNumberOfMarks() {
			return marks.size();
		}

		public int getTotalSumOfMarks() {
			int sum = 0;
			for(int mark:marks) {
				sum += mark;
			}			
			return sum;
		}

		public BigDecimal getAverageOfMarks() {
			int sum = getTotalSumOfMarks();
			BigDecimal average = new BigDecimal(sum).divide(new BigDecimal(marks.size()), 3, RoundingMode.UP);
		}

		public int getMaximumMark() {
			return Collections.max(marks);
		}

		public int getMinimumMark() {
			return Collections.min(marks);
		}

		public String toString() {
			return name + marks;
		}
	}

```


The Enhanced ```for``` loop works for ```ArrayList```s as well, just like in the case of an array

The ```Collections.max()``` and ```Collections.min()``` methods can be used to find the maximum and minimum value in an array.

### Step 14: Enhancing ```Student``` Further

Let's now add the features to add and remove a student.

```java

	package com.in28minutes.arrays;

	public class StudentRunner {
		public static void main(String[] args) {
			Student student = new Student("Ranga", 97, 98, 100);
			int number = student.getNumberOfmarks();
			System.out.println("Number of marks : " + number);
			int sum = student.getTotalSumOfMarks();			
			System.out.println("Sum of marks : " + sum);

			int maximumMark = student.getMaximumMark();
			System.out.println("Maximum of marks : " + maximumMark);
			int minimumMark = student.getMinimumMark();
			System.out.println("Minimum of marks : " + minimumMark);

			BigDecimal average = student.getAverageMarks();
			System.out.println("Average of marks : " + average);
			System.out.println(student);
			
			student.addMark(35);			
			System.out.println(student);
			student.removeMarkAtIndex(1);
			System.out.println(student);
		}
	}

```

**_Student.java_**

```java

	package com.in28minutes.arrays;
	import java.math.BigDecimal;
	import java.math.RoundingMode;
	import java.util.ArrayList;

	public class Student {
		private String name;
		private ArrayList<Integer>  marks = new ArrayList<Integer>();

		public Student(String name, int...  marks) {
			this.name = name;
			for(int mark: marks) {
				this.marks.add(mark);
			}
		}

		public int getNumberOfMarks() {
			return marks.size();
		}

		public int getTotalSumOfMarks() {
			int sum = 0;
			for(int mark:marks) {
				sum += mark;
			}		
			return sum;
		}

		public BigDecimal getAverageOfMarks() {
			int sum = getTotalSumOfMarks();
			BigDecimal average = new BigDecimal(sum).divide(new BigDecimal(marks.size()), 3, RoundingMode.UP);
		}

		public int getMaximumMark() {
			return Collections.max(marks);
		}

		public int getMinimumMark() {
			return Collections.min(marks);
		}

		public String toString() {
			return name + marks;
		}

		public void addMark(int mark) {
			marks.add(mark);
		}

		public void removeMarkAtIndex(int index) {
			marks.remove(index);
		}
	}

```

**_Console Output_**

_Number of marks : 3_

_Sum of marks : 3_

Average of marks : 3_

_Maximum of marks : 3_

_Minimum of marks : 3_

_Ranga[97,98,100]_

_Ranga[97,98,100,35]_

_Ranga[97,100,35]_

## Object Oriented Programming (*OOP*) - Revisited

In this section, we revisit the principles of *OOP*, armed with the knowledge of
* Arrays and their variants
* Built-in Java classes and utilities, and 
* Conditionals and loops (normal and enhanced). 

### Step 01: Objects Revisited - State And Behavior

The attributes of an object determine what it is made up of. At different points in an object's lifetime, the value of any of its attributes can change. 

At any given time, values of these attributes defines the object's **state**. 

In The ```MotorBike``` example, the attribute ```speed``` defines a ```MotorBike```'s state. The ```speed``` of a ```ducati``` defines its state.

How an object responds to an external event, or a message sent to it, defines its **behavior**. 

Messages are delivered to an object using methods. Methods are used to implement an object's **behavior**. 

The methods ```setSpeed```, ```increaseSpeed``` and ```decreaseSpeed``` have an effect on the observed speed of the ```MotorBike```s. The future `state` of a `MotorBike` depends on `behavior` and current `state`.

`behavior` affects `state`. And `state` affects `behavior`. 


**_MotorBikeRunner.java_**

```java

	package com.in28minutes.oops;

	public class MotorBikeRunner {
		public static void main(String[] args) {
			MotorBike ducati = new MotorBike(100);
			MotorBike honda = new MotorBike(200);
			MotorBike yamaha = new MotorBike();
			ducati.start();
			honda.start();
			yamaha.start();

			ystem.out.println(ducati.getSpeed());
			System.out.println(honda.getSpeed());
			System.out.println(yamaha.getSpeed());

			ducati.increseSpeed(50);
			yamaha.setSpeed(250);
			honda.increaseSpeed(100);
			yamaha.decreaseSpeed(50);
			System.out.println(ducati.getSpeed());
			System.out.println(honda.getSpeed());
			System.out.println(yamaha.getSpeed());
		}
	}

```


**_MotorBike.java_**

```java

	package com.in28minutes.oops;

	public class MotorBike {
		//state
		private int speed;
		//behavior
		MotorBike() {
			this(5);
		}

		MotorBike(int speed) {
			if(speed > 0)
				this.speed = speed;
		}
		
		public void start() {
			System.out.println("Bike started!");
		}

		public void setSpeed(int speed) {
			if(speed > 0)
				this.speed = speed;
		}

		public int getSpeed() {
			return this.speed;
		}

		public void increaseSpeed(int howMuch) {
			setSpeed(this.speed + howMuch);
		}

		public void decreaseSpeed(int howMuch) {
			setSpeed(this.speed - howMuch);
		}
	}

```

### Step 02: Managing ```class``` state

At a basic level, when we design a class, we decide:
* `state` - member variables
* `how to create objects` - Define constructors
* `behavior` - What methods are exposed

Consider the example of a ```Fan``` ```class```.

The above three major areas that correspond to its design could be as follows:

* State
	* make
	* radius
	* color
	* isOn
	* speed
* Constructors
	*  Fan(String make, double radius, String color)
* Behavior
	* void switchOn()
	* void SwitchOff()
	* void changeSpeed(int change)
	* String toString()

Let's try to write a simple ```Fan``` ```class```, that covers all these aspects. 

**_Fan.java_**

```java

	package com.in28minutes.oops.level2;
	
	public class Fan {
		//state
		private String make;
		private double radius;
		private String color;
		private boolean isOn;
		private byte speed;	//levels: 0 to 5

		//constructors

		public Fan(String make, double radius, String color) {
			this.make = make;
			this.radius = radius;
			this.color = color;
		}

		//methods
		public String toString() {
			return String.format("Make : %s, Radius : %f, Color : %s, Is On : %b, Speed : %d",
									make,
									radius,
									color,
									isOn,
									speed);
		}
	}

```

**_FanRunner.java_**

```java

	package com.in28minutes.oops.level2;

	public class FanRunner {
		public static void main(String[] args) {
			Fan fan = new Fan("Fan-Tastic", 0.456, "GREEN");
			System.out.println(fan);
		}
	}

```
**_Console Output_**

_Make : Fan-tastic, Radius : 0.45600, Color : GREEN, Is On : false, Speed : 0_

The fields which were not set by the constructor, namely ```isOn``` and ```speed```, assumed the language default values for their data types, namely ```false``` (for ```booelan```) and ```0``` (for ```int```).

### Step 03: Augmenting ```Fan``` With Behavior
- - - 

We need to decide what kind of behavior should be provided by a `Fan` object.

The default state attributes of the ```Fan``` class objects, namely ```make```, ```color``` and ```radius``` are fixed at manufacturing time, and cannot be altered by a user of this ```class```'s instances. 

The other two state attributes, ```isOn``` and ```speed``` need to be exposed to change by ```Fan``` object users. We will offer methods that change them.

##### Snippet-01 : The ```Fan``` ```class``` - v4

**_FanRunner.java_**

```java

	package com.in28minutes.oops.level2;

	public class FanRunner {
		public static void main(String[] args) {
			Fan fan = new Fan("Fan-Tastic", 0.456, "GREEN");
			System.out.println(fan);
			fan.switchOn();
			System.out.println(fan);
			fan.setSpeed((byte)5);
			System.out.println(fan);
			fan.switchOff();
			System.out.println(fan);
		}
	}

```

**_Fan.java_**

```java

	package com.in28minutes.oops.level2;

	public class Fan {
		//state
		private String make;
		private double radius;
		private String color;
		private boolean isOn;
		private byte speed;	//levels: 0 to 5

		//constructors
		public Fan(String make, double radius, String color) {
			this.make = make;
			this.radius = radius;
			this.color = color;
		}

		//methods
		public String toString() {
			return String.format("Make : %s, Radius : %f, Color : %s, Is On : %b, Speed : %d",
									make,
									radius,
									color,
									isOn,
									speed);
		}

		//isOn
		/*public void isOn(boolean isOn) {
			this.isOn = isOn;
		}*/

		public void switchOn() {
			isOn = true;
			setSpeed((byte)1);
		}

		public void switchOff() {
			isOn = false;
			setSpeed((byte)0);
		}

		public void setSpeed(byte speed) {
			this.speed = speed;
		}
	}

```

**_Console Output_**

_Make : Fan-Tastic, Radius : 0.45600, Color : GREEN, Is On : false, Speed : 0_

_Make : Fan-Tastic, Radius : 0.45600, Color : GREEN, Is On : true, Speed : 1_

_Make : Fan-Tastic, Radius : 0.45600, Color : GREEN, Is On : true, Speed : 5_

_Make : Fan-Tastic, Radius : 0.45600, Color : GREEN, Is On : false, Speed : 0_

##### Snippet-01 Explained

* Regarding the state attribute ```isOn```:
	* A state modifier method such as ```public void isOn(boolean)``` is not preferred, even though it does alter this attribute. This is because it is not intuitive from the ```class``` user's perspective.
	* Alternatively, methods such as ```public void switchOn()``` and ```public void switchOff()``` not only toggle the attribute ```isOn```, but are also intuitive and useful to the ```Fan``` ```class``` users (Here, the ```FanRunner``` class).

* Regarding the state attribute ```speed```:
	*  ```setSpeed``` is both intuitive as well as useful, so not much rethinking needed here
	*  ```speed``` needs to be affected by the operations ```switchOn()``` and ```switchOff()```. We have added calls to ```setSpeed()``` in these method definitions.


#### Summary

The best way to design a class is using an `Outside In` thought process:
* Who all could possibly be using my ```class```?
* What functionality would they absolutely require?

### Step 04: Programming Exercise PE-OOP-01

1. Write a simple ```Rectangle``` ```class``` , while covering the following constituents:
* State
	* length
	* width
* Constructors
* Behavior or Methods

#### Solution To PE-OOP-01

**_RectangleRunner.java_**

```java

	package com.in28minutes.oops.level2;

	public class RectangleRunner {
		public static void main(String[] args) {
			Rectangle rectangle = new Rectangle(12, 23);
			System.out.println(rectangle);
			rectangle.setWidth(25);
			System.out.println(rectangle);
			rectangle.setLength(20);
			System.out.println(rectangle);
		}
	}

```

**_Rectangle.java_**

```java

	package com.in28minutes.oops.level2;

	public class Rectangle {
		//state:
			private int length;
			private int width;
		
		//creation:
		public Rectangle(int length, int width) {
			this.length = length;
			this.width = width;
		}

		//behaviors:
		public int getLength() {
			return length;
		}

		public int getWidth() {
			return width;
		}

		public void setLength(int length) {
			this.length = length;
		}

		public void setWidth(int width) {
			this.width = width;
		}

		public int area() {
			return length * width;
		}

		public int perimeter() {
			return 2*(length + width);
		}

		public String toString() {
			return String.format("Rectangle - length : %d, width : %d, area : %d, perimeter : %d", 
									length,
									width,
									area(),
									perimeter());
		}
	}

```

**_Console Output_**

_Rectangle - length : 12, width : 23, area : 276, perimeter : 70_

_Rectangle - length : 12, width : 25, area : 300, perimeter : 74_

_Rectangle - length : 20, width : 25, area : 500, perimeter : 90_

#### Solution Explained

* A ```Rectangle``` object created without a specified ```length``` and ```width``` makes no practical sense, therefore a default constructor is not provided.

### Step 06: Understanding Object Composition

Let's take a re-look at the state attributes of the ```Fan``` ```class```:

**_Fan.java_**

```java

	package com.in28minutes.oops.level2;

	public class Fan {
		//state
		private String make;
		private double radius;
		private String color;
		private boolean isOn;
		private byte speed;
		
		//constructors
		//methods
	}

```

All member variables of 'Fan' class are primitive variables. Can we make it complex and include other classes?

##### Snippet-01 : Object composition - State

**_CustomerRunner.java_**

```java

	package com.in28minutes.oops.level2;

	public class CustomerRunner {
		public static void main(String[] args) {
			Customer customer = new Customer();
		}
	}

```

**_Address.java_**

```java

	package com.in28minutes.oops.level2;

	public class Address {
		//state
		private String doorNo;
		private String streetInfo;
		private String city;
		private String zipCode;

		//creation
		//behaviors
	}

```

**_Customer.java_**

```java

	package com.in28minutes.oops.level2;

	public class Customer {
		//state
		private String name;
		private Address homeAddress;
		private Address workAddress;

		//creation
		//behaviors
	}

```

##### Snippet-01 Explained

```Customer customer``` is composed of:
*  ```name```,
*  ```homeAddress```, and
*  ```workAddress```. 

```String``` is a built-in type, and is simple. ```Address``` is a user defined type, and is composed of:	
* ```doorNo```,
* ```streetInfo```,
* ```city```, and
* ```zipCode```
	
##### Snippet-02 : Object Composition v2 - Construction

Let's now add constructors to allow easy creation of these objects.

**_CustomerRunner.java_**

```java

	package com.in28minutes.oops.level2;

	public class CustomerRunner {
		public static void main(String[] args) {
			//Customer customer = new Customer();
			Address homeAddress = new Address("Flat No. 51", "Hiranandani Gardens", Mumbai", "400076");
			Address workAddress = new Address("Administrative Office", "Western Block", "Mumbai", "400076");
			Customer customer = new Customer("Ashwin Tendulkar", homeAddress, workAddress);
		}
	}

```

**_Address.java_**

```java

	package com.in28minutes.oops.level2;

	public class Address {
		//state
		private String doorNo;
		private String streetInfo;
		private String city;
		private String zipCode;

		//creation
		public Address(String doorNo, String streetInfo, String city, String zipCode) {
			this.doorNo = doorNo;
			this.streetInfo = streetInfo;
			this.city = city;
			this.zipCode = zipCode;
		}

		//behaviors
	}

```

**_Customer.java_**

```java

	package com.in28minutes.oops.level2;

	public class Customer {
		//state
		private String name;
		private Address homeAddress;
		private Address workAddress;

		//creation
		//workAddress not mandatory for creation
		public Customer(String name, String homeAddress) {
			this.name = name;
			this.homeAddress = homeAddress;
		}

		//behaviors
	}

```

##### Snippet-9 : Object Composition v3 : Behaviors

Let's add methods to provide behavior.

**_CustomerRunner.java_**

```java

	package com.in28minutes.oops.level2;

	public class CustomerRunner {
		public static void main(String[] args) {
			//Customer customer = new Customer();
			Address homeAddress = new Address("Flat No. 51", "Hiranandani Gardens", "Mumbai", "400076");
			Customer customer = new Customer("Ashwin Tendulkar", homeAddress);
			System.out.println(customer);
			Address workAddress = new Address("Administrative Office", "Western Block", "Mumbai", "400076");
			customer.setWorkAddress(workAddress);
			System.out.println(customer);
		}
	}

```

**_Address.java_**

```java

	package com.in28minutes.oops.level2;

	public class Address {
		//state
		private String doorNo;
		private String streetInfo;
		private String city;
		private String zipCode;

		//creation
		public Address(String doorNo, String streetInfo, String city, String zipCode) {
			super();
			this.doorNo = doorNo;
			this.streetInfo = streetInfo;
			this.city = city;
			this.zipCode = zipCode;
		}

		//behaviors
		public String toString() {
			return doorNo + ", " + streetInfo + ", " + city + " - " + zipCode;
		}
	}

```

**_Customer.java_**

```java

	package com.in28minutes.oops.level2;

	public class Customer {
		//state
		private String name;
		private Address homeAddress;
		private Address workAddress;

		//creation
		//workAddress not mandatory for creation
		public Customer(String name, String homeAddress) {
			this.name = name;
			this.homeAddress = homeAddress;
		}

		//behaviors
		//certain components of homeAddress and workAddress can be modified, not the name
		public void setHomeAddress(Address homeAddress) {
			this.homeAddress = homeAddress;
		}

		public void setWorkAddress(Address workAddress) {
			this.workAddress = workAddress;
		}

		public Address getHomeAddress() {
			return homeAddress;
		}

		public Address getWorkAddress() {
			return workAddress;
		}

		public String toString() {
			return String.format("Customer [%s] lives at [%s], works at [%s]", 
									name,
									homeAddress,
									workAddress);
		}
	}

```

**_Console Output_**

_Customer [Ashwin Tendulkar] lives at [Flat No. 51, Hiranandani Gardens, Mumbai - 400076], works at [null]_

_Customer [Ashwin Tendulkar] lives at [Flat No. 51, Hiranandani Gardens, Mumbai - 400076], works at [Administrative Office, Western Block, Mumbai - 400076]_

### Step 07: Programming Exercise PE-OOP-02

#### Exercises

Write a program that manages Books and their Reviews:

* Book:
	* Id
	* Name
	* Author
* Review:
	* Id
	* Description
	* Rating

```java

	Book book = new Book(123, "Object Oriented Programming With Java", "Ranga");
	book.addReview(new Review(10, "Great Book", 4));
	book.addReview(new Review(101, "Awesome", 5));
	System.out.println(book);

```

#### Solution To PE-OOP-02

**_BookReviewRunner.java_**

```java

	package com.in28minutes.oops.level2;

	public class BookReviewRunner {
		public static void main(String[] args) {
			Book book = new Book(123, "Object Oriented Programming With Java", "Ranga");
			book.addReview(new Review(10, "Great Book", 4));
			book.addReview(new Review(101, "Awesome", 5));
			System.out.println(book);
		}
	}

```

**_Review.java_**

```java

	package com.in28minutes.oops.level2;

	public class Review {
		private int id;
		private String description;
		private byte rating;

		public Review(int id, String description, byte rating) {
			this.id = id;
			this.description = description;
			this.rating = rating;
		}

		public String toString() {
			return "(Review-" + id + ", " + description + ", " + rating + ")";
		}
	}

```

**_Book.java_**

```java

	package com.in28minutes.oops.level2;

	public class Book {
		private int id;
		private String title;
		private String author;

		private ArrayList<Review> reviewList = new ArrayList<Review>();
		public Book(int id, String title, String author) {
			this.id = id;
			this.title = title;
			this.author = author;
		}

		public void addReview(Review review) {
			reviewList.add(review);
		}

		public String toString() {
			return "Book-" + id + ",  " + title + ", " + author + ", " + reviews);
		}
	}

```

**_Console Output_**

_Book-123, Object Oriented Programming With Java, Ranga, [(Review-10, Great Book", 4), (Review-101, Awesome, 5)]_

### Step 07: The Need For Inheritance

Let's look at two classes `Person` and `Student`.


**_Person.java_**

```java

	package com.in28minutes.oops.level2.inheritance;

	public class Person {
		private String name;
		private String email;
		private String phoneNumber;
		
		public void setName(String name) {
			this.name = name;
		}

		public String getName() {
			return name;
		}

		public void setEmail(String email) {
			this.email = email;
		}

		public String getEmail() {
			return email;
		}

		public void setPhoneNumber(String phoneNumber) {
			this.phoneNumber = phoneNumber;
		}

		public String getPhoneNumber() {
			return phoneNumber;
		}
	}

``` 

**_StudentWithoutInheritance.java_**

```java

	package com.in28minutes.oops.level2.inheritance;

	public class StudentWithoutInheritance {
		private String name;
		private String email;
		private String phoneNumber;
		private String college;
		private int year;

		public void setName(String name) {
			this.name = name;
		}

		public String getName() {
			return name;
		}

		public void setEmail(String email) {
			this.email = email;
		}

		public String getEmail() {
			return email;
		}

		public void setPhoneNumber(String phoneNumber) {
			this.phoneNumber = phoneNumber;
		}

		public String getPhoneNumber() {
			return phoneNumber;
		}

		public void setCollege(String college) {
			this.college = college;
		}

		public String getCollege() {
			return college;
		}

		public void setYear(int year) {
			this.year = year;
		}

		public int getYear() {
			return year;
		}
	}

```

In above code examples, you can see that there is a lot of 
* The member fields of ```Person```, namely ```name```, ```email``` and ```phoneNumber```, are replicated in ```Student```.
* The setter and getter methods pertaining to the above fields of ```Person``` get repliated in ```Student``` as well.


Every `Student` is a `Person`. What if we could extend `Person` class instead of duplicating everything?

#### Enter Inheritance

```Student``` **is a** ```Person```. Java supports one of the basic Object Oriented Programming Paradigms : **Inheritance**.  

```Student``` can *inherit* from ```Person```, to model the fact that a ```Student``` *is a* ```Person```. 

This is accomplished by using the Java keyword ```extends```, during class definition of ```Student```. 

```java

	public class Person {
		// <Person Definition>
	}

	public class Student extends Person {
		// <Student Definition, after reusing Person Code>
	}

```

Inheritance is a mechanism of code reuse. In this case, all the fields and methods previously defined in ```Person``` are available for ```Student``` as well.

In this Inheritance relationship, ```Person``` is called the **super-class** of ```Student```. Likewise, ```Student``` is the **sub-class** of ```Person```.

Let's now look at how we go about changing the ```Student``` ```class``` definition.

##### Snippet-02 : Student inherits from Person - v1

**_Person.java_**

```java

	package com.in28minutes.oops.level2.inheritance;

	public class Person {
		private String name;
		private String email;
		private String phoneNumber;

		public void setName(String name) {
			this.name = name;
		}

		public String getName() {
			return name;
		}

		public void setEmail(String email) {
			this.email = email;
		}

		public String getEmail() {
			return email;
		}

		public void setPhoneNumber(String phoneNumber) {
			this.phoneNumber = phoneNumber;
		}

		public String getPhoneNumber() {
			return phoneNumber;
		}
	}

``` 


**_Student.java_**

```java

	package com.in28minutes.oops.level2.inheritance;

	public class Student extends Person {
		private String collegeName;
		private int year;

		public void setCollegeName(String college) {
			this.collegeName = collegeName;
		}

		public String getCollegeName() {
			return collegeName;
		}

		public void setYear(int year) {
			this.year = year;
		}

		public int getYear() {
			return year;
		}
	}

```

**_StudentRunner.java_**

```java

	package com.in28minutes.oops.level2.inheritance;
	public class StudentRunner {
		public static void main(String[] args)
			Student student = new Student();
			// < all setter() and getter() methods of Person and Student available >
			student.setName("Ranga");			
			student.setEmail("in28minutes@gmail.com");
		}
	}

```

### Step 09:  Introducing ```Object``` class

In the Java language, every class, whether an in-built Java library class, or a user-defined class, implicitly inherits from the class ```Object```. 

This ```Object``` class is available in the Java system package ```java.lang```. This class is at the root of the Java class hierarchy. All classes, including arrays, implement/inherit the methods of this ```class```. 

Let's take a look at the ```Person``` and ```Student``` classes.

##### Snippet-01 : The Object class

**_Person.java_**

```java

	package com.in28minutes.oops.level2.inheritance;

	public class Person {
		private String name;
		private String email;
		private String phoneNumber;

		public void setName(String name) {
			this.name = name;
		}

		public String getName() {
			return name;
		}

		public void setEmail(String email) {
			this.email = email;
		}

		public String getEmail() {
			return email;
		}

		public void setPhoneNumber(String phoneNumber) {
			this.phoneNumber = phoneNumber;
		}

		public String getPhoneNumber() {
			return phoneNumber;
		}
	}

``` 


**_Student.java_**

```java

	package com.in28minutes.oops.level2.inheritance;

	public class Student extends Person {
		private String collegeName;
		private int year;
		
		public void setCollegeName(String college) {
			this.collegeName = collegeName;
		}

		public String getCollegeName() {
			return collegeName;
		}

		public void setYear(int year) {
			this.year = year;
		}

		public int getYear() {
			return year;
		}
	}

```

**_StudentRunner.java_**

```java

	package com.in28minutes.oops.level2.inheritance;

	public class StudentRunner {
		public static void main(String[] args)
			//Student student = new Student();
			//student.setName("Ranga");
			//student.setEmail("in28minutes@gmail.com");

			Person person = new Person();
			String personStr = person.toString();
			System.out.println(personStr);
			System.out.println(person);
			int hashCode = person.hashCode();			
			person.notify();
		}
	}

```

**_Console Output_**

_com.in28minutes.oops.level2.inheritance.Person@7a46a697_

_com.in28minutes.oops.level2.inheritance.Person@7a46a697_

##### Snippet-01 Explained

Methods of the ```Object``` ```class``` such as ```toString()```, ```hashCode()``` and ```notify()``` are available to objects of ```class``` ```Person``` as default implementations.

The statement ```System.out.println(person);``` actually gets translated to ```System.out.println(person.toString())```, as the Java system implicitly makes the call ```person.toString()``` as it is inherited from ```class``` ```Object``` for use in the ```String``` context.

### Step 10: Inheritance And Method Overriding

Sub-class inherit features from super-class
* state attributes : super-class member variables
* behavior components  : super-class method definitions

These are of course, available for access (and modification), and invocation, respectively, within the sub-class. 

You can also override super class method implementations in a sub class - **method overriding**. 

##### Snippet-01: Method Overriding

**_Person.java_**

```java

	package com.in28minutes.oops.level2.inheritance;

	public class Person {
		private String name;
		private String email;
		private String phoneNumber;

		public void setName(String name) {
			this.name = name;
		}

		public String getName() {
			return name;
		}

		public void setEmail(String email) {
			this.email = email;
		}

		public String getEmail() {
			return email;
		}

		public void setPhoneNumber(String phoneNumber) {
			this.phoneNumber = phoneNumber;
		}

		public String getPhoneNumber() {
			return phoneNumber;
		}

		public String toString() {
			return String.format("Person %s , Email : %s, Phone Number : %s", name, email, phoneNumber);
		}
	}

``` 

**_PersonRunner.java_**

```java

	package com.in28minutes.oops.level2.inheritance;

	public class PersonRunner {
		public static void main(String[] args)
			Person person = new Person();
			person.setName("Ranga");
			person.setEmail("in28minutes@gmail.com");
			person.setPhoneNumber("9898989898");
			String personStr = person.toString();
			System.out.println(personStr);
			System.out.println(person);
		}
	}

```

**_Console Output_**

_Person Ranga , Email : in28minutes@gmail.com, Phone Number : 9898989898_

_Person Ranga , Email : in28minutes@gmail.com, Phone Number : 9898989898_

##### Snippet-01 Explained

By defining the method ```toString()``` within the ```Person``` sub-```class```, we are overriding the default version provided by the ```Object``` super-```class```.

### Step 11: Classroom Exercise CE-OOP-01 

Create an Employee class extending Student Class with following attributes:
* Title
* Employer
* EmployeeGrade
* Salary

Create a method toString() within Employee to print all state attribute values, including those of Person.

##### Snippet-01 : Employee Inheritance

**_Person.java_**

```java

	package com.in28minutes.oops.level2.inheritance;

	public class Person {
		private String name;
		private String email;
		private String phoneNumber;

		public void setName(String name) {
			this.name = name;
		}

		public String getName() {
			return name;
		}

		public void setEmail(String email) {
			this.email = email;
		}

		public String getEmail() {
			return email;
		}

		public void setPhoneNumber(String phoneNumber) {
			this.phoneNumber = phoneNumber;
		}

		public String getPhoneNumber() {
			return phoneNumber;
		}

		public String toString() {
			return Sring.format("Person %s , Email : %s, Phone Number : %s", name, email, phoneNumber);
		}
	}

``` 

**_Employee.java_**

```java

	package com.in28minutes.oops.level2.inheritance;
	import java.math.BigDecimal;

	public class Employee extends Person {
		private String title;
		private String employerName;
		private char employeeGrade;
		private BigDecimal salary;

		public void setTitle(String title) {
			this.title = title;
		}

		public String getTitle() {
			return title;
		}

		public void setEmployerName(String employer) {
			this.employerName = employerName;
		}

		public String getEmployerName() {
			return employerName;
		}

		public void setEmployeeGrade(char  employeeGrade) {
			this.employeeGrade = employeeGrade;
		}

		public char getEmployeeGrade() {
			return employeeGrade;
		}

		public void setSalary(BigDecimal  salary) {
			this.salary = salary;
		}

		public BigDecimal getSalary() {
			return salary;
		}

		public String toString() {
			return String.format("Employee Title: %s, Employer: %s, Employee Grade: %c, Salary: %s",
									title,
									employerName,
									employeeGrade,
									salary);
		}
	}

```

**_EmployeeRunner.java_**

```java

	package com.in28minutes.oops.level2.inheritance;

	public class EmployeeRunner {
		public static void main(String[] args) {
			Employee employee = new Employee();
			employee.setName("Ranga");
			employee.setEmail("in28minutes@gmail.com");
			employee.setPhoneNumber("123-456-7890");
			employee.setTitle("Programmer Analyst");
			employee.setEmployerName("In28Minutes");
			employee.setEmployeeGrade('A');
			employee.setSalary(new BigDecimal("50000"));
			System.out.println(employee);
		}
	}

```

**_Console Output_**

_Employee Title: Programmer Analyst, Employer: In28Minutes, Employee Grade: A, Salary: 50000.0000_

##### Snippet-01 Explained

We have not printed the underlying ```Person``` object details in ```Employee.toString()``` method overriding. Let's look to do that next.

### Step 12: Constructors, And Calling ```super()``` 

The ```super``` keyword allows an sub-class to access the attributes present in the super-class. 

##### Snippet-01 : Calling Person.toString()

**_Employee.java_**

```java

	package com.in28minutes.oops.level2.inheritance;
	import java.math.BigDecimal;

	public class Employee extends Person {
		//focusing only on the toString() method
		public String toString() {
			return String.format("Employee Name: %s, Email: %s, Phone Number: %s, Title: %s, Employer: %s, Employee Grade: %c, Salary: %s",
									super.getName(),
									super.getEmail(),
									super.getPhoneNumber(),
									title,
									employerName,
									employeeGrade,
									salary);
		}
	}

```

**_EmployeeRunner.java_**

```java

	package com.in28minutes.oops.level2.inheritance;
	
	public class EmployeeRunner {
		public static void main(String[] args) {
			Employee employee = new Employee();
			employee.setName("Ranga");
			employee.setEmail("in28minutes@gmail.com");
			employee.setPhoneNumber("123-456-7890");
			employee.setTitle("Programmer Analyst");
			employee.setEmployerName("In28Minutes");
			employee.setEmployeeGrade('A');		
			employee.setSalary(new BigDecimal("50000"));
			System.out.println(employee);
		}
	}

```

**_Console Output_**

_Employee Name: Ranga, Email: in28minutes@gmail.com, Phone Number: 123-456-7890, Title: Programmer Analyst, Employer: In28Minutes, Employee Grade: A, Salary: 50000.0000_

The ```super``` keyword allows an sub-class to access the attributes present in the super-class. Hence, we were able to invoke the getter methods of the ```Person``` object within the ```Employee``` object, like this within ```Employee.toString()```
	* ```super.getName()```
	* ```super.getEmail()```
	* ```super.getPhoneNumber()```


#### Sub-Class Contructor 

What happens when a sub class object is created? Does the super class constructor get called?

##### Snippet-7 : Person class

**_Person.java_**

```java

	package com.in28minutes.oops.level2.inheritance;

	public class Person {

		public Person() {
			System.out.println("Inside Person Constructor");
		}

	}

``` 

**_Employee.java_**

```java

	package com.in28minutes.oops.level2.inheritance;
	import java.math.BigDecimal;

	public class Employee extends Person {

		public Employee() {
			//super();
			System.out.println("Inside Employee Constructor");
		}

	}

```

**_EmployeeRunner.java_**

```java

	package com.in28minutes.oops.level2.inheritance;

	public class EmployeeRunner {
		public static void main(String[] args) {
			Employee employee = new Employee();
		}
	}

```

**_Console Output_**

_Inside Person Constructor_

_Inside Employee Constructor_

##### Snippet-02 Explained

When a sub-class object is created
* sub-class constructor is called and it implicitly invokes its super-class constructor. 

The Java compiler inserts the code ```super();``` (if it is not explicitly added by the programmer) as the first statement in the body of the sub-class default constructor, here ```Employer()```. 
* The statement ```super();``` is the invocation of the super-class default constructor. 
* Hence, the body of the super-class constructor is always invoked before the body of the sub-class constructor.

##### Snippet-3 : ```Person``` - Non-Default Constructor

Let's remove the no argument constructor and add a one argument constructor to `Person` class.

```
		public Person(String name) {
			this.name = name;
		}
```

**_PersonRunner.java_**

```java

	package com.in28minutes.oops.level2.inheritance;

	public class PersonRunner {
		public static void main(String[] args)
			Person person = new Person("Ranga");
			person.setEmail("in28minutes@gmail.com");
			person.setPhoneNumber("123-456-7890");
			System.out.println(person);
		}
	}

```

**_Console Output_**

_Person Ranga , Email : in28minutes@gmail.com, Phone Number : 123-456-7890_

##### Snippet-03 Explained

When we added the constructor with one argument for ```class``` ```Employee```, the existing code in **_EmployeeRunner.java_** will cause a compilation error, because there is no longer any default constructor for ```Person``` ! 

```super()``` cannot be called from within the default constructor of ```Employee```.

One option is to put the no argument constructor back.

```java

	public Person() {
		System.out.println("Inside Person Constructor");
	}

```

But, it doesn't really make sense to create a ```Person``` without a ```name```, does it? 

The solution in this case would be to call the single-argument constructor ```Person(String)``` by an invocation such as ```super(name);```

```
		public Employee(String name, String title, String employerName, char employeeGrade) {
			super(name);
			this.title = title;
			this.employerName = employerName;
			this.employeeGrade = employeeGrade;
		}
```

**_EmployeeRunner.java_**

```java

	package com.in28minutes.oops.level2.inheritance;
	
	public class EmployeeRunner {
		public static void main(String[] args) {
			Employee employee = new Employee("Ranga", "Programmer Analyst", "In28Minutes", 'A');
			System.out.println(employee);
		}
	}

```

**_Console Output_**

_Employee Name: Ranga, Email: null, Phone Number: null, Title: Programmer Analyst, Employer: In28Minutes, Employee Grade: A, Salary: null_

##### Snippet-10 : EmployeeRunner complete

Let's provide setters to set the non mandatory attributes.

**_EmployeeRunner.java_**

```java

	package com.in28minutes.oops.level2.inheritance;

	public class EmployeeRunner {
		public static void main(String[] args) {
			Employee employee = new Employee("Ranga", "Programmer Analyst", "In28Minutes", 			'A');
			employee.setEmail("in28minutes@gmail.com");
			employee.setPhoneNumber("123-456-7890");
			employee.setSalary(new BigDecimal("50000"));
			System.out.println(employee);
		}
 	}

```

**_Console Output_**

_Employee Name: Ranga, Email: in28minutes@gmail.com, Phone Number: 123-456-7890, Title: Programmer Analyst, Employer: In28Minutes, Employee Grade: A, Salary: 50000.0000_


##### Snippet-10: ```Student``` updated

Let's add a two argument construtor to the `Student` class.

**_Student.java_**

```java

	package com.in28minutes.oops.level2.inheritance;

	public class Student extends Person {
		private String collegeName;
		private int year;
	
		public Student(String name, String collegeName) {
			super(name);
			this.collegeName = collegeName;
		}

		public String getCollegeName() {
			return collegeName;
		}

		public void setYear(int year) {
			this.year = year;
		}

		public int getYear() {
			return year;
		}

		public String toString() {
			return "Student : " + super.name() + ", College: " + collegeName;
		}
	}

```

**_StudentRunner.java_**

```java

	package com.in28minutes.oops.level2.inheritance;

	public class StudentRunner {
		public static void main(String[] args)
			//Student student = new Student();
			Student student = new Student("Ranga", "IIT Bombay");
			System.out.println(student);
		}
	}

```

**_Console Output_**

_Student : Ranga, College : IIT Bombay_

### Step 13: Multiple Inheritance, Reference Variables And ```instanceof```

In other programming languages, Multiple Inheritance is allowed. A class can directly inherit from two or more classes. 

However, in Java, direct Multiple Inheritance is not allowed.

##### Snippet-01 : Multiple Inheritance

```java

	jshell> class Animal {
	   ..>> }
	| created class Animal
	jshell> class Pet {
	   ..>> }
	| created class Pet

	jshell> class Dog extends Animal, Pet {
	   ..>> }
	| Error:
	| '{' expected
	| class Dog extends Animal, Pet {
	|_________________________^
	jshell>**

```

`class Dog extends Animal, Pet {}` throws an error. You cannot extend two classes.

#### Inheritance Chains

However you can create an inheritance chain.
*  ```class``` ```C``` **is a** ```class``` ```B```
*  ```class``` ```B``` **is a** ```class``` ```A```

Let's check out a small code snippet.

##### Snippet-02 : An Inheritance Chain

`Dog``` **is a** ```Pet```, ```Pet``` **is a** ```Animal```. This is an example of what is called an **inheritance hierarchy**.

```java

	jshell> class Animal {
	   ..>> }
	| created class Animal
	jshell> class Pet extends Animal {
	   ..>> public void groom() {
	   ..>> System.out.println("Pet Groom");
	   ..>> }
	   ..>> }
	| created class Pet_
	jshell> class Dog extends Pet {
	   ..>> }
	| created class Dog
```

 If you want, you can visualize in your mind as :  *```Dog``` --> ```Pet``` --> ```Animal``` --> ```Object```* (Yes, ```Object``` is sitting at the top of *all* inheritance hierarchies in Java!)

The statement ```Dog dog = new Dog();``` sets off constructor invocations up the inheritance hierarchy:
	*  ```Dog()``` invokes ```Pet()```
		*  ```Pet()``` invokes ```Animal()```
			*  ```Animal()``` invokes ```Object()```


```java
	jshell> Dog dog = new Dog();
	dog ==> Dog@23a6e47f
```

The expression ```dog.toString()``` does a traversal up the inheritance hierarchy as well:
	* Since ```Dog.toString()``` is not defined, the compiler looks for ```Pet.toString()```
	* Since ```Pet.toString()``` is not defined, the compiler looks for ```Animal.toString()```
	* Since ```Animal.toString()``` is not defined, the compiler looks for ```Object.toString()```, which is always provided as the default implementation for all sub-classes of ```class``` ```Object``` in Java.

```java
	jshell> dog.toString();
	$1 ==> "Dog@23a6e47f"
```

The invocation ```dog.groom();``` is also resolved by traversing up the inheritance hierarchy.

```java
	jshell> dog.groom();
	"Pet Groom"
```


The statement ```Pet pet = new Dog();``` is really interesting. In Java, it is permitted for a *super-class reference variable to reference a sub-class object instance*.

Through such a reference, method invocations are also permitted, and the correct thing gets done. Hence, ```pet.groom();``` causes the output "*```Pet Groom```*".

However, the converse assignment is not allowed. *A sub-class reference variable*  **_cannot_** *reference a super-class object instance*. 
	* The statement ```Dog dog = new Pet();``` therefore, causes a compiler error. 

```java
	jshell> Pet pet = new Dog();
	pet ==> Dog@22d37d54
	jshell> pet.groom();
	Pet Groom
```

```java
	jshell> Dog dog = new Pet();
	| Error:
	| incompatible types: Pet cannot be converted to Dog
	| Dog dog = new Pet();
	|___________^-------^
```



The ```instanceof``` operator is to find the relationship between an object and a class. If the object is an instance of the class or its sub class, it returns true. 


```java
	jshell> pet instanceof Pet
	$2 ==> true
	jshell> pet instanceof Dog
	$3 ==> true
```

The ```instanceof``` operator throws an error if the object and class are unrelated.

```java
	jshell> pet instanceof String
	| Error:
	| incompatible types: Pet cannot be converted to java.lang.String
	| pet instanceof String
	|_^-^
	jshell> pet instanceof Animal
	$4 ==> true
	jshell> pet instanceof Object
	$5 ==> true
```

The ```instanceof``` operator returns ```false``` if the object is an instance of a super class of the class provided.

```java
	jshell> Animal animal  new Animal();
	animal ==> Animal@3632be31
	jshell> animal instanceof Pet
	$6 ==> false
	jshell> animal instanceof Dog
	$7 ==> false
	jshell> animal instanceof Object
	$8 ==> true
	jshell>

```

### Step 14: Introducing Abstract Classes

An ```abstract class``` can contain ```abstract``` methods.

An abstract method does not have a method definition.

Here's how a typical class looks like. You can create methods inside the class and you can create instances of the class.

```java

	jshell> class Animal {
	   ..>> public void bark() {
	   ..>> System.out.println("Animal Bark");
	   ..>> }
	   ..>> }
	| created class Animal
	jshell> Animal animal = new Animal();
	animal ==> Animal@335eadca
	jshell> animal.bark();
	Animal Bark
```

Let's see how to create an abstract class:

```java
	jshell> abstract class AbstractAnimal {
	   ..>> abstract public void bark();
	   ..>> }
	| created class AbstractAnimal
```

The syntax is simple: add `abstract` keyword before the class.

An ```abstract class``` cannot be instantiated.
```java
	jshell> AbstractAnimal animal = new AbstractAnimal();
	| Error:
	| AbstractAnimal is abstract; cannot be instantiated.
	| AbstractAnimal animal = new AbstractAnimal();
	|^--------------------------------------------^
	jshell>
```

However, it can be sub-classed, creating inheritance hierarchies below it.  A sub-class of an abstract class (often called a **concrete class**) must override its ```abstract``` methods. 


```java
	jshell> class Dog extends AbstractAnimal {
	   ..>> }
	| Error:
	| Dog is not abstract and does not override abstract method bark() in AbstractAnimal
	| class Dog extends AbstractAnimal {
	|^----------------------------------...
	jshell> class Dog extends AbstractAnimal {
	   ..>> public void bark() {
	   ..>> System.out.println("Bow Bow");
	   ..>> }
	   ..>> }
	| created class Dog
	jshell> Dog dog = new Dog();
	dog ==> Dog@5a8e6209
	jshell> dog.bark();
	Bow Bow
	
```

### Step 15: Abstract Classes - Design Aspects

Why do we need an abstract class?

Consider a feast being prepared at a home, and several dishes are on the menu for the event. Obviously, each dish would have certain procedure for it to be prepared. Cooking any dish normally involves following a tried and tested recipe, and its preparation boils down to these basic steps:
* Prepare the Ingredients
* Cook the Recipe
* Cleanup (the Mess created!)

These steps would be different for each dish but the order of steps remain the same.


##### Snippet-01 : The Recipe Hierarchy 

Let's use abstract class to build the recipe.

**_AbstractRecipe.java_**

```java

	package com.in28minutes.oops.level2;

	public abstract class AbstractRecipe {
		public void execute() {
			prepareIngredients();
			cookRecipe();			
			cleanup();
		}

		abstract void prepareIngredients();
		abstract void cookRecipe();
		abstract void cleanup();
	}

```

We defined abstract methods for each of the steps and created an `execute` method calling them. `execute` method ensures that the order of method call is followed.

You can define implementations implementing the abstract methods.

**_CurryRecipe.java_**

```java

	package com.in28minutes.oops.level2;

	public class CurryRecipe extends AbstractRecipe {
		public CurryRecipe() {
			System.out.println("[Curry Preparation Method]");
		}

		@Override
		void prepareIngredients() {
			System.out.println("Get Vegetables Cut and Ready");
			System.out.println("Get Spices Ready");
		}

		@Override
		void cookRecipe() {
			System.out.println("Steam And Fry Vegetables");
			System.out.println("Cook With Spices");
			System.out.println("Add Seasoning");
		}

		@Override
		void cleanup() {
			System.out.println("Discard unused Vegetables");
			System.out.println("Discard unused Spices");
		}
	}

```

**_RecipeRunner.java_**

```java

	package com.in28minutes.oops.level2;

	public class RecipeRunner {
		public static void main(String[] args) {
			CurryRecipe curryRecipe = new CurryRecipe();
			curryRecipe.execute();
		}
	}

```

**_Console Output_**

_[Curry Preparation Method]_

_Get Vegetables Cut and Ready_

_Get Spices Ready_

_Steam And Fry Vegetables_

_Cook With Spices_

_Add Seasoning_

_Discard unused Vegetables_

_Discard unused Spices_

##### Snippet-01 Explained

`CurryRecipe` defines what needs to be done in each step. When we invoke the `execute` method, the steps are executed in order.

##### Snippet-02 : MicrowaveCurryRecipe

We can easily create more recipes.

**_MicrowaveCurryRecipe.java_**

```java

	package com.in28minutes.oops.level2;
	
	public class MicrowaveCurryRecipe extends AbstractRecipe {
		public MicrowaveCurryRecipe() {
			System.out.println("[Curry Microwave Method]");
		}

		@Override
		void prepareIngredients() {
			System.out.println("Get Vegetables Cut and Ready");
			System.out.println("Switch on Microwave");
		}

		@Override
		void cookRecipe() {
			System.out.println("Microwave Vegetables");
			System.out.println("Add Seasoning");
		}

		@Override
		void cleanup() {
			System.out.println("Switch Off Microwave");
			System.out.println("Discard unused Vegetables");
		}
	}

```

**_RecipeRunner.java_**

```java

	package com.in28minutes.oops.level2;

	public class RecipeRunner {
		public static void main(String[] args) {
			MicrowaveCurryRecipe mcirowaveRecipe = new MicrowaveCurryRecipe();
			microwaveRecipe.execute();
		}
	}

```


**_Console Output_**

_[Curry Microwave Method]_

_Get Vegetables Cut and Ready_

_Switch on Microwave_

_Microwave Vegetables_

_Add Seasoning_

_Switch off Microwave_

_Discard unused Vegetables_

##### Snippet-02 Explained

`MicrowaveCurryRecipe` defines what needs to be done in each step. When we invoke the `execute` method, the steps are executed in order. 

#### Summary

This pattern is called a `Template method` pattern. You define an abstract class with the order of steps defined. You leave the implementation of each of the steps to the sub classes.

### Step 16: Abstract Classes - Puzzles

Let's look a few FAQ regarding abstract classes.

An ```abstract class``` can be created, without any ```abstract``` member methods.

```java

	jshell> abstract class AbstractTest {
	   ...>}
	| creates abstract class AbstractTest
```

An ```abstract class``` can be a sub class to create another ```abstract class```, without overriding any of the super-class ```abstract``` methods.

```java
	jshell> abstract class AbstractAlgorithm {
	   ...> abstract void flowChart();
	   ...> }
	| creates abstract class AbstractAlgorithm
	jshell> abstract class AlgorithmTypeOne extends AbstractAlgorithm {
	   ...> }
	| creates abstract class AlgorithmTypeOne

```

An ```abstract class``` can have member variables.
```java
	jshell> abstract class AbstractAlgorithm {
	   ...> private int stepCount;
	   ...> }
	| replaced abstract class AbstractAlgorithm
```

An ```abstract class``` can have non-abstract methods.
```java
	jshell> abstract class AbstractAlgorithm {
	   ...> private int stepCount;
	   ...> public int getStepCount() {
	   ...> return stepCount;
	   ...> }
	   ...> }
	| replaced abstract class AbstractAlgorithm
	jshell>

```


### Step 17: Introducing Interfaces
- - - 

What does a "*gaming console*" mean to you?

A device that has buttons or other controls on it, that enable us to play video games.

What are the typical buttons on it?
- Arrows - up down left right
- Select
- etc

Gaming console offers an interface to play your games.

Who provides the implementation of what happens when a button is clicked? The game implementor - for example, the implementor of Mario game or the Chess game.

How do you represent this in Java program?


**_GamingConsole.java_**

```java

	package com.in28minutes.oops.level2.interfaces;

	public interface GamingConsole {
		public void up();
		public void down();
		public void left();
		public void right();
	}

```


```interface``` ```GamingConsole``` contains methods without definitions. 

Who provides the implementations?

Welcome `MarioGame`.

**_MarioGame.java_**

```java

	package com.in28minutes.oops.level2.interfaces;

	public class MarioGame implements GamingConsole {
		@Override
		public void up() {
			System.out.println("Jump");
		}

		@Override
		public void down() {
			System.out.println("Go into a hole");
		}

		@Override
		public void left() {
		}

		@Override
		public void right() {
			System.out.println("Go Forward");
		}
	}

```

`MarioGame` provides a definition for all the methods declared in the interface `GamingConsole`. Syntax is simple. `class MarioGame implements GamingConsole` and implement all the methods.

Let's look at how you can run these games.

**_GameRunner.java_**

```java

	package com.in28minutes.oops.level2.interfaces;

	public class GameRunner {
		public static void main(String[] args) {
			MarioGame game = new MarioGame();
			game.up();
			game.down();
			game.left();
			game.right();
		}
	}

```


**_Console Output_**

_Jump_

_Go into a hole_

_Go forward_

##### Snippet-01 Explained

The main advantage of having an interface is that it can be used to enforce a contract for its implementors. 

##### Snippet-02 : Code Reuse With Interfaces

Let's look at another example - `ChessGame`.

**_ChessGame.java_**

```java

	package com.in28minutes.oops.level2.interfaces;

	public class ChessGame implements GamingConsole {

		@Override
		public void up() {
			System.out.println("Move Piece Up");
		}

		@Override
		public void down() {
			System.out.println("Move Piece Down");
		}

		@Override
		public void left() {
			System.out.println("Move Piece Left");
		}

		@Override
		public void right() {
			System.out.println("Move Piece Right");
		}
	}

```

Running it is simple. All that you need to do is to comment out `MarioGame game = new MarioGame();` and replace it with an implementation of `ChessGame`.

**_GameRunner.java_**

```java

	package com.in28minutes.oops.level2.interfaces;

	public class GameRunner {
		public static void main(String[] args) {
			//MarioGame game = new MarioGame();
			ChessGame game = new ChessGame();
			game.up();
			game.down();
			game.left();
			game.right();
		}
	}

```

**_Console Output_**

_Move Piece Up_

_Move Piece Down_

_Move Piece Left_

_Move Piece Right_

##### Snippet-2 explained

In the same ```GamerRunner``` ```class```, if we now instantiate a ```ChessGame``` object instead of a ```MarioGame``` one, none of the other code needs to change. This is because both ```MarioGame``` and ```ChessGame``` implement the same ```interface```, ```GamingConsole```. 

#### Using Interface as type for reference variable

```GamingConsole``` is an interface.```MarioGame``` and ```ChessGame``` are it's implementations.

Let's try this -  `GamingConsole game = new ChessGame();`

**_GameRunner.java_**

```java

	package com.in28minutes.oops.level2.interfaces;

	public class GameRunner {
		public static void main(String[] args) {
			GamingConsole game = new ChessGame();
			game.up();
			game.down();
			game.left();
			game.right();
		}
	}

```

**_Console Output_**

_Move Piece Up_

_Move Piece Down_

_Move Piece Left_

_Move Piece Right_

#### Explained
`GamingConsole game = new ChessGame();` - You can store an implementation of an interface into a reference variable of the type of the interface.

How does this help?

Let's look at the next example:

##### Snippet-4 : GameRunner Version 4

**_GameRunner.java_**

```java

	package com.in28minutes.oops.level2.interfaces;

	public class GameRunner {
		public static void main(String[] args) {
			GamingConsole game = new MarioGame();
			game.up();
			game.down();
			game.left();
			game.right();
		}
	}

```

**_Console Output_**

_Jump_

_Go into a hole_

_Go forward_

##### Snippet-04 Explained

You can replace `GamingConsole game = new ChessGame()` with `GamingConsole game = new MarioGame()` and now the program runs the `MarioGame`. Isn't it awesome?

### Step 18: Using Interfaces To Design APIs

Consider a Software Development project, which involves programming a fairly large and complex application.  Project team (Team A) decided to out-source part of this project to an external team (Team B). Let's say this external team needs to implement a farily complex algorithm to achieve a specific task, and which needs to interface with the rest of the application. Work on both parts of the application needs to proceed simultaneously.

Suppose the algorithm logic is implemented using a single method:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;```int complexAlgorithm(int number1, int number2);```

How do we ensure that the work done by both the teams remains compatible?

They start with defining an interface.

**_ComplexAlgorithm.java_**

```java
  
	package com.in28minutes.oops.level2.interfaces;

	public interface ComplexAlgorithm {
		int complexAlgorithm(int number1, int number2);
	}

```

Now the teams can go on their merry way. Team A can create a stub for the interface `OneComplexAlgorithm` and start working on their project.

**_OneComplexAlgorithm.java_**

```java

	package com.in28minutes.oops.level2.interfaces;

	public class OneComplexAlgorithm {
		public int complexAlgorithm(int number1, int number2) {
			return number1 + number2;
		}
	}

```

Team B can take time to implement the actual algorithm.

**_ActualComplexAlgorithm.java_**

```java

	package com.in28minutes.oops.level2.interfaces;

	public class ActualComplexAlgorithm {
		public int complexAlgorithm(int number1, int number2) {
			//Your complex implementation will be present here..
			return number1 * number2;
		}
	}

```

### Step 19: Interfaces - Puzzles And Interesting Facts
- - -  

Let's look at a few examples to understand interfaces further.


An ```interface``` can be extended by another ```interface```. We can have an inheritance hierarchy purely consisting of interfaces.

```java

	jshell> interface InterfaceOne {
	   ...> void methodOne();
	   ...> }
	| created interface InterfaceOne

	jshell> interface InterfaceTwo extends InterfaceOne {
	   ...> void methodTwo();
	   ...> }
	| created interface InterfaceTwo
```

An implementation of interface should implement all its methods including the methods in its super interfaces.

```java
	jshell> class Implementation implements InterfaceTwo {
	   ...>}
	| Error:
	| Implementation is not abstract and does not implement abstract method methodTwo() of 	InterfaceTwo
	| class Implementation implements InterfaceTwo {
	|^---------------------------------------------...

	jshell> public class Implementation implements InterfaceTwo {
	   ...> public void methodTwo() {}
	   ...> }
	| Error:
	| Implementation is not abstract and does not implement abstract method methodOne() of 	InterfaceOne
	| class Implementation implements InterfaceTwo {
	|^---------------------------------------------...

	jshell> public class Implementation implements InterfaceTwo {
	   ...> public void methodTwo() {}
	   ...> public void methodOne() {}
	   ...> }
	| created class Implementation
```

If a class is declared as abstract, it can skip providing implementations for all interface methods.
```java
	jshell> public abstract class AbstractImplementation implements InterfaceTwo {
	   ...> public void methodOne() {}
	   ...> }
	| created class AbstractImplementation
```

```interfaces``` cannot have member variables. An ```interface``` can only have declared **constants**

```java
	jshell> interface InterfaceThree {
	   ...> int test;
	   ...> }
	| Error:
	| = expected 
	| int test;
	|_________^

	jshell> interface InterfaceThree {
	   ...> int test = 5;
	   ...> }
	| created interface InterfaceThree
```

Starting from Java SE 8, an interface can provide a default implementation of the methods it provides.  It can be done by including the keyword ```default``` in the signature of that method, and providing a body to that method in its definition.


```java
	jshell> interface InterfaceFour {
	   ...> public default void print() {
	   ...> System.out.println("default print");
	   ...> }
	   ...> }
	| created interface InterfaceFour

	jshell> class TestPrint implements InterfaceFour {
	   ...> }
	| created class TestPrint


	jshell> TestPrint testPrint = new TestPrint();
	testPrint ==> TestPrint@6ebc05a6
	jshell> testPrint.print();
	default print
```

Implementations of ```interface``` can override the default method implementation.

```java
	jshell> class ParticularPrint implements InterfaceFour {
	   ...> public void print() {
	   ...> System.out.println("particular print");
	   ...> }
	   ...> }
	| created class ParticularPrint
```
```java
	jshell> ParticularPrint particularPrint = new ParticularPrint();
	particularPrint ==> ParticularPrint@5fad14c4
	jshell> particularPrint.print();
	particular print
	jshell>

```

No method declared inside an ```interface``` can be qualified with the ```private``` access specifier. However, an ```abstract class``` can have ```private``` methods declared within.


#### Why do we need ```default``` method implementations.

Let's consider a `Provider` interface with three implementations.

```java

	public interface Provider {
		public void doSomething();
	}

	public class ImplementorOne {
		@Override
		public void doSomething() {
			System.out.println("Do One");
		}
	}

	public class ImplementorTwo {
		@Override
		public void doSomething() {
			System.out.println("Do Two");
		}
	}

	public class ImplementorThree {
		@Override`
		public void doSomething() {
			System.out.println("Do Three");
		}
	}

```

What happens if a new method is added to the `interface`?

```java

	public interface Provider {
		public void doSomething();
		public void doMore();
	}

```

Compilation Error! All implementations classes ```ImplementationOne```, ```ImplementationTwo``` and ```ImplementationThree``` **must** me updated to implement ```doMore()``` in each case. 

Alternative : provide a default implementation for `doMore`.

```java

	public interface Provider {
		public void doSomething();
	
		public default void doMore(){
			System.out.println("Do More");
		}
	}

```

No other code needs to immediately change, and specific implementation classes can override this default version, as and when needed.

This is especially useful in building and extending frameworks. You are not breaking a user of your framework interface when you add new methods to the interface.

### Step 20:  ```abstract class``` And ```interface``` : A Comparison

```abstract class``` and ```interface``` are very different, except that they have a very similar syntax. 

When would you want to use them in your application?

#### interface

```interface``` is a **Contract**.

An ```interface``` is primarily used when you have two software components that need to communicate with each other, and there is a need to establish a contract. 

Recall the following example: `ComplexAlgorithm` defines the interface which helps both the teams involved.

```java

	package com.in28minutes.oops.level2.interfaces;
	public interface ComplexAlgorithm {
		int complexAlgorithm(int number1, int number2);
	}

```

#### abstract class

An ```abstract class``` is primarily used when you want to generalize behavior by creating a super class. 

Recall the following example we had discussed:

```java

	public abstract class AbstractRecipe {
		public void execute() {
			prepareIngredients();
			cookRecipe();
			cleanup();
		}

		abstract void prepareIngredients();
		abstract void cookRecipe();
		abstract void cleanup();
	}

```
 
#### Syntactical Comparison

Here are important syntactical differences:
* No method declared inside an ```interface``` can be qualified with a ```private``` access specifier. However, an ```abstract class``` can have ```private``` methods.
* An ```interface``` cannot have declared member variables. An ```abstract class``` can have member variable declarations.
* A ```class``` or an ```abstract class``` can implement multiple ```interface```s. But, an ```interface``` can extend only one ```interface```, and a ```class``` or an ```abstract class``` can extend only one ```class``` or ```abstract class```.

### Step 21: Programming Exercise PE-OOP-03

#### Exercises

TODO

#### Solution To PE-OOP-03

#### Solution - 1

#### Solution - 2

### Step 21: Introducing Polymorphism

TODO

# Introducing Collections

Arrays are not dynamic data structures. They can store only a fixed maximum number of elements.

Inserting or removing elements into an array needs a lot of work.

Collections are in-built implementations available to support dynamic data structures in Java programs. The commonly used collections are based on Lists, Trees and Hash Tables. 

Java provides very good collection implementations.

To make it simple to understand all collections, we will start with the interfaces - such as ```List```, ```Set```, ```Queue```, ```Map``` and others. 

After that, we will look at implementations of these interfaces, such as ```LinkedList```, ```HashTable``` and  ```TreeMap```, among others.

#### The Collection Interfaces

Let's start with the `List` interface

#### The ```List``` ```interface```

The ```List``` ```interface``` is used to implement an **ordered collection** in Java programs. An ordered collection is one, where the programmer has control over the position where an element can be inserted into, or accessed from the collection.

If an element's insertion position is not specified, it is added at the end of the ```List```.

A ```List``` typically allows *duplicate* elements. 
 
##### Snippet-1 : Creating a List

We can see examples of creating a list and accessing element data below:

```java

	jshell> List<String> words = List.of("Apple", "Bat", "Cat");
	words ==> [Apple, Bat, Cat]
	jshell> words.size()
	$1 ==> 3
	jshell> words.isEmpty()
	$2 ==> false
	jshell> words.get(0)
	$3 ==> Apple
	jshell> words.contains("Dog")
	$4 ==> false
	jshell> words.contains("Cat")
	$5 ==> true
	jshell> words
	words ==> [Apple, Bat, Cat]
	jshell> words.indexOf("Cat")
	$6 ==> 2
	jshell> words.indexOf("Dog")
	$7 ==> -1
	jshell>

```

#### ```List``` Immutability

Consider the ```List``` ```words``` we created in the last snippet.

```List<String> words = List.of("Apple", "Bat", "Cat");```

Lists created using the ```static``` ```of``` method are *immutable*.

```java

	jshell> List<String> words = List.of("Apple", "Bat", "Cat");
	words ==> [Apple, Bat, Cat]
	jshell> words.add("Dog");
	| java.lang.UnsupportedOperationExcetion thrown:
	| at ImmutableCollections.uoe (ImmutableCollections.java:71)
	| at ImmutableCollections$AbstractImmutableList.add (ImmutableCollections.java:77)
	| at (#15:1)
	jshell>

```

#### Creating A Mutable ```List```s

The way to create ```List``` data structures that can be updated over time, is to instantiate built-in ```collection``` classes that implement the ```List``` interface. 

Examples are ```ArrayList```, ```LinkedList``` and ```Vector```.

##### Snippet-3: Mutable Lists

Let's look at a few examples:

```java

	jshell> List<String> words = List.of("Apple", "Bat", "Cat");
	words ==> [Apple, Bat, Cat]

	jshell> List<String> wordsArrayList = new ArrayList<String>(words);
	wordsArrayList ==> [Apple, Bat, Cat]

	jshell> List<String> wordsLinkedList = new LinkedList<String>(words);
	wordsLinkedList ==> [Apple, Bat, Cat]

	jshell> List<String> wordsVector = new Vector<String>(words);
	wordsVector ==> [Apple, Bat, Cat]

	jshell> wordsArrayList.add("Dog");
	$1 ==> true

	jshell> wordsArrayList
	wordsArrayList ==> [Apple, Bat, Cat, Dog]

	jshell>

```

#### ```ArrayList``` vs ```LinkedList``` 

```ArrayList``` uses an array to store elements.
* Positional access and modification of elements is very efficient, with constant-time algorithmic complexity.
* Insertion and deletion of elements are expensive. In a 20 element list, to insert an element at first position, all 20 elements should be moved.

The data structure used to implement a ```LinkedList``` is of the type linked-list, which is a chain of blocks of memory slots.
* Inserting and Deleting values is easy. This is because in a chain of blocks, each link is nothing but a reference to the next block. Insertion only involves adjustment of these links to accommodate new values, and does not require extensive copying and shifting of existing elements.
* Positional access and modification of elements is less efficient than in an ```ArrayList```, because access always involves traversal of links.

Optimization: the underlying data structure for a ```LinkedList``` is actually a doubly-linked list, with each element having both forward and backward links to elements around it. 

#### ```Vector``` vs ```ArrayList```

```Vector``` has been with Java since v1.0, whereas ```ArrayList``` was added later, in v1.2. Both of them use an array as the underlying data structure. 

```Vector``` is thread-safe. In ```Vector```, all methods are ```synchronized```. 

> Look at other thread safe `List` implementations as `Vector` has poor concurrency.

#### ```List``` Operations
We will examine common ```List``` operations on an ```ArrayList```. Similar operations can also be done on a ```LinkedList``` or a ```Vector```.

##### Snippet-4 : List Insertions

We look at examples for
* Insertion at end (default)
* Positional insertion
* Inserting duplicate entries is allowed
* Adding all elements of an external list, to the current list
	* At the end
	* Positional insertion is also available, as in single element insertion

```java

	jshell> List<String> words = List.of("Apple", "Bat", "Cat");
	words ==> [Apple, Bat, Cat]
	jshell> List<String> wordsArrayList = new ArrayList<String>(words);
	wordsArrayList ==> [Apple, Bat, Cat]
	jshell> wordsArrayList.add("Dog");
	$1 ==> true
	jshell> wordsArrayList
	wordsArrayList ==> [Apple, Bat, Cat, **Dog**]
	jshell> wordsArrayList.add("Elephant");
	$2 ==> true
	jshell> wordsArrayList
	wordsArrayList ==> [Apple, Bat, Cat, Dog, **Elephant**]
	jshell> wordsArrayList.add(2, "Ball");
	*jshell> wordsArrayList
	wordsArrayList ==> [Apple, Bat, **Ball**, Cat, Dog, Elephant]
	jshell> wordsArrayList.add("Ball");
	jshell> wordsArrayList
	wordsArrayList ==> [Apple, Bat, Ball, Cat, Dog, Elephant, **Ball**]
	jshell> List<String> newList = List.of("Yak", "Zebra");
	newList ==> [Yak, Zebra]
	jshell> wordsArrayList.addAll(newList);
	$3 ==> true
	jshell> wordsArrayList
	wordsArrayList ==> [Apple, Bat, Ball, Cat, Dog, Elephant, Ball,  **Yak**, **Zebra**]
	jshell>

```


##### Snippet-5 : Element Modification

Let's look at examples of
* Modifying elements at a specific position.
* Deleting elements

```java

	jshell> wordsArrayList
	wordsArrayList ==> [Apple, Bat, Ball, Cat, Dog, Elephant, Ball,  Yak, Zebra]
	jshell> wordsArrayList.set(6, "Fish");
	$4 ==> "Ball"
	jshell> wordsArrayList
	wordsArrayList ==> [Apple, Bat, Ball, Cat, Dog, Elephant, **Fish**,  Yak, Zebra]
	jshell> wordsArrayList.remove(2);
	$5 ==> "**Ball**"
	jshell> wordsArrayList
	wordsArrayList ==> [Apple, Bat, Cat, Dog, Elephant, Fish,  Yak, Zebra]
	jshell> wordsArrayList.remove("Dog");
	$6 ==> true
	jshell> wordsArrayList
	wordsArrayList ==> [Apple, Bat, Cat, Elephant, Fish,  Yak, Zebra]
	jshell> wordsArrayList.remove("Dog");
	$6 ==> false
	jshell>

```

##### Snippet-6 : Iterating within ArrayList

Let's now look at how to iterate around the contents of a `List`

Basic for loop:

```java

	jshell> List<String> words = List.of("Apple", "Bat", "Cat");
	words ==> [Apple, Bat, Cat]
	jshell> for(int i=0; i<words.size(); i++) {
	...> System.out.println(words.get(i));
	...> }
	Apple
	Bat
	Cat
```

Using enhanced for loop:
```java
	jshell> for(String word:words) {
	...> System.out.println(word);
	...> }
	Apple
	Bat
	Cat
```

Using iterators:
```java
	jshell> Iterator wordsIterator = words.iterator();
	wordsIterator ==> java.util.AbstractList$Itr@3712b94
	jshell> while(wordsIterator.hasNext()) {
	...> System.out.println(wordsIterator.next());
	...> }
	Apple
	Bat
	Cat
```
#### Choosing Between Iteration Modes
- - - 

* For non-mutating iterations, an enhanced ```for``` loop is the most convenient
* For mutating iterations:
* Deletions: An enhanced ```for``` loop is not recommended, as we saw in the example. ```"Bat"``` was removed, but ```"Cat"``` was not, because the iteration itself was affected.
* Iterators can be used for such iterations.


##### Snippet-6

```java

	jshell> List<String> words = List.of("Apple", "Bat", "Cat");
	words ==> [Apple, Bat, Cat]
	jshell> List<String> wordsAL = new ArrayList<>(words);
	wordsAL ==> [Apple, Bat, Cat]
	jshell> for(String word:words) {
	  ...> if(word.endsWith("at"))
	   ...> System.out.println(word);
	   ...> }
	   ...> }
	Bat
	Cat
	jshell> for(String word:wordsAL) {
	   ...> if(word.endsWith("at"))
	   ...> wordsAL.remove(word);
	   ...> }
	   ...> }
	jshell> wordsAL
	wordsAL ==> [Apple, Cat]
	jshell> Iterator wordsIterator = wordsAL.iterator();
	wordsIterator ==> java.util.AbstractList$Itr@3712b94
	jshell> while(wordsIterator.hasNext()) {
	   ...> if(wordsIterator.next().endsWith("at")){
	   ...> wordsIterator.remove();
	   ...> }
	   ...> }
	jshell> wordsAL
	wordsAL ==> [Apple]
	jshell>

```

#### ```List``` : Type Safety

A ```List``` collection does not store primitives. It only stores object references. When we attempt to store primitive types, such as those of ```int```, ```char``` or ```double```, they get implicitly converted to their wrapper class types, namely ```Integer```, ```Character``` and ```Double``` respectively. Primitive data type elements get *auto-boxed*.

##### Snippet-7 : Type safety

The ```ArrayList.indexOf()``` method is not overloaded, there is only one version. SO, when passed an ```int``` argument, it is auto-boxed to an ```Integer``` object, and the method gets executed. 
* However, the ```ArrayList.remove()``` method has two overloaded versions:
	* ```ArrayList.remove(int index)``` : attempts to delete an element at the specified index in the ```ArrayList```
	* ```ArrayList.remove(Object o)``` : attempts to delete the specified element, if ti is present in the ```ArrayList	```.

```java

	jshell> List values = List.of("A", 'A', 1, 1.0);
	values ==> ["A", 'A', 1, 1.0]
	jshell> values.get(2)
	$1 ==> 1
	jshell> values.get(2) instanceof Integer
	$2 ==> true
	jshell> values.get(1) instanceof Character
	$3 ==> true
	jshell> values.get(3) instanceof Double
	$4 ==> true
	jshell> List<String> textValues = List.of("A", 'A', 1, 1.0);
	| Error
	| Error
	| List<String> textValues = List.of("A", 'A', 1, 1.0);
	|___________________________^------------------------^
	jshell> List<Integer> numbers = List.of(101, 102, 103, 104, 105);
	numbers ==> [101, 102, 103, 104, 105]
	jshell> numbers.indexOf(101)
	$5 ==> 0
	jshell> List<Integer> numbersAL = new ArrayList<>(numbers);
	numbersAL ==> [101, 102, 103, 104, 105]
	jshell> numbersAL.indexOf(101)
	$6 ==> 0
	jshell> numbersAL.remove(101)
	java.lang.IndexOutOfBoundsException!!
	jshell> numbersAL.remove(Integer.valueOf(101))
	$7 ==> true
	jshell> numbersAL
	numbersAL ==> [102, 103, 104, 105]
	jshell>

```

#### Sorting a ```List```

##### Snippet-8 : List sort

The ```List``` obtained from ```List.of()``` is immutable, hence cannot be sorted itself. Hence, create a mutable ```ArrayList``` out of it.

The ```ArrayList.sort()``` method requires the definition of a ```Comparator``` object. Easier option is to use ```Collections.sort()``` instead.



```java

	jshell> List<Integer> numbers = List.of(123, 12, 3, 45);
	numbers ==> [123, 12, 3, 45]
	jshell> List<Integer> numbersAL = new ArrayList<>(numbers);
	numbersAL ==> [123, 12, 3, 45]
	jshell> numbersAL.sort();
	| Error:
	| required: java.util.Comparator<? super java.lang.Integer>
	| numbersAL.sort();
	|^-------------^
	jshell> Collections.sort(numbersAL);
	jshell> numbersAL
	numbersAL ==> [3, 12, 45, 123]
	jshell>

```

#### Sorting List

##### Snippet-9 : Sorting List

Let's create a Student class and try to sort it using `Collections.sort`


**_Student.java_**

```java

	package collections;
	
	public class Student {
		private int id;
		private String name;
		
		public Student(int id, String name) {
			super();
			this.id = id;
			this.name = name;
		}

		public int getId() {
			return id;
		}

		public void setId(int id) {
			this.id = id;
		}

		public String getName() {
			return name;		
		}

		public void setName(String name) {
			this.name = name;
		}

		public String toString() {
			return id + " " + name;
		}
	}

```

**_StudentsCollectionRunner.java_**

```java

	package collections;
	import java.util.Collections;
	import java.util.List;
	import java.util.ArrayList;

	public class StudentsCollectionRunner {
		public static void main(String[] args) {
			List<Student> students = List.of(new Student(1, "Ranga"),
											new Student(100, "Adam"),
											new Student(2, "Eve"));
			ArrayList<Student> studentsAl = new ArrayList<>(students);
			System.out.println(studentsAl);
			Collections.sort(studentsAl);
			System.out.println(studentsAl);
		}
	}

```

**_Console Output_**

**_COMPILER ERROR_**

##### Snippet-9 Explained

To the method ```Collections.sort()```, only those ```List```s can be passed, the type of whose elements ```T```, implements the ```Comparator<? super T>``` ```interface```. 

```Student``` does not implement the interface. Result - Compilatino error.
##### Snippet-10 : Implementing Comparator Interface

**_StudentsCollection.java_**

```java

	package collections;
	import java.util.Comparable;

	public class Student implements Comparable<Student> {
		// Same as earlier
		@Override
		public int compareTo(Student that) {
			return Integer.compare(this.id, that.id);
		} 
	}

```

**_StudentsCollectionRunner.java_**

```java

	package collections;
	import java.util.Collections;
	import java.util.List;
	import java.util.ArrayList;

	public class StudentsCollectionRunner {
		public static void main(String[] args) {
			List<Student> students = List.of(new Student(1, "Ranga"),
											new Student(100, "Adam"),
											new Student(2, "Eve"));
			ArrayList<Student> studentsAl = new ArrayList<>(students);
			System.out.println(studentsAl);			
			Collections.sort(studentsAl);
			System.out.println(studentsAl);
		}
	}

```


**_Console Output_**

_[1 Ranga, 100 Adam, 2 Eve]_

_[1 Ranga, 2 Eve, 100 Adam]_

##### Snippet-10 Explained

`Integer.compare(x, y)`  returns the value 0 if x == y; a value less than 0 if x < y; and a value greater than 0 if x > y. 

If you change the order of parameters:

```java

	@Override
	public int compareTo(Student that) {
		return Integer.compare(that.id, this.id);
	}

``` 

Output changes to:

_[100 Adam, 2 Eve, 1 Ranga]_

#### The ```Comparator``` ```interface```

What if there is a need for sorting Student's in multiple ways? What if we want to sort Students in ascending order of id's in some situations and in descending order of id's in some other situations?

```Collections.sort``` has an overloaded version that has a signature that looks like:

```java

	@SuppressWarnings({"unchecked", "rawtypes" })
	public static <T> sort(List<T> list, Comparator<? super T> c)
		list.sort(c);
	}

``` 

To be able to invoke this version of ```Collections.sort```, we will need to define a suitable ```Comparator``` implementation, that works with ```Student``` objects.

As you may have already guessed, we would need to define two different ```Comparator``` implementations: one for ascending sort, and another for descending sort.

##### Snippet-11 : Implementing Student Comparators

```java

	package collections;
	import java.util.Collections;
	import java.util.List;
	import java.util.ArrayList;
	import java.util.Comparator;

	class DescStudentComparator implements Comparator<Student> {
		@Override
		public int compare(Student student1, Student student2) {
			return Integer.compare(student2.getId(), student1.getId());		
		}
	}

```

```java

	public class StudentsCollectionRunner {
		public static void main(String[] args) {
			List<Student> students = List.of(new Student(1, "Ranga"),
											new Student(100, "Adam"),
											new Student(2, "Eve"));
			ArrayList<Student> studentsAl = new ArrayList<>(students);
			System.out.println(studentsAl);			
			Collections.sort(studentsAl);
			System.out.println("Ascending : " + studentsAl);
			Collections.sort(studentsAl, new DescStudentComparator());
			System.out.println("Descending : " studentsAl);
		}
	}

```

**_Console Output_**

_[1 Ranga, 100 Adam, 2 Eve]_

_Ascending : [1 Ranga, 2 Eve, 100 Adam]_

_Descending : [100 Adam, 2 Eve, 1 Ranga]_

#### ```sort``` method Of ```List```

You can call `sort` method on the `List` by passing it a `Comparator` implementation - `studentsAl.sort(new AscStudentComparator())`.

##### Snippet-12 : Comparator for ArrayList.sort()


**_StudentsCollectionRunner.java_**

```java

	package collections;
	import java.util.Collections;
	import java.util.List;
	import java.util.ArrayList;
	import java.util.Comparator;

	public class StudentsCollectionRunner {
		public static void main(String[] args) {
			List<Student> students = List.of(new Student(1, "Ranga"),
											new Student(100, "Adam"),
											new Student(2, "Eve"));

			ArrayList<Student> studentsAl = new ArrayList<>(students);
			System.out.println(studentsAl);
			studentsAl.sort(new AscStudentComparator());
			System.out.println("Asc : " + studentsAl);			
			studentsAl.sort(new DescStudentComparator());
			System.out.println("Desc : " + studentsAl);
		}
	}

```

**_Console Output_**

_[1 Ranga, 100 Adam, 2 Eve]_

_Asc : [1 Ranga, 2 Eve, 100 Adam]_

_Desc : [100 Adam, 2 Eve, 1 Ranga]_

### The ```Set``` ```interface```

Mathematically, a set is a collection of unique items. Similarly, the Java ```Set``` ```interface``` also specifies a contract for collections having unique elements.
* If ```object1.equals(object2)``` returns ```true```, then only one of ```object1``` and ```object2``` have a place in a ```Set``` implementation.

There is no positional element access provided by the ```Set``` implementations.

##### Snippet-13 : Set

Let's look at a few examples:

The collection returned by ```Set.of()``` is immutable, hence does not support the ```add()```  method. 

```java

	jshell> Set<String> set = Set.of("Apple", "Banana", Cat");
	set ==> [Banana, Apple, Cat]
```


Create a ```HashSet``` collection instead, which supports the ```add()```, in order to test the uniqueness property of a ```Set```.



```java
	jshell> set.add("Apple");
	| java.lang.UnsupportedOperationException thrown:
	jshell> Set<String> hashSet = new HashSet<>(set);
	hashSet ==> [Apple, Cat, Banana]
```

The ```HashSet.add()``` operation returns a ```false``` value, indicating that inserting a duplicate "Apple" entry has failed.

```java
	jshell> hashSet.add("Apple");
	$1 ==> false
	jshell> hashSet
	hashSet ==> [Apple, Cat, Banana]
```


Note that when the ```hashSet``` was constructed using the ```set```, the order of the elements got permuted/changed. Also originally, when we created the ```set``` from the ```Set.of()``` method, the order printed was different from the order of initialization. This confirms the fact that a ```Set``` collection does not give any importance to element order, and therefore, does not support positional access. Hence, the compiler error on call to ```hashSet.add(int, String)```.


```java
	jshell> hashSet.add(2, "Apple");
	| Error:
	| no suitable method found for add(int, java.lang.String)
	| hashSet.add(2, "Apple");
	|^----------^
	jshell>

```

#### Understanding Data Structures

##### Hash Table
* Hash Table: A data structure that attempts to combine the best of both worlds:	
	* Very efficient element access
	* Very efficient element insertion and deletion 
* Buckets : They are the slots in the hash table, into which elements are inserted and chained together. As you can see, a hash table is effectively a large array of buckets, each containing a small linked list.
* Hashing: A procedure called **hashing** used in the construction of the Hash Table. The term **hash** generally means *mix up the order of elements*.
* Hashing Function: A formula to determine/compute which bucket a particular element gets inserted into. For illustration: ```hash(elem)``` could compute ```elem mod 13``` mathematically, and uses that value to index into the table, to locate the bucket insertion. The ```Object.hashCode()``` could be used as a hashing function.
* Collisions: Leads to chaining within a bucket, where a linked list grows. The larger the table, and the cleverer the hashing function, the lesser the chance for collisions.

##### Tree
* Tree: Stores elements in sorted order. For every node in the tree, elements of all nodes in its left sub-tree are lesser than its contained element. Conversely, elements of all nodes in its right sub-tree are greater than its contained element.
* Insertions: Given any node, we know by comparing the new element with the node's element, where to go about inserting it, to maintain sorted order.
* Access : More efficient than linked lists.

#### ```Set``` Implementations

* HashSet
* LinkedHashSet
* TreeSet

##### Snippet-14 : HashSet

In a ```HashSet```, elements are neither stored in the order of insertion, nor in sorted order.

```java

	jshell> Set<Integer> numbers = new HashSet<>();
	numbers ==> []
	jshell> numbers.add(765432);
	$1 ==> true
	jshell> numbers.add(76543);
	$2 ==> true
	jshell> numbers.add(7654);
	$3 ==> true
	jshell> numbers.add(765);
	$4 ==> true
	jshell> numbers.add(76);
	$5 ==> true
	jshell> numbers
	numbers ==> [765432, 7654, 76, 765, 76543]
	jshell>

```
##### Snippet-15 : LinkedHashSet

In a ```LinkedHashSet```, elements are stored in the order of insertion.

```java

	jshell> Set<Integer> numbers = new LinkedHashSet<>();
	numbers ==> []
	jshell> numbers.add(765432);
	$1 ==> true
	jshell> numbers.add(76543);
	$2 ==> true
	jshell> numbers.add(7654);
	$3 ==> true
	jshell> numbers.add(765);
	$4 ==> true
	jshell> numbers.add(76);
	$5 ==> true
	jshell> numbers
	numbers ==> [765432, 76543, 7654, 765, 76]
	jshell> numbers.add(7654321);
	$5 ==> true
	jshell> numbers
	numbers ==> [765432, 76543, 7654, 765, **7654321**]
	jshell>

```

##### Snippet-16 : TreeSet
- - - 

In a ```TreeSet```, elements are stored in sorted order.

```java

	jshell> Set<Integer> numbers = new TreeSet<>();
	numbers ==> []
	jshell> numbers.add(765432);
	$1 ==> true
	jshell> numbers.add(76543);
	$2 ==> true
	jshell> numbers.add(7654);
	$3 ==> true
	jshell> numbers.add(765);
	$4 ==> true
	jshell> numbers.add(76);
	$5 ==> true
	jshell> numbers
	numbers ==> [76, 765, 7654, 76543, 765432]
	jshell> numbers.add(7);
	$5 ==> true
	jshell> numbers
	numbers ==> [**7**, 76, 765, 7654, 76543, 765432]
	jshell>

```
#### Exercise Set

- - - 
1. Create a ```List`` of characters, such as:

	```List<Character> list = List.of('A', 'Z', 'A', 'B', 'Z, 'F);```

* Write a procedure to list out the unique characters in this list
* Write a procedure to list out these unique characters in sorted order
* Write a procedure to list out these unique characters in the order in which they were present in the original list 

#### Solution

**_SetRunner.java_**

```java

	package collections;
	import java.util.List;
	import java .util.Set;
	import java.util.HashSet;
	import java.util.LinkedHashSet;
	import java.util.TreeSet;

	public class SetRunner {
		public static void main(String[] args) {
			List<Character> characters = List.of('A', 'Z', 'A', 'B', 'Z, 'F);
			Set<Character> hashSetChars = new HashSet<>(characters);
			System.out.println("Unique Characters: " + hashSetChars);
			Set<Character> treeSetChars = new TreeSet<>(characters);
			System.out.println("Sorted Order: " + treeSetChars);			
			Set<Character> linkedSetChars = new LinkedHashSet<>(characters);
			System.out.println("Inserted Order: " + linkedSetChars);  
		}	
	}

``` 

**_Console Output_**

_Unique Characters: [A, B, F, Z]_

_Sorted Order: [A, B, F, Z]_

_Inserted Order: [A, Z, B, F]_

#### Solution Explained

In this example, the order to elements traversed in ```hashSetChars``` happened to be the same as that in ```treeSetChars```. Such an order is not always guaranteed, as we saw in the earlier examples.

#### ```TreeSet``` In Depth

* Super-Interfaces
	* Set
	* NavigableSet

##### Snippet-16 : NavigableSet Operations

Let's look at few operations:

```java

	jshell> TreeSet<Integer> numbers = new TreeSet<>(Set.of(65, 54, 34, 12, 99));
	numbers ==> [12, 34, 54, 65, 99]
	jshell> numbers.floor(40);
	$1 ==> 34
```
```floor()``` method is inclusive, ```lower()``` is exclusive

```java
	jshell> numbers.floor(34);
	$2 ==> 34
	jshell> numbers.lower(34);
	$3 ==> 12
```

```ceiling()``` method is inclusive, ```higher()``` is exclusive

```java
	jshell> numbers.ceiling(36);
	$4 ==> 54
	jshell> numbers.ceiling(34);
	$5 ==> 34
	jshell> numbers.higher(34);
	$6 ==> 54
```

```subSet(Object, Object)``` method is only lower-inclusive. So, the left bound is like ```lower()```, and right bound is like ```higher()```. The overloaded version ```subSet(Object, boolean, Object, boolean)``` can be used to configure lower- and upper inclusiveness of the returned subset.

```java
	jshell> numbers.subSet(20, 80);
	$7 ==> [34, 54, 65]
	jshell> numbers.subSet(34, 54);
	$8 ==> [34]
	jshell> numbers.subSet(34, 65);
	$9 ==> [34, 54]
	jshell> numbers.subSet(34, true, 65, true);
	$10 ==> [34, 54, 65]
	jshell> numbers.subSet(34, false, 65, false);
	$11 ==> [54]
```

```headSet()``` returns the subset of elements preceding the given element value. ```tailsSet()``` returns the subset of elements succeeding the given element value
```java
	jshell> numbers.headSet(50);
	$12 ==> [12, 34]
	jshell> numbers.tailSet(50);
	$13 ==> [54, 65, 99]
	jshell>

```

#### The ```Queue``` Interface

```Queue``` ```interface``` : ```extends``` the ```Collection``` ```interface```. 
* Elements are arranged in order of processing, such as in a To-Do List.

#### The ```PriorityQueue``` Collection

The ```PriorityQueue``` collection is a built-in Java ```class```, that ```implements``` the ```Queue``` ```interface```. Elements are stored in a sorted natural order, by default. We can also specify a different custom order, called the *order of priority* (customized by the programmer).

##### Snippet-17 : PriorityQueue

The ```PriorityQueue``` ```queue``` stores the strings in ascending alphabetic order by default. 

* ```queue.poll()``` de-queue's the element at the beginning of the natural order 


```java

	jshell> Queue<String> queue = new PriorityQueue<>();
	numbers ==> [12, 34, 54, 65, 99]
	jshell> queue.poll();
	$1 ==> null
	jshell> queue.offer("Apple");
	$2 ==> true
	jshell> queue.addAll(List.of("Zebra", "Monkey", "Cat"));
	$3 ==> true
	jshell> queue
	queue ==> [Apple, Cat, Monkey, Zebra]
	jshell> queue.poll();
	$4 ==> "Apple"
	jshell> queue
	queue ==> [Cat, Monkey, Zebra]
	jshell> queue.poll();
	$5 ==> "Cat"
	jshell> queue.poll();
	$6 ==> "Monkey"
	jshell> queue.poll();
	$7 ==> "Zebra"
	jshell> queue.poll();
	$8 ==> null
	jshell>

```

##### Snippet-18 : Custom Priority PriorityQueue

A custom priority order on the elements in a PriorityQueue can be specified by passing an implementation of ```Comparator<? super T>``` ```interface``` to the ```PriorityQueue<T>``` constructor. 

Let's implement a `StringLengthComparator`.

**_QueueRunner.java_**

```java

	package collections;
	import java.util.Comparator;
	import java.util.List;
	import java.util.Queue;
	import java.util.PriorityQueue;

	class StringLengthComparator implements Comparator<String> {
		@Override
		public int compare(String left, String right) {
			return Integer.compare(left.length(), right.length());
		}
	}

	public class QueueRunner {
		public static void main(String[] args) {
			Queue<String> queue = new PriorityQueue<>(new StringLengthComparator());
			queue.addAll(List.of("Zebra", "Monkey", "Cat"));
			queue.poll();
			queue.poll();
			queue.poll();
			queue.poll();
		}
	}

```

**_Console Output_**

_Cat_

_Zebra_

_Monkey_

_null_


#### The ```Map``` ```interface```
The ```Map``` ```interface``` specifies a contract to implement collections of elements, that are in the form of ```(key, value)``` pairs.  

Let's say you want to store how many times a character is repeated in a sequence of characters.
* If the sequence inserted is: ```{'A', 'C', 'A', 'C', 'E', 'C', 'M', 'D', 'H', 'A'}```
* The map contents would end up being: ```{('A', 3), ('C', 3), ('E', 1), ('M', 1), ('D', 1), ('H', 1)}```.

Since the kind of elements stored in a map (```(key, value)``` pairs)  are different from any other collection categories in Java, the ```Map``` ```interface``` is unique. So unique, that it even does not extend the ```Collection``` ```interface```! 

The ```interface``` definition looks something like:

```java

	public interface Map<K, V> {

		//Method Declarations

	}

```

* The Java collection classes that ```implement``` the ```Map``` ```interface``` are:
	* ```HashMap```
	* ```HashTable```
	* ```LinkedHashMap```
	* ```TreeMap```

#### ```Map``` Collections : Concepts

* ```HashMap```
	* Unordered
	* Unsorted
	* Key's ```hashCode()``` value is used in the hashing function
	* Allows a key with a ```null``` value.

* ```HashTable```
	* Thread-safe version of ```HashMap```. Has ```synchronized``` methods where required.
	* Unordered
	* Unsorted
	* Key's ```hashCode()``` value is used in the hashing function
	* Does not allow a ```null``` key.

* ```LinkedHashMap```
	* Insertion order of elements is maintained (which is optional as well)
	* Unsorted
	* Iteration is faster
	* Insertion and Deletion are slower

* ```TreeMap```
	* Additionally implements the ```NavigableMap``` ```interface```
	* Elements are maintained in sorted order of keys

#### ```Map``` ```interface``` : Basic Operations

##### Snippet-19 : Basic Map Operations

The ```Map.of()``` method takes a sequence of objects, which are interpreted as being key and value entries in alternation. 
* The total number of arguments is expected to be an even number. 
* This method creates an immutable ```Map```, with the ```(key, value)``` pairs in no specific order.


```java

	jshell> Map<String, Integer> map = Map.of("A", 3, "B", 5, "Z", 10);
	map ==> {Z=10, A=3, B=5}
	jshell> map.get("Z");
	$1 ==> 10
	jshell> map.get("A");
	$2 ==> 3
	jshell> map.get("C");
	$3 ==> null
	jshell> map.size();
	$4 ==> 3
	jshell> map.isEmpty();
	$5 ==> false
	jshell> map.containsKey("A");
	$6 ==> true
	jshell> map.containsKey("F");
	$7 ==> false
	jshell> map.containsValue(3);
	$8 ==> true
	jshell> map.containsValue(4);
	$9 ==> false
	jshell> map.keySet();
	$10 ==> [Z, A, B]
	jshell> map.values();
	$11 ==> [10, 3, 5]
	jshell>

```

##### Snippet-20 : Mutable Maps

To be able to add values to a map, let's create a `HashMap`.

```java

	jshell> Map<String, Integer> map = Map.of("A", 3, "B", 5, "Z", 10);
	map ==> {Z=10, A=3, B=5}
	jshell> Map<String, Integer> hashMap = new HashMap<>(map);
	hashMap ==> {A=3, Z=10, B=5}
	jshell> hashMap.put("F", 5);
	$1 ==> null
	jshell> hashMap
	hashMap ==> {A=3, Z=10, B=5, F=5}
	jshell> hashMap.put("Z", 11);
	$2 ==> 10
	jshell> hashMap
	hashMap ==> {A=3, Z=11, B=5, F=5}
	jshell>

```

#### ```Map``` Collections: Comparing Operations
##### Snippet-21 : ```Map``` Implementations

```HashMap``` elements are not guaranteed to be stored either in inserted order, or in the sorted order of keys.

```java

	jshell> HashMap<String, Integer> hashMap = new HashMap<>();
	hashMap ==> {}
	jshell> hashMap.put("Z", 5);
	$1 ==> null
	jshell> hashMap.put("A", 15);
	$2 ==> null
	jshell> hashMap.put("F", 25);
	$3 ==> null
	jshell> hashMap.put("L", 250);
	$4 ==> null
	jshell> hashMap
	hashMap ==> {A=15, F=25, Z=5, L=250}
```

```LinkedHashMap``` elements are stored in inserted order.
```java
	jshell> LinkedHashMap<String, Integer> linkedHashMap = new LinkedHashMap<>();
	linkedHashMap ==> {}
	jshell> linkedHashMap.put("Z", 5);
	$5 ==> null
	jshell> linkedHashMap.put("A", 15);
	$6 ==> null
	jshell> linkedHashMap.put("F", 25);
	$7 ==> null
	jshell> linkedHashMap.put("L", 250);
	$8 ==> null
	jshell> linkedHashMap
	hashMap ==> {Z=5, A=15, F=25, L=250}
```

```TreeMap``` elements are stored in the natural sorted order of the keys.


```java	
	jshell> TreeMap<String, Integer> treeMap = new TreeMap<>();
	treeMap ==> {}
	jshell> treeMap.put("Z", 5);
	$9 ==> null
	jshell> treeMap.put("A", 15);
	$10 ==> null
	jshell> treeMap.put("F", 25);
	$11 ==> null
	jshell> treeMap.put("L", 250);
	$12 ==> null
	jshell> treeMap
	treeMap ==> {A=15, F=25, L=250, Z=5}
	jshell>

```

#### Exercise Set
1. Given the string:  ```"This is an awesome occassion. This has never happened before."```, do the following processing on it:
	* Find the number of occurrences of each unique character in this string
	* Find the number of occurrences of each unique word in this string
#### Solution

**_MapRunner.java_**

```java

	package collections;
	import java.util.Map;
	import java.util.HashMap;

	public class MapRunner {
		public static void main(String[] args) {
			String str = "This is an awesome occassion. This has never happened before.";
			char[] characters = str.toCharArray();
			Map<Character, Integer> occurrences = new HashMap<>();
			for(char character:characters) {
				Integer count = occurrences.get(character);			
				if(count == null) {
					occurrences.put(character, 1);
				} else {
					occurrences.put(character, count+1);
				}
			}
			System.out.println(occurrences);
			String words = text.split(" ");
			Map<String, Integer> frequency = new HashMap<>();
			for(String word:words) {
				Integer number = frequency.get(word);
				if(number == null) {
					frequency.put(word, 1);
				} else {
					frequency.put(word, number+1);
				}
			}
			System.out.println(frequency);
		}
	}

```

#### Revisiting ```TreeMap```
Let's look at some more interesting operations of Data Structures based on ```TreeMap```.
##### Snippet-13 : Treemap Operations

Entries in a ```TreeMap``` are always sorted. 

```java

jshell> TreeMap<String, Integer> treeMap = new TreeMap<>();
treeMap ==> {}
jshell> treeMap.put("F", 25);
$1 ==> null
jshell> treeMap.put("Z", 5);
$2 ==> null
jshell> treeMap.put("L", 250);
$3 ==> null
jshell> treeMap.put("A", 15);
$4 ==> null
jshell> treeMap.put("B", 25)
$5 ==> null
jshell> treeMap.put("G", 25);
$6 ==> null
jshell> treeMap
treeMap ==> {A=15, B=25, F=25, G=25, L=250, Z=5}
```

`TreeMap` implements ```NavigableMap``` ```interface``` as well.

```java
jshell> treeMap.higherKey("B");
$7 ==> "F"
jshell> treeMap.higherKey("C");
$8 ==> "F"
jshell> treeMap.ceilingKey("B");
$9 ==> "B"
jshell> treeMap.ceilingKey("C");
$10 ==> "F"
jshell> treeMap.lowerKey("B");
$11 ==> "A"
jshell> treeMap.floorKey("B");
$12 ==> "B"
jshell> treeMap.firstEntry();
$713 ==> A=15
jshell> treeMap.lastentry();
$14 ==> Z=5
jshell> treeMap.subMap("C", "Y");
$7 ==> {F=25, G=25, L=250}
jshell> treeMap.subMap("B", "Z");
$7 ==> {B=25, F=25, G=25, L=250}
jshell> treeMap.subMap("B", true, "Z", true);
$7 ==> {B=25, F=25, G=25, L=250, Z=5}
jshell>

```

#### Java Collections : Conclusions With Tips

The collection interfaces we have explored, as well as their implementation classes, are:
* ```List```
* ```Set```
* ```Queue```
* ```Map```

Let's quickly review what we've learnt:
* When you use a "Hashed" Java collection (hash table based), such as ```HashMap``` or ```HashSet```, it will be unordered, unsorted and will iterate over its elements in no particular order.
* When you encounter a "Linked" Java collection (linked list based), such as a ```LinkedHashSet``` or a ```LinkedHashMap```, it will maintain insertion order, but will be unsorted. 
* When we make use of a "Tree"-based Java collection (stored in a tree data structure), such as ```TreeSet``` or ```TreeMap``` it always maintains natural sorted order. It would implement one of the navigable category of interfaces, such as ```NavigableSet``` or ```NavigableMap```.

## Introducing Generics

Recommended Videos
- Generics - https://www.youtube.com/watch?v=v4o0wyFPwEs

Why do we need Generics? 

Let's look at a scenario where want to write a wrapper class around the ```ArrayList``` data structure, maybe to do some better custom error-checking and stuff. For now, we will just look at basic wrapper functionality, the error checking intent is just an excuse!

##### Snippet-1

**_GenericsRunner.java_**

```java

	package com.in28minutes.generics;
	import com.in28minutes.generics.MyCustomList;
	
	public class GenericsRunner {
		public static void main(String[] args) {
		MyCustomList list = new MyCustomList();
		list.addElement("Element-1");
		list.addElement("Element-2");
		list.addElement("Element-3");
		}
	}

```


**_MyCustomList.java_**

```java

	package com.in28minutes.generics;

	public class MyCustomList {
		ArrayList<String> list = new ArrayList<>();
		
		public void addElement(String element) {
			list.add(element);
		}

		public void removeElement(String element) {
			list.remove(element);
		}
	}

```

##### Snippet-1 Explained

The ```MyCustomList``` ```class``` is a wrapper for ```ArrayList``` of ```String```s. Insertion and deletion of elements into this data structure is straightforward. 

Let's sy I would want to create `MyCustomList` for other types. Should we write additional wrapper classes ```MyCustomList``` and so on?

Let's look at an example:

##### Snippet-2 : Implementing a Generic

**_MyCustomList.java_**

```java

	package com.in28minutes.generics;
	
	public class MyCustomList<T> {
		ArrayList<T> list = new ArrayList<>();
		
		public void addElement(T element) {
			list.add(element);
		}

		public void removeElement(T element) {
			list.remove(element);
		}

		public String toString() {
			return list.toString();
		}
	}

```

**_GenericsRunner.java_**

```java

	package com.in28minutes.generics;
	import com.in28minutes.generics.MyCustomList;

	public class GenericsRunner {
		public static void main(String[] args) {
			MyCustomList<String> list = new MyCustomList<>();
			list.addElement("Element-1");			
			list.addElement("Element-2");
			System.out.println(list);			
			
			MyCustomList<Integer> list2 = new MyCustomList<>();			
			list2.addElement(Integer.valueOf(5));
			list2.addElement(Integer.valueOf(9));
			System.out.println(list2);
		}
	}

```

**_Console Output_**

_[Element-1, Element-2]_

_[5, 9]_

##### Snippet-2 Explained

The identifier ```T``` in the definition of the Generic ```class``` ```MyCustomList<T>``` is a placeholder for the actual type of the container. It is this placeholder that truly converts the ```MyCustomList``` ```class``` into a template.

The naming convention for these type placeholders is:
	* Always use UpperCase letters of the alphabet (such as ```T```, or ```S```), or
	* intuitive words such as ```TYPE```

At the time of actual instantiation of ```MyCustomList``` inside ```GenericsRunner.main```, this placeholder is substituted by the actual type:
* When ```MyCustomList<String> list``` is created, ```T``` is substituted by ```String```
* When ```MyCustomList<Integer> list2``` is created, ```T``` is substituted by ```Integer```

#### Exercise Set - 18
1. Write a method ```get``` inside the generic class ```MyCustomList```, which returns the element at a particular index (passed as argument) in its list storage.
#### Solution

**_MyCustomList.java_**

```java

	package com.in28minutes.generics;

	public class MyCustomList<T> {
		ArrayList<T> list = new ArrayList<>();
		
		public void addElement(T element) {
			list.add(element);
		}

		public void removeElement(T element) {
			list.remove(element);
		}

		public String toString() {
			return list.toString();
		}

		public T get(int index) {
			return list.get(index);
		}
	}

```

**_GenericsRunner.java_**

```java

	package com.in28minutes.generics;
	import com.in28minutes.generics.MyCustomList;

	public class GenericsRunner {
		public static void main(String[] args) {
			MyCustomList<String> list = new MyCustomList<>();
			list.addElement("Element-1");
			list.addElement("Element-2");			
			String text = list.get(0);
			System.out.println(text);

			MyCustomList<Integer> list2 = new MyCustomList<>();
			list2.addElement(Integer.valueOf(5));
			list2.addElement(Integer.valueOf(9));
			Integer num = list2.get(1);
			System.out.println(num);
		}
	}

```

**_Console Output_**

_Element-1_

_9_

#### Solution Explained

We have defined a method ```MyCustomList<T>.get``` whose return type is generic as well. The return type has the same placeholder ```T``` as the template in the definition of ```MyCustomList<T>```.
* For ```MyCustomList<String> list```, ```list.get``` returns a ```String```
* For ```MyCustomList<Integer> list2```, ```list2.get``` returns an ```Integer```

#### Implementing Type Restrictions on Generics

We saw above that we could use ```MyCustomList<T>``` to be instantiated into data structures for storing ```String```s as well as for ```Integer```s. 

What if we wanted to to use ```MyCustomList<T>``` purely for storing numeric values?	
##### Snippet-3 : Generic Type Restrictions	
**_MyCustomList.java_**	
```java	
	package com.in28minutes.generics;	
	public class MyCustomList<T extends Number> {	
		ArrayList<T> list = new ArrayList<>();	
			
		public void addElement(T element) {	
			list.add(element);	
		}	
		public void removeElement(T element) {	
			list.remove(element);	
		}	
		public String toString() {	
			return list.toString();	
		}	
		public T get(int index) {	
			return list.get(index);	
		}	
	}	
```	
**_GenericsRunner.java_**	
```java	
	package com.in28minutes.generics;	
	import com.in28minutes.generics.MyCustomList;	
	public class GenericsRunner {	
		public static void main(String[] args) {	
			//MyCustomList<String> list = new MyCustomList<>();	
			MyCustomList<Long> list1 = new MyCustomList<>();	
			list1.addElement(5l);	
			list1.addElement(7l);	
			Long long = list1.get(0);				
			System.out.println(long);	
			MyCustomList<Integer> list2 = new MyCustomList<>();	
			list2.addElement(Integer.valueOf(5));	
			list2.addElement(Integer.valueOf(9));	
			Integer num = list2.get(1);	
			System.out.println(num);	
		}	
	}	
```	
**_Console Output_**	
_5_	
_9_	
When we specify `T extends Number` as the type, we can use all the methods in the API of ```class``` ```Number``` are available for use. 	
#### Generic Methods	
We can create generic methods as well. Let's look at a few examples:	
##### Snippet-4 : Generic Method	
**_GenericsRunner.java_**	
```java	
	package com.in28minutes.generics;	
	import com.in28minutes.generics.MyCustomList;	
	public class GenericsRunner {	
		static <X> X doSomething(X value) {	
			return value;	
		}	
		static <X extends List> void duplicate(X list) {	
			list.add(list);	
		}	
		public static void main(String[] args) {	
			String text = doSomething("Hello");	
			Integer value = doSomething(Integer.valueOf(7));	
			ArrayList<String> list = doSomething(new ArrayList<String>(List.of("A", "B", C")));	
			duplicate(list);	
			System.out.println(list);				
			LinkedList<Integer> list2 = doSomething(new LinkedList<String>(List.of(1, 2, 3)));	
			duplicate(list2);	
			System.out.println(list2);	
		}	
	}	
```	
**_Console Output_**	
_[A, B, C, A, B, C]_	
_[1, 2, 3, 1, 2, 3]_	
#### Generics And Wild-Cards 	
You can use wild card with generics too - `? extends Number`	
##### Snippet-5	
**_GenericsRunner.java_**	
```java	
	package com.in28minutes.generics;	
	import com.in28minutes.generics.MyCustomList;	
	public class GenericsRunner {	
		static double sumOfNumberList(List<? extends Number> numbers) {	
			double sum = 0.0;				
			for(Number number:numbers) {	
				sum += number;	
			}	
			return sum;	
		}	
		public static void main(String[] args) {	
			System.out.println(sumOfNumberList(List.of(1, 2, 3, 4, 5)));	
			System.out.println(sumOfNumberList(List.of(1.1, 2.1, 3.1, 4.1, 5.1)));	
			System.out.println(sumOfNumberList(List.of(1l, 2l, 3l, 4l, 5l)));	
		}	
	}	
```	
**_Console Output_**	
_15.0_	
_15.5_	
_15.0_	
##### Snippet-5 Explained	
The symbol ```?``` in the definition of the method ```static double sumOfNumberList(List<? extends Number> numbers)``` is the **wild-card** symbol. It denotes the fact that in order to be a valid argument to ```sumOfNumberList```, ```numbers``` can be a ```List``` of any elements, so long as all of them are of type sub-classed from ```Number```. 	
* This includes ```Integer```, ```Long```, ```Short```, ```Byte```, ```Float``` and ```Double```. 	
* It also includes their primitive type counterparts, since they can be converted implicitly to their Wrapper class counterparts. 	
* Of course, all these elements of ```List``` ```numbers``` need to be of a homogeneous type.	
#### Restricted Heterogeneous Lists	
The generic wildcard we saw in the previous section is referred to as a **Upper-Bounded Wild-Card**. It can be used to specify homogeneous types with a restriction. There is another category of wild-cards called **Lower-Bounded Wild-Card**, which can be used with create **Heterogeneous** types of elements , within the restriction. Here is an example.	
##### Snippet-6 : More wild-cards	
**_GenericsRunner.java_**	
```java	
	package com.in28minutes.generics;	
	import com.in28minutes.generics.MyCustomList;	
	public class GenericsRunner {	
		static void addAFewNumbers(List<? super Number> numbers) {	
			numbers.add(1);	
			numbers.add(1l);	
			numbers.add(1.0);				
			numbers.add(1.0l);	
		}	
		public static void main(String[] args) {	
			List<Number> numberList = new ArrayList<>();	
			addAFewNumbers(numberList);	
			System.out.println(numberList);	
		}	
	}	
```	
**_Console Output_**	
_[1, 1, 1.0. 1.0]_	
## Introduction to Functional Programming	
What's all the fuss around Functional Programming about?	
Let's find out.	
Functional Programming Videos	
- Part 1 - https://www.youtube.com/watch?v=aFCNPHfvqEU 	
- Part 2 - https://www.youtube.com/watch?v=5Xw1_IREXQs	
### Step 01: Introducing Functional Programming	
Let's look at a typical program to loop around a list and print its content.	
##### Snippet-01 : OOP List Traversal 	
**_FunctionalProgrammingRunner.java_**	
```java	
	package com.in28minutes.functionalprogramming;	
	import java.util.List;	
	public class FunctionalProgrammingRunner {	
		public static void main(String[] args) {	
			List<String> list = List.of("Apple", "Banana", "Cat", "Dog");	
			for(String str:list) {	
				System.out.println(str);	
			}	
		}	
	}	
```	
**_Console Output_**	
_Apple_	
_Banana_	
_Cat_	
_Dog_	
##### Snippet-01 Explained	
Above approach focuses on the **how**.	
We looped around the list, accessed individual elements of a ```List``` and did  ```System.out.println()``` to print each element. 	
Functional Programming allows us to focus on the **what**.	
##### Snippet-02 : ```printBasic()``` And ```printFunctional()``` 	
**_FunctionalProgrammingRunner.java_**	
```java	
	package com.in28minutes.functionalprogramming;	
	import java.util.List;	
	public class FunctionalProgrammingRunner {	
		public static void main(String[] args) {	
			List<String> list = List.of("Apple", "Banana", "Cat", "Dog");	
			//printBasic(list);	
			printFunctional(list);	
		}	
		public static void printBasic(List<String> list) {	
			for(String str:list) {	
				System.out.println(str);	
			}	
		}	
		public static void printFunctional(List<String> list) {	
			list.stream().forEach(	
									element -> System.out.println(element)	
								 );										
		}	
	}	
```	
**_Console Output_**	
_Apple_	
_Banana_Cat_	
_Dog_	
##### Snippet-02 Explained	
`list.stream().forEach(element -> System.out.println(element))` - for each element in list stream, print it.	
```element -> System.out.println(element)``` is called a **lambda expression**.	
### Step 02: Looping Through A ```List```	
In the previous step , we use this snippet of code - `list.stream().forEach(element -> System.out.println(element))`	
We are **"Passing a function as a method argument"**. 	
Let's use JShell to explore this further.	
Let's try to print a list of numbers. 	
##### Snippet-01 : Loop Using FP	
```java	
	jshell> List<Integer> list = List.of(1, 4, 7, 9);	
	list ==> [1, 4, 7, 9]	
	jshell> list.stream().forEach(elem -> System.out.println(elem));	
	1	
	4	
	7	
	9	
	jshell>	
		
```	
##### Snippet-01 Explained	
`elem -> System.out.println(elem)` is a lambda expression. For each element in list stream, execute the lambda expression.	
### Step 03:  Filtering Results	
A ```Stream``` is a sequence of values. The ```filter()``` method can be used to filter the ```Stream``` elements based on some logic.	
  	
##### Snippet-01 : Using ```filter()```	
`printBasicWithFiltering` shows the usual approach of filtering.  `printFPWithFiltering` shows the functional approach.	
```java	
	package com.in28minutes.functionalprogramming;	
	import java.util.List;	
	public class FunctionalProgrammingRunner {	
		public static void main(String[] args) {	
			List<String> list = List.of("Apple", "Bat", "Cat", "Dog");	
			//printBasicWithFiltering(list);	
			printFPWithFiltering(list);	
		}	
		public static void printBasicWithFiltering(List<String> list) {	
			for(String str:list) {	
				if(str.endsWith("at")) {	
					System.out.println(str);	
				}	
			}	
		}	
		public static void printFPWithFiltering(List<String> list) {	
			list.stream()	
				.filter(elem -> elem.endsWith("at"))	
				.forEach(element -> System.out.println(element));	
		}		
	}	
```	
**_Console Output_**	
_Bat_	
_Cat_	
##### Snippet-02 : Printing even/odd numbers	
Let's look at how to filter numbers.	
```java	
	jshell> List<Integer> list = List.of(1, 4, 7, 9);	
	list ==> [1, 4, 7, 9]	
	jshell> list.stream().forEach(elem -> System.out.println(elem));	
	1	
	4	
	7	
	9	
	jshell> list.stream().filter(num -> num%2 == 1).forEach(elem -> System.out.println(elem));	
	1	
	7	
	9	
	jshell> list.stream().filter(num -> num%2 == 0).forEach(elem -> System.out.println(elem));	
	4	
	jshell>	
```	
##### Snippet-02 Explained	
Typically, these are the conditions we write	
* ```num``` is odd : ```if(num % 2 == 1) { /*  */ }```	
* ```num``` is even : ```if(num % 2 == 0){ /*  */ }```	
In the above example, we are using lambda expression to define the same conditions. 	
* ```num``` is odd: ```num -> num%2 == 1```	
* ```num``` is even: ```num -> num%2 == 0```	
### Step 05: Streams - Aggregated Results	
Sometimes we want to aggregate data into a single result. For example, we might want to add all the numbers between ```1``` and ```10```. Or we may want to calculate the average maximum temperature in our city over a month's time. 	
##### Snippet-01 : Sum Of A Sequence	
Let's look at how to use `reduce` method to calculation the sum.	
**_FPNumberRunner.java_**	
```java	
	package com.in28minutes.functionalprogramming;	
	import java.util.List;	
	public class FPNumberRunner {	
		public static void main(String[] args) {	
			List<Integer> numbers = List.of(4, 6, 8, 13, 3, 15);	
			//System.out.println(printBasicSum(numbers));	
			int sum = numbers.stream()	
							 .reduce( 	
									 0,	
									 (num1, num2) -> num1 + num2	
									);	
			System.out.println(sum);	
		}	
		void printBasicSum(List<Integer> numbers) {	
			int sum=0;	
			for(int num:numbers) {	
				sum += num;	
			}			
			System.out.println(sum);	
		}	
	}	
```	
**_Console Output_**	
_49_	
##### Snippet-01 Explained	
The ```reduce()``` method acts on a pair of elements at a time. The *initial-value* is  ```0```. The lambda expression `(num1, num2) -> num1 + num2` is executed on the elements of the list, a pair at a time.	
 	
#### Classroom Exercise CE-01	
1. Given the list ```(4, 6, 8, 13, 3, 15)```, compute:	
	* The sum of even numbers in the list.	
	* The sum of odd numbers in the list.	
#### Solution To CE-01	
**_FPNumberRunner.java_**	
```java	
	package com.in28minutes.functionalprogramming;	
	import java.util.List;	
	public class FPNumberRunner {	
		public static void main(String[] args) {	
			List<Integer> numbers = List.of(4, 6, 8, 13, 3, 15);	
			printFPEvenSum(numbers);				
			printFPOddSum(numbers);	
		}	
		void printFPEvenSum(List<Integer> numbers) {	
			int sum = numbers.stream()	
							 .filter(elem -> elem %2 == 0)	
							 .reduce(0, (num1, num2) -> num1 + num2);	
			System.out.println("Even Numbers Sum: " + sum);	
		}	
		void printFPOddSum(List<Integer> numbers) {	
			int sum = numbers.stream()	
							 .filter(elem -> elem %2 == 1)	
							 .reduce(0, (num1, num2) -> num1 + num2);	
			System.out.println("Odd Numbers Sum: " + sum);	
		}	
	}	
```	
**_Console Output_**	
_Even Numbers Sum: 18_	
_Odd Numbers Sum: 31_	
### Step 06: Functional Programming v Structured Programming	
Let's have a re-look at the **_FPNumberRunner.java_** program from the previous step. We wrote two variants of the same task that computed the sum of a list of numbers:	
* ```basicSum()```: that used the traditional approach	
* ```fpSum()``: which followed the *FP* scheme of things	
Let's use them as benchmarks, to illustrate the core differences between *SP* and *FP*. 	
1. **Structured Programming** (**SP**)	
```java	
	public int basicSum(List<Integer> numbers) {	
		int sum=0;	
		for(int num:numbers) {	
			sum += num;	
		}	
		return sum;	
	}	
```	
2. **Functional Programming** (**FP**)	
```java	
	public int  fpSum(List<Integer> numbers) {	
		int sum = numbers.stream()	
						 .reduce(0, (num1, num2) -> num1 + num2);	
		return sum;	
	}	
```	
How are these different?	
* **Mutations** (changes to program data):	
	1. *SP*: Within ```basicSum()```, the variable ```sum``` (a sort of worker variable) is initialized to ```0```, and undergoes *mutations* across iterations of the ```for``` loop. 	
	2. *FP*: We just set up an initial value for ```reduce()``` to work with. We don't have any mutation.	
* The **what** and **how** of computation:	
	1. *SP*: We specify both *what* to do, and *how* to do it. The code loops through the list elements using a ```for```, while also updating the aggregate value in ```sum```.	
	2. *FP*: We are focused on *what* to do, and very little on the *how* part. ```reduce()``` takes care of what numbers from the *stream* to add up, and you don't bother about how to select them from the *stream*. 	
### Step 07: Some FP Terminology 	
Let's look at some *FP* terminology a little more formally.	
#### Lambda Expression	
```java	
	(num1, num2) -> num1 + num2	
```	
is equivalent of this method	
```java	
	int basicSum(int num1, int num2) {		
		return num1 + num2;	
	}	
``` 	
A lambda expression can have multiple lines of Java code as well:	
```java	
	(num1, num2) -> {	
		System.out.println(num1 + " " + num2);	
		return num1 + num2;	
	}	
```	
Why take our word for all this? Let's put this code into an IDE, and then run it, to see for ourselves.	
##### Snippet-01 : Lambda Expression	
**_FPNumberRunner.java_**	
```java	
	package com.in28minutes.functionalprogramming;	
	import java.util.List;	
	public class FPNumberRunner {	
		public static void main(String[] args) {	
			List<Integer> numbers = List.of(4, 6, 8, 13, 3, 15);	
			System.out.println(numbers);	
			printFPSum(numbers);	
		}	
		void printFPSum(List<Integer> numbers) {	
			int sum = numbers.stream()	
							 .reduce(0,	
									 (num1, num2) -> {	
														System.out.println(num1 + " " + num2);	
														return num1 + num2;	
													 }	
			System.out.println("Even Numbers Sum: " + sum);			
		}	
	}	
```	
**_Console Output_**	
_[4, 6, 8, 13, 3, 15]_	
_0 4_	
_4 6_	
_10 8_	
_18 13_	
_31 3_	
_34 15_	
_49_	
#### Stream	
A Stream is a sequence of elements. You can perform different kinds of operations on a stream. 	
* **Intermediate Operations**: An operation that *takes a stream* - for example, applies a lambda expression - and produces *another stream* of elements as its result.	
* **Terminal Operations**: A stream operation that takes a stream - for example, applies a lambda expression -  and returns a single result (A single primitive-value/object, or a single collection-of-objects). ```reduce()``` and ```forEach()``` are a couple of such operations.	
### Step 08: Intermediate Stream Operations	
Output of an intermediate stream operation is another stream. 	
The most popular intermediate stream operations are: 	
* ```sorted()```	
* ```distinct()```	
* ```filter()```	
* ```map()```	
In this step, let's check them out one by one.	
##### Snippet-01 : ```sorted()``` and other operations	
```java	
	jshell> List<Integer> numbers = List.of(3, 5, 8, 213, 45, 4, 7);	
	numbers ==> [3, 5, 8, 213, 45, 4, 7]	
	jshell> numbers.stream().sorted().forEach(elem -> System.out.println(elem));	
	3	
	4	
	5	
	7	
	8	
	45	
	213	
	jshell> List<Integer> numbers = List.of(3, 5, 3, 213, 45, 5, 7);	
	numbers ==> [3, 5, 3, 213, 45, 5, 7]	
	jshell> numbers.stream().distinct().forEach(elem -> System.out.println(elem));	
	3	
	5	
	213	
	45	
	7	
	jshell> numbers.stream().distinct().sorted().forEach(elem -> System.out.println(elem));	
		
	3	
	5	
	7	
	45	
	213	
	jshell> numbers.stream().distinct().map(num -> num*num).forEach(elem -> System.out.println(elem));	
	9	
	25	
	45369	
	2025	
	49	
	jshell>	
```	
##### Snippet-01 Explained	
* ```sorted()``` preserves the elements of the consumed stream in the result, but also puts them in natural sorted order (Increasing order for numbers, alphabetical order for strings).	
* ```distinct()``` returns a stream retaining only the unique elements of the input stream. This method maintains the relative order of retained elements.	
* You can chain together more than one intermediate operation, such as ```sorted()``` followed by ```distinct()``` above. Such code is sometimes called a *pipeline*.	
*  ```map()``` : Applies a lambda expression to compute new results from the input stream elements. It then returns a stream of these results as output. In our example, ```map()``` takes each element in the ```Stream``` object created by ```number.stream()``,` to its square value.	
### Step 09: Programming Exercise FP-PE-01	
#### Exercises	
1. Write a program to print the squares of the first 10 positive integers.	
2. Create a list of the character strings "Apple", "Banana" and "Cat". Print all of them in lower-case.	
3. Create a list of the character strings "Apple", "Banana" and "Cat". Print the length of each string.	
#### Solutions To FP-PE-01	
**_FPNumberRunner.java_**	
```java	
	package com.in28minutes.functionalprogramming;	
	public class FPNumberRunner {	
		public static void printFPSquares() {	
			IntStream.range(1, 11).	
					  map(num -> num*num).	
					  forEach(elem -> System.out.println(elem));	
		}	
		public static void printLowerCases(List<String> list) {	
		}	
		public static void printLengths(List<String> list) {	
			list.stream()	
				.map(s -> s.length())	
				.forEach(elem -> System.out.println(elem);	
		}	
		public static void main(String[] args) {	
			printFPSquares();	
			List<String> list = List.of("Apple", "Banana", "Cat");	
			printLowerCases(list);			
			printLengths(list);	
		}	
	}	
```	
**_Console Output_**	
_1_	
_4_	
_9_	
_16_	
_25_	
_36_	
_49_	
_64_	
_81_	
_100_	
_apple_	
_banana_	
_cat_	
_5_	
_6_	
_3_	
#### Solution Explained	
* The ```map()``` method accepts a lambda expression.	
### Step 10:  Terminal Operations	
A terminal operation returns a single result (A single object/data-unit, or a single collection). It does not return an output stream.	
Commonly used instances of this are:	
* ```reduce()```	
* ```max()``` and ```min()```	
```java	
	jshell> IntStream.range(1, 11).reduce(0, (n1, n2) -> n1 + n2);	
	$1 ==> 55	
```	
```max()``` expects a lambda expression providing a ```Comparator<T>``` implementation.  ```Integer.compare(n1,n2)``` is an implementation of the ```Comparator<T>``` interface for comparing integers. 	

What if there are no numbers in the Stream? What should be returned? As a Java programmer, we grew up to hate `null`. You don't want to return `null` back.	

The ```Optional``` type provides an alternative: 	

* You can query an ```Optional``` object to check if it contains a valid result, by invoking ```isPresent()``` on it. 	
* You can get that result by calling ```get()``` on the same object.	


```java	
	jshell> List.of(23, 12, 34, 53).stream().max();	
	| Error:	
	| method max() in interface java.util.stream.Stream<T> cannot be applied to given types
	| required : java.lang.Comparator<? super java.lang.Integer>	
	| found : no argument	
	| List.of(23, 12, 34, 53).stream().max();	
	|^-----------------------------------^	
	jshell> List.of(23, 12, 34, 53).stream().max((n1, n2) -> Integer.compare(n1, n2));	
	$2 ==> Optional[53]	
	jshell> $2.isPresent()	
	$3 ==> true	
	jshell> List.of(23, 12, 34, 53).stream().max((n1, n2) -> Integer.compare(n1, n2)).get();	
	$4 ==> 53	
	jshell>	
```	
- - - 	
### Step 11: More Stream Operations	

Let's now play around with a few more terminal operations, such as ```min()``` (terminal operation), and ```filter()``` (intermediate operation). 

##### Snippet-01 : min() and max()	

Using ```min()``` is similar to ```max()```.	

```java	
	jshell> List.of(23, 12, 34, 53).stream().max((n1, n2) -> Integer.compare(n1, n2)).get()	
	$1 ==> 53	
	jshell> List.of(23, 12, 34, 53).stream().min((n1, n2) -> Integer.compare(n1, n2)).get()	
	$2 ==> 12	
	jshell>	
		
```	
##### Snippet-02 : Odd and Even Numbers	

```collect()``` method can be called to collect the result of ```filter()``` into a list. `Collectors.toList()` is the utility method used.

```java	
	jshell> List.of(23, 12, 34, 53).stream().filter(e -> e%2==1).forEach(e -> 	System.out.println(e))	
	23	
	53	
	jshell> List.of(23, 12, 34, 53).stream().filter(e -> e%2==1).collect(Collectors.toList());	
	$1 ==> [23, 53]	
	jshell>	
```	

#### Classroom Exercise FP-CE-02

1. From a list of 23, 12, 34, 53, create a list of the even numbers in it.	
2. Create a list of squares of the first 10 positive integers.	

#### Solutions To FP-CE-02	

**_FunctionalProgrammingRunner.java_**	
```java	
	package com.in28minutes.functionalprogramming;	
	public class FPNumberRunner {	
		public static void main(String[] args) {	
			List<Integer> numbers = List.of(23, 12, 34, 53);	
			List<Integer> evens = numbers.stream()	
										 .filter(n -> n%2==0)	
										 .collect(Collectors.toList());	
			List<Integer> tenSquares = IntStream.range(1, 11)	
												.map(n -> n*n)	
												.boxed()	
												.collect(Collectors.toList());	
		}	
	}	
```	
#### Solution Explained	
* Solution to #1 is straightforward, given that we already know how to use ```filter()```.	
* Solution #2 uses ```boxed()``` method to convert an ```IntPipeline``` to a ```Stream```. After that, what follows is routine stuff.	
### Step 12: The ```Optional<T>``` ```class```	
In an earlier section, we wrote and ran the following code:	
```java	
	jshell> List.of(23, 12, 34, 53).stream().max((n1, n2) -> Integer.compare(n1, n2));	
	Optional[53]	
	jshell>	
```	
In order to get the result in a form you would appreciate, we modified this code to look like:	
```java	
jshell> List.of(23, 12, 34, 53).stream().max((n1, n2) -> Integer.compare(n1, n2)).get();	
53	
jshell>	
```	
```max()``` is a stream operation, that needs to consume a stream. It is possible that the input stream is empty. In that case, the maximum value would be ```null```. It is undesirable in *FP* to encounter an exception during a stream operation. It is extremely inelegant if we are asked to handle an exception in an *FP* code pipeline. 	
The ```Optional<T>``` ```class``` was introduced in Java SE 8, as a lifeline in such situations. It covers the possibility of absence of (or ```null```) result from a terminal stream operation. The following example illustrates how you can query, and access the result from, an ```Optional<T>``` object. 	
```java	
	jshell> List.of(23, 45, 67, 12).stream().filter(num -> num % 2 == 0).max( (n1, n2) -> 	Integer.compare(n1, n2) )	
	$1 ==> Optional[12]	
	jshell> $1.get()	
	$2 ==> 12	
	jshell> $1.isPresent()	
	$3 ==> true	
```	
In case the result is empty, then the value stored in the result is not ```null```, it is ```Optional.empty```.	
```java	
	jshell> List.of(23, 45, 67).stream().filter(num -> num % 2 == 0).max( (n1, n2) -> 	Integer.compare(n1, n2) )	
	$4 ==> Optional.empty	
	jshell> $4.isPresent()	
	$5 ==> false	
	jshell> $4.orElse(0)	
	$6 ==> 0	
```	
You can provide a default value for the result using the method ```orElse()```.	
```java	
	jshell> List.of(23, 45, 67).stream().filter(num -> num % 2 == 0).max( (n1, n2) -> 	Integer.compare(n1, n2) ).orElse(0)	
	$7 ==> 0	
	jshell> List.of(23, 45, 67, 34).stream().filter(num -> num % 2 == 0).max( (n1, n2) -> 	Integer.compare(n1, n2) ).orElse(0)	
	$8 ==> 34	
	jshell>	
```	
### Step 13: Functional Interfaces : ```Predicate```	
When we define a lambda expression , a lot of things happen behind the scenes. 	
An important concept is a *functional interface*.	
Let's explain this term using an example. 	
The following code takes a behind-the-scenes look at ```filter()```.	
##### Snippet-01: Lambda behind-the-scenes - v1	
**_LambdaBehindTheScenesRunner.java_**	
```java	
	package com.in28minutes.functionalprogramming;	
	import java.util.List;	
	public class LambdaBehindTheScenesRunner {	
		public static void main(String[] args) {	
			List.of(23, 43, 34, 45).stream()	
								   .filter(num -> num%2 == 0)	
								   .forEach(e -> System.out.println(e));	
		}	
	}	
```	
**_Console Output_**	
_34_	
_36_	
_48_	
##### Snippet-01 Explained	
The signature of ```filter()``` reads is `Stream<T> java.util.stream.Stream.filter(Predicate<? super T> predicate)`.  In this case, ```T``` is ```java.lang.Integer```. 	
```filter()``` accepts an  object implementing the ```Predicate``` interface, as its argument. It returns a stream, consisting of those elements from the input stream, that match this predicate. 	
Conventionally speaking, a predicate is a logical condition. This predicate is applied to each element, to determine if it should be included in the output stream.	
The ```Predicate<T>``` ```interface is``` an example of a  *Functional Interface*. This interface has one method ```boolean test(T t)```. 	
		
Instead of `num -> num%2 == 0`, let's implement a `EvenNumberPredicate`.	
```java	
	@FunctionalInterface	
	public interface Predicate<? super T> {	
		boolean test(T t) { /*  */ }	
			//...	
		}	
	}	
		
```	
##### Snippet-02: lambda behind the scenes - v2	
**_LambdaBehindTheScenesRunner.java_**	
```java	
	package com.in28minutes.functionalprogramming;	
	import java.util.List;	
	import java.util.function.Predicate;	
	class EvenNumberPredicate implements Predicate<Integer> {	
		@Override	
		public boolean test(Integer number) {	
			return (number%2 == 0);	
		}	
	}	
	public class LambdaBehindTheScenesRunner {	
		public static void main(String[] args) {	
			List.of(23, 43, 34, 45, 36, 48).stream()	
										   .filter(new EvenNumberPredicate())	
										   .forEach(e -> System.out.println(e));	
		}	
	}	
```	
**_Console Output_**	
_34_	
_36_	
_48_	
##### Snippet-02 Explained	
```EvenNumberPredicate``` implements the ```Predicate<Integer>``` interface, and overrides the ```test()``` method.	
Something similar to ```EvenNumberPredicate``` is created when we use lambda expressions ```num -> num%2 == 0```.	
### Step 14: Functional Interfaces : ```Consumer```	
Let's look at another Functional Interface - ```Consumer<S>```.	
```forEach()``` on a stream is actually defined as - ```forEach(Consumer<? super S> action)```	
The ```Consumer<S>``` interface has the following definition:	
```java	
	@FunctionalInterface	
	public interface Consumer<? super S> {	
		void accept(S s) { /*  */ }		
		
		//...	
		
	}	
```	
The lambda expression used inside ```forEach()``` and other such stream operations, actually represent a `Consumer` implementation. 	
##### Snippet-01	
Let's implement a `SysOutConsumer`.	
**_FunctionalProgrammingRunner.java_**	
```java	
	package com.in28minutes.functionalprogramming;	
	import java.util.List;	
	import java.util.stream.Stream;	
	import java.util.function.Consumer;	
	import java.util.function.Predicate;	
	class EvenNumberPredicate implements Predicate<Integer> {	
		@Override	
		public boolean test(Integer num) {	
			return num%2 == 0;	
		}	
	}	
	class SysOutConsumer implements Consumer<Integer> {	
		@Override	
		public void accept(Integer num) {	
			System.out.println(num);	
		}	
	}	
	public class FPNumberRunner {	
		public static void main(String[] args) {	
			List<Integer> numbers = List.of(23, 12, 34, 45, 36, 48);	
			//List<Integer> evens = numbers.stream()	
										   .filter(n -> n%2==0)	
										   .collect(Collectors.toList());	
			List<Integer> evensToo = numbers.stream()	
										    .filter(new EvenNumberPredicate())	
											.collect(Collectors.toList());	
			numbers.stream()	
				   .filter(new EvenNumberPredicate())	
				   .forEach(new SysOutConsumer());	
		}	
	}	
```	
**_Console Output_**	
_12_	
_34_	
_36_	
_48_	
##### Snippet-01 Explained	
* The code actually speaks for itself. The steps to customize a ```Consumer<S>``` implementation are quote simple, and straightforward.	
* The final code that involves both a custom ```Predicate<T>```, and a custom ```Consumer<S>``` is still quite compact and elegant! 	
### Step 15: More Functional Interfaces	
Let's now look at what happens behind the scenes, for the stream operation ```map()```. Suppose we wanted to print out the squares of all even numbers in a given list.	
##### Snippet-01 : ```map()``` Behind The Scenes - v1	
```java	
	package com.in28minutes.functionalprogramming;	
	import java.util.List;	
	import java.util.stream.Stream;	
	import java.util.function.Consumer;	
	import java.util.function.Predicate;	
	class EvenNumberPredicate implements Predicate<Integer> {	
		@Override	
		public boolean test(Integer num) {	
			return num%2 == 0;	
		}	
	}	
	class SysOutConsumer implements Consumer<Integer> {	
		@Override	
		public void accept(Integer num) {	
			System.out.println(num);	
		}	
	}	
	public class FPNumberRunner {	
		public static void main(String[] args) {	
			List<Integer> numbers = List.of(23, 12, 34, 45, 36, 48);	
			numbers.stream()			
				   .filter(new EvenNumberPredicate())	
				   .map(n -> n*n)	
				   .forEach(new SysOutPredicate());	
		}	
	}	
```	
**_Console Output_**	
_1156_	
_1296_	
_2304_	
##### Snippet-01 Explained 	
The signature of the ```map()``` intermediate stream operation is :	
```java	
	<R> Stream<R> map(Function<?super T, ? extends R> mapper){}	
```	
```Function``` is shown below.	
```java	
	@FunctionalInterface	
	public interface Function<T,R> {	
		R apply(T t);	
	}	
```	
The method ```apply()``` accepts a ```T``` object as argument, and returns another object of type ```R```. In effect, any ```Function``` implementation can map object of one type to another.	
##### Snippet-02 : ```map()``` Behind The Scenes - v2	
Let's implement a `NumberSquareMapper`.	
```java	
	package com.in28minutes.functionalprogramming;		
	import java.util.List;	
	import java.util.stream.Stream;	
	import java.util.function.Consumer;	
	import java.util.function.Predicate;	
	import java.util.function.Function;	
	class EvenNumberPredicate implements Predicate<Integer> {	
		@Override	
		public boolean test(Integer num) {	
			return num%2 == 0;	
		}	
	}	
	class SysOutConsumer implements Consumer<Integer> {	
		@Override	
		public void accept(Integer num) {	
			System.out.println(num);	
		}		
	}	
	class NumberSquareMapper implements Function<Integer, Integer> {	
		@Override	
		public Integer apply(Integer number) {	
			return number * number;	
		}		
	}	
	public class FPNumberRunner {	
		public static void main(String[] args) {	
			List<Integer> numbers = List.of(23, 12, 34, 45, 36, 48);	
			numbers.stream()	
				   .filter(num -> num%2 == 0)	
				   .map(n -> n*n)	
				   .forEach(e -> System.out.println(e));	
			numbers.stream()	
				   .filter(new EvenNumberPredicate())	
				   .map(new NumberSquareMapper())	
				   .forEach(new SysOutPredicate());	
		}	
	}	
```	
**_Console Output_**	
_1156_	
_1296_	
_2304_	
**_1156_**	
**_1296_**	
**_2304_**	
### Step 16: Introducing Method References	
What is a method reference?	
Let's look at an example.	
##### Snippet-01: Method References - v1	
**_MethodReferencesRunner.java_**	
```java	
	package com.in28minutes.functionalprogramming;	
	import java.util.List;	
	public class MethodReferencesRunner {	
		public static void main(String[] args)	
			List.of("Ant", "Bat", "Cat", "Dog", "Elephant").stream()	
														   .map(s -> s.length())	
														   .forEach(l -> System.out.println(l));	
		}	
	}	
```	
**_Console Output_**	
_3_	
_3_	
_3_	
_3_	
_8_	
##### Snippet-02 : Method References - v2 	
Method references make it easy to create lambda expressions.	
`l -> System.out.println(l)` can be replaced with `System.out::println`.	
**_MethodReferencesRunner.java_**	
```java	
	package com.in28minutes.functionalprogramming;	
	import java.util.List;	
	public class MethodReferencesRunner {	
		public static void main(String[] args) {	
			List.of("Ant", "Bat", "Cat", "Dog", "Elephant").stream()	
														   .map(s -> s.length())	
														   .forEach(l -> System.out.println(l));	
			List.of("Ant", "Bat", "Cat", "Dog", "Elephant").stream()	
														   .map(s -> s.length())	
														   .forEach(System.out::println);	
		}	
	}	
```	
##### Snippet-03: Method References - v3	
Let's define a static method `print` and use it using a method reference.	
`MethodReferencesRunner::print` is same as `l -> MethodReferencesRunner.print(l)`	
**_MethodReferencesRunner.java_**	
```java	
	package com.in28minutes.functionalprogramming;	
	import java.util.List;	
	public class MethodReferencesRunner {	
		public static void print(Integer number) {	
			System.out.println(number);	
		}	
		public static void main(String[] args) {	
			List.of("Ant", "Bat", "Cat", "Dog", "Elephant").stream()	
														   .map(s -> s.length())	
														   .forEach(l -> MethodReferencesRunner.print(l));	
			List.of("Ant", "Bat", "Cat", "Dog", "Elephant").stream()	
														   .map(s -> s.length())	
														   .forEach(MethodReferencesRunner::print);	
		}	
	}	
```	
##### Snippet-04 : Method References - v4	
Instance method calls can also be replaced with their method references.	
On a `String`, `String::length` is the same as `s -> s.length()`.	
**_MethodReferencesRunner.java_**	
```java	
	package com.in28minutes.functionalprogramming;	
	import java.util.List;	
	public class MethodReferencesRunner {	
		public static void print(Integer number) {	
			System.out.println(number);	
		}	
		public static void main(String[] args) {	
			List.of("Ant", "Bat", "Cat", "Dog", "Elephant").stream()	
														   .map(s -> s.length())	
														   .forEach(MethodReferencesRunner::print);	
			List.of("Ant", "Bat", "Cat", "Dog", "Elephant").stream()	
														   .map(String::length)	
														   .forEach(MethodReferencesRunner::print);	
		}	
	}	
```	
#### Classroom Exercise FP-CE-03	
1. Using method references, write java functional code to determine the maximum even number,  in a given list of integers.	
#### Solution To FP-CE-03	
**_MethodReferencesRunner.java_**	
```java	
	package com.in28minutes.functionalprogramming;	
	import java.util.List;	
	public class MethodReferencesRunner {	
		public static void print(Integer number) {	
			System.out.println(number);	
		}	
		public static void main(String[] args) {	
			int max = List.of(23, 45, 67, 34).stream()			
											 .filter(num -> num % 2 == 0)	
											 .max( (n1, n2) -> Integer.compare(n1, n2) )	
											 .orElse(0);	
			System.out.println(max);	
			int maximum = List.of(23, 45, 67, 34).stream()				
												 .filter(MethodReferencesRunner::isEven)	
												 .max(Integer::compare)	
												 .orElse(0);	
			System.out.println(maximum);	
		}	
		public static booelan isEven(Integer number) {	
			return (number %2 == 0);	
		}	
	}	
```	
**_Console Output_**	
_34_	
**_34_**	
#### Summary	
In this step, we:	
* Understood what is a method reference	
* Learned that both built-in, and user defined class methods can be invoked using method references	
* Observed that method references work for static and non-static methods	
### Step 17: FP - Functions As First-Class Citizens 	
Are functions first class citizens in Java?	
Here are few questions to think about?	
* Can you pass a function as an argument to a method?	
* Can you assign a function to a variable?	
* Can you obtain a function as a return value, from a method invocation?	
#### Passing function as method argument	
We looked at several examples of this earlier.	
In the example below, `num -> num % 2 == 0` is passed to `filter` method.	
```	
int max = List.of(23, 45, 67, 34).stream()			
								 .filter(num -> num % 2 == 0)	
								 .max( (n1, n2) -> Integer.compare(n1, n2) )	
								 .orElse(0);	
```	
#### Storing functions in reference variables	
`evenPredicate` and `oddPredicate` represent functions.	
```java	
	package com.in28minutes.functionalprogramming;	
	import java.util.List;	
	import java.util.function.Predicate;	
	public class FPNumberRunner {	
		public static void main(String[] args) {	
			List<Integer> numbers = List.of(23, 12, 34, 45, 36, 48);	
			Predicate<? super Integer> evenPredicate = num -> num % 2 == 0;				
			Predicate<? super Integer> oddPredicate = num -> num % 2 == 1;	
			numbers.stream()	
				   .filter(evenPredicate)	
				   .map(n -> n*n)	
				   .forEach(e -> System.out.println(e));	
		}	
	}	
```	
**_Console Output_**	
_1156_	
_1296_	
_2304_	
#### Returning functions from methods	
`createEvenPredicate` and `createOddPredicate` are examples of methods returning functions.	
```java	
	import java.util.stream.Stream;	
	import java.util.function.Predicate;	
	public class FPNumberRunner {	
		public static Predicate<? super Integer> createEvenPredicate() {	
			return num -> num%2 == 0;	
		}	
		public static Predicate<? super Integer> createOddPredicate() {	
			return num -> num%2 == 1;	
		}	
		public static void main(String[] args) {	
			List<Integer> numbers = List.of(23, 12, 34, 45, 36, 48);	
			//Predicate<? super Integer> evenPredicate = num -> num % 2 == 0;	
			//Predicate<? super Integer> evenPredicate = createEvenPredicate();	
			numbers.stream()	
				   //.filter(num -> num%2 == 0)	
				   //.filter(evenPredicate)	
				   .map(n -> n*n)	
				   .forEach(e -> System.out.println(e));	
		}	
	}	
```	
**_Console Output_**	
_1156_	
_1296_	
_2304_	
#### Summary	
In this step, we observed that the following is true for a function:	
* It can be passed as a method argument	
* It can be stored in a reference variable	
* It can be  returned from a method	
## Threads and Concurrency	
So far, we've only seen programs that run like a single horse, running round a race course. 	
However, it often makes sense for a program's *main task* to be split into smaller ones (let's call them *sub-tasks*).  	
Imagine an ant-colony, where a large number of worker ants toil together, to complete what the Queen Ant tells them to do. Groups of ants that are part of separately tasks, work with a free hand.	
The concept of **concurrency** in programming is very similar to what an ant colony is in nature. 	
### Step 01: Concurrent Tasks: Extending ```Thread```	
In Java, you can run tasks in parallel using threads.  Let's first write a simple program.	
##### Snippet-1	
**_ThreadBasicsRunner.java_**	
```java	
	public class ThreadBasicsRunner {	
		public static void main(String[] args) {	
			//Task1	
			for(int i=101; i<=199; i++) {	
				System.out.print(i + " ");	
			}	
			System.out.println("\n Task1 Done");	
			//Task2	
			for(int i=201; i<=299; i++) {	
				System.out.print(i + " ");	
			}	
		
			System.out.println("\n Task2 Done");	
			//Task3	
			for(int i=301; i<=399; i++) {	
				System.out.print(i + " ");				
			}	
			System.out.println("\n Task3 Done");	
			System.out.println("Main Done");	
		}	
	}	
```	
**_Console Output_**	
_101 102 103 104 105 106 107 108 109 110 111 112 113 114 115 116 117 118 119 120 121 122 123 124 125 126 127 128 129 130 131 132 133 134 135 136 137 138 139 140 141 142 143 144 145 146 147 148 149 150 151 152 153 154 155 156 157 158 159 160 161 162 163 164 165 166 167 168 169 170 171 172 173 174 175 176 177 178 179 180 181 182 183 184 185 186 187 188 189 190 191 192 193 194 195 196 197 198 199_	
_Task1 Done_	
_201 202 203 204 205 206 207 208 209 210 211 212 213 214 215 216 217 218 219 220 221 222 223 224 225 226 227 228 229 230 231 232 233 234 235 236 237 238 239 240 241 242 243 244 245 246 247 248 249 250 251 252 253 254 255 256 257 258 259 260 261 262 263 264 265 266 267 268 269 270 271 272 273 274 275 276 277 278 279 280 281 282 283 284 285 286 287 288 289 290 291 292 293 294 295 296 297 298 299_	
_Task2 Done_	
_301 302 303 304 305 306 307 308 309 310 311 312 313 314 315 316 317 318 319 320 321 322 323 324 325 326 327 328 329 330 331 332 333 334 335 336 337 338 339 340 341 342 343 344 345 346 347 348 349 350 351 352 353 354 355 356 357 358 359 360 361 362 363 364 365 366 367 368 369 370 371 372 373 374 375 376 377 378 379 380 381 382 383 384 385 386 387 388 389 390 391 392 393 394 395 396 397 398 399_	
_Task3 Done_	
_Main Done_	
##### Snippet-1 Explained	
As you can see, the execution of all three ```for``` loops (that really are independent tasks) is sequential. This is how all our code so far has been running!	
### Thread Creation	
There are two ways in which you can create a thread to represent a sub-task, within a program. They are:	
* Define your own thread ```class``` to sub-class the **```Thread```** ```class```.	
* Define your own thread ```class``` to implement the **```Runnable```** ```interface```.	
In this step, we will focus on the first alternative.	
##### Snippet-01 : A simple Java thread class	
**_ThreadBasicsRunner.java_**	
```java	
	class Task1 extends Thread {	
		public void run() {	
			System.out.println("Task1 Started ");	
			for(int i=101; i<=199; i++) {	
				System.out.print(i + " ");	
			}	
			System.out.println("\nTask1 Done");	
		}		
	}	
	public class ThreadBasicsRunner {	
		public static void main(String[] args) {	
			//Task1	
			Task1 task1 = new Task1();	
			task1.start();	
			//Task2	
			for(int i=201; i<=299; i++) {	
				System.out.print(i + " ");	
			}	
			System.out.println("\nTask2 Done");	
			//Task3	
			for(int i=301; i<=399; i++) {	
				System.out.print(i + " ");	
			}	
			System.out.println("\nTask3 Done");	
			System.out.println("\nMain Done");	
		}		
	}	
```	
**_Console Output_**	
```	
Task1 Started 	
201 101 202 102 203 103 204 104 105 205 206 106 207 107 208 108 209 109 210 110 211 111 212 112 213 113 214 114 215 115 216 116 217 218 117 219 118 220 119 221 120 222 121 122 223 123 224 124 225 125 226 126 227 127 228 128 229 129 230 130 231 131 232 132 233 133 234 134 235 135 236 136 237 137 238 138 239 139 240 140 241 141 242 142 243 143 244 144 245 145 246 247 146 248 147 249 148 250 149 251 150 252 151 253 152 254 153 255 154 256 155 257 156 258 157 259 158 260 159 261 160 262 161 263 162 264 163 265 164 266 165 267 166 268 167 269 168 270 169 271 170 272 171 273 172 274 173 275 174 276 175 277 278 279 176 280 177 281 178 179 282 180 181 182 283 183 284 184 285 185 286 186 287 187 288 289 188 290 189 291 190 292 191 293 192 294 193 194 295 195 196 296 197 297 298 299 198 	
Task2 Done	
301 199 302 	
Task1 Done	
303 304 305 306 307 308 309 310 311 312 313 314 315 316 317 318 319 320 321 322 323 324 325 326 327 328 329 330 331 332 333 334 335 336 337 338 339 340 341 342 343 344 345 346 347 348 349 350 351 352 353 354 355 356 357 358 359 360 361 362 363 364 365 366 367 368 369 370 371 372 373 374 375 376 377 378 379 380 381 382 383 384 385 386 387 388 389 390 391 392 393 394 395 396 397 398 399 	
Task3 Done	
Main Done	
```	
##### Snippet-01 Explained	
We defined a ```Task1``` ```class``` to denote our sub-task, with a ```run()``` method definition. However,  when we create such a thread within our ```main()``` method, we don't seem to be invoking ```run()``` in any way! What's happening here? 	
A thread can be created and launched, by calling a generic method named ```start()```. method. Calling ```start()``` will invoke the individual thread’s ```run()``` method.	
From the console output, we see that the output of *Task1* overlaps with those of tasks labeled *Task2* and *Task3*. *Task1* is running in parallel with main which is running (*Task2*, *Task3*).	
#### Summary	
In this step, we:	
* Discovered how to define a thread by sub-classing ```Thread```	
* Demonstrated how to run a Thread	
### Step 02: Concurrent Tasks - Implementing Runnable	
##### Snippet-01 : Implementing Runnable	
In **Step 01**, we told you that there are two ways a thread could represent a sub-task, in a Java program. One was by sub-classing a ```Thread```, and the other way is to implement ```Runnable```. We saw the first way a short while ago, and it's time now to explore the second. The following example will show you how it's done.	
**_ThreadBasicsRunner.java_**	
```java	
	class Task1 extends Thread {	
		public void run() {	
			System.out.println("Task1 Started ");	
			for(int i=101; i<=199; i++) {	
				System.out.print(i + " ");	
			}	
			System.out.println("\nTask1 Done");	
		}	
	}	
	class Task2 implements Runnable {	
		@Override	
		public void run() {	
			System.out.println("Task2 Started ");	
			for(int i=201; i<=299; i++) {	
				System.out.print(i + " ");			
			}	
			System.out.println("\nTask2 Done");	
		}	
	}	
	public class ThreadBasicsRunner {	
		public static void main(String[] args) {	
			System.out.print("\nTask1 Kicked Off\n");	
			Task1 task1 = new Task1();	
			task1.start();	
			System.out.print("\nTask2 Kicked Off\n");	
			Task2 task2 = new Task2();	
			Thread task2Thread = new Thread(task2);	
			task2Thread.start();	
			System.out.print("\nTask3 Kicked Off\n");	
			for(int i=301; i<=399; i++) {	
				System.out.print(i + " ");	
			}	
			System.out.println("\nTask3 Done");	
			System.out.println("\nMain Done");	
		}	
	}	
```	
**_Console Output_**	
```	
Task1 Kicked Off	
Task1 Started 	
101 102 103 104 105 106 107 108 109 110 111 	
Task2 Kicked Off	
112 113 114 115 116 117 118 119 120 121 122 123 124 125 126 127 128 129 130 131 132 133 134 135 136 137 138 139 140 141 142 143 144 145 146 147 148 149 150 151 152 153 154 155 156 157 158 159 160 161 162 163 164 165 166 167 168 169 170 171 172 173 174 175 176 177 178 179 180 181 182 183 184 185 186 187 188 189 190 191 192 193 194 195 196 197 198 199 	
Task1 Done	
Task3 Kicked Off	
Task2 Started 	
201 202 203 204 205 206 207 208 209 210 211 212 213 301 214 215 216 217 218 302 219 220 221 222 223 224 225 226 227 228 303 229 230 231 232 233 234 235 236 237 238 239 240 241 242 243 244 245 246 247 248 249 250 251 252 253 254 255 256 257 258 259 260 261 262 263 264 265 266 267 304 268 269 270 271 272 273 274 275 276 277 278 279 280 281 282 283 284 285 286 305 287 288 289 290 291 292 293 294 295 296 297 298 299 	
Task2 Done	
306 307 308 309 310 311 312 313 314 315 316 317 318 319 320 321 322 323 324 325 326 327 328 329 330 331 332 333 334 335 336 337 338 339 340 341 342 343 344 345 346 347 348 349 350 351 352 353 354 355 356 357 358 359 360 361 362 363 364 365 366 367 368 369 370 371 372 373 374 375 376 377 378 379 380 381 382 383 384 385 386 387 388 389 390 391 392 393 394 395 396 397 398 399 	
Task3 Done	
Main Done	
```	
##### Snippet-01 Explained	
In this example, we implemented ```Runnable``` by implementing the ```run()``` method from ```Runnable``` interface.	
To run Task2 which is implementing `Runnable` interface, we used this code. We are using the `Thread` constructor passing an instance of `Task2`.	
```java	
Task2 task2 = new Task2();	
Thread task2Thread = new Thread(task2);	
task2Thread.start();	
```	
You can see from the output that all three tasks are running in parallel.	
#### Summary	
In this step, we:	
* Explored another way to create threads, by implementing the ```Runnable``` ```interface```	
* Learned to run a thread created using ```Runnable``` ```interface```	
 	
### Step 03: The Thread Life-cycle  	
A Java Thread goes through a sequence of **states** during its lifetime. The term **life-cycle** is used to describe this fact, and clearly defines what specific state a thread could be in, at various points of time. 	
Let's consider the following example we explored recently, in _**Step 02**_:	
```java	
	class Task1 extends Thread {	
		public void run() {	
			for(int i=101; i<=199; i++) {	
				System.out.print(i + " ");	
			}	
		}		
	}	
	class Task2 implements Runnable {	
		@Override	
		public void run() {	
			for(int i=201; i<=299; i++) {	
				System.out.print(i + " ");	
			}	
		}	
	}	
	public class ThreadBasicsRunner {	
		public static void main(String[] args) {	
			Task1 task1 = new Task1();	
			task1.start();	
			Task2 task2 = new Task2();	
			Thread task2Thread = new Thread(task2);	
			task2Thread.start();	
			for(int i=301; i<=399; i++) {				
				System.out.print(i + " ");	
			}	
		}	
	}	
```	
Different states of a thread are:	
* **NEW**: A thread is in this state as soon as it's been created, but its ```start()``` method hasn't yet been invoked.	
 	
	* For *Task1* : After the execution of ```Task1 task1 = new Task1();```	
	* For *Task2* : After the execution of ```Task2 task2 = new Task2();  task2Thread = new Thread(task2);```	
* **TERMINATED/DEAD**: When all the statements inside a thread's ```run()``` method have been been completed, that thread is said to have terminated.	
A thread can be in any one of the remaining three states, after its ```start()``` method has been invoked.	
 	
* **RUNNING**: If the thread is currently running.	
* **RUNNABLE**: If the thread is not currently running, but is ready to do so at any time.	
* **BLOCKED/WAITING**: If the thread is not currently running on the processor, but is not ready to execute either. This may be the case if it's waiting for an external resource (such as a user's input) or another thread.	
#### Summary	
In this step, we:	
* Discussed different states of a Thread with an example	
### Step 04: Thread Priorities	
Java allows you to *request* the thread scheduler, to change the priority of a thread. The priority of any thread always lies in a fixed range - ```MIN_PRIORITY = 1``` to ```MAX_PRIORITY = 10```.  The default priority that's assigned to any thread, is ```NORM_PRIORITY = 5```. 	
A request to change this priority is done by invoking the static ```setPriority(int)``` method, available in the ```Thread``` ```class```. This request may or may not be honored in response, so be prepared for that! 	
### Step 05: Communicating Threads	
Any program where threads are not explicitly created is a single-threaded application. The thread that we refer to here is the *main thread*, executing the program's ```main()``` method.	
Sometimes, threads might depend on one another. 	
Let consider the example from **Step 02**. We want to add a condition - *Task3* should execute only after *Task1* terminates.	
**_ThreadBasicsRunner.java_**	
```java	
	class Task1 extends Thread {	
		public void run() {	
			System.out.println("Task1 Started ");	
			for(int i=101; i<=199; i++) {	
				System.out.print(i + " ");	
			}	
		}	
	}	
	class Task2 implements Runnable {	
		@Override	
		public void run() {	
			System.out.println("Task2 Started ");	
			for(int i=201; i<=299; i++) {	
				System.out.print(i + " ");	
			}	
			System.out.println("\nTask2 Done");	
		}	
	}	
	public class ThreadBasicsRunner {	
		public static void main(String[] args) {	
			System.out.print("\nTask1 Kicked Off\n");	
			Task1 task1 = new Task1();			
			task1.start();	
			System.out.print("\nTask2 Kicked Off\n");	
			Task2 task2 = new Task2();	
			Thread task2Thread = new Thread(task2);	
			task2Thread.start();	
			
			task1.join();	
				
			System.out.print("\nTask3 Kicked Off\n");	
			for(int i=301; i<=399; i++) {	
				System.out.print(i + " ");	
			}	
			System.out.println("\nTask3 Done");	
			System.out.println("\nMain Done");	
		}	
	}	
```	
##### Snippet-5 Explained	
```task1.join()``` waits until task1 completes. So, the code after ```task1.join()``` will executed only on completion of `task1`.	
If we want *Task3* to be executed only after both *Task1* and *Task2* are done, the code in ```main()``` needs to look as follows:	
##### Snippet-6 : Task3 after Task1 and Task2	
**_ThreadBasicsRunner.java_**	
```java	
	public static void main(String[] args) {	
		System.out.print("\nTask1 Kicked Off\n");	
		Task1 task1 = new Task1();	
		task1.start();	
		System.out.print("\nTask2 Kicked Off\n");	
		Task2 task2 = new Task2();	
		Thread task2Thread = new Thread(task2);	
		task2Thread.start();	
		task1.join();	
		task2Thread.join();	
		System.out.print("\nTask3 Kicked Off\n");	
		for(int i=301; i<=399; i++) {	
			System.out.print(i + " ");	
		}	
		System.out.println("\nTask3 Done");	
		System.out.println("\nMain Done");	
			
	}	
```	
##### Snippet-6 Explained	
It is important to note that *Task1* and *Task2* are still independent sub-tasks. The thread scheduler is free to interleave their executions. However, *Task3* is kicked off only after both of them terminate.	
#### Summary	
In this step, we:	
* Understood the need for thread communication	
* Learned that Java provides mechanisms for threads to wait for each other	
* Observed how the ```join()``` method can be used to sequence thread execution	
  	
### Step 07: ```synchronized``` Methods, And ```Thread``` Utilities	
When a thread gets tired, you can put it to bed. Heck, you can do it even when it's fresh and raring to go! It's under your control, remember? 	
The ```Thread``` class provides a couple of methods:	
* ```public static native void sleep(int millis)``` : Calling this method will cause the thread in question, to go into a *blocked* / *waiting* state for **at least** ```millis``` milliseconds.	
* ```public static native void yield()``` : Request thread scheduler to execute some other thread. The scheduler is free to ignore such requests.	
##### Snippet-01 : Thread utilities	
**jshell>** ```Thread.sleep(1000)```	
**jshell>** ```Thread.sleep(10000)```	
**jshell>**	
##### Snippet-7 Explained	
* ```Thread.sleep(1000)``` causes the ```JShell``` prompt to appear after a delay of *at least* 1 second. This delay is even more visible, when we execute ```Thread.sleep(10000)```.	
### Step 08: Drawbacks of earlier approaches	
We saw few of the methods for synchronization in the `Thread` class	
* ```start()```	
* ```join()```	
* ```sleep()```	
* ```wait()```	
Above approaches have a few drawbacks:	
* **No Fine-Grained Control**: Suppose, for instance , we want *Task3* to run after *any one* of *Task1* or *Task2* is done. How do we do it?	
* **Difficult to maintain**: Imagine managing 5-10 threads with code written in earlier examples. It would become very difficult to maintain. 	
* **NO Sub-Task Return Mechanism**: With the ```Thread``` ```class``` or the ```Runnable``` ```interface```, there is no way to get the result from a sub-task.	
### Step 09: Introducing ```ExecutorService```	
In order to address the serious limitations of the ```Thread``` API, a new ```Executor Service``` was added in **Java SE 5**. 	
The ```ExecutorService``` is a framework you can use to manage threads in your code, better.  It has built-in ways to:	
* Create and launch threads more intuitively	
* Manage thread state and its life-cycle more easily	
* Synchronize between threads with more control, and	
* Handle groups of threads neatly	
The ```ExecutorService``` provides utilities to achieve each one of these. Let's start with thread creation, which the next example takes care of.	
##### Snippet-01 : Creating a Thread	
**_ExecutorServiceRunner.java_**	
```java	
	import java.util.concurrent.ExecutorService;	
	import java.util.concurrent.Executors;	
		
	class Task1 extends Thread {	
		public void run() {	
			System.out.println("Task1 Started ");	
			for(int i=101; i<=199; i++) {	
				System.out.print(i + " ");	
			}	
			System.out.println("\nTask1 Done");	
		}	
	}	
	class Task2 implements Runnable {	
		@Override	
		public void run() {	
			System.out.println("Task2 Started ");	
			for(int i=201; i<=299; i++) {	
				System.out.print(i + " ");	
			}	
			System.out.println("\nTask2 Done");	
		}	
	}	
	public class ExecutorServiceRunner {	
		public static void main(String[] args) {	
			ExecutorService executorService = Executors.newSingleThreadExecutor();	
			executorService.execute(new Task1());	
			executorService.execute(new Thread(new Task2()));	
		}	
	}	
```	
**_Console Output_**	
_Task1 Started_	
_101 102 103 104 105 106 107 108 109 110 111 112 113 114 115 116 117 118 119 120 121 122 123 124 125 126 127 128 129 130 131 132 133 134 135 136 137 138 139 140 141 142 143 144 145 146 147 148 149 150 151 152 153 154 155 156 157 158 159 160 161 162 163 164 165 166 167 168 169 170 171 172 173 174 175 176 177 178 179 180 181 182 183 184 185 186 187 188 189 190 191 192 193 194 195 196 197 198 199_	
_Task1 Done_	
_Task2 Started_	
_201 202 203 204 205 206 207 208 209 210 211 212 213 214 215 216 217 218 219 220 221 222 223 224 225 226 227 228 229 230 231 232 233 234 235 236 237 238 239 240 241 242 243 244 245 246 247 248 249 250 251 252 253 254 255 256 257 258 259 260 261 262 263 264 265 266 267 268 269 270 271 272 273 274 275 276 277 278 279 280 281 282 283 284 285 286 287 288 289 290 291 292 293 294 295 296 297 298 299_	
_Task2 Done_	
##### Snippet-01 Explained	
`ExecutorService executorService = Executors.newSingleThreadExecutor()` creates a single threaded executor service. That's why the tasks ran serially, one after the other.	
##### Snippet-02 : main runs in parallel	
Let's update the main method to do more things:	
```java	
	public class ExecutorServiceRunner {	
		public static void main(String[] args) {	
			ExecutorService executorService = Executors.newSingleThreadExecutor();	
			executorService.execute(new Task1());	
			executorService.execute(new Thread(new Task2()));	
			System.out.print("\nTask3 Kicked Off\n");	
			for(int i=301; i<=399; i++) {	
				System.out.print(i + " ");	
			}	
			System.out.println("\nTask3 Done");	
			System.out.println("\nMain Done");	
			executorService.shutdown();	
		}	
	}	
```	
**_Console Output_**	
```	
Task1 Started 	
101 	
Task3 Kicked Off	
102 301 103 302 104 303 105 304 106 305 107 306 108 109 110 111 112 307 113 114 115 116 117 118 119 120 121 122 308 123 309 124 310 125 311 126 312 127 313 128 314 129 315 130 316 131 132 133 317 134 318 135 319 136 137 320 138 321 139 322 140 323 141 324 142 325 143 326 144 145 146 147 327 148 149 328 150 329 151 330 152 331 332 153 154 155 156 157 158 159 160 161 162 163 164 165 166 167 168 169 170 171 172 173 174 175 176 177 178 179 180 181 182 183 184 185 186 187 188 189 190 191 192 193 333 194 334 195 196 335 197 198 199 336 	
Task1 Done	
337 338 Task2 Started 	
339 201 202 203 204 205 206 207 340 341 208 209 210 211 212 213 214 215 216 217 218 219 220 342 221 222 223 224 225 343 344 226 345 346 227 347 348 228 229 349 230 231 232 350 233 351 352 234 235 236 237 238 239 240 241 242 243 244 245 246 247 248 353 249 354 355 250 356 251 357 358 252 359 253 360 254 255 361 256 362 363 257 258 364 259 365 366 260 367 261 262 368 263 264 369 265 370 266 371 267 268 372 269 373 270 374 375 271 376 377 272 378 273 379 274 380 275 381 382 276 277 383 278 384 279 385 386 280 387 281 388 282 283 284 389 285 390 391 286 392 287 393 288 394 395 289 396 290 397 291 398 399 	
Task3 Done	
Main Done	
292 293 294 295 296 297 298 299 	
Task2 Done	
```	
##### Snippet-02 Explained	
The only order that we see in the resulting chaos is: *Task2* starts execution only after *Task1* is done.	
Threads managed by `ExecutorService` run in parallel with `main` method.	
### Step 10: Executor -  Customizing Number Of Threads	
With the ```ExecutorService```, it is possible to create a *pool* of threads.	
The following examples will show you how you can create thread pools of varying kinds, and of course, of different sizes. 	
##### Snippet-03 : Executors for Concurrent threads	
**_ExecutorServiceRunner.java_**	
```java	
	public class ExecutorServiceRunner {	
		public static void main(String[] args) {	
			ExecutorService executorService = Executors.newFixedThreadPool(2);	
			executorService.execute(new Task1());	
			executorService.execute(new Thread(new Task2()));	
			System.out.print("\nTask3 Kicked Off\n");	
			for(int i=301; i<=399; i++) {	
				System.out.print(i + " ");	
			}	
			System.out.println("\nTask3 Done");	
			System.out.println("\nMain Done");	
			executorService.shutdown();	
		}	
	}	
```	
**_Console Output_**	
```	
Task1 Started 	
Task3 Kicked Off	
301 101 302 303 304 Task2 Started 	
305 306 102 307 103 201 104 308 105 202 106 309 107 203 108 310 109 110 204 111 311 112 205 113 312 114 206 115 313 116 207 117 314 118 208 119 315 120 209 121 316 122 210 317 211 123 212 318 213 124 125 126 127 128 319 129 320 214 321 130 322 215 323 131 324 216 325 132 326 217 327 133 328 218 329 134 330 219 331 135 332 220 333 136 334 221 335 137 336 222 337 138 338 223 339 139 340 224 341 140 342 225 343 141 344 226 345 142 346 227 347 143 228 348 144 349 229 350 145 351 230 352 146 353 231 354 147 355 232 356 148 357 233 358 149 359 234 360 150 361 235 362 151 363 236 364 237 152 238 365 239 153 240 366 241 242 154 243 367 244 155 245 368 246 156 157 247 369 248 158 249 370 250 159 251 252 253 254 255 256 257 258 259 260 261 262 263 264 265 266 371 267 372 373 374 268 269 160 270 271 375 376 377 378 379 380 381 382 383 161 162 163 164 165 384 166 272 167 168 169 170 171 172 385 173 386 387 273 388 389 174 390 391 274 392 175 393 275 394 176 395 276 396 397 177 398 178 179 277 180 399 181 278 182 183 	
Task3 Done	
Main Done	
184 185 279 280 281 282 283 186 187 284 285 286 188 189 287 288 289 190 191 290 192 291 193 292 194 293 195 196 294 295 296 297 298 299 	
Task2 Done	
197 198 199 	
Task1 Done	
```	
##### Snippet-03 Explained	
We created `ExecutorService` by using `Executors.newFixedThreadPool(2)`. So, 'ExecutorService` uses two parallel threads at a maximum.	
* *Task1* and *Task2* execute concurrently as part of the ```ExecutorService```, and	
* The thread running ```main()``` executes concurrently with this thread pool, created by ```ExecutorService```.	
##### Snippet-04 : All-Executor Task Execution	
Let's create a simple example to allow to play with 'ExecutorService'.	
**_ExecutorServiceRunner.java_**	
```java	
	import java.util.concurrent.ExecutorService;	
	import java.util.concurrent.Executors;	
	class Task extends Thread {	
		private int number;	
			
		public Task(int number) {	
			this.number = number;	
		}	
		public void run() {	
			System.out.println("Task " + number + " Started");	
			for(int i=number*100; i<=number*100+99; i++) {	
				System.out.print(i + " ");	
			}	
			System.out.println("\nTask " + number +" Done");	
		}	
	}	
	public class ExecutorServiceRunner {	
		public static void main(String[] args) {	
			ExecutorService executorService = Executors.newFixedThreadPool(2);	
			executorService.execute(new Task(1));	
			executorService.execute(new Task(2));	
			executorService.execute(new Task(3));	
			executorService.shutdown();	
		}	
	}	
```	
##### Snippet-04 Explained	
`Executors.newFixedThreadPool(2)` - Two threads in parallel. The thread ```new Task(3)``` is executed only after any one of ```new Task(1)``` and ```new Task(2)``` have completed their execution.	
##### Snippet-04 : Larger Thread Pool Size	
```java	
	public class ExecutorServiceRunner {	
		public static void main(String[] args) {	
			ExecutorService executorService = Executors.newFixedThreadPool(3);	
			executorService.execute(new Task(1));	
			executorService.execute(new Task(2));	
			executorService.execute(new Task(3));	
			executorService.execute(new Task(4));	
			executorService.execute(new Task(5));	
			executorService.execute(new Task(6));	
			executorService.execute(new Task(7));	
			executorService.shutdown();	
		}	
	}	
```	
##### Snippet-04 Explained	
We made the pool larger to 3:	
* Initially Tasks ```1```, ```2```, ```3``` are added to the ```ExecutorService``` and are started.	
* As soon as any one of them is terminated, another task from the thread pool is picked up for execution, and so on. A classic case of musical chairs, with regard to the slots available in the ```ExecutorService``` thread pool, is played out here!	
#### Summary	
In this step, we:	
* Explored how one can create pools of threads of the same kind, using the ```ExecutorService```	
* Noted how one could specify the size of a thread pool	
### Step 11:  ```ExecutorService```: Returning Values From Tasks	
##### Snippet-01: Returning a Future Object	
So far, we have only seen sub-tasks that are largely independent, and which don't return any result to the main program that launched them.	
To be able to return a value from a Thread, Java provides a ```Callable<T>``` interface.	
The next example tells you how to implement ```Callable<T>```, and use it with ```ExecutorService```.	
**_ExecutorServiceRunner.java_**	
```java	
	import java.util.concurrent.ExecutorService;	
	import java.util.concurrent.Executors;	
	import java.util.concurrent.Callable;	
	class CallableTask implements Callable<String> {	
		private String name;	
		public CallableTask(String name) {	
			this.name = name;	
		}	
		@Override	
		public String call() throws Exception {	
			Thread.sleep(1000);	
			return "Hello " + name;	
		}	
	}	
	public class CallableRunner {	
		public static void main(String[] args) throws InterruptedException, ExecutionException {	
			ExecutorService executorService = Executors.newFixedThreadPool(1);	
			Future<String> welcomeFuture = executorService.submit(new CallableTask("in28Minutes"));	
			System.out.println("CallableTask in28Minutes Submitted");	
			String welcomeMessage = welcomeFuture.get();	
			System.out.println(welcomeMessage);	
			executorService.shutdown();	
		}	
	}	
```	
**_Console Output_**	
_CallableTask in28Minutes Submitted_	
_Hello in28Minutes_	
##### Snippet-01 Explained	
- `class CallableTask implements Callable<String>` - Implement `Callable`. Return type is `String`	
- `public String call() throws Exception {` - Implement `call` method and return a `String` value back.	
-  ```executorService.submit(new CallableTask(String))``` adds a callable task to its thread pool. This puts the task thread in a **RUNNABLE** state. Subsequently, the program goes ahead to invoke its ```call()``` method.	
- `welcomeFuture.get()` - Ensures that the `main` thread waits for the result of the operation. 	
#### Summary	
In this step, we:	
* Understood the need for a mechanism, to create sub-tasks that return values	
* Discovered that Java has a ```Callable<T>``` interface to do exactly this	
* Saw that the ```ExecutorService``` is capable of managing ```Callable``` threads	
### Step 11: Executors - Waiting For Many Callable Tasks To Complete	
```ExecutorService``` framework also allows you to create a pool of ```Callable``` threads. Not only that, you can collect their return values together.	
##### Snippet-01 : Waiting for Multiple ```Callable``` Threads 	
**_MultipleCallableRunner.java_**	
```java	
	import java.util.concurrent.ExecutorService;	
	import java.util.concurrent.Executors;	
	import java.util.concurrent.Callable;	
	class CallableTask implements Callable<String> {	
		private String name;	
		public CallableTask(String name) {	
			this.name = name;	
		}	
		@Override	
		public String call() throws Exception {	
			Thread.sleep(1000);	
			return "Hello " + name;	
		}	
	}	
	public class MultipleCallableRunner {	
		public static void main(String[] args) throws InterruptedException, ExecutionException {	
			ExecutorService executorService = Executors.newFixedThreadPool(1);	
			List<CallableTask> tasks = List.of(new CallableTask("in28Minutes"),	
												new CallableTask("Ranga"),	
												new CallableTask("Adam"));	
			List<Future<String>> welcomeAll = executorService.invokeAll(tasks);	
			for(Future<String> welcomeFuture : welcomeAll) {	
				System.out.println(welcomeFuture.get());	
			}	
			executorService.shutdown();	
		}	
	}	
```	
**_Console Output_**	
_Hello in28Minutes_	
_Hello Ranga_	
_Hello Adam_	
##### Snippet-01 Explained	
The ```invokeAll()``` method of  ```ExecutorService``` allows for a list of ```Callable``` tasks to be launched in the thread pool. Also, a ```List``` of ```Future``` objects can be used to hold return values, one for each such ```Callable``` thread.	
The list of return values can be accessed only after **all** the threads are done, and have returned their results. 	
This can be verified from the console output. all the planned welcome messages are printed in one go, but only after a wait of at least ```3000``` milliseconds has been completed.	
Let's now see what scenario would pan out with a larger thread pool size. 	
##### Snippet-02 : List of Callable tasks with larger thread pool	
```java	
	public class MultipleCallableRunner {	
		public static void main(String[] args) throws InterruptedException, ExecutionException {	
			ExecutorService executorService = Executors.newFixedThreadPool(3);	
			List<CallableTask> tasks = List.of(new CallableTask("in28Minutes"),	
												new CallableTask("Ranga"),	
												new CallableTask("Adam"));	
			List<Future<String>> welcomeAll = executorService.invokeAll(tasks);	
			for(Future<String> welcomeFuture : welcomeAll) {	
				System.out.println(welcomeFuture.get());	
			}	
			executorService.shutdown();	
		}	
	}	
```	
**_Console Output_**	
_Hello in28Minutes_	
_Hello Ranga_	
_Hello Adam_	
##### Snippet-02 Explained	
The welcome messages all get printed in a batch again, but their collective wait gets shorter. This is because:	
* The thread pool size is now ```3```, not ```2``` as earlier. This means all the three tasks can be put in the **RUNNABLE** state at once. 	
* Then, they go into their **BLOCKED** state also almost simultaneously, which means their collective wait time is much less than ```3000``` milliseconds. That's one advantage of a larger thread pool!	
#### Summary 	
In this step, we:	
* Learned that it's possible to collect the return values of a pool of ```Callable``` threads, at one go.	
* This is done using the ```invokeAll()``` method for their launch, and specifying a ```List``` of ```Future``` objects to hold these results	
* Changing the thread pool size for such scenarios can change response time dramatically	
### Step 12:  Executor - Wait Only For The Fastest Task	
Let's look at how you can wait for any of the three tasks to complete.	
##### Snippet-01 : Wait only for fastest	
```java	
	public class MultipleAnyCallableRunner {	
		public static void main(String[] args) throws InterruptedException, ExecutionException {	
			ExecutorService executorService = Executors.newFixedThreadPool(3);	
			List<CallableTask> tasks = List.of(new CallableTask("in28Minutes"),	
												new CallableTask("Ranga"),	
												new CallableTask("Adam"));	
			String welcomeMessage = executorService.invokeAny(tasks);	
			System.out.println(welcomeMessage);	
			executorService.shutdown();	
		}	
	}	
```	
**_Console Output_**	
_Hello Ranga_	
**_Console Output_**	
_Hello in28Minutes_	
**_Console Output_**	
_Hello Ranga_	
**_Console Output_**	
_Hello Adam_	
##### Snippet-01 Explained	
The method ```invokeAny()``` returns when the first of the sub-tasks is done. Also, the returned value is not a ```Future``` object. It's the return value of the ```call()``` method.	
We can see that over different executions, the order of console output changes. This is because: 	
* All three tasks are created together, in a thread pool of size ```3```. 	
* Therefore, these are independent threads, going into their **RUNNABLE** states almost at once. 	
#### Summary	
In this step, we:	
* Learned that ```ExecutorService``` has a way to return the first result, from a poll of ```Callable``` threads	
## Introduction To Exception handling	
Recommended Exception handling Videos	
- https://www.youtube.com/watch?v=34ttwuxHtAE	
There are two kinds of errors a programmer faces:	
* **Compile-time** Errors: Flagged by the compiler when it detects syntax or semantic errors.	
* **Run-time** Errors: Detected by the run-time environment when executing code	
Example runtime errors include:	
* Running out of *heap-memory* for objects, or space for the method *call stack*	
* Dividing a number by ```0```	
* Trying to *read* from an *unopened* file	
Exceptions are *unexpected* conditions; their occurrence does not make a programmer bad (or good, for that matter). It is a programmer's responsibility to be *aware* of potential exceptional conditions in her program, and use a mechanism to *handle* them effectively.	
Handling an exception generally involves two important aims:	
1. Provide a useful message to the end user.	
2. Log enough information to help a programmer identify root cause.	
### Step 01: Introducing Exceptions	
In the previous step, we gave you a few instances of exceptions, such as your program running out of memory, or your code trying to divide a number by ```0```. 	
Want to see a live example of the Java run-time throwing an exception? The next example will satisfy your thirst.	
##### Snippet-1 : Exception Condition	
**_ExceptionHandlingRunner.java_**	
```java	
	package com.in28minutes.exceptionhandling;	
		
	public class ExceptionHandlingRunner {	
		public static void main(String[] args) {	
			callMethod();	
			System.out.println("callMethod Done");			
		}	
		static void callMethod() {	
			String str = null;	
			int len = str.length();	
			System.out.println("String Length Done");	
		}			
	}		
```	
**_Console Output_**	
**_java.lang.NullPointerException_**	
_Exception in thread "main" java.lang.NullPointerException_	
_at com.in28minutes.exceptionhandling.ExceptionHandlingRunner.callMethod (ExceptionHandlingRunner.java:8)_	
_at com.in28minutes.exceptionhandling.ExceptionHandlingRunner.main (ExceptionHandlingRunner.java:4)_	
##### Snippet-01 Explained	
A ```java.lang.NullPointerException``` is **thrown** by the Java run-time when we called ```length()``` on the `null` reference.	
If an exception is not handled in the entire call chain, including `main`, the exception is thrown out and the program terminates. ```System.out.println()``` statements after the exception are never executed. 	
The runtime prints the **call stack trace** onto the console. 	
For instance, consider this simple ```class``` ```Test```:	
```java	
	public class Test {	
		public static void main(String[] args) {	
			callOne();	
		}	
		public static void callOne() {	
			callTwo();	
		}	
		public static void callTwo() {	
			callThree();	
		}	
		public static void callThree() {	
			String name;	
			System.out.println("This name is %d characters long", name.length());	
		}	
	}	
``` 	
However, the code name.length() used in ```callThree()``` caused a ```NullPointerException``` to be thrown. However, this is  not handled, and the console coughs up the following display:	
			
_Exception in thread "main" java.lang.NullPointerException_	
_at Test.callThree(Test.java:13)_	
_at Test.callTwo(Test.java:9)_	
_at Test.callOne(Test.java:6)_	
_at Test.main(Test.java:3)_	
This is nothing but a call trace of the stack, *frozen in time*.	
#### Summary	
In this step, we:	
* Saw a live example of an exception being thrown	
* Understood how a call trace on the stack appears when a exception occurs	
* Reinforced this understanding with another example	
### Step 02: Handling An Exception	
In Java, exception handling is achieved through a **```try```-```catch```** *block*. 	
##### Snippet-01 : Handling An Exception	
**_ExceptionHandlingRunner.java_**	
```java	
	package com.in28minutes.exceptionhandling;	
		
	public class ExceptionHandlingRunner {	
		public static void main(String[] args) {	
			method1();	
			System.out.println("main() Done");	
		}	
			
		static void method1() {	
			method2();	
			System.out.println("method1() done");	
		}	
		static void method2() {	
			try {	
				String str = null;	
				int len = str.length();	
				System.out.println("method2() Done");	
			} catch (Exception ex) {	
			}	
		}	
	}	
```	
**_Console Output_**	
_method1() Done_	
_main() Done_	
##### Snippet-01 Explained	
We have handled an exception here with a ```try```-```catch``` block. Its syntax resembles this:	
```java	
	try {	
		//< program-logic code block >	
	} catch (Exception e) {			
		//< exception-handling code block >	
	}	
```	
The exception (the ```NullPointerException```) still occurs after adding this block, but now it's actually **caught**. Although we did nothing with the caught exception, we did avoid a sudden end of the program.	
The statements following  ```int len = str.length()``` in `method2` are not executed. 	
However, all of ```method1()```'s code was run (with the ```"method1 Done"``` message getting printed). ```main()``` method also completed execution successfully.	
The program thus terminated gracefully. ```method1()``` and ```main()``` are both unaware of the ```NullPointerException``` occurring within ```method2()```.	
##### Snippet-02: Print Debug Information	
Let's add `ex.printStackTrace();`.	
**_ExceptionHandlingRunner.java_**	
```java	
	package com.in28minutes.exceptionhandling;	
	public class ExceptionHandlingRunner {	
		public static void main(String[] args) {	
			method1();	
			System.out.println("main() Done");	
		}	
		static void method1() {	
			method2();	
			System.out.println("method1() done");	
		}	
		static void method2() {	
			try {	
				String str = null;	
				int len = str.length();	
				System.out.println("method2() Done");	
			} catch (Exception ex) {	
				ex.printStackTrace();	
			}	
		}	
	}	
```	
**_Console Output_**	
**_java.lang.NullPointerException_**	
_Exception in thread "main" java.lang.NullPointerException_	
_at com.in28minutes.exceptionhandling.ExceptionHandlingRunner.method2 (ExceptionHandlingRunner.java:14)_	
_at com.in28minutes.exceptionhandling.ExceptionHandlingRunner.method1 (ExceptionHandlingRunner.java:8)_	
_at com.in28minutes.exceptionhandling.ExceptionHandlingRunner.main (ExceptionHandlingRunner.java:4)_	
_method1() Done_	
_main() Done_	
```printStackTrace()``` is provided by the ```Exception``` ```class```, which every exception inherits from. This method prints the frozen call trace of the program when the exception occurred, but without terminating the program. The code next continues to run.	
The stack trace provides useful information to you, the programmer,to debug the exception scenario.	
#### Summary	
In this step, we:	
* Were introduced to Java's basic mechanism to handle exceptions, the ```try```-```catch``` block	
* Saw how a program runs and ends gracefully, when an exception is handled	
* Observed how the ```printStackTrace``` method gives debug information to the programmer	
### Step 03: The ```Exception``` Hierarchy 	
The code in the ```try```-```catch``` block above does not work by black magic. From the call trace, it's clear that this program encounters a ```NullPointerException``` in ```method1()```. What's surprising, is that it was caught by a ```catch``` clause meant for an ```Exception```! The reason this worked is because ```NullPointerException``` **is-a** ```Exception```.	
You heard right! Java has a hierarchy of exception types, rooted at ```class``` ```Exception```. For instance, 	
* ```NullPointerException``` **is-a** ```RuntimeException```, and 	
* ```RuntimeException``` **is-a** ```Exception```. 	
* So effectively, ```NullPointerException``` **is-a** ```Exception```!	
Different branches of this inheritance-tree actually denote different exception categories. We'll dwell on this topic a little later.  	
##### Snippet-01 : Catching NullPointerException	
Let's add an additional catch for `NullPointerException` in method2.	
**_ExceptionHandlingRunner.java_**	
```java	
	package com.in28minutes.exceptionhandling;	
		
	public class ExceptionHandlingRunner {	
		public static void main(String[] args) {	
			method1();	
			System.out.println("main() Done");	
		}	
		static void method1() {	
			method2();	
			System.out.println("method1() done");			
		}	
		static void method2() {	
			try {	
				String str = null;	
				int len = str.length();	
				System.out.println("method2() Done");	
			} catch (NullPointerException e) {	
				System.out.println("NullPointerException");	
			} catch (Exception ex) {	
				ex.printStackTrace();	
			}	
		}	
	}	
```	
**_Console Output_**	
**_NullPointerException_**	
_method1() Done_	
_main() Done_	
##### Snippet-01 Explained	
_Among all the ```catch``` clauses following the ```try```, **one and only one** of them, may get executed. The **first** ```catch``` clause to **match**, **in serial order** after the ```try```, always gets executed. If **none** match, the exception is **not handled**._	
We placed an additional ```catch``` block within ```method2()```, to handle ```NullPointerException``` . Typically, the most specific exception class is matched. Hence the catch block for `NullPointerException` matches.	
You need to order the ```catch``` blocks after a ```try```, from more-specific to less-specific matches.   	
##### Snippet-02 : Catching another exception	
```java	
	package com.in28minutes.exceptionhandling;	
	public class ExceptionHandlingRunner {	
		public static void main(String[] args) {	
			method1();	
			System.out.println("main() Done");	
		}	
		static void method1() {	
			method2();	
			System.out.println("method1() done");	
		}	
		static void method2() {	
			try {	
				int[] numbers = {1, 2};	
				int num = numbers[3];	
				System.out.println("method2() Done");	
			} catch (NullPointerException e) {	
				System.out.println("NullPointerException");	
			} catch (Exception ex) {	
				ex.printStackTrace();	
			}	
		}	
	}	
```	
**_Console Output_**	
**_ArrayIndexOutOfBoundsException : 3_**	
_Exception in thread "main" java.lang.ArrayIndexOutOfBoundsException_	
_at com.in28minutes.exceptionhandling.ExceptionHandlingRunner.method2 (ExceptionHandlingRunner.java:14)_	
_at com.in28minutes.exceptionhandling.ExceptionHandlingRunner.method1 (ExceptionHandlingRunner.java:8)_	
_at com.in28minutes.exceptionhandling.ExceptionHandlingRunner.main (ExceptionHandlingRunner.java:4)_	
_method1() Done_	
_main() Done_	
##### Snippet-02 Explained	
```ArrayIndexOutOfBoundsException``` **is-a** ```IndexOutOfBoundsException```, which **is-a** ```RuntimeException```, which in turn **is-a** ```Exception```.  	
```ArrayIndexOutOfBoundsException``` is not a sub class of ```NullPointerException```. Hence, it does not match with the first catch block. ```ArrayIndexOutOfBoundsException``` is a sub class of  ```Exception```. Hence, that ```catch``` block matched, and the statement ```ex.printStackTrace();``` within it ran.	
If we omit the handler for ```Exception```, the ```ArrayIndexOutOfBoundsException``` is not caught by this ```try```-```catch``` block. Since it is not handled in ```method1()```, or even later in ```main()```, our program would have to stop suddenly. 	
 	
#### Summary	
In this step, we:	
* Learned that there is an exception hierarchy in Java, rooted at ```Exception```	
* Looked at an example that could cause multiple exceptions to occur	
* Observed how a handler for ```Exception``` could match any exception	
- - - 	
### Step 04:  The Need For ```finally```	
When an exception occurs, the programmer's world can turn upside-down in a matter of moments. If not handled, the program terminates all of a sudden, with no light at the end of the tunnel.	
##### Snippet-01 : Unreleased Resources	
**_FinallyRunner.java_**	
```java	
	package com.in28minutes.exceptionhandling;	
	import java.util.Scanner;	
	public class FinallyRunner {	
		public static void main(String[] args) {	
			Scanner scanner = new Scanner(System.in);	
			// ... Program logic, probably using scanner input	
			int num = numbers[5];	
			System.out.println("Before scanner close");	
			scanner.close();	
		}	
	}	
```	
**_Console Output_**	
_Exception in thread "main" java.lang.ArrayIndexOutOfBoundsException_	
_at com.in28minutes.exceptionhandling.FinallyRunner.main (FinallyRunner.java:8)_	
##### Snippet-01 Explained	
This example makes use of `Scanner` object to read from console. Ideally a `Scanner` object should be closed using ```scanner.close();```. 	
However, in our example, it is not called because a line before it threw an exception. (```int num = numbers[5];``` tries to access the 5th element of a 4-element array). 	
What this means, is a system resource that has been acquired, is never released. 	
It's important to ensure that any acquired resource is always released; whether on normal or abrupt termination. Let's see how you do this while handling an exception.	
##### Snippet-02 : Releasing Resources	
**_FinallyRunner.java_**	
```java	
	package com.in28minutes.exceptionhandling;	
	import java.util.Scanner;	
	public class FinallyRunner {	
		public static void main(String[] args) {	
			Scanner scanner = null;	
			try {	
				scanner = new Scanner(System.in);	
				// ... Program logic, probably using scanner input	
				int[] numbers = {1, 2, 3, 4};	
				int num = numbers[5];	
			} catch (Exception e) {	
				e.printStackTrace();	
			} finally {	
				if(scanner != null) {	
					System.out.println("Before scanner close");	
					scanner.close();	
				}			
			}	
			System.out.println("Before exiting main");	
		}	
	}	
```	
**_Console Output_**	
**_ArrayIndexOutOfBoundsException_**	
_Exception in thread "main" java.lang.ArrayIndexOutOfBoundsException_	
_at com.in28minutes.exceptionhandling.FinallyRunner.main (FinallyRunner.java:10)_	
_Before scanner close_	
_Before exiting main_	
##### Snippet-02 Explained	
Code in ```finally``` is almost always executed - even when there are exceptions. 	
We added a null check on `scanner` since ```scanner = new Scanner(System.in);``` could also result in an exception.	
```java	
	} finally {	
		if(scanner != null) {	
			System.out.println("Before scanner close");	
			scanner.close();	
		}	
	}	
```	
#### Summary	
In this step, we:	
* Observed how exceptional conditions could result in resource leaks	
* Learned about the ```finally``` clause in a ```try```-```catch``` block	
### Step 05: Programming Puzzles -  PP-01	
#### Puzzle-01	
* Would the ```finally``` clause be executed if	
	* The statement ```//str = "Hello";``` remains as-is	
	* The statement ```//str = "Hello";``` has its comments removed? 	
```java	
 	
	public static void method3() {	
		Connection connection = new Connection();	
		connection.open();	
		try {	
			String str = null;	
			//str = "Hello";	
			str.toString();	
			return;			
		} catch(Exception e) {			
		} finally {	
			connection.close();	
		}	
	}	
```	
* **_Answer_**	
	* Yes	
	* Yes	
#### Puzzle-02	
* When will code in a ```finally``` clause not get executed?	
* **_Answer_**	
	* In case of statements within the same ```finally``` clause, preceding this code, throwing an exception 	
	* In case of a JVM crash. This can be simulated in some scenarios by calling ```System.exit``` with an appropriate ```int``` argument, within an appropriate ```catch``` clause of the same ```try```-```catch```-```finally``` clause.	
 	
#### Puzzle-03	
* Will the following code, a ```try```-```finally``` without a ```catch```?	
```java	
	public static void method4() {	
		Connection connection = new Connection();	
		connection.open();	
		try {	
			String str = null;	
			//str = "Hello";	
			str.toString();	
			return;	
		} finally {	
			connection.close();	
		}		
	}	
```	
* **_Answer_** : Yes	
#### Puzzle-04	
* Will the following code, a ```try``` without a ```catch``` or a ```finally```?	
```java	
	public static void method5() {	
		Connection connection = new Connection();	
		connection.open();	
		try {	
			String str = null;	
			//str = "Hello";	
			str.toString();	
			return;	
		}	
	}	
```	
* **_Answer_** : No	
### Step 06: Handling Exceptions: Do We Have A Choice?	
Sometimes, in Java you are forced to handle exceptions.	
##### Snippet-02: Checked Exceptions - v1	
**_CheckedExceptionRunner.java_**	
```java	
	package com.in28minutes.exceptionhandling;	
		
	public class CheckedExceptionRunner {	
		public static void main(String[] args) {	
			Thread.sleep(2000);	
		}	
	}	
```	
##### Snippet-02 Explained 	
**_This program will not compile!_**	
The reason we get flagged by a compiler error, lies in the signature of the ```sleep()``` method. Here is its definition within the ```Thread``` ```class```:	
```java	
	public static native void sleep(long millis) throws InterruptedException {	
		//...	
	}	
```	
This declaration is a bit different from what you normally expect for a method, isn't it!  It contains a **```throws``` specification**. 	
When a method `throws` an Exception, the calling method should:	
* Handle it using ```try```-```catch``` block	
* Or declare `throws` in its signature	
Let's use ```try```-```catch``` block to start off.	
##### Snippet-03: Checked Exceptions - v2	
**_CheckedExceptionRunner.java_**	
```java	
	package com.in28minutes.exceptionhandling;	
	public class CheckedExceptionRunner {	
		public static void main(String[] args) {	
			try {	
				Thread.sleep(2000);	
			} catch (InterruptedException e) {	
				e.printStackTrace();	
			}	
		}	
	}	
```	
##### Snippet-03 Explained	
* ```main()```, which is the caller of ```sleep()```, chooses the option of handling ```InterruptedException``` with a ```try```-```catch``` block.	
#### The ```throws``` keyword	
```throws``` is used to declare that a method might throw exceptions. This involves a ```throws``` keyword, followed by a list of exception types. 	
##### Snippet-04 : Method with risky code #1	
```java	
	package com.in28minutes.exceptionhandling;	
	public class CheckedExceptionRunner {	
		public static void main(String[] args) {	
			try {	
				riskyMethod();	
				Thread.sleep(2000);	
			} catch (InterruptedException e) {	
				e.printStackTrace();	
			}	
		}	
		public static void riskyMethod() throws InterruptedException {	
			Thread.sleep(5000);	
		}	
	}	
```	
##### Snippet-04 Explained	
Here, we have removed the ```try```-```catch``` block within ```riskyMethod()```, because we want to follow another way of managing the exception. As an alternative, we added a ```throws``` specification to ```riskyMethod()``` to make the code compile. 	
We made `main` method handle the exception.	
#### Summary	
In this step, we:	
* Discovered that certain exceptions in Java do not force you to handle them	
* Learned that all the rest must be managed/handled	
* Observed that there are two ways to manage those "Checked" exceptions:	
	* Handling with a ```try```-```catch``` block	
	* Using a ```throws``` specification 	
### Step 08: The Java Exception Hierarchy	
Right at the root (top, we mean), the Java exception hierarchy looks like this:	
```java	
	class Error extends Throwable{}	
	class Exception extends Throwable{}		
	class InterruptedException extends Exception{}	
	class RuntimeException extends Exception{}	
	class NullPointerException extends RuntimeException{}	
	...	
```	
Once an ```Error``` occurs, there is nothing a programmer could do. Examples include: 	
*  The JVM running out of heap memory space	
An `Exception` can be handled. There are two types of Exceptions.	
* ```RuntimeException``` and its sub-classes. These come under the category of **unchecked exceptions**. Another example we've seen is ```NullPointerException```, which inherits from ```RuntimeException```.	
* All other sub-classes of ```Exception```, excluding the sub-tree rooted at ```RuntimeException```, are called **checked exceptions**. An instance we've encountered is ```InterruptedException```.	
If a method throws a **checked exception** is called, then either:	
* The method call must be enclosed in a ```try```-```catch``` block for proper handling, or 	
* The caller must throw this exception out, to its own caller. Its signature must also be enhanced using a ```throws``` specification. 	
If an **unchecked exception** is involved, then:	
*  You have the options of handling with  ```try```-```catch``` block.	
*  It is not mandatory to handle it.	
A **checked** exception **must** be handled, whereas as **unchecked** exception **may or may not** be handled.	
#### Summary	
In this step, we:	
* Discovered that within the Java exception hierarchy, there are two categories:	
	* Checked exceptions	
	* Unchecked exceptions	
* There are different strategies to manage these two categories	
### Step 09: Throwing an Exception	
So far, we have seen how to handle an exception, that is thrown by a built-in Java method. Now, let's explore how we can alert a user about exceptional conditions in our own code, by **throwing** exceptions. 	
##### Snippet-01 : Throwing An Exception	
**_ThrowingExceptionRunner.java_**	
```java	
	package com.in28minutes.exceptionhandling;	
	class Amounts {	
		private String currency;	
		private int amount;	
		public Amounts(String currency, int amount) {	
			super();	
			this.currency = currency;	
			this.amount = amount;	
		}	
		public void add(Amount that) {	
			if(!this.currency.equals(that.currency)) {	
				throw new RuntimeException("Currencies Don't Match");	
			}	
			this.amount += that.amount;	
		}	
		public Sring toString() {	
			return amount + " " + currency;	
		}	
	}	
	public class ThrowingExceptionRunner {	
		public static void main(String[] args) {	
			Amount amount1 = new Amount("USD", 10);	
			//Amount amount2 = new Amount("USD", 20);	
			Amount amount2 = new Amount("EUR", 20);	
			amount1.add(amount2);	
			System.out.println(amount1);	
		}	
	}	
```	
**_Console Output_**	
_Exception in thread "main" java.lang.RuntimeException:Currencies Don't Match_	
_at com.in28minutes.exceptionhandling.ThrowingExceptionRunner.main (ThrowingExceptionRunner.java:26)_	
##### Snippet-01 Explained	
Since adding ```10 USD``` and ```20 EUR``` does not make sense in the real world, it's important to tell the user that ```add()``` won't work for different currencies. The most direct way is to throw an exception, which the code ```throw new RuntimeException("Currencies Don't Match");``` does. 	
This thrown exception object can be handled inside ```main()```. By calling ```printStackTrace()``` on the caught exception reference,  you get debug information like before.	
##### Snippet-02 : Throwing a Checked Exception	
`Exception` is a Checked Exception. If a method throws an instance of `Exception` class, it needs to declare it -  `public void add(Amount that) throws Exception {`.	
**_ThrowingExceptionRunner.java_**	
```java	
	package com.in28minutes.exceptionhandling;	
		
	class Amounts {	
		private String currency;	
		private int amount;	
		public Amounts(String currency, int amount) {	
			super();	
			this.currency = currency;	
			this.amount = amount;	
		}	
		public void add(Amount that) throws Exception {	
			if(!this.currency.equals(that.currency)) {	
				throw new Exception("Currencies Don't Match : " + this.currency + " &  that.currency);	
			}	
				this.amount += that.amount;	
		}	
		public String toString() {	
			return amount + " " + currency;	
		}	
	}	
	public class ThrowingExceptionRunner {	
		public static void main(String[] args) {	
			Amount amount1 = new Amount("USD", 10);	
			//Amount amount2 = new Amount("USD", 20);	
			Amount amount2 = new Amount("EUR", 20);	
		try {	
				amount1.add(amount2);	
				System.out.println(amount1);	
			} catch(Exception e) {	
				e.printStackTrace();	
			}	
		}	
	}	
```	
**_Console Output_**	
**_java.lang.RuntimeException:Currencies Don't Match : USD & EUR_**	
_Exception in thread "main" java.lang.RuntimeException:Currencies Don't Match_	
_at com.in28minutes.exceptionhandling.ThrowingExceptionRunner.main (ThrowingExceptionRunner.java:26)_	
```Exception``` is not a ```RuntimeException``` or one of its sub-classes, it is a checked exception. So, it needs to be declared when it is thrown - `public void add(Amount that) throws Exception`. 	
#### Summary	
In this step, we:	
* Learned that it is possible to throw an exception from code inside any method we write	
* When a method throws checked exception, it should declare it.	
### Step 10: Throwing A Custom Exception	
It is also possible for you to throw a custom exception. You can do this by defining your own exception ```class```, only that it must inherit from one of the built-in exception classes. Note that:	
* If you sub-class a checked exception, your exception also becomes checked.	
* If you sub-class an unchecked exception, your exception would be unchecked. 	
##### Snippet-01 : Throw a custom exception	
**_ThrowingExceptionRunner.java_**	
```java	
	package com.in28minutes.exceptionhandling;	
	class CurrenciesDoNotMatchException extends Exception {	
		public CurrenciesDoNotMatchException(String msg) {	
			super(msg);	
		}	
	}	
	class Amounts {	
		private String currency;	
		private int amount;	
		public Amounts(String currency, int amount) {	
			super();	
			this.currency = currency;	
			this.amount = amount;	
		}	
		public void add(Amount that) throws Exception {	
			if(!this.currency.equals(that.currency)) {	
				throw new CurrenciesDoNotMatchException("Currencies Don't Match : " + this.currency + " & " + that.currency);	
			}	
			this.amount += that.amount;	
		}	
		public String toString() {	
			return amount + " " + currency;	
		}	
	}	
	public class ThrowingExceptionRunner {	
		public static void main(String[] args) {	
			Amount amount1 = new Amount("USD", 10);	
			//Amount amount2 = new Amount("USD", 20);	
			Amount amount2 = new Amount("EUR", 20);	
			try {	
				amount1.add(amount2);	
				System.out.println(amount1);	
			} catch(Exception e) {	
				e.printStackTrace();	
			}	
		}	
	}	
```	
**_Console Output_**	
**_com.in28minutes.exceptionhandling.CurrenciesDoNotMatchException : Currencies Don't Match : USD & EUR_**	
_Exception in thread "main" com.in28minutes.exceptionhandling.CurrenciesDoNotMatchException : Currencies Don't Match : USD & EUR_	
_at com.in28minutes.exceptionhandling.ThrowingExceptionRunner.main (ThrowingExceptionRunner.java:26)_	
##### Snippet-01 Explained	
The class ```CurrenciesDoNotMatchException``` clearly is a checked exception. Hence, rules that apply for throwing and handling checked applications, apply to it as well.	
If instead, ```CurrenciesDoNotMatchException``` were to sub-class ```RuntimeException```, it would be an unchecked exception. Adding the ```throws``` specification to the ```add()``` definition would not be needed. Also, no method in the call sequence of ```add()``` is required to handle it.	
#### Summary	
In this step, we:	
* Discovered that Java allows you to define your own custom exception classes	
* Whether a custom exception is checked or unchecked, depends on which exception it sub-classes.	
* Saw an example of how to raise and handle a custom exception	
### Step 11: Introducing ```try```-With-Resources 	
```try```-with-resources makes managing resource in a ```try```-```catch```-```finally``` block. Let's look at an example.	
##### Snippet-01: try-with-resources	
```java	
	package com.in28minutes.exceptionhandling;	
	import java.util.Scanner;	
	public class TryWithResourcesRunner {	
		public static void main(String[] args) {	
			try (Scanner scanner = new Scanner(System.in)) {	
				// ... Program logic, probably using scanner input	
				int[] numbers = {1, 2, 3, 4};	
				int num = numbers[5];	
			}	
			//scanner.close();	
		}	
	}	
```	
##### Snippet-01 Explained	
The ```try```-with-resources version was introduced in Java SE 7. It encloses the resource to be managed within parentheses, along with the ```try``` keyword. 	
In this case, ```Scanner``` is compatible with such resource management, because it's defined to implement the ```Closeable``` ```interface```. This interface in turn, is a sub-class of the ```abstract class``` ```AutoCloseable```.	
```Closeable extends AutoCloseable{};```	
```Scanner implements Closeable{};```	
 	
For ```try```-with-resources, a ```catch``` and/or a ```finally``` clause are not mandatory.	
Also, the call to ```scanner.close``` is no longer required.	
#### Summary	
In this step, we:	
* Discovered a veriant of the ```try```-```catch```-```finally``` block, called ```try```-with-resources	
* Saw that it can be used to manage resource cleanly, provided the resource implements the ```AutoCloseable``` ```interface```.	
### Step 12: Programming Puzzle Set PP_02 	
#### Puzzle-01	
* Does the following program handle the exception thrown?	
```java	
	try {		
			AmountAdder.addAmounts(new Amount("RUPEE", 5), new Amount("RUPEE", 5);	
			String str = null;	
			str.toString();	
		} catch(CurrenciesDoNotMatchException ex) {	
			ex.printStackTrace();	
		}	
```	
* **_Answer : No_**	
#### Puzzle-01 Explained	
The exception thrown is a ```NullPointerException```, whereas the one we are trying to catch is a ```CurrenciesDoNotMatchException```. 	
#### Puzzle-02	
* Does the following code compile?	
```java	
	try {	
			AmountAdder.addAmounts(new Amount("RUPEE", 5), new Amount("RUPEE", 5);	
			String str = null;	
			str.toString();	
		} catch(Exception e) {	
			e.printStackTrace();	
		} catch(CurrenciesDoNotMatchException ex) {	
			ex.printStackTrace();			
		}	
```	
**_Answer : No_**	
#### Puzzle-02 explained	
The order of ```catch``` clauses for exceptions needs to be from less specific to more specific.  ```CurrenciesDoNotMatchException``` is a sub-class of ```Exception```. Hence, error.	
#### Puzzle-03	
* Does the following code compile?	
```java	
	try {	
	} catch (IOException | SQLException ex) {	
		ex.printStackTrace();	
	}	
```	
* **_Answer : Yes_**	
#### Puzzle-03 Explained	
This feature was added in Java SE 7.	
## File Operations	
We would be aware that any computer has a hard disk, on which information is stored. This information is stored in units called **files**. For ease of access, file are grouped together and organized into **directories**. The operating system has a sub-system called the **file-system**, which  has the responsibility of interfacing system and user programs, with files and directories on disk. 	
The Java Runtime System also communicates with the native file-system, and makes use of its services to provide a file programming interface to Java programmers. 	
In this section, we will explore a few basic ways in which programmers can interact with the native file-system, through the platform independent Java file API. 	
#### Listing Directory Contents	
When we develop a Java software project in the Eclipse IDE environment, the root folder of the project has several interesting file and sub-folders contained within it. From now on, we use the terms "folder" and "directory" interchangeably, as they have equivalent meanings. 	
Let's write a simple Java program to list the contents of one such project folder. 	
##### Snippet-1 : Listing Directory Contents	
The ```java.nio.file``` system package has a bunch of utility ```class```es and ```interface```s to help us navigate the native file system.	
**_DirectoryScanRunner.java_**	
```java	
	package com.in28minutes.files;	
	import java.nio.file.Files;	
	import java.nio.file.Paths;	
	import java.io.IOException;	
	public class DirectoryScanRunner {	
		public static void main(String[] args) throws IOException {	
			Files.list((Paths.get(".")).forEach(System.out::println);	
		}	
	}	
```	
**_Console Output_**	
_./.classpath_	
_./.project_	
_./.DS_Store_	
_./bin_	
_./resources_	
_./src_	
##### Snippet-1 Explained	
A ```Path``` ```class``` is the entity used to denote a **pathname** in Java NIO Library. NIO stands for "New I/O", which was introduced in Java SE, replacing the earlier, very awkward File I/O Library. It is no longer new though, but that's another issue! 	
"```.```" denotes the current directory in the file-system. 	
The ```Paths.get()``` method returns the path-name of the specified directory in a format that the ```Files.get()``` method understands.	
The ```Files.get()``` method does a **lazy traversal** of the directory it is provided with, in the sense that:	
* It lists regular files it encounters.	
* When faced with directory files, it merely lists them, without recursively traversing them.	
The contents of the root directory are listed as path-names, with each path-name being relative to the root directory.	
   	
##### Snippet-2 : Recursive Directory Traversal	
We can specify level 2 in `Files.walk(currentDirectory, 2)`. So, folders until level 2 are scanned.	
**_DirectoryScanRunner.java_**	
```java	
	package com.in28minutes.files;	
	import java.nio.file.Files;	
	import java.nio.file.Path;	
	import java.nio.file.Paths;	
	import java.io.IOException;	
	public class DirectoryScanRunner {	
		public static void main(String[] args) throws IOException {	
			Path currentDirectory = Paths.get(".");	
			//Files.list(currentDirectory).forEach(System.out::println);	
			Files.walk(currentDirectory, 2).forEach(System.out::println);	
		}	
	}	
```	
**_Console Output_**	
_./.classpath_	
_./.project_	
_./.DS_Store_	
_./bin_	
_./bin/files_	
_./resources_	
_./src_	
_./src/files_	
##### Snippet-3 : Level-4 Traversal	
**_DirectoryScanRunner.java_**	
```java	
	package com.in28minutes.files;	
	import java.nio.file.Files;		
	import java.nio.file.Path;	
	import java.nio.file.Paths;	
	import java.io.IOException;	
	public class DirectoryScanRunner {	
		public static void main(String[] args) throws IOException {	
			Path currentDirectory = Paths.get(".");	
			Files.walk(currentDirectory, 4).forEach(System.out::println);	
		}	
	}	
```	
**_Console Output_**	
_./.classpath_	
_./.project_	
_./.DS_Store_	
_./bin_	
_./bin/files_	
_./bin/files/DirectoryScanRunner.class_	
_./resources_	
_./src_	
_./src/files_	
_./src/files/DirectoryScanRunner.java_	
##### Snippet-4 : Only list .java files during traversal	
We use a predicate `Files.walk(currentDirectory, 4).filter(predicate)` to filter only Java files.	
**_DirectoryScanRunner.java_**	
```java	
	package com.in28minutes.files;	
	import java.nio.file.Files;	
	import java.nio.file.Path;	
	import java.nio.file.Paths;	
	import java.util.function.Predicate;	
	import java.io.IOException;	
	public class DirectoryScanRunner {	
		public static void main(String[] args) throws IOException {	
			Path currentDirectory = Paths.get(".");	
			Predicate<? super Path> predicate = path -> String.valueOf(Path).contains(".java");	
			//Files.walk(currentDirectory, 4).forEach(System.out::println);	
			Files.walk(currentDirectory, 4).filter(predicate)	
										   .forEach(System.out::println);	
		}	
	}	
```	
**_Console Output_**	
_./src/files/DirectoryScanRunner.java_	
##### Snippet-5 : Filtered Traversal with find()	
We can use a matcher - `Files.find(currentDirectory, 4, matcher)` which is configured to check the path attribute for .java extension - `(path, attributes) -> String.valueOf(path).contains(".java")`	
**_DirectoryScanRunner.java_**	
```java	
	package com.in28minutes.files;	
	import java.nio.file.Files;	
	import java.nio.file.Path;	
	import java.nio.file.Paths;	
	import java.util.function.Predicate;	
	import java.nio.file.attribute.BasicFileAttributes;	
	import java.util.function.BiPredicate;	
	import java.io.IOException;	
	public class DirectoryScanRunner {	
		public static void main(String[] args) throws IOException {	
			Path currentDirectory = Paths.get(".");	
			//Predicate<? super Path> predicate = path -> String.valueOf(path).contains(".java");	
			//Files.walk(currentDirectory, 4).filter(predicate).forEach(System.out::println);	
			BiPredicate<Path, BasicFileAttributes> matcher = 	
			(path, attributes) -> String.valueOf(path).contains(".java");	
			Files.find(currentDirectory, 4, matcher);	
		}	
	}	
```	
**_Console Output_**	
_./src/files/DirectoryScanRunner.java_	
##### Snippet-6 : Filtering directories	
**_DirectoryScanRunner.java_**	
```java	
	package com.in28minutes.files;	
	import java.nio.file.Files;	
	import java.nio.file.Path;	
	import java.nio.file.Paths;	
	import java.util.function.Predicate;	
	import java.nio.file.attribute.BasicFileAttributes;	
	import java.util.function.BiPredicate;	
	import java.io.IOException;	
	public class DirectoryScanRunner {	
		public static void main(String[] args) throws IOException {	
			Path currentDirectory = Paths.get(".");	
			//BiPredicate<Path, BasicFileAttributes> matcher = 	
			//(path, attributes) -> String.valueOf(path).contains(".java");	
				
			BiPredicate<Path, BasicFileAttributes> directoryMatcher = 	
			(path, attributes) -> attributes.isDirectory();	
			Files.find(currentDirectory, 4, directoryMatcher);	
		}	
	}	
```	
**_Console Output_**	
_./bin_	
_./bin/files_	
_./resources/_	
_./src/_	
_./src/files_	
We are making use of a matcher checking `attributes.isDirectory()`.	
##### Snippet-7 : Reading a File	
**_./resources/data.txt_**	
```123.122```	
```asdfghjkl```	
```Apple```	
```Bat```	
```Cat```	
**_FileReadRunner.java_**	
```java	
	package com.in28minutes.files;	
	import java.nio.file.Files;	
	import java.nio.file.Paths;	
	import java.io.IOException;	
	public class FileReadRunner {	
		public static void main(String[] args) throws IOException {	
			Path pathFileToRead = Paths.get("./resources/data.txt");	
			List<String> lines = Files.readAllLines(pathFileToRead);	
			System.out.println(lines);	
		}	
	}	
```	
**_Console Output_**	
_[123.122, asdfghjkl, Apple, Bat, Cat]_	
`Files.readAllLines(pathFileToRead)` makes it easy to read content of a file to list of String values.	
##### Snippet-8 : Streamed File Read	
`Files.readAllLines(pathFileToRead)` makes it easy to read content of a file. However, streaming is a better options when reading large files or when less memory is available.	
**_./resources/data.txt_**	
```123.122```	
```asdfghjkl```	
```Apple```	
```Bat```	
```Cat```	
**_FileReadRunner.java_**	
```java	
	package com.in28minutes.files;	
	import java.nio.file.Files;	
	import java.nio.file.Paths;	
	import java.io.IOException;	
	public class FileReadRunner {	
		public static void main(String[] args) throws IOException {	
			Path pathFileToRead = Paths.get("./resources/data.txt");	
			//List<String> lines = Files.readAllLines(pathFileToRead);	
			//System.out.println(lines);	
			Files.lines(pathFileToRead).forEach(System.out::println);	
		}	
	}	
```	
**_Console Output_**	
_123.122_	
_asdfghjkl_	
_Apple_	
_Bat_	
_Cat_	
`Files.lines(pathFileToRead)` returns a stream which can be consumed as needed.	
##### Snippet-9 : Printing file contents in lower-case	
We can use `map` function to map to `String::toLowerCase`	
**_./resources/data.txt_**	
```	
123.122	
asdfghjkl	
Apple	
Bat	
Cat	
```	
**_FileReadRunner.java_**	
```java	
	package com.in28minutes.files;	
	import java.nio.file.Files;	
	import java.nio.file.Paths;	
	import java.io.IOException;	
	public class FileReadRunner {	
		public static void main(String[] args) throws IOException {	
			Path pathFileToRead = Paths.get("./resources/data.txt");	
			//Files.lines(pathFileToRead).forEach(System.out::println);	
			Files.lines(pathFileToRead)	
				 .map(String::toLowerCase)	
				 .forEach(System.out::println);	
		}	
	}	
```	
**_Console Output_**	
_123.122_	
_asdfghjkl_	
_apple_	
_bat_	
_cat_	
##### Snippet-9 : Filtering file contents	
You can also filter file content using the `filter` method.	
**_FileReadRunner.java_**	
```java	
	package com.in28minutes.files;	
	import java.nio.file.Files;	
	import java.nio.file.Paths;	
	import java.io.IOException;	
	public class FileReadRunner {	
		public static void main(String[] args) throws IOException {	
			Path pathFileToRead = Paths.get("./resources/data.txt");	
			//Files.lines(pathFileToRead).forEach(System.out::println);	
			//Files.lines(pathFileToRead).map(String::toLowerCase).forEach(System.out::println);	
			Files.lines(pathFileToRead)	
				 .map(String::toLowerCase)	
				 .filter(str -> str.contains("a"))	
				 .forEach(System.out::println);	
		}	
	}	
```	
**_Console Output_**	
_asdfghjkl_	
_apple_	
_bat_	
_cat_	
##### Snippet-10 : Writing to a file	
`Files.write` can be used to write to a file.	
**_FileWriteScanner.java_**	
```java	
	package com.in28minutes.files;	
	import java.nio.file.Files;	
	import java.nio.file.Paths;	
	import java.io.IOException;	
	public class FileWriteRunner {	
		public static void main(String[] args) throws IOException {	
			Path pathFileToWrite = Paths.get("./resources/file-write.txt");	
			List<String> list = List.of("Apple", "Boy", "Cat", "Dog", "Elephant");	
			Files.write(pathFileToWrite, list);	
		}		
	}	
```	
**_./resources/file-write.txt_**	
```	
Apple	
Boy	
Cat	
Dog	
Elephant	
```	
## Concurrency : Advanced Topics	
Let's create a simple counter.	
##### Snippet-1: Atomic Operations : Counter	
**_Counter.java_**	
```java	
	package com.in28minutes.concurrency;	
	public class Counter {	
		private int i = 0;	
		public void increment() {	
			i++;	
		}	
		public int getI() {	
			return i;	
		}	
	}	
```	
**_ConcurrencyRunner.java_**	
```java	
	package com.in28minutes.concurrency;	
	public class ConcurrencyRunner {	
		public static void main(String[] args) {	
			Counter counter = new Counter();	
			counter.increment();	
			counter.increment();	
			counter.increment();				
			System.out.println(counter.get());	
		}	
	}	
```	
##### Snippet-1 Explained	

Quite straightforward!	

#### Counter ```increment()``` method is NOT Atomic!	

Let's look at the code. It seemingly involves just one operation.	

```java	
	public void increment() {	
		i++;	
	}	
```	
The operation ```i++``` actually involves the following steps:	
- Step 1. Read the value of ```i``` from memory into the CPU registers	
- Step 2. Increment the value in the CPU registers	
- Step 3. Store the incremented value back into the memory location of ```i```	
```i++``` is not an atomic operation. 	

##### What if `increment` is not atomic?	

Let's take an example of two Threads, ```T1``` and ```T2``` running in ```ConcurrencyRunner``` access a single ```Counter``` object instance. 	

Let's say the threads concurrently invoke the `increment` and `getI`.	

Assume the initial value of ```i``` is ```15```. Let's take a closer look at a possible scenario:	
-  ```T1``` calls ```increment()``` first, and successfully completes Step 1 of ```i++```. Gets a value of 15.	
-  The scheduler switches threads to ```T2```.	
-  ```T2``` calls ```increment()``` first, and successfully completes Step 1 of ```i++```.Gets a value of 15.	
- The scheduler switches to ```T1```.  ```T1``` resumes execution of ```increment()```, and completes steps 2 and 3 of ```i++```. Completes execution of ```increment()```. Value of ```i``` is over-written with ```16```.	
- The scheduler switches to ```T2```. In it's CPU register context, i is ```15```, not ```16```. ```T2``` resumes execution of ```increment()```, and completes steps 2 and 3 of ```i++```. Completes execution of ```increment()```.Value of ```i``` in the ```Counter``` instance is over-written with ```16```.	

Ideally, the final value of ```i``` after two ```increment```s should have been ```17```. This would result when the operations run serially one after the other.

This scenario, where the result of a concurrent computation (involving a sequence of operations) depends on the relative order of execution of those operations by the threads involved, is called a **race condition**.	

There is a popular English saying: "There is many a slip, between the cup and the lip". This refers to the fact that anything can happen between the time when we hold a cup of tea in our hands, and the time when we actually get to take a sip of the tea.	

This definitely rings true here. 	

The increment operation is not actually not as smooth as it seems. because it is not atomic, slip-ups can and will often occur. This brings us to the concept of **Thread-Safety**. 	

A method is said to be thread-safe, if it can be run in a concurrent environment (involving several concurrent invocations by independent threads) without *race-conditions*. 	
#### Revisited : The ```synchronized``` Keyword	

Adding the keyword ```synchronized``` to the signature of a ```class``` method makes it thread safe.	

##### Snippet-2	

**_Counter.java_**	
```java	
	package com.in28minutes.concurrency;	
	public class Counter {	
		private int i = 0;	
		synchronized public void increment() {	
			i++;	
		}	
		public int getI() {	
			return i;	
		}	
	}	
```	
##### Snippet-2 Explained	
After adding `synchronized` keyword to the method `increment`, only one thread will be able to execute the method, at a time. Hence, race condition is avoided.	
##### Snippet-3 : less concurrency	
`synchronized` keyword make the code thread safe. However, it causes all other threads to wait. This can result in performance issues. Let's look at an example:	
**_BiCounter.java_**	
```java	
	package com.in28minutes.concurrency;	
	public class BiCounter {	
		private int i = 0;	
		private int j = 0;	
		synchronized public void incrementI() {	
			i++;	
		}	
		synchronized public void incrementJ() {	
			j++;	
		}	
		public int getI() {	
			return i;	
		}	
		public int getJ() {	
			return j;	
		}	
	}	
```	
**_ConcurrencyRunner.java_**	
```java	
	package com.in28minutes.concurrency;	
	public class ConcurrencyRunner {	
		public static void main(String[] args) {	
			BiCounter counter = new BiCounter();	
			counter.incrementI();	
			counter.incrementJ();	
			counter.incrementI();	
			System.out.println(counter.get());	
		}	
	}	
```	
##### Snippet-3 Explained	
Both ```incrementI()``` and ```incrementJ()``` of ```class``` ```BiCounter``` are ```synchronized```. Therefore, at any given time, at most one thread can execute either of these methods! Which means that, while a thread  ```T1``` is executing ```counter.incrementI()``` within ```ConcurrencyRunner.main()```, another thread ```T2``` **is not allowed to execute** ```counter.incrementJ()```!	
Just imagine, if there are a total of ```12``` threads wanting to increment ```counter```. When one thread is running, the other ```11``` have to wait! 	
#### Synchronization With Locks	
Let's look at another synchronization option - `Locks`	
##### Snippet-4: BiCounter With Locks	

**_BiCounterWithLocks.java_**	

```java	
	package com.in28minutes.concurrency;	
	import java.util.concurrent.locks.ReentrantLock;	
	public class BiCounterWithLocks {	
		private int i = 0;	
		private int j = 0;	
		private Lock LockForI = new ReentrantLock();	
		private Lock LockForJ = new ReentrantLock();	
		public void incrementI() {	
			lockForI.lock();	
			i++;	
			lockForI.unlock();	
		}	
		public void incrementJ() {	
			lockForJ.lock();	
			j++;	
			lockForJ.unlock();	
		}	
		public int getI() {	
			return i;	
		}	
		public int getJ() {	
			return j;	
		}	
	}	
```	

##### Snippet-4 Explained	

`i++` and `j++` are the pieces of code to protect. We use two locks lockForI and lockForJ. If a thread wants to execute `i++`, it needs to first get a lock to it - implemented using `lockForI.lock()`. Once it performs the operation, it can release the lock `lockForI.unlock()`. 	
The ```Lock```s ```lockForI``` and ```lockForJ``` are totally independent of each other. Therefore, a thread ```T2``` can execute ```j++``` within ```incrementJ()```, at the same time that thread ```T1``` is executing ```i++``` within ```incrementI()```.	
  	
#### Atomic Classes	

The operation ```i++```, small though it might seem, gave us quite a bit headache! 	

If a seemingly minute operation might need so much worrying about, imagine writing concurrent data structures that manipulate linked lists with multiple link operations! 	
It would be really nice if someone could take care of these tiny operations for us, otherwise we would have  hard time finding out what code to definitely lock, and what code need not be!	

Java addresses this issue for basic data types, by providing a few classes that are inherently thread-safe. A good example is ```AtomicInteger```, which is a wrapper around the ```int``` primitive type.	

##### Snippet-5 : AtomicInteger	


**_BiCounterWithAtomicInteger.java_**
```java	
	package com.in28minutes.concurrency;	
	import java.util.concurrent.atomic.AtomicInteger;	
	public class BiCounterWithAtomicInteger {	
		private AtomicInteger i = new AtomicInteger();	
		private int AtomicInteger = new AtomicInteger();	
		public void incrementI() {	
			i.incrementAndGet();	
		}	
		public void incrementJ() {	
			j.incrementAndGet();	
		}	
		public int getI() {	
			return i.get();	
		}	
		public int getJ() {	
			return j.get();	
		}	
	}	
```	
##### Snippet-5 Explained	

`incrementAndGet` is atomic. So, `BiCounterWithAtomicInteger` does not need to worry about synchronization.

#### Concurrent Collections	

Java gave us a ready-made solution for thread-safe primitive data, with wrappers such as ```AtomicInteger```. The reasons this approach worked for ```int``` were:	
* Simple, small-sized underlying type	
* Wide-spread potential usage	

How about collections? 	

Java provides classes like `Vector` (synchronized version of `ArrayList`) which can provide thread safety. But, these inherit the problems with using synchronized. 	
What are other options?	


##### Snippet-6 : Need For ConcurrentMap	

The code within the ```for``` loop does a `get` and then a `put`. It is not thread safe.	

**_MapRunner.java_**	
```java	
	package com.in28minutes.collections;	
	import java.util.HashMap;	
	public class MapRunner {	
		public static void main(String[] args) {	
			String str = "Hello World";	
			Map<Character, Integer> occurrences = new HashMap<>();	
			char[] characters = str.toCharArray();	
			for(char character:characters) {	
				Integer count = occurrences.get(character);	
				if(count == null) {	
					occurrences.put(character, 1);	
				} else {	
					occurrences.put(character, count + 1);	
				}	
			}	
		}	
	}	
```	


Concurrent Collections provide atomic versions of operations such as those encountered above:	
* If entry does not exist, then create and initialize	
* If entry exists, then update	


#### The ```ConcurrentMap``` ```interface```	

The ```interface``` ```ConcurrentMap``` has methods to implement compound operations. Such operations include:	
```	
V putIfAbsent(K key, V value);	
V computeIfPresent(K key,	
            BiFunction<? super K, ? super V, ? extends V> remappingFunction)	
```	

##### Snippet-7 : ConcurrentHashMap Logic - Stage 1	


```LongAdder``` provides an atomic `increment` method, which we are making use of to make the code a little more thread safe. However, different threads could be executing ```occurrences.get()``` and ```occurrences.put()``` in parallel. A race condition can still occur.	


**_ConcurrentMapRunner.java_**	

```java	
	package com.in28minutes.concurrency;	
	import java.util.Map;	
	import java.util.HashTable;	
	import java.util.concurrent.atomic.LongAdder;	
	public class ConcurrentMapRunner {	
		public static void main(String[] args) {	
			    String str = "ABCD ABCD ABCD";	
			    for(char character:str.toCharArray()) {	
			      LongAdder longAdder = occurances.get(character);	
			      if(longAdder == null) {	
			        longAdder = new LongAdder();	
			      }	
			      longAdder.increment();	
			      occurances.put(character, longAdder);	
			    }	
		}	
	}	
	
```	

**_Console Output_**	

_[ =2, A=3, B=3, C=3, D=2]_	


##### Snippet-8 : ConcurrentHashMap Logic - Stage 2	

We can use the method ```computeIfAbsent()``` from the ```collection``` ```ConcurrentHashMap``` to reduce the code to a single, atomic operation.	

**_ConcurrentMapRunner.java_**	

```java	
	package com.in28minutes.concurrency;	
	import java.util.concurrent.ConcurrentMap;	
	import java.util.concurrent.ConcurrentHashMap;	
	import java.util.concurrent.atomic.LongAdder;	
	public class ConcurrentMapRunner {	
		public static void main(String[] args) {	
		    ConcurrentMap<Character, LongAdder> occurances = new ConcurrentHashMap<>();	
		    	
		    String str = "ABCD ABCD ABCD";	
		    for(char character:str.toCharArray()) {	
		      occurances.computeIfAbsent(character, ch -> new LongAdder()).increment();	
		    }	
		    	
		    System.out.println(occurances);	
	  }	
	  
	}	
```	
**_Console Output_**	


_[ =2, A=3, B=3, C=3, D=2]_	



#### ```ConcurrentHashMap```	


In ```HashTable```, all methods are synchronized. 	

In ```ConcurrentHashMap```, data structure is organized into disjoint regions. Access methods use different ```Locks``` for different regions, reducing performance impact during concurrent access. 	

#### Concurrent Collections : Copy-On-Write Optimization	
All values in Copy-On-Write collections are stored in an internal immutable (not-changeable) array. A new array is created if there is any modification to the collection.	
Read operations are not synchronized. Only write operations are synchronized.	

Copy on Write approach is used in scenarios where reads greatly out number write’s on a collection. 	

`CopyOnWriteArrayList` & `CopyOnWriteArraySet` are implementations of this approach. 	

Copy on Write collections are typically used in Subject – Observer scenarios, where the observers very rarely change. Most frequent operations would be iterating around the observers and notifying them.	

##### Snippet-9 : CopyOnWriteArrayList	

**_CopyOnWriteArrayListRunner.java_**	
```java	
	package com.in28minutes.concurrency;	
	import java.util.List;	
	import java.util.concurrent.CopyOnWriteArrayList;	
	public class CopyOnWriteArrayListRunner {	
		public static void main(String[] args) {	
			List<String> list = new CopyOnWriteArrayList<>();	
			// Total of 3 threads doing add()'s, maybe in a separate method	
			list.add("Ant");	
			list.add("Bat");	
			list.add("Cat");	
			//Total of 10000 threads looping on get(), again, in a separate method	
			for(String element:list) {	
				System.out.println(element);	
			}	
		}	
	}	
	
```	


##### Snippet-9 Explained	

```CopyOnWriteArrayList.add()``` method is a ```synchronized``` method. And the copy-on-write algorithm ensures that the copying is performed in a thread-safe manner, after which the write is done on a separate copy, while the ```get()```'s continue on the original array. Once the ```add()``` is done, the collection starts using the new array, and discards the old one. This strategy continues for the lifetime of the program.	

The ```CopyOnWriteArrayList.get``` method is NOT ```synchronized```, since on the array that the reads work, there will be no direct write through an ```add()```.

Copy-On-Write collections should only be used for the specific usage scenarios, viz., very large number of data structure traversals (data element reads only), compared to mutations (data element insertions/deletions/modifications). In this way, high concurrency is achieved for traversals.
