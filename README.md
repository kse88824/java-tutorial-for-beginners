# Java Tutorial For Beginners
 
**"Learning Java In 150 Steps"** 책에 오신것을 환영합니다.

저는 **Ranga Karanam** 이고, 20년이 넘는 프로그래밍 경력을 가지고 있습니다.

저는 프로그래밍을 사랑합니다. ```in28minutes``` 를 시작할 때 저의 목표 중 하나는 프로그래밍을 쉽게 배울 수 있도록 하는 것이었습니다. 저희가 놀라운 강의를 만들 수 있도록 도와주신 전 세계 30만명의 학습자분들께 감사합니다.

**In28Minutes** 에서는, 저희는 매일 "어떻게 하면 멋진 학습 경험을 만들 수 있을까?"하고 스스로에게 묻습니다. 

이 책에서는, 여러분은 Java와 함께 **객체** **지향적** 코드를 배우게 될 것이며, 많은 예제들,실습들, 팁들을 접하게 될 것입니다. 저희는 Java 사용자들을 위해 많은 예시를 들며 코드를 쓰는 방법을 알아보려고 노력할 것입니다.

본 가이드를 개선하는데 도움을 주시려면 - **Fork, Pull Requests, Shares and Likes 를 추천드립니다**!

## Table of Contents

* [Chapter 01 - 프로그래밍 소개와 Print-Multiplication-Table](#프로그래밍-소개와-print-multiplication-table)
* [Chapter 02 - 함수의 이해](#함수의-이해)
* [Chapter 03 - 자바 플랫폼의 이해](#자바-플랫폼의-이해)
* [Chapter 04 - 이클립스](#이클립스)
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
* 코드 편집기에서 Java 코드를 개발하는 것이 힘을 주는 느낌이라는 결론을 내렸다!

### Step 07: The JVM, JRE And JDK

What are *JVM*, *JRE* and the *JDK*? 

Apart from the fact that all start with a '*J*', there are important differences in what they contain, and what they do. 

The following list gives you a bird's eye view of things.

The **JVM** runs your program bytecode.


**JRE** = **JVM** + **Libraries** + **Other Components**

* *Libraries* are built-in Java utilities that can be used within any program you create. ```System.out.println()``` was a method in ```java.lang```, one such utility.
* *Other Components* include tools for debugging and code profiling (for memory management and performance).


**JDK** = **JRE** + **Compilers** + **Debuggers**

* *JDK* refers to the **Java Development Kit**. It's an acronym for the bundle needed  to compile (with the compiler) and run (with the *JRE* bundle) your Java program.

An interesting way to remember this organization is:

* **JDK** is needed to **Compile and Run** Java programs

* **JRE** is needed to **Run** Java Programs

* **JVM** is needed to **Run Bytecode** generated from Java programs

Let's check a couple of scenarios to test your understanding.

**Scenario 1**: You give *Planet.class* file to a friend using a different operating system. What does he need to do to run it? 

First, install **JRE** for his operating system. Run using *java Planet* on the terminal. He does not need to run  *javac*, as he already has the bytecode. 

**Scenario 2**: You gave your friend the source file *Planet.java*. What does he need to do to run it? 

Install *JDK* of a compatible version. Compile code using *javac Planet.java*. Run *java Planet* on his terminal.

In summary

* **Application Developers** _need_ **==> JDK**

* **Application Users** _need_ **==> JRE**

#### Summary

In this step, we:
* Understood the differences in the scope-of-work done by the JVM, JRE and JDK
* Realized how each of them could be invoked by different terminal commands, such as *javac* and *java*.

## Eclipse

TODO - Need Revision 

### Introducing Java Software Development with Eclipse

* Features of the Eclipse IDE (Integrated Development Environment)
	* Installation & Configuration
	* Workspace Creation & Configuration
	* Project Creation & Organization
		* JRE Version Selection and Included Libraries 
		* Eclipse Java Perspectives
		* Source Files Organization into Folders
		* Packages?
	* IDE User Interface Description
		* Perspective
		* Views
		* Console Content and Display Options

* Creating a new Java ```class``` in Eclipse (And related source file)
	* Package name
		* A Java solution to solving a problem could be composed of several application components. It is considered good programming arctice to identify a class for each distinct component. Package is the Java way to organize classes in source code.
		* Analogy: Eatables in a Refrigerator (Freezer, Chill-Tray, Vegetable-Tray, Bottle-Rack)
	* Public method stub : can be used to create a default ```public static void main(String[] args)``` signature
	* (Include Snapshots)
		* Class creation pop-up, with selected options
		* Default generated source code in editor window

	* Customizing the generated source code to our needs
		* Syntax Highlighting
			* Keywords
			* Built-in Types
			* Constant literals: numbers, strings
		* Auto-suggest feature of eclipse as code is being typed in

	* The "Run as --> Java Application" Option to compile-and-run the source code
		* Option is avaibale only for classes that have a main() method


#### Using Eclipse in Debug Mode

Execution of the Multiplication Table Program can be done Step by-step. That is, the entire application dies not execute at one go, printing the final output onto the console. We can stall its flow at several steps, by taking control of its execution using the Eclipse IDE. This is possible in a special mode of Eclipse, called **Debug Mode**. 

The process is called **Debugging**, because this mode is heavily used not just to have fun seeing what happens, but also to detect and fix software **bugs**. A bug is a defect in the program being written, that leads to its incorrect execution. The process of removing bugs is called debugging. Humans being humans, programming errors are but natural, and a debug mode in the IDE is worth its wight in gold to the programmer. Here is how Eclipse facilitates debugging of Java applications.

* Prior to debugging application, we need to set few **Break-Points**. A Break-Point is a statement in the source of the program, before which execution under debug mode is suspended, and control is passed to the programmer.
* The overall state of the data in the suspended program is available to the programmer at that particular break-point. He/she gets to specify one or more break-points in the program, and when the execution is suspended, a list of possible actions can be performed, including: 
	* Reading & modifying data variables 
	* Resuming program execution 
	* Re-executing current statement
	* Skipping all statements till the next break-point
	
	and others.

* The Eclipse IDE provides a very user-friendly and intuitive interface to the programmer for controlling execution of a program in Debug Mode (Provide Snapshots of IDE at various stages of Debug Mode execution).
	* Setting and Removing a Break-point (also Toggling)
	* Stepping over a method call, or into and out of a method body (during a method call)
		* Stepping into ```int print()``` and ```int print(int)``` and ```int print(int,int,int)``` gives us interesting infromation, but stepping into ```System.out.printf``` can freak you out! So, you may want to step over it. 
	* For nested method calls, examine the method call **Stack Trace** (Call child, call parent relationship)
		* Example : ```int print()```, ```int print(int)``` and ```int print(int,int,int)``` method call chain of ```class MultiplicationTable```.
	* Viewing and Modifying current state of data variables, at a break point
	* Stepping through from one statement to another in the source code
		* As we step through, observe the view displaying changes in data variable values
		* Example of ```for``` loop control variable ```i```, inside method ```int print(int,int,int)``` of ```class MultiplicationTable```
		* Observe that execution exits from the ```for``` loop when the condition ```i<=10``` is no longer ```true```.
	* Re-executing a line of code
	* Skipping execution of all statements till next break-point
	* Ignoring all remaining breakpoints, resume execution of code till completion

### Eclipse IDE Keyboard Shortcuts

* Code Text Editor Shortcuts
* New Project/Class Creation Shortcuts
* Search for a Class

### Differences between JShell and IDE

Variables just declared, but used without an initialization, will flag a compilation  error in an IDE! But not so, it seems, in JShell. In regular software, variable initialization at point of declaration (called a "defintion", as we already know) is mandatory. 

##### Snippet-1 : JShell redefines variables on demand

```java

	jshell> int i = 2
	$1 ==> 2
	jshell> int i = 4
	$2 ==> 4
	jshell> long i = 1000
	$3 ==> 1000
	jshell>

```


When the following code (similar to the one given to JShell) is compiled manually or by IDEs such as Eclipse, it will flag errors! 

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

That is because Java source code is governed by strict **Scope Rules**.



Let's have another look at where we have reached with our solution, to the *PMT-Challenge* problem. Only now, let's change the code arrangement.

##### Snippet-01: Revisited - The *PMT-Challenge*

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

* We have now split the code into two source files: 
	* **_MultiplicationTable.java_**: Houses the ```MultiplicationTable``` ```class``` definition, with some methods we need.
	* **_MultiplicationRunner.java_**: Acts as the client of the ```MultiplicationTable``` ```class```, to invoke its functionality. It defines a ```main()``` method, that instantiates a ```MultiplicationTable```object, and invokes its ```print()``` method.
* After this code was rearranged, we still got it to work!

#### Print-Multiplication-Table: Enhancements

* We now want to enhance our current solution to this challenge, even though we've come a long way. **"Once you get the whiff of success, sky is the limit!"**. Here is the changes we need:
	* Pass the number whose table needs to be printed, as an argument
	* Pass the (continuous) range of numbers, whose index entries in the table are to be printed. (For example, printing the table entries for ```6```, with entries for indexes between ```15``` to ```30```).

One way to achieve all this, would involve overloading the ```print()``` method. The next example is one such attempt.

##### Snippet-02: print() overloaded

Overloading ```print()``` works for us, and we now support three ways in which to display  any table:

```java

		public static void print() {
			for(int i=1; i<=10;i++) {
				System.out.printf("%d * %d = %d", 5, i, 5*i).println();
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

The default table for ```5```, with entries fixed within ```1``` to ```10```. 

```java

		public static void print(int number) {
			for(int i=1; i<=10;i++) {
				System.out.printf("%d * %d = %d", number, i, number*i).println();
			}
		}

```

**_Console Output_**

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

Printing a table for any number, but with entries fixed between ```1``` and ```1```.

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

Displaying a table for any number, with entries for any range

The full code:

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

There is an issue with the code for ```class MultiplicationTable```. In the final print format, what if we are asked to replace the multiplication symbol '```*```' with an '```X```', so that school kids like it better? Since there are three calls to ```System.out.printf()```, one in each ```print()``` version, we make three changes.

##### Snippet-3: Code Duplication

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

**_Console Output_**

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

##### Snippet-3 Explained

* Humans make mistakes. The programmer missed out on changing the format symbol in the code for ```void print(int, int)```, but we don't recommend punishment. He could be overworked, or could only be the maintainer of code someone else wrote years ago! The point is not to blame human flaws (there are many), but to show how code duplication causes errors. This issue arises frequently with overloaded methods, point blank. 
* Instead of trying to change human nature, can we change our software? Let's have a closer look at ```print()```:
	* The method ```void print()``` prints the multiplication table for ```5``` only, in the default range ```1``` to ```10```.
	* The method ```void print(int)``` outputs the table for any number, but only in the fixed range from ```1``` to ```10```.
	* The method ```void print(int,int,int)``` displays the table for any number, in any range of entries.
	
#### A Solution: Code Reuse

There is something huge we observe in the previous example. All overloaded versions of ```print()``` have nearly the same code!

* ```print(int)``` has wider usage potential than ```print()```. The latter is a special case, as it prints only the for  ```5```.  We can achieve what ```print()``` does, by passing a **fixed** parameter value of ```5``` to ```print(int)```. It's simple: invoke ```print(int)``` within ```print()```, by passing ```5``` to it.
* The point to note is, that **a more specialized function can be implemented-in-terms-of a more general function**. 

Let's now reorganize this part of the code.

##### Snippet-4: Code Reuse

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

##### Snippet-4 Explained

When we call a method inside another, the method call statement is replaced by its body (with actual arguments replacing the formal ones). In the new definition of ```int print()``` above, the code executed during the call will be:

```java

	for(int i=1; i<=10;i++) {
		System.out.printf("%d * %d = %d", 5, i, 5*i).println();
	}

```

#### Extending Code Reuse

* The method ```int print(int,int,int)``` is a more general version of ```int print(int)```. We can achieve what the latter computes, by passing **fixed** range of indexes, namely  ```1``` and ```10```, as arguments to the former. have look into he code that follows.

##### Snippet-5 : Extending code reuse

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

**_Console Output_**

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

##### Snippet-5 Explained

* This example merely extended what we did in the previous example. We will will take this extension one level further now! Yes, you guessed right. We will implement ```print()``` in terms of ```print(int,int,int)```.

##### Snippet-6 : Extending code reuse (contd.)

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

##### Snippet-6 Explained

*  By extending the same logic of code reuse, the method ```int print(int,int,int)``` can be used to implement the logic of ```int print()```. Just pass in a number parameter ```5```, as well as the fixed range parameters ```1``` and ```10```, in a call to the former. ```int print()``` is thus **implemented-in-terms-of** ```int print(int,int,int)```.

* Our new version of ```class MultiplicationTable``` looks like this:

##### Snippet-7: Extending Code Reuse (Contd.)

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

* The logic of the ```class MutliplicationRunner``` does not change at all:

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

##### Snippet-7 Explained

Neat, isn't it! To make our program school kid friendly, we just need to change one character in the code, take a peek below.

##### Snippet-8 : Extending Code Reuse (Contd.)

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

**_Console Output_**

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

##### Snippet-8 Explained

Software Development is an iterative process. The best code that we want to write does not happen at one go. It starts off at a certain level, and can always be improved. More importantly, such improvements needs to be remembered, to be applied again at different points in the same program, and across programs. This process is called **Code Refactoring**. Thought we'd keep you posted.

#### Summary

In this step, we:

* Explored how to reorganize the code for *PMT-Challenge* into a ```class```
* Understood that overloading works the same way for ```class``` methods
* Observed that code reuse is possible across overloaded versions of a ```class``` method

## Object Oriented Progamming (OOP)

How do you design great Object Oriented Programs?

Let's find out

Recommended Videos:
- Object Oriented Progamming - Part 1 - https://www.youtube.com/watch?v=NOD802rMMCw
- Object Oriented Progamming - Part 2 - https://www.youtube.com/watch?v=i6EztA-F8UI

### Step 01: Object Oriented Progamming (OOP) - Basic Terminology

Let's consider a few examples before we get to Object Oriented Progamming.

Humans think in a step by step process.

Let's say I've to take a flight from London to New York. This is how I would think:

- Take a cab to London Airport
- Check in
- Pass Security
- Board the flight
- Wish the Hostess
- Take Off
- Cruise
- Land
- Get off the plane
- Take a cab to ..

Procedural programming is just a reflection of this thought process. A procedural program for above process would look something like this:

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

Object Oriented Programming (OOP) brings in a new thought process around this. 

How about thinking in terms of the different Actors? How about storing data related to each actor right beside itself? How about giving them some responsiblity and let them do their own actions?

Here's how our program would look like when we think in terms of different actors and give them data and responsibilities

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

Do not worry about the implementation details. Focus on the difference in approaches.

We have **encapsulated** data and methods into these entities, which are now called **objects**. We have defined object boundaries, and what it can (and cannot) do. 

An object has
* **State** : Its data
* **Behavior** : Its operations

The ```position``` of an ```Airplane``` can change over time. The operations that can be performed on an ```Airplane``` include ```takeOff()```, ```land()``` and ```cruiseMode()```. Each of these actions can change its ```position```. Therefore, an object's behavior can affects its own state.

It's now time to introduce you to some core **OOP** terms, which will make our future discussions easier.

#### OOP Terminology 

Let's visit and enhance  the ```Planet``` example we had written a few sections ago. This time, let's also explore the conceptual angle.

**_Planet_**

```java

	class Planet
		name, location, distanceFromSun // data / state / fields
		rotate(), revolve() // actions / behavior / methods

	earth : new Planet
	venus : new Planet

```

Let's look at some **OOP** terminology.

A **class** is a template. An **object** is an instance of a class. In above example, `Planet` is a class. `earth` and `venus` are objects.
* ```name```, ```location``` and ```distanceFromSun``` compose object state.
* ```rotate()``` and ```revolve()``` define object's behavior.

**Fields** are the elements that make up the object state. Object behavior is implemented through **Methods**.

Each Planet has its own state:
* ```name```: "Earth", "Venus"
* ```location``` : Each has its own orbit
* ```distanceFromSun``` : They are at unique, different distances from the sun

Each has its own unique behavior:
* ```rotate()``` : They rotate at different rates (and in fact, different directions!)
* ```revolve()``` : They revolve round the sun in different orbits, at different speeds

#### Summary

In this step, we:

* Understood how OOP is different from Prodedural Programming
* Learned about a few basic OOP terms

### Step 02: Programming Exercise PE-01

#### Exercises

In each of the following systems, identify the basic entities involved, and organize them using object oriented terminology:

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

### Step 03: Creating ```MotorBike``` ```class``` 

In this series of examples, we want to model your pet mode of transport, a motorbike. We want to create motorbike objects and play around with them.

We will start with two java files: 
* **_MotorBike.java_**, which contains the ```MotorBike``` ```class``` definition. This ```class``` will encapsulate our motorbike state and behavior 
* **_MotorBikeRunner.java_**, with ```class MotorBikeRunner``` holding a ```main``` method, our program's entry point

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

**_Console Output_**

_Bike started!_

_Bike started!_

##### Snippet-1 Explained

We started off creating a simple `MotorBike` class with a `start` method. We created a couple of instances and invoked the `start` method on them.

We created two classes because we believe in `Seperation of Concerns`: 
- `MotorBike` class is responsible for all its data and behavior.
- `MotorBikeRunner` class is responsible for running MotorBike examples.

#### Summary

In this step, we:

* Defined a ```MotorBike``` ```class``` allowing us to further explore *OOP* concepts in the next steps

### Step 04:  Programming Exercise OO-PE-02

#### Exercises

1. Write a small Java program to create a ```Book``` ```class```, and then create instances to represent the following book titles:
	* "The Art Of Computer Programming"
	* "Effective Java"
	* "Clean Code"

#### Solution

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

**_Console Output_**

_The Art Of Computer Programming_

_Effective Java_
	
_Clean Code_

### Step 05: ```MotorBike``` -  Representing State

An object encapsulates both *state* and *behavior*. 

*State* defines "the condition of the object at a given time". *State* is represented by **member variables**. 

In the ```MotorBike``` example, if we need a ```speed``` attribute for each ```MotorBike```, here is how we would include it.

##### Snippet-1 : MotorBike with state variable speed

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

**_Console Output_**

_Bike started!_

_Bike started!_

##### Snippet-4 Explained

```int speed;``` within ```MotorBike```, defines a member variable. 

It can be accessed within objects such as ```ducati``` and ```honda```, by qualifying it with the object name (```ducati``` or ```honda```).

```
ducati.speed = 100;
honda.speed = 80;

```

```ducati``` has its own value for ```speed```, and so does ```honda```. These values are independent of each other. Changing one does not affect the other.

#### Classroom Exercise CE-OO-01

1. Update the ```Book``` ```class``` created previously to include a member variable named ```noOfCopies```, and demonstrate how it can be set and updated independently for each of the three titles specified earlier.

#### Solution

TODO

### Step 07: ```MotorBike``` - get() and set() methods

In the previous step. we were merrily modifying the ```speed``` attribute within the ```ducati``` and ```honda``` objects directly, from within the ```main()``` program. 

```java
	public class MotorBikeRunner {
		public static void main(String[] args) {
			//... Other code
			ducati.speed = 100;
			honda.speed = 0;
		}
	}
```

This did work fine, but it breaks the fundamental principle of encapsulation in **OOP**. 

*"A method of one object, should not be allowed to directly access the state of another object. To do so, such an object should only be allowed to invoke methods on the target object*".

In other words, a member variable should not be directly accessible from methods declared outside its ```class```.

##### Snippet-3 : MotorBike class with private attributes

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

**_Console Output_**

_Bike started!_

_Bike started!_

##### Snippet-3 Explained

By declaring ```speed``` as ```private```, we provide ```MotorBike``` with something called **access control**. Java keywords such as ```public``` and ```private``` are called **access modifiers**. They control what external objects can access within a given object.

Let's look at ```this.speed = speed;``` in the body of method ```setSpeed()```:
*  An member variable always belongs to a specific instance of that ```class```.
*  A method argument behaves just like a local variable inside that method.
*  To differentiate between the two,  ```this``` is used. The expression ```this.speed``` refers to the member variable ```speed``` of a ```Motorbike``` object. ```setSpeed()``` would be invoked on that very object.  

Code written earlier within ```MotorBikeRunner```, such as ```ducati.speed = 100;``` would now result in errors! The correct way to access and modify ```speed``` is to invoke appropriate methods such as  ```setSpeed()```, on ```MotorBike``` objects.

#### Classroom Exercise CE-OO-02

1. Update the ```class``` ```Book``` to make sure it no longer breaks Encapsulation principles.

#### Solution

TODO

#### Summary

In this step, we:
* Learned about the need for access control to implement encapsulation
* Observed that Java provides access modifiers (such as ```public``` and ```private```) for such control 
* Understood the need for ```get()``` and ```set()``` methods to access object data

- - - 
### Step 08: Accessing Object State

Encapsulation is needed to protect an object's state from direct access by other objects. We were able to protect the state of ```MotorBike``` objects by declaring ```speed``` to be ```private```. We have created a sort of rigid situation here, since the ```private``` declaration of ```speed``` forbids even a *get* access. How do we address this issue? Again, the answer is to provide a method for reading the current ```speed```.

##### Snippet-4 : ```getSpeed()``` of ```MotorBike```

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

**_Console Output_**

_Bike started!_

_Bike started!_

_Current Ducati Speed is : 100_

_Current Honda Speed is : 80_

##### Snippet-4 Explained

Defining a method such as ```getSpeed()``` allows us to access the current```speed``` of a ```MotorBike``` object.

```
		int getSpeed() {
			return this.speed;
		}
```


> Eclipse has a very handy feature. When the state elements (member variables) of a class have been defined, it can generate default get() and set() methods for each of them. You would want to use this regularly, to save on time and typing effort. `Right click on class > Generate Source > Generate Getters and Setters`

#### Summary

In this step, we:

* Understood how access control forces us to provide ```get()``` methods as well
* Explored a few Eclispe tips to generate ```get()``` and ```set()``` versions for each ```class``` attribute  

### Step 10: Default Object State

What happens if a data element inside an object is not initialized with a value?

##### Snippet-5 : Default Initialization of Object State

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

**_Console Output_**

**_Current Honda Speed is : 0_**

##### Snippet-6 Explained

When we instantiate an object, all its state elements are always initialized, to the default values of their types. Inside ```MotorBike```, ```speed``` is declared to be an ```int```, and so is initialized to ```0```. This happens even before any method of ```MotorBike``` is called, including ```start()```.

You can see that `honda.getSpeed()` printed `0` even though we did not explictly initialize it.

Default 

#### Summary

In this step, we:
* Learnt that default values are assigned to object member variables.

### Step 10: Encapsulation: Its Advantages

At the heart of encapsulation, is the need to protect object's state. From whom? Other objects. 

Let's look at an example to understand Encapsulation better.

##### Snippet-7 : Advantage of Encapsulation

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

**_Console Output_**

_Bike started!_

**_Current Ducati Speed is : -100_**

##### Snippet-01 Explained

For a motorbike, ```-100``` might be an invalid speed. Currently, we do not have any validation. Having a method ```setSpeed``` allows us to add validation. 

Let's see how to do that.

##### Snippet-02 : Speed Validity Check

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

The output of this snippet is:

_Bike started!_

**_Current Ducati Speed is : 0_**

##### Snippet-8 Explained

```setSpeed()``` checks `if(speed > 0)` and does not update speed for negative values. 

> This is not perfect solution because the caller of the `setSpeed` method assumes that he was successful. Ideally, we should throw an Exception indicating validation error. We will talk about Exceptions later.

#### Summary

In this step, we:

* Explored the first advantage of encapsulation - A provision for adding data validation
* Highlighted how such validation can be done, using the ```Motorbike``` example

### Step 11: Encapsulation - Advantages (Code Reuse)

We've understood quite a few things about encapsulation under *OOP*.

Suppose at different points of time, we want to increase the speeds of both Honda and Ducati bikes by a fixed amount, say ```100 mph```. The logic would be simple, right? Fetch the current ```speed``` of each bike, increment that fetched value by ```100```, and then set the new value back into that bike's ```speed```. The following example puts the above logic into action.

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

##### Snippet-1 Explained

Notice the repeated code within ```MotorBikeRunner```? The code for updating the ```speed``` of ```ducati```, is almost the same as that for ```honda```. Remember at the start of this book, we said something like this:

*"The goal of any computer program is to make a task easier, less cumbersome and more elegant for the programmer."*

*OOP* achieves all thus through encapsulation! The idea is to *encapsulate* repeated logic within a method, and pass object-specific information to it as arguments. The next example shows you one way of doing it.

##### Snippet-2 : Speed Increase through Code Encapsulation

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

##### Snippet-2 Explained

The method ```increaseSpeed()``` has been added to ```MotorBike```. It can be invoked on the ```ducati``` and ```honda``` objects.

Let's now add a feature to ```MotorBike```, by which ```speed``` can be decreased.

##### Snippet-3 : Speed Increase And Decrease through Code Encapsulation

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

##### Snippet-3 Explained

The method ```decreaseSpeed()``` has been added to ```MotorBike```. It can be invoked on the ```ducati``` and ```honda``` objects inside the ```main()``` method of ```MotorBikeRunner```.

On of the things you can observe again is ***Negative Speed Values***. Our validation needs to be improved.

##### Snippet-4 : Validation across methods, repeated!

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

##### Snippet-4 Explained

We have achieved data validation, because attempts to decrease the ```speed``` of ```ducati``` and ```honda``` below ```0``` are now ignored. 

But this has come at a cost,  which is *code bloat*.

How do we reduce duplication?

##### Snippet-5: Validation by code reuse

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

##### Snippet-5 Explained

The idea behind this solution is, that an *update* is the same as a ```set()``` operation. Since ```setSpeed()``` already has a validation check, it can be called inside both ```increaseSpeed()``` and ```decreaseSpeed()``` with appropriate parameters. 

In this way, the validation logic would be reused across update methods.

> Be always careful. Duplication of logic makes your code difficult to maintain.

#### Summary

In this step, we:

* Started exploring the next advantage of encapsulation - code reuse
* Mapped this understanding to the ```MotorBike``` example, building on data validation  

### Step 12: Programming Exercise PE-OO-03

#### Exercises

1. Use an encapsulation technique to write methods for the ```Book``` ```class```, that
	* Increase the number of books
	* Decrease the number of books

#### Solution

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

**_Console Output_**

_The Art Of Computer Programming_

_Effective Java_
	
_Clean Code_

_5_

_5_

_5_

### Step 13: Introducing Constructors   

When we create Ducati and Honda motorbikes, we may want to configure them with some start speeds. 

Suppose our whim is that a Ducati bike starts with 100 mph, and a Honda with 200 mph. 


##### Snippet-1: MotorBike Constructor

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

##### Snippet-1 Explained

We defined a single-argument constructor for ```MotorBike```, whosw definition looks like this:

```public MotorBike(int speed){ /* Constructor Code Goes Here  */ }```

The constructor is a method, whose name is the same as the ```class``` name. All Java rules for a method apply to constructors as well. Constructor cannot be directly called. 

A constructor is always invoked when a ```class``` object is created, using the ```new``` keyword. A constructor for a ```class``` could accept zero, one or more than one arguments. Let's next write some full-blooded code for a ```MotorBike``` constructor.


#### Summary

In this step, we were introduced to the concept of a ```class``` constructor

### Programming Exercise PE-OO-04, And More On Constructors

#### Exercises

1. Rewrite the ```Book``` ```class``` solution by using a constructor, which accepts an integer argument specifying the initial number of copies to be published:
	* "The Art Of Computer Programming" : 100 copies
	* "Effective Java" : 75 copies
	* "Clean Code" : 60 copies

#### Solution To PE-OO-04

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

**_Console Output_**

_The Art Of Computer Programming_

_100_

_Effective Java_

_75_
	
_Clean Code_

_60_

#### More on Constructors

We enjoyed defining the ```MotorBike``` ```class``` and checking out the behavior of its instances, ```ducati``` and ```honda```. 

When we started off , we created instances of `MotorBike` classes using:

```MotorBike ducati = new MotorBike();```

Did you notice something familiar? Doesn't the expression ```new MotorBike()``` look like a constructor call? 

As it turns out, it is a constructor call on ```MotorBike```! 

When we define a ```class``` in Java (even a seemingly empty one), some behind-the-scene magic happens. Consider one such ```class``` ```Cart```:

```java

	class Cart {

	};

```

This ```class``` has neither state, nor behavior. When we try to create instances of this "empty" ```class```:

```java

	class CartRunner {
		public static void main(String[] args) {
			Cart cart = new Cart();
		}
	}

```

The code seems to compile, execute and get initialized quite smoothly! What happens is, that the compiler silently generates a **default constructor** for ```Cart```. 

A default constructor is one that accepts no arguments. It is as if the ```Cart``` ```class``` were defined this way:

```java

	class Cart {
		public Cart() {
		}
	};

```

A constructor may also have overloaded definitions. 

Let's now try to create ```MotorBike``` instances with default initialization, just as we did with ```Cart```.

##### Snippet-2 : Default Motorbike Construction?

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

**_Console Output_**

**_Compiler Error_**

##### Snippet-2 Explained

The compiler flags an error with **_MotorBikeRunner.java_**! `MotorBike yamaha = new MotorBike();` is failing compilation. Why?

No default constructor is generated here! If you provide any constructor definition in a class, the compiler will not add a default constructor. **Do them all yourself, if you don’t like what I do for you!** is what it yells back.

If you need the default constructor, you can explicitly add it.

##### Snippet-3 : Programmer-defined default constructor

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

##### Snippet-3 Explained

We defined a zero-argument constructor ```MotorBike()```, to enable default object initialization. But what are we doing in its body with the statement ```this(5);```? 

We have called the constructor ```MotorBike(int)```, qualified with the ```this``` keyword, within ```Motorbike()```. 

## Primitive Data Types

Earlier, we looked at basic Java types (including ```int```, ```double``` and ```boolean```), and got a little familiar with them.

We used literal values, declared variables and formed expressions using them. 

Java **primitive types** include:
* Integer Types
	* ```byte```
	* ```short```
	* ```int```
	* ```long```
* Floating-Point Types
	* ```float```
	* ```double```
* Character Type
	* ```char```
* Logical Type
	* ```boolean```

In this section, let's play with each of these types to understand them further.

### Step 01: The Integer Types

Integers are not much of a mystery, are they? They've been part of us since our school days, and we normally prefer them over other numbers (they scare us less!). 

Java supports them with ease, and we have coded quite a few examples using them, already. 

Java also has a **wrapper class** corresponding to each of them, which make their primitive versions more versatile. The wrapper classes we are talking about are:

* ```Byte```: for ```byte```
* ```Short```: matching ```short```
* ```Integer``` corresponding to ```int```
* ```Long```: about ```long```

Let's see how we can work with them.

##### Snippet-01 : Integer Sizes

Look at all the information these tiny classes hold for you! As they say, **_"fore-warned is fore-armed"_**. Depending on the data (range and size) your program handles, you decide which types to use, to store them.

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

#### Integer Type Conversions

Problems will (and should) arise if we attempt to store large data into smaller bins. The compiler warns the programmer about such issues by flagging errors. However, if the programmer is aware of the risks and intends to go ahead, **explicit casts** are her tools to push the code through.

Operations in the other direction (storing a smaller data value in a larger bin), is a piece of cake for the compiler. Such a conversion is called an **implicit cast**.

##### Snippet-02 : Integer Type Conversions 

Attempting to store a ```long``` value into an ```int``` variable will give us a compiler error. However, you can use an explicit cast, such as ```i = (int) l;```.

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

**_The compiler is not responsible for the type-safety of this statement. The onus is on me, the programmer._**

Remember our earlier statement on possible incorrect program behavior? As you can see, a different value got stored in ```i```.

#### Summary

In this step, we:

* Explored the wrapper classes present for the primitive integer types
* Understood the different capacities and data ranges of these types
* Examined how to use explicit and implicit casts

### Step 02: Integer Representations, And Other Puzzles

In a decimal system, the allowed digits are ```0``` through ```9```. When a value of ```10``` is encountered, the number of digits increases by 1, and its representation is "```10```".

Those familiar with number systems would know that decimal is not the only system that computers understand. 

Other number systems that the Java language supports are **Octal** (Base-8) and **Hexadecimal** (Base-16). 

In an Octal system, the allowed digits are ```0``` through ```7```, and a value ```8``` is represented by "```010```". The leading ```0``` is added only to distinguish the octal format from the decimal one. 

In a Hexadecimal system, the allowed digits are ```0``` through ```9```, followed by ```a``` through ```f``` (or ```A``` through ```F```). A value of ```16``` is represented by "```0x10```". Here, a leading ```0x``` is added to help the compiler recognize Hexa decimal representation.

Let's see how Java supports these three number systems.

##### Snippet-01 : Storing Octal and Hexadecimal in Integer types

There are no number-system specific integer types in Java! The same ```int``` type is used to store decimal, octal and hexadecimal values. 

If we adhere to to number system conventions about valid digits and understand the compiler hints, we get no surprises.

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

##### Snippet-02 : More Integer Type-casting

There are two kinds of assignments:
* Literal-to-variable assignment: With ```short s = 123456;```, the data is clearly out of range (this is known at compile-time). The compiler flags an error.
* Variable-to-variable assignment:  Consider ```sh = in;```. The value stored in ```int in``` at that stage was ```4567```, which is well within the range of the ```short``` type. The compiler chooses not to take chances and flags an error. This can again be preempted with a explicit cast `sh = (short) in`.


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

#### Built-In Operators For Integer Types

We already had a glimpse of arithmetic operators for the integer types:
* ```+```
* ```-```
* ```*```
* ```/```
* ```%```
* ```++``` (both prefix and post-fix increment)
* ```--``` (both prefix and post-fix increment)

The increment and decrement operators are an interesting case, as they are actually short-hands for multiple statements. When we use their prefix and post-fix versions, we need to look out for side-effects.

##### Snippet-03 : Increment & Decrement Operators

With post-fix increment, such as in ```int j = i++;```, the increment takes place *after* the assignment is done. ```j``` gets the value before increment.
```java

	jshell> int i = 10;
	i ==> 10
	jshell> int j = i++;
	j ==> 10
	jshell> i
	i ==> 11
```

When prefix increment is involved, as with ```int n = ++m;```, the increment is carried out *before* the assignment. ```n``` gets the value after increment.

```java
	jshell> int m = 10;
	m ==> 10
	jshell> int n = ++m;
	n ==> 11
	jshell> m
	m ==> 11
```

With post-fix decrement, as with ```int l = k--;```, the decrement occurs *after* the assignment is done. As far as prefix decrement is concerned, such as in ```int q = --p;```, the decrement is performed *before* the assignment.

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

#### Summary:

In this step, we:

* Looked at the number-systems supported in Java for integers
* Examined how prefix and post-fix versions work for increment and decrement operators

- - -	
### Step 03: Classroom Exercise CE-01 (With Solutions)

#### Exercise Set

1. Create a Java ```class``` ```BiNumber``` that stores a pair of integers, and has the following functionality:

	* Can be created by passing its initial two numbers to store
	* Must Support Addition and Multiplication operations on the stored integers
	* An operation to double the values of both numbers
	* Operations to access each number individually
	
In short, we must be able to write code like this in the ```main``` method of  our runner class:

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

**_Console Output_**

_5_

_6_

_4_

_6_

### Step 05: Floating-Point Types

You would recall there are two types in Java to support floating-point numbers:
* ```double```: The default type for floating-point literals, with a capacity of 8 bytes
* ```float```: A narrower, less precise representation for floating-point data. It has a capacity of 4 bytes.

Let's quickly refresh what we know, with a few code snippets.

##### Snippet-01 : double and float

Default floating point type in Java is `double`. A ```float``` literal must be accompanied with a trailing ```f``` or ```F```.


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

##### Snippet-02 : Operators for type double

You can use operators `++`, `--` and `%` on double. 

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

You would need an explicit cast to convert a float to an integer value `int i = (int)f`.

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
#### Summary

In this step, we:

* Saw how we create literals and variables of the floating-point types
* Understood the differences between ```double``` and ```float```

### Step 06: Introducing BigDecimal

Compact though they are, ```double``` and ```float``` are not very precise representations of floating-point numbers. 

In fact, they are not used in computations that require high degrees for accuracy, such as scientific experiments and financial applications. The next example shows you why.


```java

	jshell> 34.56789876 + 34.2234
	$1 ==> 68.79129875999999
```

The literal expression ```34.56789876 + 34.2234``` should evaluate to ```68.79129876```. Above addition is not really accurate.

This is due to a flaw in floating-point representations, used in the ```double``` and ```float``` types.

The ```BigDecimal``` class was introduced in Java to tide over these problems.

Accuracy of ```BigDecimal``` representation is retained only when ```String``` literals are used to build it.



```java

	jshell> BigDecimal number1 = new BigDecimal("34.56789876");
	number1 ==> 34.56789876
	jshell> BigDecimal number2 = new BigDecimal("34.2234");
	number2 ==> 34.2234_
```

A ```BigDecimal``` type can be used to create only **immutable** objects. The values in an *immutable* object cannot be changed after creation. 

You can see that the value of number1 is not changed on executing `number1.add(number2)`. To get the result of the sum, we create a new variable `sum`.

```java
	jshell> number1.add(number2);
	$2 ==> 68.79129876
	jshell> number1
	number1 ==> 34.56789876
	jshell> BigDecimal sum = number1.add(number2);
	sum ==> 68.79129876
```

#### Summary

In this step, we:

* Learned that ```double``` and ```float``` are not very precise data types
* Were introduced to the ```BigDecimal``` built-in data type
* Understood that ```BigDecimal``` is immutable
* Saw that accuracy is best achieved when you construct ```BigDecimal``` data using string literals 

### Step 06: BigDecimal Operations

Let's look at a few other operations defined in the ```BigDecimal``` class.

##### Snippet-01: Arithmetic Operations

All BigDecimal operations support only BigDecimal operands.

```java

	jshell> BigDecimal number1 = new BigDecimal("11.5");
	number1 ==> 34.56789876
	jshell> BigDecimal number2 = new BigDecimal("23.45678");
	number2 ==> 23.45678
	jshell> number1.add(number2);
	$1 ==> 34.95678
```

```BigDecimal``` does not jell well with primitive types.

```java
	jshell> int i = 5;
	i ==> 5
	jshell> number1.add(i);
	| Error:
	| incompatible types: int cannot be converted to java.math.BigDecimal
	| number1.add(i);
	|_____________^
```

We can add, multiple, divide or subtract `BigDecimal` values.

```java
	jshell> number1.add(new BigDecimal(i));
	$2 ==> 16.5
	jshell> number1.multiply(new BigDecimal(i));
	$3 ==> 67.5
	jshell> number1.divide(new BigDecimal(100));
	$4 ==> 0.115
	jshell>

```

#### Summary

In this step, we:

* Explored the ```BigDecimal``` methods for doing some basic arithmetic
* Found that ```BigDecimal``` has constructors accepting most basic Java numeric types

### Step 07: Classroom Exercise CE-02

#### Exercise-Set

Write a Program that does a Simple Interest computation for a Principal amount. Recall that the formula for such a calculation is:

`Total amount (TA) = Principal Amount (PA) + ( PA * Simple Interest (SI) Rate * Duration In Years (N))`

In essence, write a ```SimpleInterestCalculator``` ```class``` that can be used in the following manner:

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

**_Console Output:_**

_6187.50000_

#### Tip: The ```import``` Statement

The Java ```import``` statement is Required in each source file that uses a ```class``` from another ```package```. Hence, both **_SimpleInterestCalculator.java_** (```class``` definition) and **_SimpleInterestCalculatorRunner.java_** (runner ```class``` definition) need to import ```class``` ```java.math.BigDecimal```.

```package java.lang.*``` is imported by default. 

The ```.*``` suffix indicates that all classes in the ```package``` ```java.lang``` are being imported.

#### Summary

In this step, we:

* Used ```BigDecimal``` values in a stand-alone Java program
* Learnt how to make use of built-in Java packages, through the ```import``` statement 

### Step 08: ```boolean```, Relational and Logical Operators

The Java ```boolean	``` data type is one that holds only one of two values: ```true``` or ```false```. Both labels are case-sensitive. We have seen examples of built-in comparison operators, such as ```==```, ```!=``` and ```>```, that evaluate expressions to  give us ```boolean``` results. Let us do a quick recap of some of these.

##### Snippet-01 : Relational Operators : Recap

Relational Operators are used mainly for comparison. They accept operands of non-```boolean``` primitive data types, and return a ```boolean``` value.

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

#### Logical Operators

Java also has logical operators that are used in expressions. Logical operators expect ```boolean``` operands. Expressions involving these are used for forming ```boolean``` conditions in code, including within  ```if```, ```for``` and ```while``` statements.  The prominent logical operators are:

* ```&&``` : logical **AND**
* ```||``` : **OR**
* ```!``` : **NOT**

Let's learn how we use them in our code.

##### Snippet-02 : Logical Operators

We would want to find if `i` is between `15` and `25`.  An expression `i >= 15 && i <= 25` can be used. Details below.

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

An expression with```&&``` evaluates to ```true``` only if **both** its ```boolean``` operands evaluate to ```true```.

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

##### Snippet-02 Explained

The next example helps us visualize truth tables for the prominent logical operators.

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

#### Summary

In this step, we:

* We're introduced to the ```boolean``` primitive type
* Understood where logical operators are used in Java programs
* Explored the truth-tables of commonly used logical operators

### Step 09: Short-Circuit Evaluation (With Puzzles)

Consider code below. The expression ```j > 15 && i++ > 5``` evaluates to ```false``` as expected. `j>15` is `false` as `j` has a value of `15`. 


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

You can also observe that the value of i remains unchanged `10`.  

Why? Because ```i++ > 5``` was not even evaluated.
Why? `&&` is lazy. It saw that `j > 15` is false. Irrespective of the result of second expression, the result of this `&&` would be false. So, it does NOT evaluate the second expression.

***A more detailed explanation***

The expression ```j > 15 && i++ > 5``` was scanned from left to right. As the first operand to ```&&``` evaluated to ```false```, the compiler got lazy. `&&` avoids evaluating expressions that don't affect the final result. The optimization has a name: **Short-Circuit Evaluation**, also called **lazy evaluation**.


The logical operator ```&``` is another version of the logical **AND** operation, that does away with lazy evaluation. 

Both operands to ```&``` are always evaluated. 

```java

	jshell> j > 15 & i++ > 5
	$1 ==> false
	jshell> j
	j ==> 15
	jshell> i
	i ==> 11
	jshell>

```

Similarly, the logical **OR** operator also has two versions: 
* The ```||``` operator we saw earlier. This exhibits lazy evaluation.
* The ```|``` operator, without lazy evaluation.

It is bad programming practice for our code to depend on the compiler's lazy evaluation. It makes code less readable, and can hide difficult-to-fix software bugs. It obviously adds to the code maintenance burden, so don't do it unless you like being in your peers' bad books.        

#### Summary

In this step, we:

* Examined conditions involving logical operators, that had lazy evaluation
* Observed that the lazy evaluation depends on the operator's truth-table
* Saw versions of the operators without lazy evaluation
* Learned that code depending on lazy-evaluation, is less readable 

### Step 10: Character Types
 
Earlier, we explored how we could store basic keyboard characters(called **ascii-code** characters), such as:
* Upper-Case and lower-case letters (A-Z, a-z)
* Numeric characters (0-9)
* Punctuation and other special characters (such as ',', '$', '{', etc.)

Turns out Java supports a much larger family of character encoding sets, called **Unicode**. All Unicode characters can be input to, understood and processed by, as well as output from your code. 

##### Snippet-01 : Unicode characters

Not all Unicode characters can be input from your keyboard. But Java allows you to  handle their values from your code, if you deal correctly with their format.

```java 
 
	jshell> char ch = '"';
	ch ==> '"'
	jshell> char c = '\u0022';
	c ==> '"'
```

Integer values can be stored in ```char``` variables. If the value is within a meaningful range, it also corresponds to the **ascii** value of a keyboard character. 

```java
	jshell> char cn = 65;
	cn ==> 'A'
```

Integer arithmetic can be performed on `char` data.

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


#### Summary

In this step, we:

* Were introduced the the ```char``` data type
* Learned that Unicode takes the character set beyond your keyboard
* An ascii character is ```char``` value, encoded by an integer value

### Step 11: Programming Exercise PE-02

#### Exercise Set

1. Write a Java class ```MyChar``` that is a special type of ```char```. An object of type ```MyChar``` is created round an input ```char``` data element, and has operations that do the following:
	* Check if the input character is a:
		* Numeric Digit
		* Letter of the Alphabet
		* Vowel (Either upper-case or lower-case)
		* Consonant (Either upper-case or lower-case) NOTE: A letter is a consonant if not a vowel
	* Print all the letters of the Alphabet in
		* Upper-Case
		* Lower-Case

In Essence, a runner ```class``` for ```MyChar``` would have its ```main``` method run code similar to:

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

**_Console Output_** :

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

**_Console Output_** :

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

**_Console Output_** :

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

### Step 15: The Primitive Types - A Review

In this section, we built on our knowledge of the primitive Java types. 

* We first got familiar with built-in wrappers for the integer types, that store useful type information. 
* Going from the integer to the floating-point types, we examined type compatibility, and how the compiler warns you about common pitfalls. We used explicit casts to force type conversions, and learned that implicit type conversions are quite common.
* We moved on to the ```BigDecimal``` class, a floating-point type with greater precision and accuracy. 
* Next in line was ```boolean```, where we built on what we know of logical expressions. We focused on the logical operators, more so on short-circuit evaluation of their expressions. 
* We saw how dependency on side-effects, and on lazy evaluation, is not a good programming practice.
* Finally, we got to the ```char``` type, and were pleasantly surprised to know, that the keyboard is not the limit.

## Introducing Conditionals - if, switch and more

Decision making is a part of our daily lives. Computers do tasks for humans, so even programs need to make decisions. They do this by checking logical conditions, which evaluate to ```boolean``` values. 

In the following steps, we will explore the following **conditional** statements:

* ```if```
* ```if```-```else```
* ```if```-```else if```-```else```
* ```switch```  

What better way to master these basics, than using them to solve a programming challenge? 

Here we go!

#### Programming Challenge : Design A Menu (The *Menu-Challenge*)

* Ask the User for input:
	* Enter two numbers
	* Choose the arithmetic to do on those:
		* Add
		* Subtract
		* Multiply
		* Divide
* Perform the Operation
* Publish the Result

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

#### Summary

In this step, we:

* Discussed how input affects the control-flow of a program
* Listed out the conditionals available with Java
* Selected a programming challenge to help us learn about conditions

### Step 01: The ```if``` and ```if```-```else``` Conditionals

An ```if``` statement is the most basic way to manage control-flow in a program. A ```boolean``` condition is tested, and if found to be ```true```, some code is executed. Otherwise, that code is not run. 

* "**_Do Something when ```condition``` is ```true```_**"

Conceptually, the ```if``` statement looks like this:

```java

	if(condition) {
		<if-body>
	}

```

An ```if```-```else``` statement improves over the plain ```if```. We can now choose between executing two pieces of code, depending on what ```condition``` evaluates to.

* "**_Do Something when ```condition``` is ```true```, something else when ```condition``` is ```false```_**"

An ```if```-```else``` statement boils down to the following:

```java

	if(condition) {
		<if-body>
	} else {
		<else-body>
	}

```

If ```condition``` is found to be ```true```, the statement block ```<if-body>``` is executed, otherwise ```<else-body>``` is run.

Let's now look at a examples that make use of these conditionals.

##### Snippet-01 : ```if``` behavior

In this example:
*  we have used compound comparison operators such as ```<=``` and ```>=```, which also evaluate to ```boolean``` values. 
*  Also used, are logical operators such as ```&&``` and ```||```, which both accept and return values of type ```boolean```.



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

```if```-```else``` allows us to specify code to execute when a condition is `false`.

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

**_Console Output_**

_i != 25_

##### Snippet-03 : chained if-else v2

We would want to test a number for 3 conditions - `value is 24`, `value is 25` or `value is not 24 and 25`. Let's consider the code from the example below.

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

**_Console Output_**

_i = 25_

_i != 25 and i != 24_

##### Snippet-03 Explained

What just happened here? The value of ```i``` is set to ```25``` within the program, so like in the previous example, only **_i = 25_** should have been printed. 

Why the extra print?

We started off trying to check fro 3 possibilities:
	* ```i``` being equal to ```25```
	* ```i``` being equal to ```24```
	* Neither of the above

We get wrong output, because ```i == 25``` in first ```if``` is independent from ```i == 24``` in the ```if```-```else``` that follows it. 

Our decision making is not continuous. We need a tighter conditional to deal with more than two alternatives. We will explore this topic in the next step.

#### Summary

In this step, we:

* Learned about the ```if``` and ```if```-```else``` conditionals
* Tried out a few examples to see how they are used

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
	| method max() in interface java.util.stream.Stream
