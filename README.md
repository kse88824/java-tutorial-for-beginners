# Java Tutorial For Beginners
 
 본 저장소는 [java-tutorials-for-beginners](https://github.com/in28minutes/java-tutorial-for-beginners)을 한글로 번역합니다.
 
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
* [Chapter 10 - Array(배열)와 ArrayList](#array와-arraylist)
* [Chapter 11 - 객체 지향 프로그래밍 (*OOP*) - 복습](#객체-지향-프로그래밍-oop---복습)
* [Chapter 12 - 컬렉션의 이해](#컬렉션의-이해)
* [Chapter 13 - 제네릭의 이해](#제네릭의-이해)
* [Chapter 14 - 함수형 프로그래밍 소개](#함수형-프로그래밍-소개)
* [Chapter 15 - 스레드와 동시 실행](#스레드와-동시-실행)
* [Chapter 16 - 예외 처리의 이해](#예외-처리의-이해)
* [Chapter 17 - 파일 다루기](#파일-다루기)
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

### Step 02: The ```if```-```else if```-```else``` 조건문

```if```-```else if```-```else``` 구문은 우리가 직면하고 있는 해결하는 동시에 두 가지 이상의 조건을 시험하려고 한다. 
다음의 예를 보자.

##### Snippet-01 :  ```if```  조항에 일치하는 경우

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

**_콘솔창 출력_**

_i = 25_

이제 ```i```에 다른 값을 부여해보자.

##### Snippet-02: ```else if``` 조항에 일치하는 경우

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

**_콘솔창 출력_**

**_i = 24_**

##### Snippet-02 설명

* ```i```가 ```24```를 가지고 있는 상황에서 다른 조건(```i == 24```와 일치하는 것)은 ```참```으로 평가된다.

이제 지금까지 유일하게 미개척된 ```else```조항을 알아보자.

##### Snippet-03: ```else``` 조항에 일치하는 경우

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

**_콘솔창 출력_**

**_i != 25 and i != 24_**

##### Snippet-03 설명

```i```에게 ```26```이라는 값이 주어지면 처음의 두 조건은 거짓이다. 따라서, else의 코드가 실행된다.

 ```if```-```else if```-```else``` 구문에서는  _**한번에 단 한개만** ```참```으로 평가된다. 또한 일치하는 조항에 해당하는 코드 블록이 실행된다. 이는 조건이 *복제* 또는 *오버랩* 되더라도 보장된다. 그런 시나리오에서는 ```if```에서 첫 번째 조건만이 ```참```으로 평가될 것이다. 나머지 가능한 시도들은 점검조차 하지 않고 있다._
 


#### 요약

이번 단계에서는

* ```if```-```else if```-```else```조건문을 배웠다.
* 각 절이 실행될 때 점검하는 방법을 알아보았다.
* 조건부 코드 실행과 관련하여 Java에서 보장한 사항을 이해했다.

### Step 03:  Puzzles on ```if```

다음 퍼즐의 결과를 추측해보십시오.

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
 

> 아무것도 출력되지 않는다. 왜냐하면 코드는 이런 방식으로 구성되기 때문이다.

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

> 명시적 블록이 없는 경우, if문 옆에 있는 구문만 if문 블록의 일부로 간주한다.

### Step 04: Reading User Input
- - - 

*Menu-Challenge*의 구문을 다시 한 번 살펴보자:

#### *Menu-Challenge*

* 사용자에게 입력 요청:
	* 두 개의 숫자를 입력하십시오.
	* 산술 연산을 선택하여 다음 작업을 수행하십시오.
		* 더하기
		* 빼기
		* 곱하기
		* 나누기
* 작업 수행
* 결과 게시

우리는 ```if```-```else if```-```else```라는 조건문이 어떻게 작동하는지 잘 알고 있다. 그러나 우리가 모르는 것은 그러한 조건부가 무작위 입력을 받았을 때 어떻게 행동할 것인가 하는 것이다. 이러한 시나리오를 테스트하기 위해 다음 단계는 코드 내에서 콘솔 입력을 수행하는 방법을 배우는 것이다.

다음 예에서 바로 해볼 것이다.


##### Snippet-01: Reading console input

자바는 콘솔에서 사용자 입력을 스캔하기 위해 ```Scanner```라는 이름의 ```class```를 내장하고 있다. 이 유틸리티에서 프로그래머인 여러분은 다음을 해야 할 것이다:
* ```java.util.Scanner``` ```class```를 ```import```하시오 (여기서 우리는 이클립스 IDE에 코드를 작성하고 있다)
* ```Scanner```타입의 ```scanner```객체를 만드십시오. 여기에는 ```new```연산자를 통해 ```Scanner``` 생성자를 호출하는 것도 포함된다. ```scanner```를 콘솔 입력으로 묶어주는 ```System.in```도 생성자 매개변수로 전달해 주어야 한다.
* 콘솔에서 정수 입력을 읽으려면 ```scanner.nextInt()```를 호출해야 한다. 사용자 입력을 완료하려면 키보드의 <Enter>키를 눌러야 한다. 그 숫자는 당신의 코드로 전달된다.

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

**_콘솔창 출력_**

_Enter Number1: 35_

_The number you entered is: 35_


#### 요약

이 단계에서는

* *Menu-Challenge* 문제 구문을 다시 살펴본 결과, 사용자 입력을 읽어야 함을 알게 되었다.
* 이러한 요구를 충족시키기 위한  ```Scanner``` 유틸리티의 기본적 용도에 대해 알아보았다.

### Step 05: *Menu-Challenge* : 더 많은 입력 읽기

*Menu-Challenge*는 단일 사용자 입력에서 중지되지 않는다. 콘솔에 입력하려면 총 3개의 숫자를 입력해야 한다. 그러면 우리는 어떻게 계속해서 입력을 요청하고, 입력이 주어졌을 때 그것을 읽을 수 있을까?

##### Snippet-01 : *Menu-Challenge* 구현

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

**_콘솔창 출력_**

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

##### Snippet-01 설명

```scanner.nextInt()```를 반복적으로 호출하는 것은 사용자가 입력하는 숫자를 계속 읽게 될 것이다. 또한 사용자는 키보드의 <Enter>키를 눌러 각 입력을 전송할 필요가 있다.

우리는 필요한 세 가지 값을 모두 읽을 수 있을 뿐만 아니라 콘솔에 써넣었다. 사용자들은 이제 우리가 그 데이터를 얻었음을 알 수 있다!

#### 요약

이번 단계에서는

* 콘솔에서 두 개 이상의 입력을 읽는 방법을 파악했다.
* 프로그램 내에서 값이 어떻게 판독되고, 보존되고, 사용할 수 있는지 보여줬다.

### Step 06: *Menu-Challenge* - 입력 읽기, 결과 연산, 출력값 게시

우리는 이전 단계를 지났으니 어떤 것도 당신이 *Menu-Challenge*를 완성하는 것을 막을 수 없다고 생각한다! 여기 한 가지 방법이 있다. 

##### Snippet-01 : 모든 연산

위의 해결책은 매우 간단한 것이다. 이것은 *Menu-Chanllenge*를 해결하기 위해 우리가 학습한 입력과 점검한 조건식을 결합한 메커니즘이다.

```if```-```else```_```else if```구문은 총 ```5```개의 조항을 포함한다:
* ```4```개의 조건(```4```개의 연산을 지원하는 ```choice```)을 확인하기 위해, 한 개의```if```와 세 개의 ```else```-```if```항이 그러한 역할을 한다.
*```choice```에 해당하는 마지막 기본 조건은 ```else```로 처리된다.

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

**_콘솔창 출력_**

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

**_콘솔창 출력_**

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


#### 요약

이번 단계에서는,

* 조건식에 대한 지식과 최근에 배운 콘솔 입력 값 수집에 대한 것들을 결합했다.
* 궁극적으로는 *Menu-Challenge*문제를 해결했다.

### Step 07: ```switch``` 소개

우리의 초기 흐름 제어 관리 조건문 목록에도 ```switch```라는 구문이 적혀있던 것을 기억하는가. ```switch```도 여러 조건문을 시험하며 ```else```조건문처럼 디폴트 가능성을 다룰 수 있다. 개념적으로 ```switch문```은 다음과 같다.

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

```default``` 구문은 어느 사례도 일치하지 않을 때 실행된다. 

 ```break;``` 구문은 성공적으로 일치한 후 스위치문을 벗어나기 위해 사용된다.

```switch문```을 어떻게 사용하는지 예제를 통해 살펴보자.

##### Snippet-01: ```switch```문

```switch```를 사용하면 상당히 읽기 쉬운 코드로 연결될 수 있지 않은가? 우리가 이전 단계에서 사용한 ```if```-```else if```-```else```구문과 비교해 보자.

모든 ```case```절에서 ```break```라는 구문을 뺴는 것은 매우 흔한 오류이다. 그것은 **switch-fall-through**라는 상황을 초래한다. 여기서는 특정 ```case```절과 일치하더라도 ```break```절이 어디선가 부딪힐 때 까지 이 절에 따른 모든 구문은 순차적으로 실행된다!

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

`break`를 추가하면 매칭된 케이스만이 실행된다.

```java
	jshell> switch(i) {
	   ..>> case 1 : System.out.println("1"); break;
	   ..>> case 5 : System.out.println("5"); break;
	   ..>> default : System.out.println("default"); break;
	   ..>> }
	1
	jshell>
	
```

##### Snippet-02: MenuScanner 리팩토링

자, 이제 `MenuScanner`예제를 리팩토링하기 위해 `switch`구문을 사용해보자.

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

**_콘솔창 출력_**

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

**_콘솔창 출력_**

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

#### 요약

이번 단계에서는

* ```switch```조건문을 탐색했다.
* ```if문```과 동일한 제어 흐름을 어떻게 구현할 수 있는지 확인했다.
* Java 제어 흐름 보증을 위해 올바른 코딩의 중요성을 학습했다.

### ```switch```에 관한 퍼즐

이제 다양한 조건문으로 즐거운 시간을 보내자. 이 퍼즐들은 여러분이 여전히 깨어 있다는 것을 보장할 뿐만 아니라, 생각할 충분한 양분을 줄 것이다.


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

### Step 09: ```if문```들과 ```switch문``` 비교

조건문을 선택하는 방법에 대해 알기 위해 이 두 가지 접근법을 비교하고, 대조해 봅시다.

먼저 ```if```-```else if```-```else```구문을 사용한 예가 있다.

##### Snippet-01 : ```if```를 사용한 포맷된 출력

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


**_콘솔창 출력_**

_number1 : 5_

_number2 : 2_

_choice : 1_

_result : 7_

다음으로 ```switch```를 포함한 예가 있다.

##### Snippet-02 : ```switch```를 사용한 포맷된 출력

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

**_콘솔창 출력_**

_number1 : 5_

_number2 : 2_

_choice : 1_

_result : 7_

#### 요약

이번 단계에서는

* 동일한 조건문 코드가 ```if문``` 또는 ```switch문```을 사용하여 작성될 수 있다는 점에 주목했다.
* ```if문```은 그 규칙이 매우 엄격하기 때문에 틀리기 어렵다는 것을 알게 되었다. 그것은 ```boolean```의 조건문만을 평가하는 데 사용될 수 있다. 그러나 그것은 장황하지 않고 종종 읽기 어렵다.
* ```switch```조건문으로 정수 값만 확인할 수 있다는 사실을 알게 되었다. 이는 매우 간결하고 읽기 쉽다. 그러나 ```case```문과 ```default```라는 상대적인 순서는 정해져 있지 않고 ```break```라는 구문은 선택사항이다. 이는 여러분의 프로그램에 미묘한 오류로 이어질 수 있다.

### Step 10:  PE-03 프로그래밍 실습

1. 다음과 같은 연산을 하는 자바 ```클래스```를 작성하시오:
	* 0 (일요일)에서 6 (토요일) 사이의 숫자를 지정하여 평일인 경우 반환하여라.
	* 1 (1월)에서 12 (12월) 사이의 숫자를 지정하여 해당 달의 영어 이름을 반환하여라.
	* 1 (1월)에서 12 (12월) 사이의 숫자를 지정하면 해당 요일의 영어 이름을 반환하여라.
	
	
####  PE-03 솔루션

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

### Step 12: 삼항 연산자  ```?:``` 소개 
- - - 

The ternary operator ```?:``` is a logical operator, that works on three operands. Its functioning is similar to an ```if```-```else``` statement (Checking for just ```2``` conditions). Exactly one  of the two expressions is guaranteed to match.
삼항 연산자는 ```?:```은 세 개의 피연산자에 적용하는 논리 연산자이다. 그 기능은 ```if```-```else```구문(```2```개의 조건을 확인하는 것)과 비슷하다. 두 수식 중 정확히 한 수식은 일치하도록 보장되어 있다.

개념적으로, 그것의 구문은 다음과 같다.

*```결과 = ( 조건문 ? if문이 참일 경우 적용할 수식 : if문이 거짓일 경우 적용할 수식);```*
*```result = (condition ? expression-if-condition-true : expression:if-condition-false);```* 


개념적으로, 그것의 구문은 다음과 같다.

##### Snippet-01 : 삼항 연산자

`?:` 는 사용하기 쉽다. 아래에 몇 가지 예제를 살펴보자:

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

boolean타입이 아닌 다른 값으로 반환할 수 있다.

```java
	jshell> String ifEven = ( i%2==0 ? "YES" : "NO");
	ifEven ==> "NO"
	jshell> i = 6;
	i ==> 6
	jshell> ifEven = ( i%2==0 ? "YES" : "NO");
	ifEven ==> "YES"
```

두 식 모두 같은 타입의 값을 반환해야 한다.

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


#### 요약

이번 단계에서는

In this step, we:

* 좀 더 세밀한 자바 조건문인 ```?:```연산자를 발견했다.
* 대부분의 경우 ```if```-```else```구조로 작동하는 것을 보았다.

## 반복문

TODO 

### 자바 반복문 구조 복습: ```for``` and ```while```

여러분들이 기억할지 모르겠지만 ```for```반복문의 구조는 다음과 같다

```
for(initialization; condition; update) {```

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;```//<Statements Body>```

```}``` 

```

반복문 내부의 ```<Statements Body>```는 ```조건문```이 ```참```인 경우만 실행된다. 퍼즐을 어떻게 활용할 수 있는지 몇 가지 살펴봅시다.

##### Snippet 1 : 첫 번째 루프 퍼즐
```

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
```

##### Snippet-1 설명

```for```반복문의 세 가지 요소는 모두 선택적인 것들이다.

* ```initialziation```
* ```condition```
* ```update```
- - -

## 참조형 타입

### Step 01: 참조형 타입 소개

우리가 객체를 생성할 때 뒷부분에서는 어떤 일이 일어나는가?

```java

	jshell> class Planet {
	..>>}
	| created class Planet
	jshell> Planet jupiter = new Planet();
	jupiter ==> Planet@31a5c39e
```

`jupiter`라는 객체는 어디에 저장되어 있는가?

모든 자바 객체는 `Heap` 또는 `Heap Memory`에 생성된다.

Planet의 새로운 인스턴스를 만들면, 힙에 생성된다.

```java
	jshell> new Planet()
	$18 ==> Planet@3f49dace
```

`new Planet()` 은 힙에 객채를 생성했다. 위 예제의 `Planet@3f49dace`를 보면 객체는 힙의 `3f49dace`주소에 저장된다.


```java
	jshell> Planet jupiter = new Planet();
	jupiter ==> Planet@31a5c39e
```

`Planet jupiter = new Planet()` 은 두 가지 역할을 한다.
- 힙 `new Planet()`에 객체를 생성한다. 위의 예에서 객체는 힙 위치 `31a5c39e`에 생성된다.
- 힙에 있는 객체의 참조를 변수 `jupiter`에 저장한다. 위의 예에서 `31a5c39e`는 변수 `jupiter`에 저장된 값이다. 그것이 새로운 객체가 만들어진 객체의 위치이다.

다른 예를 들어보자.

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

`Heap`에 새로운 `Animal`객체 두 개가 만들어진다. 이들의 메모리 위치(`참조`)는 참조 변수인 `dog`과 `cat`에 저장되어 있다.

자바에서는 모든 클래스를 참조형 타입이라고도 한다. 기본형 변수 인스턴스를 제외하고, 모든 인스턴스 또는 객체는 힙에 저장된다. 객체에 대한 참조는 `jupiter`,`dog`,`cat` 등의 참조 변수에 저장된다.

#### 요약

이번 단계에서는
In this step, we:

* 참조가 무엇인지 알아보았다.
* 참조 변수의 내용이 어떻게 생겼는지 살펴보았다.

### Step 02: 참조: 사용법 및 퍼즐

참조 변수를 가지고 놀아보자.

프로그래머가 초기화하지 않은 참조는 자바 컴파일러가 ```null```로 초기화된다. ```null```은 **빈 공간**을 나타내는 특별한 변수이다. 다시 말해, ```Animal``` ```nothing```은 아무것도 의미하지 않는 것이다!


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
```cat```에 ```nothing```을 참조하는 것은 ```new animal(15)```(```cat```에 저장된)으로 만들어진 객체의 주소를 ```nothing```에 할당하는 것이다.

```java
	jshell> Animal dog = new Animal(12);
	dog ==> Animal@27c20538
	jshell> Animal cat = new Animal(15);
	cat ==> Animal@6e06451e_

	jshell> nothing = cat;
	nothing ==> 6e06451e
```

`nothing`과 `cat`이 `heap`의 같은 위치를 가리키고 있다. `nothing.id=10`을 할 때 우리는 `nothing`과 `cat`이 가리키는 객체의 `id`를 모두 바꾼다.

```java
	jshell> nothing.id = 10;
	$1 => 10
	jshell> cat.id
	$2 => 10
```

`nothing`을 `dog`이 참조하는 객체를 가리키도록 바꾸자.

```java
	jshell> nothing = dog;
	dog ==> 27c20538
	jshell> nothing.id;
	$3 => 12
	jshell>

```
`nothing.id`과 `dog`는 동일한 객체를 가리키기 때문에,`nothing.id`는 `dog`가 참조하는 객체의 값을 출력할 수 있다.

다음은 유의해야 할 몇 가지 중요한 사항이다.

* `nothing = dog` - 참조 간 할당은 참조된 객체 전체를 복사하지 않는다. 오직 참조만 복사한다. 할당 후 두 참조 변수는 동일한 객체를 가리킨다.
* `nothing.id =10` - 참조를 사용하여 참조하는 객체를 수정할 수 있다.

#### 참조 변수들 비교

예를 보자.

기본형 변수를 사용하여 할당은 값을 복사한다.

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

`j=i`는 `i`의 값을 `j`에 복사한다. 나중에 `j`의 값이 바뀌어도 `i`는 영향받지 않는다.


기본형 타입의 변수를 비교하는 것은 그 값을 비교하는 것이다.

```java
	jshell> i == j;
	$4 ==> false
	jshell> j = 5;
	j ==> 5
	jshell> i == j;
	$5 ==> true
```


몇 가지 참조형 변수를 만들어보자.

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

참조형 변수를 비교할 때, 우리는 여전히 값을 비교하고 있다. 그러나, 이 값은 참조로, 객체가 저장되는 메모리 위치의 주소이다. 참조된 객체 내부에 저장된 값은 비교에 사용되지 않는다.

```cat```과 ```ref```모두 ```new Animal(10)```을 사용하여 만든 ```Animal```의 단일 객체를 참조한다. `==`는 true를 반환한다.
```java
	jshell> cat == dog;
	$6 ==> false
	jshell> cat == ref;
	$7 ==> true
```

```dog=dog2```를 비교하는 것은 이 변수들이 가리킨 메모리 저장공간이 다르기 때문에 ```거짓```으로 평가한다. 이들은 ```id```필드(```12```)와 같은 값을 가지고 있다. 하지만 이는 중요하지 않다!

```java
	jshell> dog == dog2;
	$8 ==> false
	jshell>

```



#### 요약

이번 단계는

* 초기화 및 할당하는 동안 참조 변수가 작동하는 방식을 이해했다.
* 참조 변수에 대한 ```null```값의 관련성을 확인했다.
* 참조가 기본형 타입의 값과 어떻게 다른지 관찰했다.


### Step 03: ```String``` 소개

```"Hello"```,```"qwerty"```,```"PDF"```와 같은 일련의 문자열들은 다른 자료형들과 매우 다르다.

자바에서 일반적으로 일련의 문자열들은 ```String``` ```class```로 표현된다.

```String```은 여러 가지 내장된 유틸리티 메소드들을 제공한다. 

몇 가지 예를 보자.

```java

	jshell> "Test".length()
	$1 ==> 4
```

```"Test"```는 문자열 리터럴이기 때문에 컴파일러는 내부적으로 객체를 들어 ```String```이라는 타입을 부여하고 메모리를 할당한다. ```length()```는 ```String```의 메소드이기 때문에 ```"Test"``` 객체에서 호출될 수 있다.

아래의 예에서. ```str```은 ```"Test"``` 값을 포함하고 있는 ```String```을 참조한다. ```String```의 객체를 만드는 것은 자바에서 우리가 일반적으로 객체를 만드는 방법과는 다르다.
```String```의 생성자를 만들 필요는 없다. 이를 ```BigDecimal```객체를 만드는 방법과 비교해 보자.

```java
	jshell> String str = "Test";
	str ==> "Test"
	jshell> BigDecimal bd = new BigDecimal("1.0");
	bd ==> 1.0
```

String의 인덱스는 배열과 마찬가지로 ```0```부터 시작한다. ```charAt(int)``` 메소드는 인자 값을 인덱스로 취하고, 그 자리에 존재하는 문자열 기호를 반환한다.


```java
	jshell> str.charAt(0)
	$2 ==> 'T'
	jshell> str.charAt(2)
	$3 ==> 's'
	jshell> str.charAt(3)
	$4 ==> 't'
```

```substring()```메소드는 ```String```의 참조를 반환하고 있으며, 다음과 같은 오버로딩된 버전도 있다.
* ```substring(int,int)```메소드는 낮은 인덱스에서 시작하여 상위 인덱스 바로 앞에서 끝나는 일련의 문자열을 반환한다.
* ```substring(int)''' 메소드는 해당 인덱스에서 문자열 끝까지 일련의 문자열을 반환한다.


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


#### 요약

이번 단계에서는:

* 일련의 문자열을 나타내는 ```String```클래스가 소개되었다.
* ```String```클래스의 몇몇 유틸리티 메소드를 탐색했다.

### Step 04: PE-01 프로그래밍 실습과 ```String``` 유틸리티

#### 실습

1. 주어진 텍스트 문자열을 분리하여 개별의 문자들로 출력하는 메소드를 작성하라.

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

```String```클래스는 ```java.lang```패키지에 내장된 일부분이다. 그것은 일반적인 텍스트를 처리하기 위한 몇 가지 메소드를 제공한다. 그들 중 몇몇을 살짝 들여다볼까?

##### Snippet-01: ```String``` 유틸리티들

다음은 아래 예에서 사용되는 몇 가지 메소드입니다.
* ```indexOf()```: 두 가지 오버로딩된 버전이 있다. ```indexOf(char)```은 문자열에서 문자가 처음으로 생성되는 위치를 반환한다. ```indexOf(String)```은 문자열 내에서 처음으로 문자열이 시작하는 위치를 반환한다.
* ```lastIndexOf()``` : ```indexOf()```와 비슷하지만, "*처음*"이 아닌 "**마지막으로**" 대체한다.
* ```startsWith()``` : 문자열이 *특정한 문자*로 시작하는 경우 ```true```를 반환하고, 그렇지 않으면 ```false```를 반환한다.
* ```endsWith()``` : 문자열이 *특정한 문자*로 끝나는 경우 ```true```를 반환하고, 그렇지 않으면 ```false```를 반환한다.
* ```isEmpty()``` : 문자열이 비어 있으면 ```true```를, 그렇지 않으면 ```false```를 반환한다.
* ```equals()``` : 문자열이 인자와 같으면 ```true```를 반환하고, 그렇지 않으면 ```false```를 반환한다.
* ```equalsIgnoreCase()``` : 문자열이 인자와 같으면 ```true```를 반환하고 이 문자열은 무시한다. 그렇지 않으면 ```false```를 반환한다.


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


#### 요약

이번 단계에서는

* 작은 챌린지를 통해 ```String```프로그래밍 기술을 사용했다.
* 간단하면서도 유용한 ```String```유틸리티 집합을 살펴보았다.

### Step 05: ```String``` 의 불변

"**불변(immutable)**"이라는 단어를 들으면 어떤 생각이 떠오르는가? 

"불변"이라는 단어는 "변환성"의 개념 혹은 "변환"의 가능성과 관련이 있다.

"**변환**"은 "**바뀌는 것**"을 의미한다. 따라서 "불변"은 "**변경 불가**"를 의미한다.

```String``` 객체는 불변한다. 생성한 후에는 값을 변경할 수 없다.

```concat()```메소드는 두 개의 ```String``` 객체를 하나로 합친다. 


```java

	jshell> String str = "in28Minutes";
	str ==> "in28Minutes"
	jshell> str.concat(" is awesome")
	$1 ==> "in28Minutes is awesome"
```

그러나, `str`을 참조한 원래 값은 변경되지 않는다. `concat`메소드는 새로운 `String`객체를 만들어낸다.


```
	jshell> str
	str ==> "in28Minutes"
```

```concat()```과 마찬가지로 ```toUpperCase()```, ```toLowerCase()```,```trim()``` 메소드는 새로운 ```String```객체를 반환한다.

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

#### 요약

이번 단계에서는

* ```String```객체가 불변임을 이해했습니다.
* 새로운 객체를 반환하는 ```String```유틸리티들을 확인했습니다.

### Step 06:  더 많은 ```String``` 유틸리티들 

```+```기호는 덧셈만을 의미한다고 생각하지 않았나? 어떤 학생이라도 그렇다고 할 것이고, 그렇지 않으면 비웃을 것이다.

우리는 ```int```와 ```double```과 같은 기본형 숫자 타입들도 살펴보았다.

자바는 산수 교과서를 엄격하게 따르지 않는다.

```+```는 ```String```연결 연산자로도 사용될 수 있다.

```+```의 동작들은 이렇다.
* ```+```의 두 피연산자가 모두 숫자일 경우, 산술 연산 ```+```(덧셈)이 수행된다.
* 만일 피연산자 중 하나라도 ```String```이라면, 문자열 연결이 이루어진다.


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

아래의 예에서 `i + 20`을 출력할 때 다른 값들이 출력되는 것을 볼 수 있다.

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

```join()```은 일련의 `String` 값을 결합하는 데 사용된다. 

```java
	jshell> String.join(",", "2", "3", "4");
	$8 ==> "2,3,4"
```

```replace(String, String)```은 첫 번째 서브 문자열(첫 번째 인자)을 두 번째 서브 문자열(두 번째 인자)로 대치한다. `char`데이터 타입과도 호환된다.

```java
	jshell> "abcd".replace('a', 'z');
	$9 ==> "zbcd"
	jshell> "abcd".replace("ab", "xyz");
	$10 ==> "xyzcd"
	jshell>

```


#### 요약

이번 단계에서는

* ```+```연산자가 ```String``` 연결로 오버로딩될 수 있다는 것을 알았다.
* 상황에 따라 ```+```가 피연산자를 어떻게 해석하는지 관찰한다.
* ```join()```과 ```replace```와 같은 몇 가지 ```String```유틸리티 메소드를 알아보았다.

### Step 07: 변경 가능한 텍스트 저장

```StringBuffer``` 와 ```StringBuilder``` 는 문자열 리터럴을 수정할 수 있게 한다.

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

어떤 것을 사용할지 어떻게 선택하나요?
* `StringBuffer`은 스레드에 안전하다. 만약 멀티 스레드 프로그램을 작성하고 있다면 ```StringBuffer```를 사용하라. (스레드에 대해서는 나중에 나올 섹션에서 자세히 설명하겠다.)
* 그렇지 않으면 실행 시간과 메모리 사용 모두에서 더 나은 성능을 제공하는 ```StringBuilder```를 사용해야한다.

#### 요약

이번 단계에서는

* ```StringBuffer```와 ```StringBuilder```에 대해 배웠다.


### Step 08: 래퍼 클래스 소개 

자바의 각 기본형 타입에는 내장된 **래퍼 클래스**가 있다. 이 래퍼 클래스 도한 불변이다. (이와 비슷한 ```final```은 나중에)

다음은 자바에 내장된 래퍼 클래스 및 해당하는 기본형 타입 목록이다.
* ```byte``` : ```Byte```
* ```short``` : ```Short```
* ```int``` : ```Integer```
* ```long``` : ```Long```
* ```float``` : ```Float```
* ```double``` : ```Double```
* ```char``` : ```Character```
* ```boolean``` : ```Boolean```

코드에서 이러한 래퍼를 사용하는 주된 동기는 다음과 같다:
* 기본형 타입에 대응하는 타입 정보 접근
* 기본형 데이터가 w자동으로 객체 참조 타입으로 승격되는 자동 박싱 (Auto-Boxing) 기능
* 데이터 구조 (*컬렉션*이라고 함)를 중심으로 기본형 데이터 이동과 래퍼 스타일의 데이터 사용
* Auto-Boxing feature, where a primitive data is automatically promoted to an object  reference type
* Moving primitive type data around data structures (called *collections*), using their wrapper-style counterparts

다음 단계에서 이러한 동기들을 살펴보자.

#### 요약

이번 단계에서는

* 기본형 타입에서 사용할 수 있는 래퍼 클래스에 대해 알아보았다.
* 사용할 경우 이점에 대해 배웠다.

### Step 09: 래퍼 객체 생성하기

이제 래퍼 클래스가 무엇인지, 그리고 각 기본형 타입에 해당하는 래퍼 클래스가 무엇인지 알게 되었으니, 시험해 보자.

`new`를 사용하여 래퍼 클래스의 인스턴스를 만드는 것은 간단하다. 아래의 예시를 보자.

```java

	Integer hundred = new Integer("100");
	Boolean b1 = new Boolean("true"); //true
	Boolean b1 = new Boolean("True"); //true
	Boolean b1 = new Boolean("false"); //false
	Boolean b1 = new Boolean("False"); //false
	Boolean b1 = new Boolean("other arbitrary string"); //false

```
또한 ```valueOf()```메소드를 ```Integer```와 ```Float```같은 타입 내에서 사용하여 래퍼 객체를 만들 수도 있다.

```java

	Float floatWrapper = Float.valueOf(57.0f);
	int floatToInt = floatWrapper.intValue(); // 57
	Integer seven = Integer.valueOf("111", 2);
	Integer.toString(seven, 2);

```

#### valueOf와 new를 사용하여 래퍼 객체를 생성하는 것의 차이

```Integer.valueOf()```는 힙에서 동일한 가치를 지닌 기존의 ```Integeer```객체를 재사용한다. 동일한 값의 객체가 힙에 있으면 기존 객체에 대한 참조가 반환된다. 그렇지 않으면 새로 만들어진 ```Integer```객체의 참조가 반환된다.

래퍼 클래스는 불변하다. 따라서 위의 접근법이 효율적이고 명확하다.


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
#### 요약

이번 단계에서는

In this step, we:

* 기본형 데이터를 위한 래퍼 객체를 만드는 방법은 두 가지가 있다.
* ```valueOf()```는 불변성을 이용하여 효율성을 향상시킨다는 것을 알게 되었습니다.

### Step 10: Auto-Boxing과 일부 래퍼 상수

**자동 박싱(Auto-Boxing)** 은 자바 언어에서 **syntactic sugar**의 예이다. 이는 새로운 기능을 제공하지는 않지만 코드의 가독성을 향상시킨다.

자동 박싱은 ```Integer.valueOf()```에서 ```Integer```나 ```Float```등을 위해 사용하는 메커니즘을 재사용한다.

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

위의 예에서 `Integer sevenToo = 7000`은 자동박싱을 사용한다. `int`리터럴을 정수 값으로 업그레이드하고 있다. 이것은 `Integer.valueOf` 메소드를 사용하여 암묵적으로 이루어진다.

래퍼 클래스에서 사용할 수 있는 상수는 변수의 크기와 저장할 수 있는 값의 범위를 출력한다.

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


#### 요약

이번 단계에서는
In this step, we:

* 할당 연산자 경로를 사용하는 자동 박싱 메커니즘을 이해했다.
* 자동 박싱이 내부적으로 ```valueOf()```메소드를 어떻게 활용하는지 이해했다.

### Step 11: 자바의 ```Date``` API

내장된 Java 기본형 및 참조형 타입에 대한 논의는 날짜 API에 대해 배우지 않고는 끝나지 않았다고 할 수 있다.

Java SE 8 이전에는 ```Date```클래스의 인터페이스와 구현에 관한 현실적인 문제들이 많았다.

Java 8에서부터 Joda Date 프레임워크 기반의 ```Date```클래스를 위한 API를 제공하였다.

이 프레임워크 내에서 가장 중요한 세 가지 클래스는 ```LocalDate```, ```LocalTime```, ```LocalDateTime``` 이다.

##### Snippet-01 : java.time 유틸리티

```java.time.*``` 는 Jshell에서 자동으로 가져오지 않는다. 가져와보자. 

현재 날짜 및 시간 값에 엑세스하는 데 일반적으로 사용되는 유틸리티는 다음과 같다.
* ```LocalDate.now()``` : 현재 날짜 값을 읽을 수 있는 형식으로 반환한다. 
* ```LocalTime.now()``` : 현재 시간 값을 읽을 수 있는 형식으로 반환한다.
* ```LocalDateTime.now()``` : 현재 날짜와 시간 값을 조합하여 읽을 수 있는 형식으로 반환한다.

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

#### 요약

이번 단계에서는

In this step, we:

* ```java.time```패키지를 통해 제공되는 Java Date API를 살펴보았다.
* ```LocalDate```, ```LocalDate```, ```LocalTime```의 사용법을 알아보았다.

### Step 12:  ```java.time.LocalDate``` 사용해보기

우리는 어릴 때부터 달력을 봐왔다. 디지털 달력을 가지고 노는 건 어떤가?

`LocalDate`는 정보를 가져오는 메소드를 여러 가지 제공한다.
* 날짜 정보: 일/월/년 및 관련된 속성들
* 날짜 메타 데이터 정보: 윤년 여부 등 분류 관련 정보

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
```LocalDate``` 또한 불변이다. 제공된 여러 가지 메소드를 사용하여 일,월 및 연도를 더하고 뺄 수 있다. 이들 각각은 ```LocalDate```의 새로운 인스턴스를 반환한다.

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

```LocalDateTime```은 ```LocalDate```를 확장하고 시간 구성요소도 제공한다. 시간, 분, 초 및 나노초 값에 엑세스하여 계산을 수행할 수 있다.

#### 요약

이번 단계에서는

In this step, we:

* ```LocalDate``` ```클래스```가 제공하는 공통 유틸리티들을 보았다.
* ```LocalDate```,```LocalTime```, ```LocalDateTime```은 모두 불변이라는 것을 알게 되었다.

### Step 13: ```LocalDate```객체 비교

아래의 예에서 ```LocalDate```의 추가적인 유틸리티 메소드들을 살펴볼 수 있습니다.

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

아래에 보이는 메소드들을 사용하여 날짜를 비교할 수도 있다.

```java
	jshell> today.isBefore(yesterday)
	$5 ==> false
	jshell> today.isAfter(yesterday)
	$6 ==> true
	jshell>
	
```

이러한 메소드들은 ```LocalTime```과 ``LocalDateTime```클래스로도 이용할 수 있다.

## Array(배열)와 ArrayList

이제 Java - Array의 많이 사용되는 자료 구조를 이해하기 위해 다음과 같은 연습을 할 것이다.

`ArrayList`

자바 프로그램에서 학생 성적표를 모델링하여 다음과 같은 작업을 수행할 수 있도록 한다.

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

배열(Array)과 `ArrayList`와 같은 데이터 구조를 통해 동일한 종류의 여러 객체를 저장할 수 있다. 이를 **집합체**라고 한다.

### Step 01: ```배열```의 필요성

먼저 배열의 필요성에 대해 알아보자.

아래의 예를 생각해 보아라. 우리는 3개의 mark를 만들어 더하고 있다.


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

기존의 ```mark1```,```mark2```,```mark3```가 존재하는 mark 리스트에 ```mark4```라는 mark요소가 추가된다면, ```sum```은 계산하는 코드를 바꿀 필요가 있다.

이 모든 마크들은 비슷하다. 마크 그룹을 만들어 단일 변수의 일부로 저장하는 것은 어떠한가?

`mark` 배열을 만들어보자

```java

	jshell> int[] marks = {75, 60, 56};
	marks ==> int[3]{ 75,60,56 }
```
위의 예에서
* ```marks```는 ```배열```이다.
* `marks`는 여러 개의 ```int```값들을 저장한다.
* `marks`배열의 값은 3개이다.

배열에서 인덱스는 0에서 (배열의 길이 -1) 까지 실행된다. 위의 예제에서 인덱스는 0에서 2까지이다.

인덱스 연산자 '```[]```'를 사용하여 배열에서 특정 요소를 찾을 수 있다. ```marks[0]```라는 수식은 ```marks```라는 배열의 인덱스 ```0```에  저장된 첫 번째 배열 요소에 대한 매핑이다.

```java
jshell> marks[0]
$20 ==> 75

jshell> marks[1]
$21 ==> 60

jshell> marks[2]
$22 ==> 56
```
모든 값을 배열로 더하기 위해서 어떻게 코드를 작성해야 하는가?

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

위의 구조는 강화된 ```for```반복문이라고 불린다.

```mark```는 루프 제어 변수이다. 그것의 타입은 ```int```인 배열 요소의 타입과 일치해야 한다.

위의 ```for```반복문은 `mark`배열의 요소 수에 관계없이 사용할 수 있다.

### Step 02:  배열의 값 저장 및 엑세스

이 단계에서 배열에 대해 더 자세히 알아보자.

배열은 0개 이상의 요소를 저장하는 데 사용할 수 있다.


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

또한 new 연산자를 사용하여 배열을 생성할 수 있다. 이 때 배열의 크기를 지정해야 한다.

```java
	jshell> int[] marks2 = new int[5];
	marks2 ==> int[5]{ 0,0,0,0,0 }
```

배열ㅇ 인덱스를 사용하여 값을 할당할 수 있다.

`marks2[0] = 10`은 mark배열의 첫 번째 요소로 10을 저장한다.

```java
	jshell> marks2[0]
	$1 ==> 0
	jshell> marks2[0] = 10;
	$2 ==> 10
	jshell> marks2[0]
	$3 ==> 10
	jshell>

```
  
스니펫은 더 많은 예들을 보여준다.

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

`length`는 배열에서 요소의 수를 찾는데 사용될 수 있다.

```java
	jshell> marks2.length
	$6 ==> 5
	jshell> int marks3 = {};
	marks3 ==> int[0]{  }
	jshell> marks3.length
	$7 ==> 0
	
```
#### Classroom Exercise CE-AA-01

1. ```8```개의 ```int```값을 저장하기 위해 배열 ```marks```를 생성하고 ```for문```을 이용하여 그 값을 출력하는 프로그램을 작성하라.

Hint: ```mark.length```속성을 사용하라

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

### Step 04: 배열 초기화, 데이터 타입과 예외

아래 스니펫은 서로 다른 타입의 배열이 초기화 되는 방법을 보여준다.

요약: int - 0, double - 0.0, 부울 - false, 다른 객체 - null


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

배열 선언의 몇 가지 변형을 살펴보자.

기억해야 할 중요 사항
* 배열 정의의 선언 부분에는 배열의 차원이 포함되지 않아야 한다.
* 배열 정의의 할당 부분에는 배열의 차원이 포함되어야 한다.
* 배열의 모든 요소는 동일한 타입이어야 한다.

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
배열 이름은 힙에 배열이 생성되는 위치의 주소를 저장하는 참조 변수이다.

```java

	jshell> int[] marks4 = {1, 2, 3, 4, 5};
	marks4 ==> int[5]{ 1,2,3,4,5 }
	jshell> System.out.println(marks4);
	I@6c49835d
```
내장 메소드 ```Arrays.toString```은 배열의 요소를 출력하는 데 사용할 수 있다.

```java
	jshell> System.out.println(Arrays.toString(marks));
	[1, 2, 3, 4, 5]
	jshell>

```

### Step 05: 배열 유틸리티
- - - 

다음의 몇 가지 예를 살펴보자.
* 배열을 통한 반복
* 배열 요소의 대량 수정
* 배열 비교
* 배열 정렬

##### Snippet-01 : 배열을 통한 반복

강화된 ```for문```을 사용하는 것은 쉽고 직관적이다.

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

##### Snippet-02 : 배열 비교하기 & 채우기
 
```Array.fill```은 전체 배열을 지정된 값으로 채운다. 

```java

	jshell> int[] marks = new int[5];
	marks ==> int[5]{ 0,0,0,0,0 }
	jshell> Arrays.fill(marks, 100);
	jshell> marks
	marks ==> int[5]{ 100,100,100,100,100 }
```

```Array.equals```는 주어진 두 개의 배열으 비교하고, 다음의 경우에만 ```true```인 ```boolean``` 값을 반환한다.
* 두 배열의 길이가 동일함.
* 모든 인덱스에 대해 각 해당 인덱스의 요소가 동일함.

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

```Array.sort```: 한 번에 한 쌍의 요소를 비교함으로써 요소들의 위치 정렬을 수행한다.

```java
	jshell> Arrays.sort(array3);
	jshell> array3
	array3 ==> int[3]{ 2,3,3 }
	jshell>

```

### Step 06: Classroom Exercise  CE-AA-02

#### Exercise

이제 Java 배열과 내장된 유틸리티 메소드에 대한 지식을 바탕으로 시작했던 과제를 해결해보자.

```java

	Student student - new Student(name, list-of-marks);
	int number = student.getNumberOfmarks();
	int sum = student.getTotalSumOfMarks();
	int maximumMark = student.getMaximumMark();
	int minimumMark = student.getMinimumMark();
	BigDecimal average = student.getAverageMarks();

```

우리는 집합체```list-of-makrs```를 배열로 구현할 수 있다. 

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
### Step 08:  가변 인자 - 기본 사항

변수 개수의 인자를 허용할 수 있는 방법을 만들려면 어떻게 해야할까?

예를 들어보자. 중요한 부분은 매개변수 `int... values` 이다.

```java

	jshell> class Something {
	   ..>> public void doSomething(int... values) {
	   ..>> System.out.println(Arrays.toString(values));
	   ..>> }
	   ..>> };
	| created class Something
```

전형적인 매개변수는 `int values` 이었을 것이다. 이렇게 하면 매개변수 하나를 메소드에 전달할 수 있다.

`int ... values`에 있는 세 점 `...`은 무슨 차이가 있는가?

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

`doSomething`은 1개, 2개, 3개의 매개변수로 호출할 수 있다.

다른 예도 살펴보자.

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

변수 인자로 `sum`메소드를 만들었다. 어떻게 사용하는지 보자.

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
이 단계에서, 우리는 처음으로 가변적인 인자를 살펴보았다. 변수 인자를 사용하면 변수 개수의 인자를 메소드에 전달할 수 있다.

### Step 09: ```Student```를 위한 가변 인자 메소드

`Student` 수업에 몇 가지 메소드를 추가하여 가변적인 인자를 받아들이도록 해보자.

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

변수 인자 목록은 항상 메소드에 전달된 매개변수 목록의 끝에 있어야 한다. 다음 메소드 정의는 자바 컴파이러에서 **허용되지 않는다**

```java

	void process(int... values, String name) {

	}

```

- - - 
### Step 10: Arrays - Some Puzzles And Exercises 

몇 가지 퍼즐과 배열을 사용한 예제에 대해 설명한다.

객체 배열을 만들 때, 배열은 생성된 객체에 대한 참조를 유지한다.

```java

	jshell> class Person {
	   ..>> }
	| created class Person
	jshell> Person[] persons = new Person[5];
	persons ==> Person[5]{ null,null,null,null,null }
```

우리는 새로운 `Person`객체를 배열의 다른 요소에 할당할 수 있다.

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

배열 생성과 동시에 값을 초기화할 수도 있다. 

```java
	jshell> Person[] persons2 = {new Person(), new Person()};
	persons2 ==> Person[2]{ Person@3b088d51, Person@1786dec2 }
```

다음은 `String`배열을 초기화하는 방법이다.


```java
	jshell> String[] textValues = {"Apple", "Ball", "Cat"};
	textValues ==> String[2]{ "Apple","Ball","Cat" }
	jshell>
	
```

#### Classroom Exercise CE-AA-03 

#### Exercises

1. 요일이 적힌 ```String```배열을 만든다.
```Sunday```, ```Monday```, ```Tuesday```, ```Wednesday```, ```Thursday```, ```Friday```, ```Saturday```
2. 글자 수가 가장 많은 날을 찾는다.
3. 요일을 출력한다.

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

우리의 과제에 대한 구현을 살펴보자.

우리는 ```addMark()```와 ```removeMarkAtIndex()```를 제외한 대부분의 기능을 구현했다.

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

배열에서 추가 및 제거를 하고자 한다. 할 수 있을까?

배열의 크기는 컴파일 시간 정의에 따라 고정된다. 즉, 일단 배열을 정의하면 다음과 같다.

```String[] textValues = {"Apple", "Ball", "Cat"};```

textValues 배열의 크기는 3으로 고정되어 있다. 배열 내에서 값을 변경할 수 있다. 그러나 크기는 변경할 수 없다.

배열에 요소를 추가하는 방법

옵션 중 하나는
* 삽입할 추가 요소를 수용할 수 있도록 몇 개의 추가 요소 슬롯이 있는 새 배열을 생성한다.
* 기존 배열 오스를 이 새 배열의 시작 부분에 복사한다.
* 이 배열의 후단에 추가할 요소를 추가한다.

요소를 배열에서 제거해야 하는 경우,
* 그에 따라 요소 슬롯이 적은 새 배열 생성
* 제거할 요소를 제외한 기존 배열의 요소를 이 새 배열의 시작 부분에 복사한다.

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

보다시피, 이는 매우 비효율적이다. 어떻게 해결해야 할까?

### Step 12: ```ArrayList``` 소개

`ArrayList`는 배열보다 동적이다. 이는 요소를 추가하고 제거하는 연산을 제공한다.

먼저 `ArrayList`를 만들고 값을 몇 가지 추가해 보자.

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

`remove`메소드를 이용하여 값을 삭제할 수 있다.

```java

	jshell> arrayList.remove("Cat");
	$4 ==> true
	jshell> arrayList
	arrayList ==> ["Apple", "Ball"]
```

```ArrayList```인스턴스인 ```arrayList```는 거의 모든 타입의, 심지어 기본형 타입의 객체를 저장하는 데 사용될 수 있다. 비동종 타입 또한!

> 표시되는 경고 메시지는 프로그래머에게 이를 막는 힌트이다.

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

`String`값만 `ArrayList`에 저장하려고 한다. 어떻게 해야 할까?

우리는 `ArrayList`가 포함할 수 있는 요소의 타입을 지정할 수 있다.

```java

	jshell> ArrayList<String> items = new ArrayList<String>();
	items ==> []
```

위의 내용에서는 `String`값을 저장할 수 있는 `ArrayList`를 만들고 있다.

`String` 값은 추가할 수 있지만, 숫자는 추가할 수 없다.

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

나머지 연산은 일반적인 `ArrayList`와 유사하다.
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

### Step 13: ```ArrayList```를 사용한 ```Student``` 리팩토링

이제 다시 한 번 ```Student```문제를 해결해보자. 이번에는 `ArrayList`를 사용해보자.
```java

	Student student = new Student(name, <list-of-marks>);
	int number = student.getNumberOfmarks();
	int sum = student.getTotalSumOfMarks();
	int maximumMark = student.getMaximumMark();
	int minimumMark = student.getMinimumMark();	
	BigDecimal average = student.getAverageMarks();

```

##### Snippet-01 : ```Student``` 리팩토링

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

강화된 ```for문```은 배열의 경우와 마찬가지로 ```ArrayList```에도 적용된다.

```Collections.max()```와 ```Collections.min()```메소드를 사용하여 배열의 최대값과 최소값을 찾을 수 있다.

### Step 14: E ```Student``` 의 발전

이제 학생을 추가 및 제거할 기능을 추가해보자.

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

**_콘솔창 출력_**

_Number of marks : 3_

_Sum of marks : 3_

Average of marks : 3_

_Maximum of marks : 3_

_Minimum of marks : 3_

_Ranga[97,98,100]_

_Ranga[97,98,100,35]_

_Ranga[97,100,35]_

## 객체 지향 프로그래밍 (*OOP*) - 복습

이 섹션에서는 *OOP*의 원칙을 다시 살펴본다.
* 배열 및 배열의 변형
* 기본 제공 Java 클래스 및 유틸리티
* 조건문과 반복문 (일반 및 향상된 버전)

### Step 01: 객체 복습 - 상태와 행동

객체의 속성들은 객체의 구성 요소를 결정한다. 객체의 라이프타임 동안 서로 다른 지점에서 해당 속성의 값이 변경될 수 있다.

주어진 시간에 이러한 특성의 값은 객체의 **상태**를 정의한다.

```MotorBike```의 예에서 속성인 ```speed```는 ```MotorBike```의 상태를 의미한다. ```ducati```의 ```speed```는 이것의 상태를 정의한다.

객체가 외부 이벤트 또는 해당 이벤트로 보낸 메시지에 응답하는 방법은 객체의 **행동**을 정의한다.

메시지는 메소드를 사용하여 객체로 배달된다. 메소드는 객체의 **행동**을 구현하는 데 사용되는 것이다.

```setSpeed```, ```increaseSpeed```, ```decreaseSpeed```메소드는 ````MotorBike```의 속도에 영향을 준다. `MotorBike`의 미래 `상태`는 행동과 현재의 상태에 달려있다.

`상태`는 `상태`에 영향을 미친다. 그리고 `상태`는 `행동`에 영향을 미친다.

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

### Step 02: ```class``` 의 상태 관리

기본 수준에서 클래스를 설계할 때 다음을 결정한다.
* `상태` - 멤버 변수
* `객체 생성 방법` - 생성자 정의
* `행동` - 노출되는 메소드

```Fan``` ```클래스```의 예를 들어보자.

설계에 해당하는 위의 세 가지 주요 영역은 다음과 같을 수 있다.

* 상태
	* make
	* radius (반지름)
	* color (색상)
	* isOn
	* speed (속도)
	
* 생성자
	* Fan(String make, double radius, String color)
	
* 행동
	* void switchOn()
	* void SwitchOff()
	* void changeSpeed(int change)
	* String toString()

이 모든 측면을 포괄하는 간단한 ```Fan``` ```클래스```를 작성해보자.

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
**_콘솔창 출력_**

_Make : Fan-tastic, Radius : 0.45600, Color : GREEN, Is On : false, Speed : 0_

```isOn```과 ```speed```라는 이름의 생성자가 설정하지 않은 분야는 ```false```(```boolean```인 경우)와 ```0```(```int```인 경우)이라는 데이터 타입의 기본 값을 가정한다.

### Step 03: 행동으로 ```Fan``` 증강
- - - 

`Fan`객체가 어떤 행동을 해야 할지 결정해야 한다.

```Fan```클래스 객체의 기본 상태 속성, 즉, ```make```,```color````,```radius```는 생성 시점에 고정되어 있으므로 이렇나 ```클래스```인스턴스의 사용자가 변경할 수 없다.

나머지 두 가지 상태 속성인 ```isOn```과 ```speed```는 ```Fan```객체 사용자들에 의해 변경될 필요가 있다. 우리는 이들을 바꿀 수 있는 메소드를 제공할 것이다.

##### Snippet-01 : ```Fan``` `````` - v4

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

**_콘솔창 출력_**

_Make : Fan-Tastic, Radius : 0.45600, Color : GREEN, Is On : false, Speed : 0_

_Make : Fan-Tastic, Radius : 0.45600, Color : GREEN, Is On : true, Speed : 1_

_Make : Fan-Tastic, Radius : 0.45600, Color : GREEN, Is On : true, Speed : 5_

_Make : Fan-Tastic, Radius : 0.45600, Color : GREEN, Is On : false, Speed : 0_

##### Snippet-01 설명

* 상태 속성 ```isOn```에 대해서는
	* ```public void isOn(boolean)과 같은 상태 제한자가 이들의 속성을 바꾸긴 하지만 별로 선호되지 않는다. 이는 ```클래스```사용자 입장에서는 직관적이지 않기 때문이다.
	* 또는 ```public void switchOn()```과 ```public void switchOff()```와 같은 메소드들은 ```isOn```의 속성을 전환시킬 뿐만 아니라 ```Fan``` ```클래스``` 사용자돌에게도 직관적이고 유용하다.(여기서는 ```FanRunner```클래스)

* 상태 속성 ```speed```에 대해서는
	* ```setSpeed```는 직관적일 뿐만 아니라 유용하기 때문에 여기서 재고할 필요가 별로 없다.
	* ```speed```는 ```switchOn()```과 ```switchOff()```연산의 영향을 받을 필요가 있다. 이러한 메소드 정의에서 ```setSpeed()```에 대한 호출을 추가했다.

#### 요약

클래스를 설계하는 가장 좋은 방법은 `Outside In(외부인)`사고 과정을 이용하는 것이다.
* 누가 내 ```클래스```를 사용하게 될까?
* 반드시 필요한 기능은 무엇일까?

### Step 04: Programming Exercise PE-OOP-01

1. 다음과 같은 구성 요소를 다루는 간단한 ```Rectangle``` ```클래스```를 작성하시오.
* 상태
	* length
	* width
* 생성자
* 행동 또는 메소드

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

**_콘솔창 출력_**

_Rectangle - length : 12, width : 23, area : 276, perimeter : 70_

_Rectangle - length : 12, width : 25, area : 300, perimeter : 74_

_Rectangle - length : 20, width : 25, area : 500, perimeter : 90_

#### Solution Explained

* ```length```와 ```width```를 명시하지 않고 만들어진 ```Rectangle```객체는 실용적이지 못하므로 기본 생성자가 제공되지 않는다.
### Step 06: 객체의 구성 이해

```Fan``` ```클래스```의 상태 속성을 다시 한번 살펴보자.

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
`Fan`클래스의 모든 멤버 변수는 기본형 타입이다. 우리가 그것들을 복잡하게 만들고 다른 클래스를 포함시킬 수 있을까?

##### Snippet-01 : 객체 구성 -상태

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

```Customer customer```은 다음과 같이 구성되어 있다.
*  ```name```
*  ```homeAddress```
*  ```workAddress```

```String```은 내장형으로 단순하다. ```Addresss```는 사용자 정의 타입이며 다음과 같이 구성되어 있다.
* ```doorNo```
* ```streetInfo```
* ```city```
* ```zipCode```

##### Snippet-02 : 객채의 구성 v2 - 생성자

이제 이러한 객체를 쉽게 만들 수 있도록 생성자를 추가하자.

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

##### Snippet-9 : 객체의 구성 v3 : 행동

행동을 제공하는 메소드를 추가해보자.

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

**_콘솔창 출력_**

_Customer [Ashwin Tendulkar] lives at [Flat No. 51, Hiranandani Gardens, Mumbai - 400076], works at [null]_

_Customer [Ashwin Tendulkar] lives at [Flat No. 51, Hiranandani Gardens, Mumbai - 400076], works at [Administrative Office, Western Block, Mumbai - 400076]_

### Step 07: Programming Exercise PE-OOP-02

#### Exercises

책 리뷰를 관리하는 프로그램을 작성하시오.

* Book
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

**_콘솔창 출력_**

_Book-123, Object Oriented Programming With Java, Ranga, [(Review-10, Great Book", 4), (Review-101, Awesome, 5)]_

### Step 07: 상속의 필요성

`Person`과 `Student` 두 클래스를 살펴보자.

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

위의 코드 예에서 볼 수 있듯이,
* ```Person```의 멤버 변수인 ```name```,```email```,```phoneNumber```이 ```Student```의 것들과 중복된다.
* 위의 ```Person```과 관련된 setter 및 getter 메소드도 ```Student```의 것들과 중복된다.

모든 `Student`는 `Person`이다. 모든 것을 중복하는 대신 `Person` 클래스를 확장할 수 있다면 어떨까?

#### 상속 

```Student```는 ```Person```이다. 자바는 기본적인 객체 지향 프로그래밍 패러다임인 **상속**을 지원한다.

```Student```는 ```Person```에서 ```Student```는 ```Person```이라는 사실을 상속 받을 수 있다.

이는 ```Student```의 클래스 정의에서 자바 키워드 ```extends```을 사용하여 이루어진다.

```java

	public class Person {
		// <Person Definition>
	}

	public class Student extends Person {
		// <Student Definition, after reusing Person Code>
	}

```

상속은 코드를 재사용하는 메커니즘이다. 이런 경우, 이전에 ```Person```에서 정의한 모든 멤버 변수와 메소드들은 ```Student```에서도 사용할 수 있다.

이러한 상속 관계에서 ```Person```은 ```Student```의 **수퍼 클래스**(super-class)라고 불린다. 마찬가지로 ```Student```는 ```Person```의 **서브 클래스**(sub-class)이다.

이제 우리가 어떻게 ```Student``` ```클래스```의 정의를 바꿀 것인지 살펴보자.

##### Snippet-02 : Person으로부터 상속 받는 Student - v1

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

### Step 09:  ```Object``` 클래스 소개

Java 언어에서는 내장형 자바 라이브러리 클래스든, 사용자 정의 클래스든 모든 클래스가 암묵적으로 ```Object```클래스로부터 상속된다.

이 ```Object```클래스는 자바 시스템 패키지 ```java.lang```에서 얻을 수 있다. 이 클래스는 Java 클래스 계층구조의 루트이다. 배열을 포함한 모든 클래스는 이 ```클래스```의 메소드를 구현/상속한다.

```Person```과 ```Student```클래스들을 살펴보자.

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

**_콘솔창 출력_**

_com.in28minutes.oops.level2.inheritance.Person@7a46a697_

_com.in28minutes.oops.level2.inheritance.Person@7a46a697_

##### Snippet-01 Explained

```toString()```,```haschCode()```,```notify()```와 같은 ```Object``` ```클래스```의 메소드들은 ```class``` ```Person```의 객체를 기본 구현으로 사용할 수 있다.

```System.out.println(person);``` 구문은 자바 시스템이 ```person.toString()```호출을 은연중에 ```class``` ```Object```에서 상속 받아```String```문맥으로 사용되기 때문에 ```System.out.println(Person.toString())```라는 호출로 번역된다.

### Step 10: 상속과 메소드 오버라이딩

서브 클래스는 슈퍼 클래스로부터 기능을 상속받는다.
* 상태 속성 : 슈퍼 클래스의 멤버 변수
* 동작 구성 : 슈퍼 클래스의 메소드 정의

물론 서브 클래스 내에서 엑세스(및 수정), 호출에 각각 사용할 수 있다.

서브 클래스 **메소드 오버라이딩**에서 슈퍼 클래스의 메소드 구현을 재정의할 수도 있다.

##### Snippet-01: 메소드 오버라이딩

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

**_콘솔창 출력_**

_Person Ranga , Email : in28minutes@gmail.com, Phone Number : 9898989898_

_Person Ranga , Email : in28minutes@gmail.com, Phone Number : 9898989898_

##### Snippet-01 Explained

우리는 ```Person```의 서브 ```클래스``` 내에서 ```toString()```이라는 메소드를 정의함으로써 ```Object```의 슈퍼 ```클래스```가 제공하는 디폴트 버전을 재정의하고 있다.

### Step 11: Classroom Exercise CE-OOP-01 

다음 속성을 지닌 Student 클래스를 확장하는 Employee 클래스를 생성하라
* Title
* Employer
* EmployeeGrade
* Salary

Employee 내에서 toString() 메소드를 만들어 Person을 포함한 모든 상태 속성 값을 출력한다.


##### Snippet-01 : Employee 상속

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

**_콘솔창 출력_**

_Employee Title: Programmer Analyst, Employer: In28Minutes, Employee Grade: A, Salary: 50000.0000_

##### Snippet-01 Explained

```Person``` 이라는 객체의 세부 사항을 ```Employee.toString()```메소드 오버라이딩으로 출력하지 않았다. 다음에는 그렇게 하도록 해보자.

### Step 12: 생성자와 ```super()```호출

```super```키워드는 서브 클래스가 슈퍼 클래스에 존재하는 속성에 접근할 수 있게 해준다.


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

**_콘솔창 출력_**

_Employee Name: Ranga, Email: in28minutes@gmail.com, Phone Number: 123-456-7890, Title: Programmer Analyst, Employer: In28Minutes, Employee Grade: A, Salary: 50000.0000_

The ```super``` keyword allows an sub-class to access the attributes present in the super-class. Hence, we were able to invoke the getter methods of the ```Person``` object within the ```Employee``` object, like this within ```Employee.toString()```
	* ```super.getName()```
	* ```super.getEmail()```
	* ```super.getPhoneNumber()```


#### 서브 클래스 생성자

서브 클래스의 객체가 생성되면 어떻게 할까? 슈퍼 클래스의 생성자가 호출되는 걸까?

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

**_콘솔창 출력_**

_Inside Person Constructor_

_Inside Employee Constructor_

##### Snippet-02 Explained

서브 클래스 객체가 생성될 때
* 서브 클래스 생성자를 호출하고 해당 슈퍼 클래스 생성자를 암묵적으로 호출한다.

자바 컴파일러는 ```super();```코드를 (프로그래머가 명시적으로 추가하지 않은 경우) 서브 클래스의 디폴트 생성자의 본문에 첫 번째 문장으로 삽입한다.
* ```super();```라는 구문은 슈퍼 클래스의 디폴트 생성자의 호출이다.
* 따라서, 슈퍼 클래스 생성자의 본문은 항상 서브 클래스의 생성자 본문 앞에 호출된다.

##### Snippet-3 : ```Person``` - Non-Default Constructor

인수가 없는 생성자를 제거하고 하나의 인수 생성자를 'Person' 클래스에 추가하자.

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

**_콘솔창 출력_**

_Person Ranga , Email : in28minutes@gmail.com, Phone Number : 123-456-7890_

##### Snippet-03 Explained

```class``` ```Employee```를 위한 인자가 하나인 생성자를 추가했을 때, ```Person```에 더 이상 기본 생성자가 없기 때문에 기존 코드인 **_EmployeeRunner.java_** 에 컴파일 오류가 발생할 것이다!

```super()```는 ```Employee```의 기본 생성자 내에서 호출할 수 없다.

여기서 선택할 수 있는 한 가지 옵션은 인수가 없는 생성자를 다시 배치하는 것이다.


```java

	public Person() {
		System.out.println("Inside Person Constructor");
	}

```

그러나 ```name```이 없는 ```Person```을 만든다는 것은 정말 말이 안되는 일인가?

이 경우 해결책은 ```super(name);```과 같은 호출에 의해 인자가 하나인 생성자 ```Person(String)```를 호출하는 것이다.


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

필수가 아닌 속성을 설정하기 위한 setter를 제공해보자.

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

`Student`클래스에 두 개의 인자를 가지는 생성자를 추가해보자.

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

**_콘솔창 출력_**

_Student : Ranga, College : IIT Bombay_

### Step 13: 다중 상속, 참조 변수와 ```instanceof```

다른 프로그래밍 언어에서는 다중 상속이 허용된다. 클래스가 둘 이상의 클래스들로부터 직접 상속 받을 수 있다.

그러나 Java에서는 직접 다중 상속이 허용되지 않는다.

##### Snippet-01 : 다중 상속

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

두 개의 클래스를 extend 할 수 없기 때문에 `class Dog extends Animal, Pet {}` 에서는 에러가 발생한다.

#### Inheritance Chains

그러나 상속 체인은 만들 수 있다.
*  ```class``` ```C``` **is a** ```class``` ```B```
*  ```class``` ```B``` **is a** ```class``` ```A```

작은 코드로 확인해보자.

##### Snippet-02 : 상속 체인

`Dog``` **은 ** ```Pet```이다, ```Pet``` **은 ** ```Animal```이다. 이것이 **상속 계층 구조**라고 부르는 것의 예시이다.

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

원한다면 마음속에 *```Dog``` --> ```Pet``` --> ```Animal``` --> ```Object```* 를 그려볼 수 있다. (그래! 자바의 *모든* 상속 계층의 최상위는 ```Object```이다!) 

```Dog dog = new Dog();```라는 생성자 호출은 상속 계층 구조를 출발시킨다.
The statement ```Dog dog = new Dog();``` sets off constructor invocations up the inheritance hierarchy:
	*  ```Dog()``` 는 ```Pet()``` 을 호출함
		*  ```Pet()```은 ```Animal()``` 를 호출함
			*  ```Animal()```은 ```Object()```를 호출함

```java
	jshell> Dog dog = new Dog();
	dog ==> Dog@23a6e47f
```

```dog.toString()```이라는 표현은 상속 계층구조를 가로지른다
	* ```Dog.toString()```이 정의되어 있지 않기 때문에 컴파일러는 ```Pet.toString()```을 찾는다.
	* ```Pet.toString()```이 정의되어 있지 않기 때문에 컴파일러는 ```Animal.toString()```을 찾는다.
	* ```Animal.toString()```이 정의 되어있지 않기 때문에 컴파일러는 자바의 ```Object``` ```class```의 모든 하위 클래스에 항상 기본 구현으로 제공되는 ```Object.toString()```을 찾고있다.

```java
	jshell> dog.toString();
	$1 ==> "Dog@23a6e47f"
```

```dog.groom();```이라는 호출도 상속 계급을 가로지르면서 해결된다.

```java
	jshell> dog.groom();
	"Pet Groom"
```


```Pet pet = new Dog();```라는 구문은 정말 재미있다. 자바에서는 *슈퍼 클래스 참조 변수에서 하위 클래스 객체 인스턴스를 참조할 수 있다.*

이러한 참조를 통해 메소드 호출도 허용되고 , 옹바른 작업이 수행된다. 따라서 ```pet.groom();```은 "*```Pet Groom```*"이라는 출력을 발생시킨다.

그러나 역방향 할당은 허용되지 않는다. *하위 클래스 참조 변수*는 상위 클래스 객체의 인스턴스를 참조 **_할 수 없다_**.
	* 따라서 ```Dog dog = new Pet();```이라는 구문은 컴파일러 오류를 일으킨다.

	
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


```instanceof``` 연산자는 객체와 클래스의 관계를 찾는 것이다. 객체가 클래스 또는 해당 하위 클래스의 인스턴스인 경우 참이 반환된다.

```java
	jshell> pet instanceof Pet
	$2 ==> true
	jshell> pet instanceof Dog
	$3 ==> true
```

```instanceof```연산자는 객체와 클래스가 관련이 없는 경우 오류 메시지를 출력한다.

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

```instanceof```연산자는 만약 그 객체가 해당 클래스의 슈퍼클래스의 객체라면 ```false```를 반환한다.

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

### Step 14: 추상 클래스 소개

```추상 클래스는``` ```추상적인```메소드를 포함할 수 있다.

추상 메소드는 메소드 정의를 가지고 있지 않다.

여기 전형적인 클래스가 있다. 클래스 내에 메소드를 만들고 클래스의 인스턴스들을 생성할 수 있다.

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

추상 클래스를 만드는 방법을 살펴보자:

```java
	jshell> abstract class AbstractAnimal {
	   ..>> abstract public void bark();
	   ..>> }
	| created class AbstractAnimal
```

구문은 간단하다. `abstract`키워드를 클래스 앞에 추가하면 된다.

```추상 클래스```는 인스턴스를 가질수없다.
.
```java
	jshell> AbstractAnimal animal = new AbstractAnimal();
	| Error:
	| AbstractAnimal is abstract; cannot be instantiated.
	| AbstractAnimal animal = new AbstractAnimal();
	|^--------------------------------------------^
	jshell>
```

그러나 서브 클래스가 될 수 있으며 이를 포함하는 상속 계층을 만들 수 있다. 추상 클래스의 하위 클래스(**구상 클래스**라고도 함)는 ```추상```메소드를 오버라이딩해야 한다.


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

### Step 15: 추상 클래스 - 설계 측면

왜 우리는 추상 클래스가 필요한가?

집에서 파티를 준비하고, 이벤트를 위한 메뉴에 여러 가지 음식이 있다고 생각해보자. 분명히, 각각의 요리는 특정한 준비 절차를 가지고 있을 것이다. 요리를 하는 것은 보통 시도부터 레시피를 따르는 것을 포함하며, 그 준비는 다음과 같은 기본적인 단계로 요약된다.
* 재료 준비
* 레시피대로 요리
* 정리 

이 단계들은 각각의 요리마다 다를 수 있지만, 순서는 그대로이다.

##### Snippet-01 : The Recipe Hierarchy 

추상 클래스를 이용해 레시피를 작성해보자.

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

각 단계에 대해 추상 메소드를 정의하고 이를 호출하는 `excute` 메소드를 만들었다. `execute`메소드는 호출이 뒤따라 오는 것을 보장한다

추상 메소드를 구현하는 구현을 정의할 수 있다.

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

**_콘솔창 출력_**

_[Curry Preparation Method]_

_Get Vegetables Cut and Ready_

_Get Spices Ready_

_Steam And Fry Vegetables_

_Cook With Spices_

_Add Seasoning_

_Discard unused Vegetables_

_Discard unused Spices_

##### Snippet-01 Explained

`CurryRecipe`는 각 단계에서 무엇을 해야 하는지를 규정한다. `execute`메소드를 호출하면 단계가 순서대로 실행된다.

##### Snippet-02 : MicrowaveCurryRecipe

많은 레시피를 더 쉽게 만들 수 있다.

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


**_콘솔창 출력_**

_[Curry Microwave Method]_

_Get Vegetables Cut and Ready_

_Switch on Microwave_

_Microwave Vegetables_

_Add Seasoning_

_Switch off Microwave_

_Discard unused Vegetables_

##### Snippet-02 Explained

`MicrowaveCurryRecipe` 은 각 단계에서 무엇을 해야 하는지를 규정한다. `execute` 메소드를 호출하면 각 단계가 순서대로 실행된다.

#### 요약

이 패턴을 `템플릿 메소드`패턴 이라고 한다. 각 단계의 순서가 정의된 추상 클래스를 정의한다. 각 단계의 구현은 하위 클래스에 맡긴다.

### Step 16: Abstract Classes - Puzzles

추상 클래스에 대한 몇 가지 FAQ를 살펴보자.

```추상 클래스```는 어떠한 ```추상적인```멤버 함수 없이도 만들어질 수 있다.

```java

	jshell> abstract class AbstractTest {
	   ...>}
	| creates abstract class AbstractTest
```

```추상 클래스```는 어떠한 슈퍼 클래스의 ```추상```메소드도 오버라이딩하지 않고 또 다른 ```추상 클래스```를 만드는 하위 클래스가 될 수 있다.

```java
	jshell> abstract class AbstractAlgorithm {
	   ...> abstract void flowChart();
	   ...> }
	| creates abstract class AbstractAlgorithm
	jshell> abstract class AlgorithmTypeOne extends AbstractAlgorithm {
	   ...> }
	| creates abstract class AlgorithmTypeOne

```

```추상 클래스```는 멤버 변수를 가질 수 있다.

```java
	jshell> abstract class AbstractAlgorithm {
	   ...> private int stepCount;
	   ...> }
	| replaced abstract class AbstractAlgorithm
```

```추상 클래스```는 추상 메소드가 아닌 메소드를 가질 수 있다.
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


### Step 17: 인터페이스 소개
- - - 

"*게임 콘솔*"이 무엇인가?

단추나 기타 컨트롤이 있는 장치로 비디오 게임을 할 수 있다.

그 위에 있는 전형적인 버튼은 무엇인가?
- 화살표 - 상,하,좌,우
- 선택(select)
- etc

게임 콘솔은 게임을 실행할 수 있는 인터페이스를 제공한다.

누가 단추를 클릭했을 때 발생하는 동작의 구현을 제공하는가? 예를 들면, 마리오 게임이나 체스 게임 등의 구현자이다.

자바에서는 이것을 어떻게 표현할까?


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

```interface``` ```GamingConsole```은 정의가 없는 메소드들을 포함한다.

누가 구현을 제공할 것인가?

`MarioGame`을 살펴보자.


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

`MarioGame`은 게임 콘솔이라는 인터페이스에 선언된 모든 메소드에 대한 정의를 제공한다. 구문은 간단하다. `class MarioGame implements GamingConsole`은 모든 메소드를 구현한다.

이 게임을 어떻게 실행할 수 있는지 살펴보자.

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


**_콘솔창 출력_**

_Jump_

_Go into a hole_

_Go forward_

##### Snippet-01 Explained

인터페이스가 가지는 주된 장점은 구현하는 사람의 계약을 강제하는 데 사용할 수 있다는 것이다.

##### Snippet-02 : 인터페이스를 이용한 코드 재사용

또 다른 예인 `ChessGame`을 보자.

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

실행은 간단하다. `MarioGame game = new MarioGame();`을 코멘트 아웃하고 `ChessGame`의 구현으로 대체하기만 하면 된다.

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

**_콘솔창 출력_**

_Move Piece Up_

_Move Piece Down_

_Move Piece Left_

_Move Piece Right_

##### Snippet-2 explained

같은 ```GamerRunner``` ```클래스```에서 ```MarioGame```이 아닌 ```ChessGame```의 객체를 인스턴스화한다면 다른 코드는 하나도 바꿀 필요가 없다. 이는 ```MarioGame```과 ```ChessGame```이 모두 동일한 ```interface``` ```GamingConsole```을 구현하고 있기 때문이다.

#### 인터페이스를 참조 변수의 타입으로 사용

```GamingConsole```은 인터페이스이다. ```MarioGame```과 ```ChessGame```은 그 구현이다.

`GamingConsole game = new ChessGame();`을 사용해보자.

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

**_콘솔창 출력_**

_Move Piece Up_

_Move Piece Down_

_Move Piece Left_

_Move Piece Right_

#### Explained

`GamingConsole game = new ChessGame();` - 인터페이스의 구현은 인터페이스 타입의 참조 변수에 저장할 수 있다.

이것이 어떻게 도움이 될까?

다음의 예를 보자.

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

**_콘솔창 출력_**

_Jump_

_Go into a hole_

_Go forward_

##### Snippet-04 Explained

`GamingConsole game = new ChessGame()`을 `GamingConsole game = new MarioGame()`으로 대체하면 이제 프로그램은 `MarioGame`을 실행한다. 멋지지 않은가?

### Step 18: 인터페이스를 이용한 API 설계

상당히 크고 복잡한 응용 프로그램을 프로그래밍하는 소프트웨어 개발 프로젝트를 생각해보자. 프로젝트 팀 (A팀)은 이 프로젝트의 일부를 외부 팀 (B팀)에게 아웃소싱하기로 결정했다. 이 외부 팀이 특정 작업을 달성하기 위해 상당히 복잡한 알고리즘을 구현해야 하며, 나머지 응용 프로그램과 상호 작용해야 한다고 가정하자. 응용 프로그램의 두 부분에 대한 작업을 동시에 진행해야 한다.

알고리즘 논리가 단일 메소드를 사용하여 구현된다고 가정해보자.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;```int complexAlgorithm(int number1, int number2);```

두 팀이 수행한 작업이 양립할 수 있도록 하려면 어떻게 해야 하는가?

인터페이스를 정의하는 것부터 시작합시다.

**_ComplexAlgorithm.java_**

```java
  
	package com.in28minutes.oops.level2.interfaces;

	public interface ComplexAlgorithm {
		int complexAlgorithm(int number1, int number2);
	}

```

이제 그 팀들은 즐겁게 일할 수 있다. A팀은 `OneComplexAlgorithm`이라는 인터페이스를 위한 부분을 만들고 그 프로젝트를 시작할 수 있다.

**_OneComplexAlgorithm.java_**

```java

	package com.in28minutes.oops.level2.interfaces;

	public class OneComplexAlgorithm {
		public int complexAlgorithm(int number1, int number2) {
			return number1 + number2;
		}
	}

```

B팀은 실제 알고리즘을 구현하는 데 시간이 걸릴 수 있다.

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

### Step 19: Interfaces - 퍼즐과 흥미로운 사실들
- - -  

인터페이스를 더 이해하기 위해 몇 가지 예를 살펴보도록 하자.

```interface```는 또 다른 ```interface```에 의해 확장될 수 있다. 인터페이스로만 구성된 상속 계층을 가질 수 있는 것이다.

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

인터페이스의 구현은 슈퍼 인터페이스의 메소드를 포함하여 모든 메소드를 구현해야 한다.
.
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

클래스가 추상적으로 선언되면 모든 인터페이스 메소드에 대한 구현 제공을 건너뛸 수 있다.

```java
	jshell> public abstract class AbstractImplementation implements InterfaceTwo {
	   ...> public void methodOne() {}
	   ...> }
	| created class AbstractImplementation
```

```인터페이스```는 멤버 변수를 가질 수 없다. ```인터페이스```는 **상수**를 선언할 수 밖에 없다.

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
Java SE 8부터 인터페이스는 제공되는 메소드의 기본 구현을 제공할 수 있다. 그것은 그 메소드의 선언에 ```default```라는 키워드를 포함시키고 그 정의에 메소드를 제시함으로써 이루어질 수 있다. 


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

```인터페이스```의 구현은 기본 메소드 구현을 오버라이딩할 수 있다.

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

```interface```안에 선언된 어떤 메소드도 ```private```접근 지정자에는 접근할 수 없다. 그러나 ```추상 클래스```는 ```private```메소드를 내부에서도 선언할 수 있다.

#### ```기본(default)``` 메소드 구현이 필요한 이유.

세 가지 구현이 가능한 `Provider` 인터페이스를 고려해보자.

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

`interface`에 새 메소드가 추가되면 어떻게 될까?

```java

	public interface Provider {
		public void doSomething();
		public void doMore();
	}

```

컴파일 에러! ```ImplementationOne```, ```ImplementationTwo````, ```ImplementationThree``` 이 모든 구현 클래스들은 각각 ```doMore()``` 을 구현하도록 업데이트 **되어야 한다.**

대안 : `doMore`의 기본 구현을 제공한다.

```java

	public interface Provider {
		public void doSomething();
	
		public default void doMore(){
			System.out.println("Do More");
		}
	}

```

다른 코드는 즉시 변경할 필요가 없으며, 특정 구현 클래스는 필요에 다라 이 기본 버전을 오버라이드할 수 있다.

이는 특히 프레임워크를 구축하고 확장하는 데 유용하다. 인터페이스에 새 메소드를 추가할 때 프레임워크 인터페이스의 사용자는 중단되지 않는다.

### Step 20: ```추상 클래스```와 ```인터페이스``` 비교

```추상 클래스```와 ```인터페이스```는 구문이 유사하다는 점을 제외하면 매우 다르다.

그들을 언제 응용 프로그램에 사용하기를 원하는가?

#### 인터페이스

```인터페이스```는 **계약**이다.

```인터페이스```는 주로 서로 통신해야 하는 두 개의 소프트웨어 구성 요소가 있고 계약을 체결할 필요가 있을 때 사용된다.

다음 예제를 상기해보라: `ComplexAlgorithm`은 관련된 두 팀 모두에 도움이 되는 인터페이스를 정의한다.


```java

	package com.in28minutes.oops.level2.interfaces;
	public interface ComplexAlgorithm {
		int complexAlgorithm(int number1, int number2);
	}

```

#### 추상 클래스


```추상 클래스```는 주로 슈퍼 클래스를 만들어 행동을 일반화하고 싶을 때 사용된다.

앞서 논의한 다음 예를 기억해보라.

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
 
#### 구문 비교

다음은 중요한 구문 차이이다.
* ```인터페이스```안에 선언된 어떤 메소드도 ```private``` 접근 지정자에 의해 접근할 수 없다. 그러나 ```추상 클래스```는 ```private```메소드를 가질 수 있다.
* ```인터페이스```는 멤버 변수를 선언할 수 없다. ```추상 클래스```는 멤버 변수 선언을 할 수 있다.
* ```클래스``` 또는 ```추상 클래스```는 복수의 ```인터페이스```를 구현할 수 있다. 그러나 ```인터페이스```는 한 개의 ```인터페이스```만 확장할 수 있고 ```, ```클래스``` 또는 ```추상 클래스```는 한 개의 ```클래스`` 또는 ```추상 클래스```만 확장할 수 있다.

### Step 21: Programming Exercise PE-OOP-03

#### Exercises

TODO

#### Solution To PE-OOP-03

#### Solution - 1

#### Solution - 2

### Step 21: 다형성 소개

TODO

# 컬렉션의 이해

배열은 동적 자료 구조가 아니다. 고정된 최대 개수의 요소만 저장할 수 있다.

배열에 요소를 삽입하거나 제거할 때는 많은 작업이 필요하다.

컬렉션은 Java 프로그램의 동적 자료 구조를 지원하는 내장형 구현이다. 일반적으로 사용되는 컬렉션은 리스트, 트리 및 해시 테이블을 기반으로 한다.

Java는 매우 우수한 컬렉션 구현을 제공한다.

모든 컬렉션을 쉽게 이해하기 위해 ```List```,```Set```,```Queue```,```Map``` 등의 인터페이스로 시작할 것이다.

그 후에는 ```LinkedList```,```HashTable```,```TreeMap``` 등과 같은 인터페이스 구현에 대해 알아보자.

#### 컬렉션 인터페이스

`리스트` 인터페이스 먼저 시작하자.

#### ```리스트(List)``` ```인터페이스```

이 ```리스트``` ```인터페이스```는 자바 프로그램에서 **정렬된 컬렉션**을 구현하는 데 사용된다. 순서가 정렬된 컬렉션은 요소를 컬렉션에 삽입하거나 컬렉션에서 접근할 수 있는 위치를 프로그래머가 제어할 수 있는 컬렉션이다.

요소의 삽입 위치가 지정되지 않은 경우 ```리스트```의 끝에 추가된다.

```리스트```는 일반적으로 *중복* 요소를 허용한다.

##### Snippet-1 : 리스트 생성

아래에서는 리스트를 만들고 요소 데이터에 접근하는 예를 볼 수 있다.

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

#### ```리스트``` 불변성

지난 스니펫에서 우리가 만든 ```words``` ```리스트```를 생각해 보자.

```List<String> words = List.of("Apple", "Bat", "Cat");```

```static``` ```of```메소드를 사용하여 만든 리스트는 *불변하다*.

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

#### 가변적인 ```리스트``` 생성

시간이 지남에 따라 업데이트될 수 있는 ```List``` 데이터 구조를 만드느 방법인 ```List``` 인터페이스를 구현하는 내장 ```컬렉션``` 클래스를 인스턴스화하는 것이다.

```ArrayList```, ```LinkedList```와 ```Vector```가 그 예이다.

##### Snippet-3: 가변적인 리스트

몇 가지 예를 보자.

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

```어레이 리스트```는 요소를 저장하기 위해 어레이를 사용한다.
* 위치 엑세스와 요소의 수정은 매우 효율적이며, 일정한 시간 복잡도를 가진다.
* 요소를 삽입하고 삭제하는 데 비용이 많이 든다. 20개의 요소를 가진 리스트에서, 첫 번째 위치에 요소를 삽입하려면 20개 요소를 모두 이동시켜야 한다.

```연결리스트```를 구현하는 데 사용되는 데이터 구조는 메모리 슬롯 블록의 체인인 연결 리스트 타입이다.
* 값을 삽입하고 삭제한는 것은 쉽다. 블록 체인에서 각 링크는 다음 블록에 대한 참조에 불과하기 때문이다. 삽입에는 새로운 값을 수용하기 위해 이러한 링크의 조정만 필요하며, 기존 요소의 광범위한 복사 및 이동이 필요하지 않다.
* 엑세스에는 항상 링크의 횡단을 수반하기 때문에 위치의 엑세스와 요소의 수정은 ```어레이 리스트```에 비해 효율성이 떨어진다.

최적화: ```연결리스트```의 기본 데이터 구조는 사실 이중 연결리스트로, 각 요소는 그 주변의 요소들과 앞뒤로 연결되어 있다.
.
#### ```Vector``` vs ```ArrayList```

```벡터```는 자바 v1.0이후 사용되었고, ```어레이리스트```는 나중에 v1.2에서 추가되었다. 둘 다 배열을 기본 데이터 구조로 사용한다.

```벡터```는 thread-safe하다. ```벡터```에서는 모든 메소드가 ```동기화```되어있다.

> `벡터`는 동시성이 낮으므로 다른 스레드 세이프한 `리스트`구현을 보라.

#### ```List``` 연산

일반적인 ```리스트```연산을 ```어레이리스트```로 검토해볼 것이다. ```연결리스트``` 또는 ```벡터```에서도 유사한 연산이 수행될 수 있다.

##### Snippet-4 : 리스트 삽입

다음을 위한 예를 살펴보자.
* 끝단 삽입(기본값)
* 위치 삽입
* 중복 입력이 허용됨
* 현재 리스트에 외부 리스트의 모든 요소 추가
	* 맨 뒤에
	* 단일 요소 삽입과 같이 위치 삽입도 가능

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


##### Snippet-5 : 요소 수정

다음의 예를 살펴보자
* 특정 위치의 요소 수정
* 요소 삭제

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

##### Snippet-6 : 어레이 리스트 내에서 반복

이제 `리스트`의 요소들을 반복하는 방법을 살펴보자.

기본 루프:

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

강화된 루프의 사용:
```java
	jshell> for(String word:words) {
	...> System.out.println(word);
	...> }
	Apple
	Bat
	Cat
```

반복기 사용:
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

* 변경이 없는 반복의 경우 강화된 ```for```루프가 가장 편리하다.
* 변하는 반복의 경우:
* 삭제: 우리가 본 예에서 보듯이 강화된 ```for```루프는 권장되지 않는다. ```Bat```는 제거되었지만 ```Cat```은 반복 자체가 영향을 받았기 때문에 제거되지 않았다.
* 이러한 반복에는 반복기(Iterator)를 사용할 수 있다.

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

#### ```List``` : 타입 안정성

```리스트``` 컬렉션은 기본형 타입을 저장하지 않는다. 오직 객체 참조만 저장한다. 우리가 ```int```,```char```혹은 ```double```과 같은 기본형 타입을 저장하력 하면 각각 ```Integer```,```Character```,```Double```의 래퍼 클래스로 암묵적으로 전환된다. 기본형 데이터 타입 요소는 *자동 박싱*을 사용해야 한다.

##### Snippet-7 : 타입 안정성

```ArrayList.indexOf()``` 메소드는 오버로드 되지 않고 한 가지 버전만 있다. 그래서 ```int```인자를 전달하면 그것은 ```Integer```라는 객체에 자동으로 박싱되고 해당 메소드가 실행된다.
* 그러나 ```ArrayList.remove()``` 메소드는 두 가지 오버로드 버전이 있다.
	* ```ArrayList.remove(int index)``` : ```ArrayList```의 특정 인덱스에서 요소를 삭제한다.
	* ```ArrayList.remove(Object o)``` : 특정 요소가 ```ArrayList```에 있으면 삭제한다.

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

##### Snippet-8 : 리스트 정렬

```List.of()```에서 얻은 ```List```는 불변의 것이므로 스스로 정렬할 수 없다. 그러므로 그것으로부터 변형 가능한 ```ArrayList```를 만들자.

```ArrayList.sort()```메소드는 ```Comparator(비교기)``` 객체의 정의를 필요로 한다. 더 쉬운 선택은 ```Collections.sort()```를 대신 사용하는 것이다.

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

Student 클래스를 만들고 `Collections.sort`를 이용해 정렬해보자

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

**_콘솔창 출력_**

**_COMPILER ERROR_**

##### Snippet-9 Explained

```Collections.sort()``` 메소드에는 ```List```인 것만이 통과할 수 있는데 그 타입의 요소는 ```T```이며 ```Comparator<? super T>``` ```interface```를 구현하고 있다.

```Student```는 인터페이스를 구현하지 않는다. 결과 
To the method ```Collections.sort()```, only those ```List```s can be passed, the type of whose elements ```T```, implements the ```Comparator<? super T>``` ```interface```. 

```Student``` does not implement the interface. Result - Compilation error.
``컬렉션"이라는 방법에는 ``리스트"라는 것만이 통과할 수 있는데 그 유형의 요소는 ``"이다.T'sns는 ``비교자"를 구현하고 있다. 슈퍼T'''인터페이스''''' 

"'학생'은 인터페이스를 구현하지 않는다. 결과적으로 - 실행 오류(Compilation error)이다.

##### Snippet-10 : 비교기 인터페이스 구현

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


**_콘솔창 출력_**

_[1 Ranga, 100 Adam, 2 Eve]_

_[1 Ranga, 2 Eve, 100 Adam]_

##### Snippet-10 Explained

`Integer.compare(x, y)`는 x == y 인 경우 0을, x < y 인 경우 0보다 작은 값을 , x > y 인 경우 0보다 큰 값을 반환한다.

매개변수의 순서를 변경하는 경우:

```java

	@Override
	public int compareTo(Student that) {
		return Integer.compare(that.id, this.id);
	}

``` 

출력이 이렇게 바뀐다:

_[100 Adam, 2 Eve, 1 Ranga]_

#### ```비교기(Comparator)``` ```인터페이스```

여러 가지 방법으로 학생을 정렬해아 한다면 어떻게 할까? 어떤 상황에서는 ID의 오름차순으로, 다른 상황에서는 ID의 내림차순으로 정렬하려면 어떻게 해야하는 걸까?

```Collections.sort```는 다음과 같은 특징을 가지는 오버로드된 버전이 있다.

```java

	@SuppressWarnings({"unchecked", "rawtypes" })
	public static <T> sort(List<T> list, Comparator<? super T> c)
		list.sort(c);
	}

``` 

이 버전의 ```Collections.sort```를 호출할 수 있게 된다. 우리는 ```Student``` 객체와 동작하는 ```비교기```의 적절한 구현을 정의할 필요가 있을 것이다.

이미 짐작했겠지만 ```비교기```의 두 가지 실행, 즉, 하나는 오름차순, 다른 하나는 내림차순을 정의해야 한다.

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

**_콘솔창 출력_**

_[1 Ranga, 100 Adam, 2 Eve]_

_Ascending : [1 Ranga, 2 Eve, 100 Adam]_

_Descending : [100 Adam, 2 Eve, 1 Ranga]_

#### ```리스트```의 ```sort```메소드

`리스트`에서 `sort`메소드는 `비교기(Comparator)`를 전달하여 호출할 수 있다 - `studentsAl.sort(new AscStudentComparator())`

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

**_콘솔창 출력_**

_[1 Ranga, 100 Adam, 2 Eve]_

_Asc : [1 Ranga, 2 Eve, 100 Adam]_

_Desc : [100 Adam, 2 Eve, 1 Ranga]_

### The ```Set``` ```인터페이스```

수학적으로 Set(집합)는 고유한 항목의 모음이다. 마찬가지로 자바의 ```Set``` ```인터페이스``` 또한 고유한 요소를 가진 컬렉션에 대한 계약을 명시하고 있다.
* 만약 ```object1.equals(object2)```가 ```true```를 반환 한다면, 그 후 ```object1```과 ```object2```중 하나만이 ```Set``` 구현에 자리한다. 

##### Snippet-13 : Set

몇 가지 예를 살펴보자.

```Set.of()```에 의해 반환된 컬렉션은 불변이므로 ```add()``` 메소드를 지원하지 않는다.

```java

	jshell> Set<String> set = Set.of("Apple", "Banana", Cat");
	set ==> [Banana, Apple, Cat]
```

대신 ```add()```를 지원하는 컬렉션을 만들어 ```Set```의 교유성을 시험해보자.


```java
	jshell> set.add("Apple");
	| java.lang.UnsupportedOperationException thrown:
	jshell> Set<String> hashSet = new HashSet<>(set);
	hashSet ==> [Apple, Cat, Banana]
```

```HashSet.add()```연산은 ```false``` 값을 반환하며 이는 중복인 "Apple" 입력에 실패했음을 나타낸다.

```java
	jshell> hashSet.add("Apple");
	$1 ==> false
	jshell> hashSet
	hashSet ==> [Apple, Cat, Banana]
```

```hashSet```이 ```set```을 사용하여 만들어졌을 때 요소의 순서는 순열로 배치/변경된다는 점에 유의한다. 또한 원래 우리가 ```Set.of()```메소드에서 ```set```를 만들었을 때, 출력된 순서는 초기화 순서와 달랐따. 이는 ```Set```컬렉션은 요소의 순서를 중요시하지 않으므로 위치 접근을 지원하지 않는다는 사실을 확인시켜 준다. 따라서 ```HashSet.add(int, String)``` 호출 시 컴파일러 오류가 발생한다.


```java
	jshell> hashSet.add(2, "Apple");
	| Error:
	| no suitable method found for add(int, java.lang.String)
	| hashSet.add(2, "Apple");
	|^----------^
	jshell>

```

#### 데이터 구조의 이해

##### Hash Table
* 해시 테이블(Hash Table) : 두 가지 장점을 결합하려는 데이터 구조
	* 요소에 대한 접근이 매우 효율적임
	* 요소 삽입 및 삭제가 매우 효율적임
* 버킷(Buckets) : 해시 테이블의 슬롯으로, 요소를 삽입하고 서로를 체인으로 연결한다. 보다시피 해시 테이블은 사실상 버킷의 커다란 배열로, 각각에 작은 연결 리스트가 포함되어 있다.
* 해싱(Hashing) : 해시 테이블을 만들 때 사용되는 **해싱**이라는 절차이다. **해시(Hash)** 라는 용어는 일반적으로 *요소의 순서를 섞음* 을 의미한다.
* 해시 함수 : 특정 요소가 삽입되는 버킷을 결정/계산하는 공식이다. 예를 들어 ```hash(elem)```은 ```elem mod 13```을 수학적으로 계산할 수 있으며, 이 값을 사용하여 테이블로 인덱스하여 버킷 삽입 위치를 찾을 수 있다. ```Object.hashCode()```는 해싱 함수로 사용할 수 있다.
* 충돌: 연결 리스트가 늘어나는 버킷 내의 체인으로 이어진다. 테이블이 클수록, 해시 함수가 똑똑해질수록 충돌 확률은 더 낮아진다.

##### Tree
* 트리: 정렬된 순서에 요소를 저장한다.트리 내의 모든 노드의 왼쪽 서브트리는 해당 노드의 요소보다 작다. 반대로 모든 노드의 그 오른쪽 서브 트리에 있는 요소는 해당 노드의 요소보다 크다.
* 삽입: 어떤 노드가 주어져도 정렬된 순서를 유지하기 위해 기존의 노드와 비교하여 새 노드가 삽입될 자리를 찾는다.
* 접근: 연결 리스트보다 효율적

#### ```Set``` 구현

* HashSet
* LinkedHashSet
* TreeSet

##### Snippet-14 : HashSet

```HashSet```에서는 요소들이 삽입 순서나 정렬 순서에 따라 저장되지 않는다.

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

```LinkedHashSet```에서는 요소들이 삽입된 순서대로 저장된다.

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

```TreeSet```에서는 요소들이 정렬된 순서로 저장된다.

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
#### Set 예제

- - - 
1. 다음과 같은 ```List```를 만든다.

	```List<Character> list = List.of('A', 'Z', 'A', 'B', 'Z, 'F);```
	
* 이 리스트에서 고유 문자를 나열하는 절차를 작성하라
* 이러한 고유 문자를 정렬된 순서대로 나열하는 절차를 작성하라
* 이러한 고유한 문자를 원래 리스트에 있는 순서대로 나열하는 절차를 작성하라

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

**_콘솔창 출력_**

_Unique Characters: [A, B, F, Z]_

_Sorted Order: [A, B, F, Z]_

_Inserted Order: [A, Z, B, F]_

#### Solution Explained

이 예시에서 ```hashSetChars```로 정리한 원소의 순서는 ```treeSetChars```에서와 같다. 앞의 예에서 보았던 바와 같이 이러한 순서가 항상 보장되는 것은 아니다.

#### ```TreeSet``` In Depth

* 슈퍼 인터페이스
	* Set
	* NavigableSet

##### Snippet-16 : NavigableSet 연산

몇 가지 연산을 살펴보자

```java

	jshell> TreeSet<Integer> numbers = new TreeSet<>(Set.of(65, 54, 34, 12, 99));
	numbers ==> [12, 34, 54, 65, 99]
	jshell> numbers.floor(40);
	$1 ==> 34
```
```floor()``` 메소드는 포괄적이고, ```lower()``` 는 배타적이다.

```java
	jshell> numbers.floor(34);
	$2 ==> 34
	jshell> numbers.lower(34);
	$3 ==> 12
```

```ceiling()``` 메소드는 포괄적이고 , ```higher()```는 배타적이다. 

```java
	jshell> numbers.ceiling(36);
	$4 ==> 54
	jshell> numbers.ceiling(34);
	$5 ==> 34
	jshell> numbers.higher(34);
	$6 ==> 54
```

```subSet(Object, Object)``` 메소드는 하한 포함이다. 그래서 왼쪽 경계는 ```lower()```과 같고, 오른쪽 경계는 ```higher()```과 같다. 오버로딩된 버전 ```subSet(Object, boolean, Object, boolean)```은 반환된 서브 집합의 하위 집합과 상위 집합을 구성하는 데 사용될 수 있다.

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

```headSet()```은 주어진 요소 값 앞에 있는 요소의 하위 집합을, ```tailSet()```은 주어진 요소 값 뒤에 있는 요소의 하위 집합을 반환한다.

```java
	jshell> numbers.headSet(50);
	$12 ==> [12, 34]
	jshell> numbers.tailSet(50);
	$13 ==> [54, 65, 99]
	jshell>

```

####  ```큐(Queue)``` 인터페이스

```Queue``` ```인터페이스``` : ```컬렉션``` ```인터페이스```를 ```확장함.
* 구성 요소는 작업 관리 목록과 같은 처리 순서로 배열된다.


#### ```우선 순위 큐(PriorityQueue)``` 컬렉션

```우선 순위 큐``` 컬렉션은 자바의 내장 ```클래스```로, ```큐``` ```인터페이스```를 ```구현```하고 있다. 요소는 기본적으로 정렬된 자연 순서로 저장된다. 또한 *우선 순위*(프로그래머에 의해 지정됨)라고 하는 사용자 지정 순서를 정할 수 있다. 

##### Snippet-17 : 우선 순위 큐(PriorityQueue)

```우선 순위 큐```는 기본적으로 오름차순 알파벳 순서로 문자열을 저장한다.

* ```queue.poll()``` 큐의 요소들을 자연 발생 순서부터 내보낸다.


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

##### Snippet-18 : 사용자 지정 우선 순위 큐

우선 순위의 구성 요소에 대한 사용자 정의 우선 순위 순서는 ```PriorityQueue<T>```에 ```Comparator<? super T>``` ```인터페이스```의 구현을 전달하면 순서를 지정할 수 있다.

`StringLengthComparator`를 구현해 보자.

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

**_콘솔창 출력_**

_Cat_

_Zebra_

_Monkey_

_null_


#### ```Map``` ```인터페이스```

```Map``` ```인터페이스```는 ```(key, value)```의 한 쌍으로 이루어진 원소의 컬렉션을 구현하기 위한 계약을 명시하고 있다.

문자열이 일련의 문자로 반복되는 횟수를 저장한다고 가정해보자.
* ```{'A', 'C', 'A', 'C', 'E', 'C', 'M', 'D', 'H', 'A'}``` 순으로 삽입된다.
* Map 내용은  ```{('A', 3), ('C', 3), ('E', 1), ('M', 1), ('D', 1), ('H', 1)}```으로 끝난다.

Map에 저장된 요소의 종류 (```(key, value)```쌍)은 자바의 다른 컬렉션들과 달라 ```Map``` ```인터페이스```는 독특하다. 너무 독특해서 ```Collection``` ```인터페이스```를 확장하지 못한다!

```인터페이스```의 정의는 다음과 같다.

```java

	public interface Map<K, V> {

		//Method Declarations

	}

```

* ```Map``` ```인터페이스```를 ```구현```하는 자바 컬렉션 클래스들은 다음과 같다.
	* ```HashMap```
	* ```HashTable```
	* ```LinkedHashMap```
	* ```TreeMap```

#### ```Map``` Collections : Concepts

* ```HashMap```
	* 무질서
	* 정렬되지 않음
	* 해시 함수는 키의 ```hashCode()``` 값이 사용됨
	* ```null```값 허용
	* Allows a key with a ```null``` value.

* ```HashTable```
	* ```HashMap```의 Thread-safe 버전. 필요한 경우 ```synchorized```메소드를 사용한다.
	* 무질서
	* 정렬되지 않음
	* 해시 함수는 키의 ```hashCode()``` 값이 사용됨
	
* ```LinkedHashMap```
	* 요소의 삽입 순서가 유지됨
	* 정렬되지 않음
	* 반복 속도가 빠름
	* 삽입과 삭제가 느림

* ```TreeMap```
	* 추가적으로 ```NavigableMap``` ```인터페이스```를 구현함
	* 구성 요소는 정렬된 키 순서로 유지
	* Elements are maintained in sorted order of keys

#### ```Map``` ```interface``` : Basic Operations

##### Snippet-19 : 기본적인 Map 연산

```Map.of()``` 메소드는 일련의 객체들을 취하는데 이는 번갈아 가면서 key와 value 엔트리로 해석된다.

* 인자의 총 개수는 짝수일 것ㅅ이다.
* 이 메소드는 구체적인 순서가 없는 ```(key, value)```의 짝으로 불변의 ```Map```을 만들어낸다. 

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

##### Snippet-20 : 가변적인 Maps

Map에 값을 추가하려면 `HashMap`을 생성해보자.

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

#### ```Map``` 컬렉션: 비교 연산
##### Snippet-21 : ```Map``` 구현

```HashMap``` 요소는 삽입된 순서대로나 정렬된 순서로 저장된다고 보장되지 않는다.

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

```LinkedHashMap``` 요소는 삽입된 순서대로 저장된다.

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

```TreeMap``` 요소들은 자연적인 키 값의 순서대로 저장된다.


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
1. ```"This is an awesome occassion. This has never happend before."```라는 문자열이 주어졌을 때, 다음과 같은 절차를 수행하시오.
	* 이 문자열에서 각 고유 문자(character)의 발생 횟수를 찾아라
	* 이 문자열에서 각 고유 단어(word)의 발생 횟수를 찾아라

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

####  ```TreeMap``` 복습

```TreeMap```을 기반으로 한 데이터 구조의 흥미로운 연산들을 더 알아보자.

##### Snippet-13 : Treemap 연산

```TreeMap``` 내의 엔트리들은 항상 정렬된다.

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

`TreeMap`은 ```NaviagbleMap``` ```인터페이스```도 구현한다. 

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

#### 자바 컬렉션: 결론 With Tips

지금까지 살펴본 컬렉션 인터페이스와 구현 클래스는 다음과 같다.
* ```List```
* ```Set```
* ```Queue```
* ```Map```

학습한 내용을 빠르게 살펴보도록 하자.
* ```HashMap```이나 ```HashSet```과 같은 "해싱된" 자바 컬렉션(해시 테이블 기반)을 사용하면 순서가 뒤바뀌고 정렬되지 않으며 어떤 순서로도 반복할 수 있다.
* ```LinkedHashSet``` 또는 ```LinkedHashMap```과 같은 "연결된" 자바 컬렉션(연결 리스트 기반)을 사용하면 삽입 순서는 유지되지만 정렬되지 않는다.
* ```TreeSet```혹은 ```TreeMap```과 같은 트리를 기반으로 한 자바 컬렉션을 활용하면 항상 자연 정렬 순서를 유지할 수 있다. 그것은 ```Navigable```, ```NavigableMap```과 같은 탐색 가능한 인터페이스 범주 중 하나를 실행할 것ㅅ이다. 


## 제네릭의 이해

추천 영상
- Generics - https://www.youtube.com/watch?v=v4o0wyFPwEs

제네릭이 필요한 이유는 무엇일까?

```ArrayList```데이터 구조를 중심으로 래퍼 클래스를 만들고자 하는 시나리오와 error-checking 등을 더 잘 할 수 있는 시나리오를 보자. 

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

```MyCustomList``` ```클래스```는 ```String```의 ```ArrayList```를 위한 래퍼이다. 이 데이터 구조에 요소를 삽입하고 삭제하는 것은 간단하다.

다른 타입의 `MyCustomList`를 만들어보자. ```MyCustomList``` 등 추가적인 래퍼 클래스를 써야할까?

예를 들어보자.

##### Snippet-2 : 제네릭 구현

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

**_콘솔창 출력_**

_[Element-1, Element-2]_

_[5, 9]_

##### Snippet-2 Explained

제네릭 ```클래스```의 ```T``` 식별자는 ```MyCustomList<T>``` 컨테이너의 실제 타입에 대한 플레이스 홀더이다. ```MyCustomList``` ```클래스```를 템플릿으로 전환하는 것은 바로 이 플레이스 홀더이다.

이러한 타입의 플레이스 홀더에 대한 명명 규칙은 다음과 같다.
	* 항상 알파벳 대문자를 사용한다 (```T``` 혹은 ```S``` 등)
	* ```TYPE```과 같은 직관적인 단어를 사용한다
	
```GenericsRunner.main``` 내부의 ```MyCustomList```가 실제로 인스턴스화되었을 때 이 플레이스 홀더는 실제 타입으로 대채된다.
	* ```MyCustomList<String> list```가 만들어지면 ```T```는 ```String```으로 대체된다.
	* ```MyCustomList<String> list2```가 만들어지면 ```T```는 ```Integer```로 대체된다.

#### Exercise Set - 18

1. 리스트 저장소의 특정 인덱스에 요소를 반환하는 ```MyCustomList``` 제네릭 클래스 안에 ```get```메소드를 작성하라

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

**_콘솔창 출력_**

_Element-1_

_9_

#### Solution Explained

우리는 반환형이 제네릭인 ```MyCustomList<T>.get``` 메소드를 정의했다. 반환형은 ```MyCustomList<T>```의 정의에서 템플릿과 동일한 플레이스 홀더 ```T```를 가진다.
* ```MyCustomList<String> list```,```list.get```은 ```String```을 반환한다.
* ```MyCustomList<Integer> list2```, ```list2.get```은 ```Integer```를 반환한다.

#### 타입이 제한된 제네릭 구현

우리는 위에서 ```MyCustomList<T>```를 ```String```과 ```Integer```의 저장을 위한 데이터 구조로 인스턴스화 될 수 있다는 것을 보았다.

만약  ```MyCustomList<T>```를 순전히 숫자 값을 저장하기 위해서만 사용한다면 어떨까?

##### Snippet-3 : 제네릭의 타입 제한
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
**_콘솔창 출력_**	
_5_	
_9_	

`T extends Number`를 타입으로 지정할 때, ```Number``` ```클래스````의 API 내에 있는 모든 메소드가 사용 가능하다.

#### 제네릭 메소드

제네릭 메소드들도 만들 수 있따. 몇 가지 예를 살펴보자.

##### Snippet-4 : 제네릭 메소드	
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
**_콘솔창 출력_**	
_[A, B, C, A, B, C]_	
_[1, 2, 3, 1, 2, 3]_	

#### 제네릭과 와일드 카드

제네릭과 함께 와일드 카드도 사용할 수 있다. - `? extends Number`	

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
**_콘솔창 출력_**	
_15.0_	
_15.5_	
_15.0_	

##### Snippet-5 Explained	

```static double sumOfNumberList(List<? extends Number> numbers)``` 메소드의 정의 내에 있는 ```?```기호는 **와일드 카드** 기호이다. 그것은 ```sumOfNumberList```,```numbers```의 어떤 요소이든지 유효한 인자가 되기 위해서는 모든 요소가 ```Number```의 서브 클래스가 될 수 있다는 사실을 의미한다.
* 여기에는 ```Integer```, ```Long```, ```Short```, ```Byte```, ```Float``` 그리고 ```Double```이 포함된다.	
* 또한 래퍼 클래스로 암묵적으로 변환할 수 있기 때문에 기본형 타입의 상대도 포함된다.
* 물론 ```numbers``` ```리스트```의 모든 요소들은 동일한 타입일 필요가 있다.

#### 제한된 동종의 리스트

이전 섹션에서 살펴본 제네릭 와일드 카드를 **상한 제한 와일드 카드**라고 한다. 제한이 있는 동종 타입을 지정하는 데 사용할 수 있따. **하한 제한 와일드 카드**라고 하는 또 다른 와일드 카드 범주가 있으며, 이 범주는 제한 범위 내에서 **다른** 타입의 요소 생성과 함께 사용할 수 있다. 여기 예시가 있다.

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

**_콘솔창 출력_**	
_[1, 1, 1.0. 1.0]_	

## 함수형 프로그래밍 소개

함수형 프로그래밍에 대해 왜 그렇게 야단인가?
알아보자.
	
함수형 프로그래밍 동영상
- Part 1 - https://www.youtube.com/watch?v=aFCNPHfvqEU 	
- Part 2 - https://www.youtube.com/watch?v=5Xw1_IREXQs	

### Step 01: 함수형 프로그래밍 소개

리스트 내에서 루프하고 내용을 출력하는 일반적인 프로그램을 살펴보자.

##### Snippet-01 : OOP List 순회
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

**_콘솔창 출력_**	
_Apple_	
_Banana_	
_Cat_	
_Dog_	

##### Snippet-01 Explained	

위의 접근 방식은 **어떻게**에 초점을 맞춘다.
우리는 리스트를 이리저리 돌려 ```List```의 개별 요소에 접근하고 ```System.out.println()```을 수행하여 각 요소를 출력한다.
함수형 프로그래밍을 통해 **무엇을** 에도 집중할 수 있다.

##### Snippet-02 : ```printBasic()```과 ```printFunctional()``` 	

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

**_콘솔창 출력_**	
_Apple_	
_Banana_Cat_	
_Dog_

##### Snippet-02 Explained	

`list.stream().forEach(element -> System.out.println(element))` - 리스트 스트림의 각 요소를 출력한다.
```element -> System.out.println(element)```는 **람다식**이라고 불린다.

### Step 02: Looping Through A ```List```	

앞 단계에서는 각 `list.stream().forEach(element -> System.out.println(element))` 코드 조각을 사용한다
**함수를 메소드 인자로 전달**한다.
JShell을 사용하여 이 문제를 더 자세히 살펴보자.
숫자 리스트를 출력해 봅시다.

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

`elem -> System.out.println(elem)` 는 람다식이다. 리스트 스트림의 각 요소에 대해 람다식을 수행한다.

### Step 03:  결과 필터링

```스트림(Stream)```은 값의 연속이다. ```filter()```메소드는 어떤 논리에 입각하여 ```스트림```요소를 걸러내는 데 사용될 수 있다.	

##### Snippet-01 : ```filter()```	

`printBasicWithFiltering` 은 필터링의 일반적인 접근을, `printFPWithFiltering`은 함수적 접근을 보여준다.

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
**_콘솔창 출력_**	
_Bat_	
_Cat_	

##### Snippet-02 : 짝/홀수 출력	
숫자를 필터링하는 방법을 살펴보자.

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
일반적으로 이러한 조건은 다음과 같습니다.
* ```num```이 홀수: ```if(num % 2 == 1) { /*  */ }```	
* ```num```이 짝수: ```if(num % 2 == 0){ /*  */ }```	

위의 예제에서는 람다 식을 사용하여 동일한 조건을 정의합니다.
* ```num```이 홀수: ```num -> num%2 == 1```	
* ```num```이 짝수: ```num -> num%2 == 0```	

### Step 05: Streams - 집계 결과
때로는 ㄷ이터를 하나의 결과로 집계하려고 한다. 예를 들어 ```1```과 ```10```사이의 모든 숫자를 더하고 싶을 수도 있다. 또한 한 달 동안 우리 도시의 최대 온도의 평균을 계산해 볼 수도 있다.

##### Snippet-01 : 순서의 합

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

**_콘솔창 출력_**	
_49_	

##### Snippet-01 Explained
```reduce()```메소드는 한 번에 한 쌍의 요소에 작용한다. *초기 값*은 ```0```이다. 리스트 요소에서 한 번에 한 쌍씩 `(num1, num2) -> num1 + num2` 람다식이 실행된다.

#### Classroom Exercise CE-01	

1.  ```(4, 6, 8, 13, 3, 15)``` 리스트가 주어졌을 때, 다음을 연산하라
	* 리스트 내의 짝수의 합 
	* 리스트 내의 홀수의 합
	
	
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

**_콘솔창 출력_**	

_Even Numbers Sum: 18_	
_Odd Numbers Sum: 31_	

### Step 06: 함수형 프로그래밍 VS 구조적 프로그래밍

이전 단계의 **_FPNumberRunner.java_** 프로그램을 다시 살펴보자. 우리는 숫자 리스트의 합계를 계산하는 동일한 작업의 두 가지 변형을 작성했다.
* ```basicSum()```: 기존의 접근법 사용	
* ```fpSum()``: *FP* 방식을 따름

*SP*와 *FP*의 핵심적인 차이점을 벤치마크로 살펴보자

1. **구조적 프로그래밍** (**SP**)	
```java	
	public int basicSum(List<Integer> numbers) {	
		int sum=0;	
		for(int num:numbers) {	
			sum += num;	
		}	
		return sum;	
	}	
```	

2. **함수형 프로그래밍** (**FP**)
```java	
	public int  fpSum(List<Integer> numbers) {	
		int sum = numbers.stream()	
						 .reduce(0, (num1, num2) -> num1 + num2);	
		return sum;	
	}	
```	
무엇이 다른가?
* **변형** (프로그램 데이터 변경):
	1.*SP*: ```basicSum()``` 내에서 변수 ```sum```은 0으로 초기화되고, ```for문```을 반복하며 **변형**을 겪는다.
	2.*FP*: 단지 함께 일할 ```reduce()```의 초기 값을 설정했을 뿐이다. 변경은 없다.
	
* **어떤**연산을 **어떻게**하는가:
	* *SP*:  *해야하는 작업*과 처리할 *방법*을 모두 지정합니다. 이 코드는 ```for```를 사용하여 리스트 요소를 순환하는 동시에 ```sum```의 합계 값을 갱신한다.
	* *FP*: *해야하는 작업*에 초점을 맞추고 있으며 *방법*에는 거의 집중하지 않는다. ```reduce()```는 *스트림*에서 어떤 숫자를 더해야 하는지 신경 쓰는데, 당신은 *스트림*에서 어떤 숫자를 선택하느냐에 대해 신경쓰지 않아도 된다. 

### Step 07: FP 용어	

*FP*용어에 대해 좀 더 살펴보자.


#### 람다식
```java	
	(num1, num2) -> num1 + num2	
```	
이는 다음 메소드와 동일하다

```java	
	int basicSum(int num1, int num2) {		
		return num1 + num2;	
	}	
``` 	
람다식에는 다음과 같이 여러 줄의 Java 코드도 포함될 수 있다

```java	
	(num1, num2) -> {	
		System.out.println(num1 + " " + num2);	
		return num1 + num2;	
	}	
```	
이 코드를 IDE에 넣은 다음 실행해 확인해봅시다.

##### Snippet-01 : 람다식

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

**_콘솔창 출력_**	
_[4, 6, 8, 13, 3, 15]_	
_0 4_	
_4 6_	
_10 8_	
_18 13_	
_31 3_	
_34 15_	
_49_	

#### 스트림

스트림은 일련의 요소들이다. 스트림에서는 다양한 종류의 연산을 수행할 수 있다.
* **중간 연산(Intermediate Operations)**: 스트림을 다루는 연산 - 예를 들어, 람다식을 적용하고 결과로 *또 다른 스트림*을 생성
* **최종 연산(Terminal Operations)**: 스트림이 스트림을 다루는 연산 - 예를 들어, 람다식을 적용하고 단일 결과(하나의 기본형 값/객체나 단일 객체의 컬렉션)를 반환한다. ```reduce()```와 ```forEach()```는 그런 연산의 두 가지다.

### Step 08: 중간 스트림 연산	
중간 스트림 연산의 출력은 또 다른 스트림이다.
가장 널리 사용되는 중간 스트림 연산은 다음과 같다.
Output of an intermediate stream operation is another stream. 	
The most popular intermediate stream operations are: 	
* ```sorted()```	
* ```distinct()```	
* ```filter()```	
* ```map()```	
이 단계에서, 하나씩 확인해 보자.

##### Snippet-01 : ```sorted()``` 와 다른 연산들

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

* ```sorted()```는 사용된 스트림의 요소를 결과에서 보존하지만, 자연 정렬 순서(숫자의 순서 증가,문자열의 알파벳 순)로 표시하기도 한다.
* ```distinct()```는 입력 스트림의 고유 요소만을 포함하는 스트림을 반환한다. 이 메소드는 보존 요소의 상대적 순서를 유지한다.
* 위의 ```sorted()```에 이어 ```distinct()```와 같은 두 가지 이상의 중간 연산을 연결할 수 있다. 이러한 코드를 *파이프라인*이라고 한다.
* ```map()```: 람다식을 적용하여 입력 스트림 요소에서 새로운 결과를 계싼한다. 그런 다음 이러한 결과를 스트림의 출력으로 반환한다. 우리의 예에서 ```map()```은 ```number.stream()```이 만든 ```Stream```객체의 각 요소를 제곱 값으로 한다.

### Step 09: Programming Exercise FP-PE-01	
#### Exercises	

1. 처음 10개의 양의 정수의 제곱을 출력하는 프로그램을 작성하시오.
2. "Apple", "Banana", "Cat" 문자열 리스트를 작성하시오. 모두 소문자로 출력하여라.
3. "Apple", "Banana", "Cat" 문자열 리스트를 작성하시오. 각 문자열의 길이를 출력하여라.

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
**_콘솔창 출력_**	
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
* ```map()```메소드는 람다식을 수용한다.

### Step 10:  최종 연산
최종 연산은 단일 결과(단일 객체/데이터 단위 또는 단일 컬렉션)를 반환한다. 출력 스트림을 반환하지 않는다.
일반적으로 사용되는 예는 다음과 같다.

```java	
	jshell> IntStream.range(1, 11).reduce(0, (n1, n2) -> n1 + n2);	
	$1 ==> 55	
```	

```max()```는 람다식이 ```Comparator<T>``` 구현을 제공할 것으로 기대한다. ```Integer.compare(n1,n2)```는 ```Comparator<T>```의 구현이다.

스트림에 숫자가 없으면 어떡하지? 무엇을 반환해야 할까? 자바 프로그래머로서 우리는 `null`을 싫어하게 되었다. 여러분은 `null`을 반환하고 싶지는 않을 것이다.

```선택형(Optional)```타입이 대안이 될 수 있다.

* ```선택형``` 객체에서 ```isPresent()```를 호출하여 유효한 결과가 포함되어 있는지 확인할 수 있다.
* 같은 객체로 ```get()```을 호출하면 그 결과를 얻을 수 있다.

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
### Step 11: 더 많은 스트림 연산	

이제 ```min()``` (최종 연산)이나 ```filter()``` (중간 연산)과 같은 몇 가지 연산들을 더 가지고 놀아보자. 

##### Snippet-01 : min() and max()	

 ```min()``` 의 사용법은 ```max()```와 비슷하다.	

```java	
	jshell> List.of(23, 12, 34, 53).stream().max((n1, n2) -> Integer.compare(n1, n2)).get()	
	$1 ==> 53	
	jshell> List.of(23, 12, 34, 53).stream().min((n1, n2) -> Integer.compare(n1, n2)).get()	
	$2 ==> 12	
	jshell>	
		
```	
##### Snippet-02 : 짝수와 홀수

```collect()``` 메소드는 ```filter()```의 결과를 리스트로 모으기 위해 호출할 수 있다. `Collectors.toList()`는 사용되는 유틸리티 메소드이다.

```java	
	jshell> List.of(23, 12, 34, 53).stream().filter(e -> e%2==1).forEach(e -> 	System.out.println(e))	
	23	
	53	
	jshell> List.of(23, 12, 34, 53).stream().filter(e -> e%2==1).collect(Collectors.toList());	
	$1 ==> [23, 53]	
	jshell>	
```	

#### Classroom Exercise FP-CE-02

1. 23, 12, 34, 53의 리스트에서 짝수 리스트를 작성하시오.
2. 처음 10개의 양의 정수의 제곱 리스트를 만드시오.

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

* 이미 ```filter()```를 사용할 줄 안다는 점에서 1번에 대한 해결책은 간단하다.
* 2번의 솔루션은 ```boxed()```메소드를 사용하여 ```IntPipeline```을 ```Stream```으로 변환한다. 그 다음은 일상적인 일이다.

### Step 12:  ```Optional<T>``` ```클래스```	
이전 섹션에서는 다음 코드를 작성하고 실행했다.

```java	
	jshell> List.of(23, 12, 34, 53).stream().max((n1, n2) -> Integer.compare(n1, n2));	
	Optional[53]	
	jshell>	
```	
여러분이 원하는 형태로 결과를 얻기 위해 다음과 같이 코드를 수정했다.

```java	
jshell> List.of(23, 12, 34, 53).stream().max((n1, n2) -> Integer.compare(n1, n2)).get();	
53	
jshell>	
```	

```max()```는 스트림을 사용하는 스트림 연산이다. 입력 스트림은 비어있을 수도 있다. 그럴 경우 최대값은 ```null```이 된다. 스트림 연산 중 예외가 발생하는 것은 *FP*에서는 바람직하지 않다. *FP* 코드 파이프라인에서 예외를 처리하라는 요청을 받는다면 이는 정말 보고싶지 않은 일이다.
```Optional<T>``` ```클래스```는 Java SE 8에서 이러한 상황의 생명줄로 소개되었다. 그것은 최종 스트림 연산으로 인한 결과의 부재(혹은 ```null``)를 포함한다. 다음 예는 ```Optional<T>```객체에 쿼리하고 접근하는 방법을 보여준다.

```java	
	jshell> List.of(23, 45, 67, 12).stream().filter(num -> num % 2 == 0).max( (n1, n2) -> 	Integer.compare(n1, n2) )	
	$1 ==> Optional[12]	
	jshell> $1.get()	
	$2 ==> 12	
	jshell> $1.isPresent()	
	$3 ==> true	
```	

결과가 비어있는 경우 그 결과에 저장된 값은 ```null```이 아니라 ```Optional.empty```이다.

```java	
	jshell> List.of(23, 45, 67).stream().filter(num -> num % 2 == 0).max( (n1, n2) -> 	Integer.compare(n1, n2) )	
	$4 ==> Optional.empty	
	jshell> $4.isPresent()	
	$5 ==> false	
	jshell> $4.orElse(0)	
	$6 ==> 0	
```	
여러분은 ```orElse()```메소드를 사용하여 결과의 기본 값을 제공할 수 있다.

```java	
	jshell> List.of(23, 45, 67).stream().filter(num -> num % 2 == 0).max( (n1, n2) -> 	Integer.compare(n1, n2) ).orElse(0)	
	$7 ==> 0	
	jshell> List.of(23, 45, 67, 34).stream().filter(num -> num % 2 == 0).max( (n1, n2) -> 	Integer.compare(n1, n2) ).orElse(0)	
	$8 ==> 34	
	jshell>	
```	
### Step 13: 함수형 인터페이스 : ```Predicate```

람다식을 정의할 때, 뒤에서는 많은 일들이 일어난다.
중요한 개념은 *함수형 인터페이스*이다.
예를 들어 이 용어를 설명하겠다.
다음 코드는 ```filter()```를 뒤에서 바라보는 것이다.

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
**_콘솔창 출력_**	
_34_	
_36_	
_48_	

##### Snippet-01 Explained	
```filter()````의 표기는  `Stream<T> java.util.stream.Stream.filter(Predicate<? super T> predicate)`이다. 이 경우, ```T```는 ```java.lang.Integer```이다.

```filter()```는 ```Predicate```인터페이스를 구현한 객체를 인자로 받아들인다. 이 Predicate와 일치하는 입력 스트림의 요소로 구성된 스트림을 반환한다.
일반적으로 Predicate는 논리적 조건식이다. 이는 출력 스트림에 포함되어야 하는지 여부를 결정하기 위해 각 요소에 적용된다.
```Predicate<T>``` ```인터페이스```는 *함수형 인터페이스*의 한 예이다. 이 인터페이스는 ```boolean test(T t)```라는 한 가지 메소드를 가진다.

`num -> num%2 ==0` 대신 `EvenNumberPredicate`를 구현해보자.

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
**_콘솔창 출력_**	
_34_	
_36_	
_48_	

##### Snippet-02 Explained

```EvenNumberPredicate```는 ```Predicate<Integer>```인터페이스를 구현하고 ```test()```메소드를 오버라이드한다.
람다식인 ```num -> num%2 ==0```를 사용하면 ```EvenNumberPredicate```와 유사한 것이 만들어진다.

### Step 14: 함수형 인터페이스 : ```Consumer```	
또 다른 함수형 인터페이스인 ```Consumer<S>```를 살펴보자.
스트림의 ```forEach()```는 실제로 ```forEach(Consumer<? super S> action)```으로 정의된다.
```Consumer<S>``` 인터페이스는 다음과 같은 정의를 가지고 있다.

```java	
	@FunctionalInterface	
	public interface Consumer<? super S> {	
		void accept(S s) { /*  */ }		
		
		//...	
		
	}	
```	
각각에 대한 람다식과 그 밖의 스트림 연산에서 사용되는 람다식은 사실상 `Consumer`로 구현된다.

##### Snippet-01	
`SysOutConsumer`를 구현해보자.	

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
**_콘솔창 출력_**	
_12_	
_34_	
_36_	
_48_	

##### Snippet-01 Explained	
* 코드는 실제로 그 자신을 나타낸다. ```Consumer<S>```를 사용자 지정하기 위한 단계의 구현은 단순하고 간단하다.
* 사용자가 정의한 ```Predicate<T>```와 ```Consumer<S>```를 둘다 포함하는 마지막 코드는 여전히 작고 우아하다!
	
### Step 15: 더 많은 함수형 인터페이스
이제 스트림 연산 ```map()```을 위해 뒤에서 무슨 일이 벌어지는지 살펴보자. 주어진 리스트에서 모든 짝수 숫자의 제곱을 출력한다고 가정하자.

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
**_콘솔창 출력_**	
_1156_	
_1296_	
_2304_	

#### Snippet-01 Explained
중간 스트림연산 ```map()```의 특징은 다음과 같다.
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
```apply()```메소드는 ```T```라는 객체를 인자로 받아들이고, 또 다른 ```R```타입의 객체를 반환한다. 사실상 어떤 ```함수```구현이든 한 타입의 객체를 다른 타입의 객체로 매핑할 수 있다.

##### Snippet-02 : ```map()``` Behind The Scenes - v2	

`NumberSquareMapper`를 구현해보자.

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
**_콘솔창 출력_**	
_1156_	
_1296_	
_2304_	
**_1156_**	
**_1296_**	
**_2304_**	

### Step 16: 메소드 참조의 소개	
메소드 참조란 무엇인가?
여기 예를 한 번 보자.

##### Snippet-01: 메소드 참조- v1	

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
**_콘솔창 출력_**	
_3_	
_3_	
_3_	
_3_	
_8_	

##### Snippet-02 : 메소드 참조 - v2 	
메소드를 참조하면 람다식을 쉽게 만들 수 있다.
`l -> System.out.println(l)`은 `System.out::println`로 대체될 수 있다.	

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

##### Snippet-03: 메소드 참조 - v3	

정적 메소드 `print`를 정의하고 이를 메소드 참조로 사용해보자.
Let's define a static method `print` and use it using a method reference.	
`MethodReferencesRunner::print``는 `l -> MethodReferencesRunner.print(l)` 와 같다.

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

##### Snippet-04 : 메소드 참조 - v4	
인스턴스 메소드 호출을 해당 메소드 참조로 대체할 수도 있다.
`String`의 경우, `String::length`는 `s -> s.length()`와 같다.	
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

1. 메소드 참조를 이용하여, 주어진 정수 리스트에 최대 짝수를 결정하는 자바 함수형 코드를 작성하라.

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
**_콘솔창 출력_**	
_34_	
**_34_**

#### 요약	

이번 단계에서는
* 메소드 참조가 무엇인지 이해했다.
* 메소드 참조를 사용하여 내장 및 사용자 정의 클래스 메소드를 호출할 수 있다는 것을 배웠다.
* 정적 및 비정적 메소드에서 메소드 참조가 동작하는 것으로 관찰되었다.

### Step 17: FP - 일급 객체(First-Class Citizens)로서의 함수	

함수는 자바에서 일급 객체인가?
* 한 메소드의 인자로 함수를 전달할 수 있는가?
* 변수에 함수를 할당할 수 있는가?
* 메소드 호출에서 반환 값 함수를 얻을 수 있는가?

#### 메소드 인자로서의 함수 전달	

우리는 이에 대한 몇 가지 예를 앞에서 이미 보았다.
아래 예에서는 `num -> num %2 x 0`이 `filter`메소드로 전달된다.
```	
int max = List.of(23, 45, 67, 34).stream()			
								 .filter(num -> num % 2 == 0)	
								 .max( (n1, n2) -> Integer.compare(n1, n2) )	
								 .orElse(0);	
```	
#### 참조 변수에 함수 저장
`evenPredicate` 와 `oddPredicate`는 함수다.

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
**_콘솔창 출력_**	
_1156_	
_1296_	
_2304_	

#### 메소드로부터 함수 반환	
`createEvenPredicate`와 `createOddPredicate`는 함수를 반환하는 메소드의 예이다.

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
**_콘솔창 출력_**	
_1156_	
_1296_	
_2304_	

#### 요약	
이번 단계에서는, 함수에 대해 다음이 참임을 확인했습니다.
* 메소드 인수로 전달 가능함
* 참조 변수에 저장 가능함
* 메소드에서 반환 가능함

## 스레드와 동시 실행	
지금까지 경주 코스를 홀로 달리는 것처럼 실행되는 프로그램만 보아왔따.
그러나 프로그램의 *주 작업*은 작은 작업으로 나누는 것이 이치에 맞는 경우가 많다.(이를 *하위 작업*이라고 하자)
많은 일개미들이 함께 일하며 여왕 개미가 시키는 일을 완수하는 개미 군락을 상상해 보라. 개별 과제의 일부인 개미 집단은 자유자재로 일한다.	
프로그래밍에서 **동시 실행**의 개념은 개미 군집이 자연에서 존재하는 것과 매우 유사합니다.

### Step 01: 동시 실행 작업: ```Thread``` 확장

Java에서는 스레드를 사용하여 작업들을 병렬로 실행할 수 있다. 먼저 간단한 프로그램을 작성해보자.

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
**_콘솔창 출력_**	
_101 102 103 104 105 106 107 108 109 110 111 112 113 114 115 116 117 118 119 120 121 122 123 124 125 126 127 128 129 130 131 132 133 134 135 136 137 138 139 140 141 142 143 144 145 146 147 148 149 150 151 152 153 154 155 156 157 158 159 160 161 162 163 164 165 166 167 168 169 170 171 172 173 174 175 176 177 178 179 180 181 182 183 184 185 186 187 188 189 190 191 192 193 194 195 196 197 198 199_	
_Task1 Done_	
_201 202 203 204 205 206 207 208 209 210 211 212 213 214 215 216 217 218 219 220 221 222 223 224 225 226 227 228 229 230 231 232 233 234 235 236 237 238 239 240 241 242 243 244 245 246 247 248 249 250 251 252 253 254 255 256 257 258 259 260 261 262 263 264 265 266 267 268 269 270 271 272 273 274 275 276 277 278 279 280 281 282 283 284 285 286 287 288 289 290 291 292 293 294 295 296 297 298 299_	
_Task2 Done_	
_301 302 303 304 305 306 307 308 309 310 311 312 313 314 315 316 317 318 319 320 321 322 323 324 325 326 327 328 329 330 331 332 333 334 335 336 337 338 339 340 341 342 343 344 345 346 347 348 349 350 351 352 353 354 355 356 357 358 359 360 361 362 363 364 365 366 367 368 369 370 371 372 373 374 375 376 377 378 379 380 381 382 383 384 385 386 387 388 389 390 391 392 393 394 395 396 397 398 399_	
_Task3 Done_	
_Main Done_	

##### Snippet-1 Explained	
보다시피, 세 개의 ```for문```(독립적인 작업들)을 모두 실행하는 것은 순차적이다. 지금까지의 모든 코드가 이렇게 실행되었다!

### 스레드 생성	
여러분이 프로그램 내에서 하위 작업을 나타내는 스레드를 만드는 방법이 두 가지 있다. 
*  자체적인 스레드 ```클래스```를 정의하여 **```Thread```** ```클래스```를 하위 클래스화 한다.
* **```Runnable```** ```인터페이스```를 구현하는 자체적인 스레드 ```클래스```를 정의한다.

이 단계에서, 우리는 첫번째 대안에 주력할 예정이다.

##### Snippet-01 : 간단한 자바 스레드 클래스

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
**_콘솔창 출력_**	
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

우리는 ```Task1``` ```클래스```를 정의하여  하위 작업을 ```run()``` 메소드 정의를 표시하였다. 그러나 우리의 ```main()```메소드 내에서 그런 스레드를 만들어 낼 때 우리는 어떤 식으로든 ```run()```을 호출하지 않은 것 같다. 여기서 무슨 일이 일어나는가?
```start()``` 메소드라고 하는 제네릭 메소드를 통해 스레드를 만들고 시작할 수 있따. ```start()```를 호출하면 각각 스레드의 ```run()```메소드를 호출할 것이다.

콘솔 출력에서 *Task1*의 출력이 *Task2* 및 *Task3*으로 표시된 작업의 출력과 중복되는 것을 알 수 있다. *Task1*은 실행 중인 main과 병렬로 실행된다.(*Task2*,*Task3*)

#### 요약

이번 단계에서는
* ```Thread```를 하위 클래스로 하여 스레드를 정의하는 방법을 발견했다.
* 스레드를 실행하는 방법을 보였다.

### Step 02: 동시 실행 작업 - Runnable 구현
##### Snippet-01 : Implementing Runnable	
**Step 01**에서는 Java 프로그램에서 스레드가 하위 작업을 나타낼 수 있는 두 가지 방법이 있다고 알려줬다. 하나는 ```Thread```를 하위 클래스로 두는 것이고, 다른 하나는 ```Runnable```을 구현하는 것이다. 우리는 조금 전에 첫 번째 방법을 보았고, 이제 두 번째 방법을 탐험할 때이다. 다음 예에서는 이 작업으 수행 방법을 보여 준다.

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
**_콘솔창 출력_**	
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
이번 예에서 우리는 ```Runnable```인터페이스에서 ```run()```메소드를 구현하여 ```Runnable```을 구현했다.
Runnable 인터페이스를 구현하는 Task2를 실행하기 위해 이 코드를 사용했다. `Task2`의 인스턴스를 전달하여 `스레드`생성자를 사용하고 있다.

```java	
Task2 task2 = new Task2();	
Thread task2Thread = new Thread(task2);	
task2Thread.start();	
```	

출력을 통해 세 가지 작업이 모두 병려로 실행되고 있음을 알 수 있다.

#### 요약

이번 단계에서는
* ```Ruannable``` ```인터페이스```를 구현하여 스레드를 만드는 또 다른 방법을 모색했다.
* ```Runnable``` ```인터페이스```로 만든 스레드를 실행하는 법을 배웠다.

### Step 03: 스레드 생명 주기

Java 스레드는 살아있는 동안 일련의 **상태**를 거친다. **생명 주기**라는 용어는 이 사실을 설명하는 데 사용되며, 다양한 시점에서 스레드가 어떤 특정 상태에 있을 수 있는지를 명확하게 정의한다.
최근에 살펴본 _**Step 02**_의 다음 예를 살펴보자.


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

스레드의 상태는 다음과 같다.
* **NEW**: 스레드가 만들어진 직후의 상태, ```start()```메소드는 아직 호출되지 않았다.

	* *Task1*의 경우: ```Task1 task1 = new Task1();```의 실행 후
	* *Task2*의 경우:  ```Task2 task2 = new Task2();  task2Thread = new Thread(task2);```의 실행 후
* **TERMINATED/DEAD**: 한 스레드의 ```run()```메소드에 포함된 모든 구문이 완료되면, 그 스레드는 종료되었다고 한다.
```start()```메소드가 호출된 후, 나머지 세 개의 상태 중 어느 것에도 스레드가 있을 수 있다.
* **RUNNING88: 스레드가 현재 실행 중인 경우.
* **RUNNABLE**: 스레드가 현재 실행되고 있지 않지만 언제든지 실행할 수 있는 경우.
* **BLOCKED/WATING**: 스레드가 현재 프로세서에서 실행되고 있지 않고, 실행할 준비도 되지 않은 경우. 외부 리소스(예: 사용자 입력) 또는 다른 스레드를 기다리는 경우일 수 있다.

#### 요약	

이번 단계에서는

In this step, we:	
* 여러 가지 스레드 상태에 대해 예시와 함께 설명했다.

### Step 04: 스레드 우선 순위

Java에서는 스레드 스케줄러를 *요청*하여 스레드 우선 순위를 변경할 수 있따. 어떤 스레드의 우선 순위는 항상 ```MIN_Priority = 1```에서 ```MAX_Priority = 10```까지 고정된 범위에 있다. 모든 스레드에 할당된 기본 우선 순위는 ```NORM_Priority = 5```이다.
이러한 우선 순위 변경 요쳥은 ```Thread``` ```클래스```에서 사용 가능한 정적 메소드인 ```setPriority(int)```를 호출함으로써 이루어진다. 이 요청은 이에 응할 수도 있고 그렇지 않을 수도 있으므로 이에 대비하여야 한다!

### Step 05: 스레드 간의 통신
스레드가 명시적으로 생성되지 않은 프로그램은 단일 스레드 응용 프로그램이다. 여기서 우리가 언급하는 스레드는 프로그램의 ```main()```메소드를 실행하는 *메인 스레드*이다.
경우에 따라 스레드는 서로 종속될 수 있다.
**Step 02**의 예를 살펴보자.
여기에 조건을 추가하려고 한다. *Task3*는 *Task1*이 종료된 후에만 실행된다.

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

```task1.join()```은 task1이 끝나기를 기다린다. 따라서 ```task1.join()```이후의 코드는 `task1`의 완료되어야만 실행된다.
*Task1*과 *Task2*를 모두 실행한 후에만 *Task3*를 실행하려면 ```main()```의 코드는 다음과 같이 표시되어야 한다.

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

*Task1*과 *Task2*는 여전히 독립적인 하위 작업이다. 스레드 스케줄러는 자유롭게 교차 실행할 수 있다. 그러나 *Task3*는 두 작업이 모두 종료된 후에만 시작된다.

#### 요약	

이번 단계에서는
* 스레드 간의 통신의 필요성을 이해했다.
* Java가 스레드가 서로 대기할 수 있는 메커니즘을 제공한다는 것을 알게 되었다.
* ```join()```메소드를 사용하여 스레드 실행이 순서를 정하는 방법을 관찰했다.

### Step 07: ```synchronized``` 메소드와 ```Thread``` 유틸리티

스레드가 피곤해지면, 여러분은 그것을 재울 수 있다. 여러분이 지정하는 것이다. 기억나지 않는가?
```Theread```클래스는 두 가지 메소드를 제공한다.
* ```public static native void sleep(int millis)``` : 이 메소드를 호출하면 요청한 스레드가 ```millis``` 밀리초 동안 *blocked* / *wating* 상태가 될 것이다.
* ```public static native void yield()``` : 스레드 스케줄러에게 다른 스레드 실행을 요청한다. 스케줄러는 이러한 요청을 무시할 수도 있다.

##### Snippet-01 : 스레드 유틸리티	
**jshell>** ```Thread.sleep(1000)```	
**jshell>** ```Thread.sleep(10000)```	
**jshell>**	

##### Snippet-7 Explained

* ```Thread.sleep(10000)```은 ```JShell```프롬프트가 *최소* 1초 이상 지연된 후에 나타나게 한다. 이러한 지연은 우리가 ```Thread.sleep(1000)```을 실행할 때 더욱 두드러진다. 

### Step 08: 이전 접근법의 단점
`Thread`클래스에서 동기화하는 방법 중 몇 가지를 살펴보았다.
* ```start()```	
* ```join()```	
* ```sleep()```	
* ```wait()```	

위의 방법에는 몇 가지 단점이 있다.
* **세부 제어 없음**: 예를 들어, *Task1* 또는 *Task2* 중 어느 *하나*가 완료된 후 *Task3*를 실행하려고 한다. 할 수 있을까?
* **유지 및 관리 어려움**: 앞으 예에서 설명한 코드로 5~10개의 스레드를 관리한다고 가정해 보자. 매우 어려울 것이다.
* **하위 작업 반환 메커니즘이 없음**: ```Thread``` ```클래스```나 ```Runnable``` ```인터페이스```가 있으면 하위 작업에서 결과를 얻을 방법이 없다.

### Step 09: ```ExecutorService```소개
```Thread``` API의 심각한 한계를 해결하기 위해 **Java SE 5**에 새로운 ```Executor Service```가 추가되었다.
```Executor Service```는 코드 내의 스레드를 더 잘 관리하기 위해 사용할 수 있는 프레임워크이다. 다음과 같은 기본 제공 방법이 있다.
* 보다 직관적인 스레드 생성 및 실행
* 스레드 상태 및 생명주기를 보다 쉽게 관리
* 제어력이 향상된 스레드 간 동기화
* 스레드 그룹을 깔끔하게 처리

```Executor Service```는 이러한 각각의 목적을 달성하기 위한 유틸리티를 제공한다. 다음 예에서 다룰 스레드 생성부터 시작해보자.

##### Snippet-01 : 스레드 생성	
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
**_콘솔창 출력_**	
_Task1 Started_	
_101 102 103 104 105 106 107 108 109 110 111 112 113 114 115 116 117 118 119 120 121 122 123 124 125 126 127 128 129 130 131 132 133 134 135 136 137 138 139 140 141 142 143 144 145 146 147 148 149 150 151 152 153 154 155 156 157 158 159 160 161 162 163 164 165 166 167 168 169 170 171 172 173 174 175 176 177 178 179 180 181 182 183 184 185 186 187 188 189 190 191 192 193 194 195 196 197 198 199_	
_Task1 Done_	
_Task2 Started_	
_201 202 203 204 205 206 207 208 209 210 211 212 213 214 215 216 217 218 219 220 221 222 223 224 225 226 227 228 229 230 231 232 233 234 235 236 237 238 239 240 241 242 243 244 245 246 247 248 249 250 251 252 253 254 255 256 257 258 259 260 261 262 263 264 265 266 267 268 269 270 271 272 273 274 275 276 277 278 279 280 281 282 283 284 285 286 287 288 289 290 291 292 293 294 295 296 297 298 299_	
_Task2 Done_	

##### Snippet-01 Explained	
`ExecutorService executorService = Executors.newSingleThreadExecutor()` 는 단일 스레드 Executor Service를 생성한다. 그것이 이 작업이 차례로 연속된 이유이다.

##### Snippet-02 : main은 병행하게 실행됨	
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
**_콘솔창 출력_**	
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

그 결과로 발생하는 혼돈에서 볼 수 있는 유일한 순서는 *Task2*는 *Task1*이 완료된 후에만 실행을 시작한다는 것이다.
Executor Service에서 관리하는 스레드는 `main`메소드와 병행한다.

### Step 10: Executor -  스레드의 개수를 사용자 지정함
```ExecutorService```를 통해 스레드 *풀*을 만들 수 있다.
다음 예에서는 다양한 종류와 다양한 크기의 스레드 풀을 만드느 방법을 보여준다.

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
**_콘솔창 출력_**	
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
`Executors.newFixedThreadPool(2)`을 사용하여 `ExecutorService`를 만들었다. 그래서 `ExecutorService`는 최대 두 개의 병렬 스레드를 사용한다.
* *Task1*과 *Task2*는 ```ExecutorService```의 일부로 동시에 실행되며,
* ```main()```을 실행하는 스레드는 ```ExecutorService```가 만든 이 스레드 풀과 동시에 실행된다.

##### Snippet-04 : All-Executor Task Execution	
이제 `ExecutorService`를 사용할 수 있는 간단한 예를 만들어 보자.
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
`Executors.newFixedThreadPool(2)` - 두 개의 스레드가 병렬로 연결된다. ```new Task(3)```라는 스레드는 ```new Task(1)```과 ```new Task(2)```중 어느 하나라도 실행을 마친 후에야 실행된다.

##### Snippet-04 : 더 큰 사이즈의 스레드 풀	
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

풀을 더 크게 세 개로 만들어보자
* 처음에는 ```1```,```2```,```3``` 작업이 ```ExecutorService```에 추가되어 시작된다.
* 두 작업 중 하나가 종료되는 즉시 스레드 풀에서 다른 작업을 선택하여 실행할 수 있다. 

#### 요약
이번 단계에서는
* ```ExecutorService```를 이용해 같은 종류의 스레드드 풀을 어떻게 만들 수 있는지 알아봤다.
* 스레드 풀의 크기를 지정하는 방법을 설명했다.


### Step 11:  ```ExecutorService```: 작업에서 값 반환	
##### Snippet-01: Returning a Future Object	

지금까지, 우리는 대부분 독립적이고, 어떤 결과도 그것들을 시작한 메인 프로그램으로 반환하지 않는 하위 작업들만을 보아왔다.
스레드에서 값을 반환할 수 있도록 Java는 ```Callable<T>```인터페이스를 제공한다.
다음 예는 ```Callable<T>```를 실행하는 방법을 알려주며, ```ExecutorService```와 사용한다.

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
**_콘솔창 출력_**	
_CallableTask in28Minutes Submitted_	
_Hello in28Minutes_	

##### Snippet-01 Explained	
- `class CallableTask implements Callable<String>` - 반환 타입이 `String`인 `Callable`을 구현한다.
- `public String call() throws Exception ` - `call`메소드를 구현하고 `String` 값을 다시 반환한다.
- ```executorService.submit(new CallableTask(String))``` 은 스레드 풀에 Callable작업을 추가한다. 그러면 작업 스레드가 **RUNNABLE** 상태가 된다. 그 후 이 프로그램은 ```call()``메소드를 계속 한다.
- `welcomeFuture.get()` - `main`스레드가 작업 결과를 기다리게 한다.

#### 요약

이번 단계에서는

* 값을 반환하는 하위 작업을 생성하는 메커니즘의 필요성을 이해했다.
* 자바에 ```Caalable<T>``` 인터페이스가 있다는 것을 발견했다.
* ```ExecutorService```가 ```Callable```스레드를 관리할 수 있는 능력이 있는 것을 보았다.

### Step 11: Executors - Callable 작업이 완료될 때까지 기다리기
```ExecutorService``` 프레임워크는 또한 당신이 ```Callable```스레드 풀을 만들 수 있게 해준다. 뿐만 아니라 반환 값도 함께 수집할 수 있다.

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
**_콘솔창 출력_**	
_Hello in28Minutes_	
_Hello Ranga_	
_Hello Adam_	


##### Snippet-01 Explained	
```ExecutorService```의 ```invokeAll()```메소드는 ```Callable``` 작업의 리스트를 스레드 풀에서 시작할 수 있게 해준다. 또한 ```List```라는 ```Future```객체들은 이러한 ```Callable```스레드 하나 하나에 해당하는 반환값을 보유하는 데 사용될 수 있다.
반환 값 목록은 **모든** 스레드가 완료되고 결과가 반환된 후에만 접근할 수 있다.
이는 콘솔창 출력에서 확인할 수 있다. 계획된 모든 환영 메시지는 단번에 출력되지만, 최소한 ```3000```밀리초의 기다림이 끝난 뒤에야 출력된다.
이제 더 큰 스레드 풀 크기를 사용하는 시나리오가 무엇인지 알아보자.

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

**_콘솔창 출력_**	
_Hello in28Minutes_	
_Hello Ranga_	
_Hello Adam_	

##### Snippet-02 Explained	
환영 메시지는 모두 한 묶음으로 다시 출력되지만, 전체 대기 시간을 짧아진다. 그 이유는 다음과 같다.
* 스레드 풀이 사이즈는 이제 ```2```가 아니라 ```3```이다. 즉, 세 가지 작업을 모두 한 번에 ```RUNNABLE```상태로 전환할 수 있다.
* 그런 다음 이들은 **BLOCKED** 상태로 거의 동시에 진입하는데 이는 전체 대기 시간이 ```3000```밀리초보다 훨씬 짧다는 것을 의미한다. 이는 더 큰 스레드 풀의 장점이다!

#### 요약

이번 단계에서는

* ```Callable``` 스레드 풀의 반환 값을 한 번에 수집할  수 있다는 것을 알게 되었다.
* 이는 ```invokeAll()```메소드를 사용하여 실행되며, 이러한 결과를 저장할 ```Future```객체의 ```List```를 지정한다.
* 이러한 시나리오의 스레드 풀 크기를 변경하면 응답 시간도 크게 변경될 수 있다.

### Step 12:  Executor - Wait Only For The Fastest Task	
다음 세 가지 작업 중 하나가 완료될 때까지 기다릴 수 있는 방법에 대해 알아보자.

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

**_콘솔창 출력_**	
_Hello Ranga_	

**_콘솔창 출력_**	
_Hello in28Minutes_

**_콘솔창 출력_**	
_Hello Ranga_	

**_콘솔창 출력_**	
_Hello Adam_	

##### Snippet-01 Explained	
첫 번째 하위 작업이 끝나면 ```invokeAny()```라는 메소드가 반환된다. 또한 반환된 값은 ```Future```의 객체가 아니다. 그것은 ```call()```메소드의 반환 값이다.
여러 번의 실행에서 콘솔 출력의 순서가 변경되는 것을 볼 수 있다. 그 이유는 다음과 같다.
* 세 가지 작업 모두 크기가 ```3```인 스레드 풀로 같이 만들어졌다.
* 따라서 이 스레드들은 **RUNNABLE**상태로 거의 동시에 이동하는 독립적인 스레드이다.

#### 요약	

이번 단계에서는
* ```ExecutorService```가 ```Callable``` 스레드에서 첫 번째 결과를 반환할 수 있는 방법이 있다는 것을 알게되었따.

## 예외 처리의 이해

예외 처리 관련 추천 동영상
- https://www.youtube.com/watch?v=34ttwuxHtAE	

프로그래머가 직면하는 오류는 두 가지 이다.
* **컴파일 타임** 오류: 구문 또는 의미 오류를 탐지할 때 컴파일러가 플래그를 지정함.
* **런타임** 오류: 코드를 실행할 때 런타임 환경에서 오류가 감지됨.

런타임 오류의 예는 다음과 같다.
* 객체에 대한 *힙 메모리*가 부족하거나, *호출 스택* 메소드에 대한 공간 부족 
* 숫자를 ```0```으로 나눔
* *열리지 않은* 파일 *읽기* 시도
예외는 *예상하지 않은* 상황이며, 이러한 상황이 발생하더라도 프로그래머에게 나쁜(혹은 좋은) 것은 아니다. 프로그램의 잠재적 예외 조건을 *인식*하고, 이를 효과적으로 *처리*하기 위한 메커니즘을 사용하는 것은 프로그래머의 책임이다.

예외 처리는 일반적으로 두 가지 중요한 목적을 가진다.
1. 최종 사용자에게 유용한 메시지를 제공한다.
2. 프로그래머가 근본 원인을 식별하는 데 도움이 되는 충분한 정보를 기록한다.
	
### Step 01: 예외 소개
이전 단계에서 프로그램 메모리가 부족하거나 숫자를 ```0```로 나누려고 하는 코드와 같이 몇 가지 예외 사례를 제시했다.
Java 런타임에 예외를 적용하는 실제 예를 보고 싶지는 않은가? 

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

**_콘솔창 출력_**	
**_java.lang.NullPointerException_**	
_Exception in thread "main" java.lang.NullPointerException_	
_at com.in28minutes.exceptionhandling.ExceptionHandlingRunner.callMethod (ExceptionHandlingRunner.java:8)_	
_at com.in28minutes.exceptionhandling.ExceptionHandlingRunner.main (ExceptionHandlingRunner.java:4)_	

##### Snippet-01 Explained	
```java.lang.NullPointerException```은 자바 런타임에 `null` 참조로 ```length()```를 호출할 때 *던져진다*.
메인 등 전체 콜 체인에서 예외를 처리하지 않으면 해당 예외는 던져지고 프로그램은 종료된다. ```System.out.println()```구문은 예외 이후 절대 실행되지 않는다
런타임에서 **호출 스택 추적**을 콘솔에 출력한다.

예를 들어, 간단한```Test``` ```클래스```를 생각해보자.

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

그러나, ```callThree()```에 사용된 코드 name.length()는 ```NullPointerException```을 유발했다. 그러나 이 작업은 처리되지 않으며, 콘솔이 다음과 같은 디스플레이를 가져온다.
_Exception in thread "main" java.lang.NullPointerException_	
_at Test.callThree(Test.java:13)_	
_at Test.callTwo(Test.java:9)_	
_at Test.callOne(Test.java:6)_	
_at Test.main(Test.java:3)_	

이것은 *시간 내에 동결*된 스택의 호출 추적에 불과하다.


#### 요약

이번 단계에서는
* 예외가 발생하는 생생한 예를 보았다.
* 예외 발생 시 스택의 호출 추적을 표시하는 방법을 이해했다.
* 이 이해를 다른 예와 함께 보강했다.

### Step 02: 예외 처리	
자바에서는 예외 처리가 **```try```-```catch```** *블록*을 통해 이루어진다.

##### Snippet-01 : Handling an Exception	
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
**_콘솔창 출력_**	
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

예외 (```NullPointeException```)는 이 블록을 추가한 후에도 계속 발생하지만 지금은 실제로 **catch**되었다. 비록 우리가 예외를 잡아내기 위해 한 것은 없지만, 우리는 그 프로그램이 갑자기 끝나는 것을 피했다.
`method2`의 ```int len = str.length()``` 뒤의 구문들은 실행되지 않는다.
그러나 ```method1()```의 코드는 모두 실행되었다 (```"method1 Done```메시지가 출력되었다.) ```main()```메소드 또한 성공적으로 실행을 마쳤다.
그래서 그 프로그램은 우아하게 종료되었따. ```method1()```과 ```main()```은 둘 다 ```mathod2()```에서 발생하는 ```NullPointerException```에 대해 모르고 있다.

##### Snippet-02: Print Debug Information
 `ex.printStackTrace();`를 추가해보자.
 
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
**_콘솔창 출력_**	
**_java.lang.NullPointerException_**	
_Exception in thread "main" java.lang.NullPointerException_	
_at com.in28minutes.exceptionhandling.ExceptionHandlingRunner.method2 (ExceptionHandlingRunner.java:14)_	
_at com.in28minutes.exceptionhandling.ExceptionHandlingRunner.method1 (ExceptionHandlingRunner.java:8)_	
_at com.in28minutes.exceptionhandling.ExceptionHandlingRunner.main (ExceptionHandlingRunner.java:4)_	
_method1() Done_	
_main() Done_	

```printStackTrace()```는 모든 예외가 상속하는 ```Exception``` ```클래스```가 제공한다. 이 메소드는 예외 발생 시 프로그램의 중지된 호출 추적을 출력하지만 프로그램을 종료하지는 않습니다. 그 다음 코드는 계속 실행된다.
스택 추적은 예외 시나리오를 디버깅하는 데 유용한 정보를 프로그래머에게 제공한다.

#### 요약	

이번 단계에서는
* 자바의 예외를 처리하는 기본 메커니즘인 ```try```-```catch``` 블록을 도입했다.
* 예외를 처리할 때 프로그램이 어떻게 실행되고 정상적으로 종료되는지 확인했다.

### Step 03: ```Exception``` 계층 구조 	

위의 ```try```-``catch``` 블록의 코드는 마술처럼 작동하지 않는다. 호출 내역을 보면 이 프로그램이 ```method1()```에서 ```NullPointerException```을 만난다는 것은 분명하다.
놀라운 것은 그것이 ```Exception```을 의미하는 ```catch```절에 잡혔다는 점이다. 이것이 작동하는 이유는 ```NullPointerException```이 ```Exception```이기 때문이다. 
자바의 경우 ```Exception``` ```클래스```에 루트를 둔 예외 유형 계층구조가 있다. 예를 들면,
* ```NullPointerException```은 ```RuntimeException```이다.
* ```RuntimeException```은 ```Exception```이다.
* 그래서 효과적으로, ```NullPointerException```은 ```Exception```이다!

이 상속 트리의 서로 다른 분기는 실제로 다른 예외 범주를 나타낸다. 잠시 후에 이 주제에 대해 자세히 알아보도록 하자.

##### Snippet-01 : Catching NullPointerException	
method2에 추가적인 `NullPointerCatch` 캐치를 추가해보자.

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
**_콘솔창 출력_**	
**_NullPointerException_**	
_method1() Done_	
_main() Done_	

##### Snippet-01 Explained	
_```try```에 이은 ```catch```구문들 중 **단 한 개만이** 실행될 수도 있다. ```try```후 (일련의 순서로)**일치하는** **first** ```catch```절은 항상 실행된다. **아무것도** 일치하지 않는 경우 예외는 **처리되지 않는다**._ 
우리는 ```NullPointerException```을 다루기 위해 ```method2()```안에 ```catch```블록을 추가했다. 일반적으로 가장 구체적인 예외 클래스는 일치한다. 따라서 `NullPointerException`의 캐치 블록 예외가 일치한다.
보다 구체적인 일치부터 덜 구체적인 일치까지 ```try```를 한 후에 ```catch```블록을 두어야 한다.

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
**_콘솔창 출력_**	
**_ArrayIndexOutOfBoundsException : 3_**	
_Exception in thread "main" java.lang.ArrayIndexOutOfBoundsException_	
_at com.in28minutes.exceptionhandling.ExceptionHandlingRunner.method2 (ExceptionHandlingRunner.java:14)_	
_at com.in28minutes.exceptionhandling.ExceptionHandlingRunner.method1 (ExceptionHandlingRunner.java:8)_	
_at com.in28minutes.exceptionhandling.ExceptionHandlingRunner.main (ExceptionHandlingRunner.java:4)_	
_method1() Done_	
_main() Done_	

##### Snippet-02 Explained	
```ArrayIndexOutOfBoundsException``` 은 ** ```IndexOutOfBoundsException```이고, ** ```IndexOutOfBoundsException```는 ```RuntimeException```이기 때문에 최종적으로```Exception```이다.	
```ArrayIndexOutOfBoundsException``` 눈 ```NullPointerException```의 하위 클래스가 아니다. 따라서 이는 첫 번째 캐치 블록과 일치하지 않는다.
```ArrayIndexOutOfBoundsException``` is a sub class of  ```Exception```. Hence, that ```catch``` block matched, and the statement ```ex.printStackTrace();``` within it ran.	```ArrayIndexOutOfBoundsException```은 ```Exception```의 하위 클래스이다. 따라서 ```catch```블록은 매치되고, ``ex.printStackTrace();```는 실행된다.
```Exception```의 핸들러를 생략하면 ```ArrayIndexOutOfBoundsException```은 이 ```try```-```catch```블록에 잡히지 않는다. ```method1()```에서 다루지 못하거나, 심지어 ```main()```에서 다루지 못하기 때문에 우리의 프로그램은 갑자기 중단되어야 할 것이다.

#### 요약	

이번 단계에서는
* 자바에는 ```Exception```에 뿌리를 둔 예외 계층구조가 있다는 것을 알게 되었다.
* 여러 예외가 발생할 수 있는 예제를 살펴보았다.
* ```Exception```의 핸들러가 어떤 예외와 어떻게 일치하는지 관찰했다.

- - - 	
### Step 04:  ```finally```의 필요성	
예외가 발생하면 프로그래머의 세계는 순식간에 뒤집힐 수 있다. 처리되지 않으면 터널 끝에 불이 들어오지 않고 프로그램이 갑자기 종료된다.

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
**_콘솔창 출력_**	
_Exception in thread "main" java.lang.ArrayIndexOutOfBoundsException_	
_at com.in28minutes.exceptionhandling.FinallyRunner.main (FinallyRunner.java:8)_

##### Snippet-01 Explained	
이 예에서는 `Scanner` 객체를 사용하여 콘솔에서부터 읽어온다. 이상적으로 `Scanner`객체는 ```scanner.close();```를 사용하여 닫아야한다.
그러나, 이 예에서는 예외를 만들기 전의 행이 있기 때문에 이 값을 호출하지 않는다.(```int num = numbers[5];```는 4차원 배열의 다섯 번째 요소에 접근하려 한다)
즉, 획득된 시스템 리소스는 절대 놓아주지 않는다.
수집된 리소스는 정상 종료든, 갑작스러운 종료든 항상 놓아주도록 하는 것이 중요하다. 예외를 처리하는 동안 이 작업을 수행하는 방법을 알아보자.

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
**_콘솔창 출력_**	
**_ArrayIndexOutOfBoundsException_**	
_Exception in thread "main" java.lang.ArrayIndexOutOfBoundsException_	
_at com.in28minutes.exceptionhandling.FinallyRunner.main (FinallyRunner.java:10)_	
_Before scanner close_	
_Before exiting main_	

##### Snippet-02 Explained	
```finally```의 코드는 예외가 있더라도 거의 항상 실행된다.
```scanner =new Scanner(System.in);``` 또한 예외로 귀결될 수 있기 때문에 우리는 `scanner`에 null 검사를 추가했다.
.
```java	
	} finally {	
		if(scanner != null) {	
			System.out.println("Before scanner close");	
			scanner.close();	
		}	
	}	
```	
#### 요약	

이번 단계에서는
* 예외적인 조건으로 인해 리소스 누출이 어떻게 발생하는지 관찰했다.
* ```try``` - ```catch```블록의 ```finally```절에 대해 알게 되었다.

### Step 05: Programming Puzzles -  PP-01	
#### Puzzle-01	
* ```finally```절은 다음과 같은 경우에 실행될 것인가?
	* ```///str = "Hello";``` 구문이 그대로 유지된다
	* ```///str = "Hello";``` 구문이 삭제되었는가?

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
* ```finally``` 절의 코드는 언제 실행되지 않는가?
* **_Answer_**
	* 해당 코드에 앞서 동일한 ```finally```절 내에서의 구문은 예외로 한다.
	* JVM이 고장난 경우. 이는 ```System.exit```으로 호출한 일부 시나리오에서 시뮬레이션할 수 있다. 적절한 ```int```인자를 가지고, 같은 ```try```-```catch```구문의 적절한 ```catch```절에 있다.
	
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
* 다음 코드는 ```catch```없는 ```try```일까, 아니면 ```finally```일까?

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
때때로 Java에서는 예외를 처리하도록 강제한다.

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
**_이 프로그램은 컴파일되지 않는다!_**	
우리가 컴파일러 오류로 플래그를 얻은 이유는 ```sleep()```메소드의 표기에 있다. 이것은 ```Thread``` ```클래스```안에 그 정의가 있다.

```java	
	public static native void sleep(long millis) throws InterruptedException {	
		//...	
	}	
```	
이 선언은 여러분이 보통 어떤 메소드에 기대하는 것과는 좀 다르다. 그렇지 않은가? 여기에는 **```throws``` **를 포함한다.
메소드가 예외를 `던지는` 경우 호출하는 메소드는 다음을 수행해야 한다.
* ```try``` -```catch``` 블록으로 처리
* 혹은 `throws`를 선언
```try```-```catch``` 블록을 이용해 시작해보자.

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
* ```sleep()```를 호출하는 ```main()```은  ```try```-```catch```블록으로 ```InterrutedException```을 다루는 것을 선택한다.

#### ```throws``` 키워드
```throws```는 어떤 메소드가 예외를 줄 수 있다고 선언할 때 사용된다. 여기에는 ```throws``` 키워드가 포함되며 이 다음에 예외 유형 목록이 나온다.
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
여기서 ```riskyMethod()``` 내의 ```try```-```catch```블록을 제거한 것은 예외를 관리하는 방법을 따르고 싶기 때문이다. 대안으로 코드를 컴파일하기 위해 ```riskyMethod()```에 ```throws```를 추가했다.
우리는 예외를 다루는 `main`메소드를 만들어 보았다.

#### 요약
이번 단계에서는
* Java에서 특정 예외는 강제로 처리하지 않는다는 것을 발견했다.
* 나머지는 모두 관리/처리해야 한다는 것을 알게 되었다.
* 이러한 "Checked" 예외를 관리하는 방법에는 두 가지가 있다.
	* ```try```-```catch``` 블록으로 처리
	* ```throws``` 사용
	
### Step 08: 자바 예외 계층구조	
Right at the root (top, we mean), the Java exception hierarchy looks like this:	
```java	
	class Error extends Throwable{}	
	class Exception extends Throwable{}		
	class InterruptedException extends Exception{}	
	class RuntimeException extends Exception{}	
	class NullPointerException extends RuntimeException{}	
	...	
```	
한번 ```Error```가 발생하면, 프로그래머가 할 수 있는 일은 아무것도 없다. 그 예는 다음과 같다.
* 힙 메모리 공간이 부족한 JVM

`예외`는 처리될 수 있따. 예외에는 두 가지 유형이 있다.
* ```RuntimeException``과 그 하위 클래스. 이는 **Unchecked Exception** 범주에 속한다. 우리가 본 또 다른 예는 ```RuntimeExcepton```을 상속받는 ```NullPointerException```이다.
* ```RuntimeException```에 뿌리를 둔 서브 트리를 제외한 다른 모든 ```Exception```의 서브 클래스를 **checked exception**이라고 한다. 우리가 마주친 예는 ```InterruptedException```이다.
메소드에서 **checked exception**이 호출되는 경우 다음 중 하나를 수행한다.
* 메소드 호출은 적절한 처리를 위해 ```try```-```catch```블록으로 묶어야 한다.
* caller는 이 예외를 자신의 caller에게 알려야 한다. ```throws```를 사용해 표기를 강화해야 한다.

**unchecked exception**이 포함되는 경우
* ```try```-```catch``` 블록으로 처리할 수 있는 옵션이 있다.
* 처리할 의무는 없다.

**checked exception**은 반드시 처리해야 하는 반면, **unchecked exception**은 처리되지 **않을 수 있다**.

#### 요약

이번 단계에서는
* Java 예외 계층에는 두 가지 범주가 있다는 것을 발견했다. 이는 다음과 같다
	* Checked exception
	* Unchecked exception
이 두 가지를 관리하기 위한 다양한 전략이 있다.

### Step 09: Throwing an Exception	
지금까지 우리는 자바에서 기본 제공하는 메소드에서 발생하는 예외를 처리하는 방법을 살펴보았다. 이제 **예외를 발생시켜** 사용자에게 자체 코드의 예외 상황을 알리는 방법에 대해 알아보자.

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
**_콘솔창 출력_**	
_Exception in thread "main" java.lang.RuntimeException:Currencies Don't Match_	
_at com.in28minutes.exceptionhandling.ThrowingExceptionRunner.main (ThrowingExceptionRunner.java:26)_	

##### Snippet-01 Explained	
```10 USD```와 ```20 EUR```을 더한다는 것은 현실에서는 말이 되지 앟기 때문에 사용자에게 ```add()```는 서로 다른 통화에는 동작하지 않을 것이라고 말하는 것이 중요하다. 가장 직접적인 방법은 ```throw new RuntimeException("Currencies Don't Match");```코드로 예외를 두는 것이다.
이러한 예외 객체는 ```main()```안에서 처리될 수 있다. 찾아낸 예외 참조에서 ```printStackTrace()```를 호출하면 이전과 같은 디버깅 정보를 얻을 수 있다.

##### Snippet-02 : Throwing a Checked Exception	
`예외`는 Checked Exception이다. 어떤 메소드가 `Exception` 클래스의 인스턴스를 던지면 `public void add(Amount that) throws Exception` 선언이 필요하다.

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
**_콘솔창 출력_**	
**_java.lang.RuntimeException:Currencies Don't Match : USD & EUR_**	
_Exception in thread "main" java.lang.RuntimeException:Currencies Don't Match_	
_at com.in28minutes.exceptionhandling.ThrowingExceptionRunner.main (ThrowingExceptionRunner.java:26)_	

```Exception```은 ```RuntimeException```이나 그의 하위 클래스가 아니고 checked exception이다. 따라서 , 이는 던져질 때 `public void add(Amount that) throws Exception` 선언이 필요하다.	
_ 
#### 요약

이번 단계에서는
* 여러분이 작성하는 모든 메소드의 코드에서 예외를 적용할 수 있다는 것을 알게 되었다.
* 메소드에서 checked exception이 발생할 때 선언해야 한다.

### Step 10: Throwing A Custom Exception	
또한 사용자 정의 예외를 적용할 수도 있따. 기본 제공되는 예외 클래스 중 하나에서 상속해야 하는 ```클래스```만 정의하면 이러한 작업을 수행할 수 있따.
참고
* Checked exception을 서브 클래스로 두면, 상위 예외도 checked 된다.
* Unchecked exception을 서브 클래스로 두면, 상위 예외는 unchecked 된다.

##### Snippet-01 : 사용자 정의 예외	
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
**_콘솔창 출력_**	
**_com.in28minutes.exceptionhandling.CurrenciesDoNotMatchException : Currencies Don't Match : USD & EUR_**	
_Exception in thread "main" com.in28minutes.exceptionhandling.CurrenciesDoNotMatchException : Currencies Don't Match : USD & EUR_	
_at com.in28minutes.exceptionhandling.ThrowingExceptionRunner.main (ThrowingExceptionRunner.java:26)_	

##### Snippet-01 Explained
```CurrenciesDoNotMatchException``` 클래스는 분명히 checked exception이다. 따라서 checked 응용 프로그램 다루기에 적용되는 규칙도 적용된다.
그 대신 ```CurrenciesDoNotException```이 ```RuntimeException```의 하위 클래스인 경우, unchecked exception이 될 것이다. ```throws```표기를 ```add()``` 정의에 추가할 필요는 없을 것이다. 또한 ```add()```의 호출 순서에서 이를 처리할 메소드가 필요 없다.

#### 요약
이번 단계에서는
* Java에서는 사용자  예외 클래스를 정의할 수 있다.
* 사용자 정의 예외의 checked나 unchecked는 해당 예외의 하위 클래스의 예외에 따라 달라진다.
* 사용자 정의 예외를 생성하고 처리하는 방법을 보았다.

### Step 11:  ```try```-With-Resources 소개 	
```try```-with-resouces는 자원 관리를 ```try```-```catch```-```finally``` 블록으로 만든다. 예를 들어 보자.
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
```Try``` with resources 버전은 JAVA SE 7에 도입되었다. 관리할 리소스를 괄호 안에 ```try```키워드와 함께 묶는다.
이 경우, ```Scanner```은 ```Closeable``` ```인터페이스```를 구현하도록 정의되기 때문에 이러한 리소스 관리와 호환된다. 이 인터페이스는 ```추상 클래스```인 ```AutoCloseable```의 하위 클래스이다.
```Closeable extends AutoCloseable{};```	
```Scanner implements Closeable{};```	
 
```try```-with-resources를 위해서는, ```catch```나 ```finally```절이 의무적인 것은 아니다.
또한 ```scanner.close```라는 호출도 더 이상 필요하지 않다.

#### 요약	

이번 단계에서는
* ```try```-```catch```-```finally``` 블록, 즉 ```try```-with-resources를 발견했다.
* 리소스가 ```AutoCloseable``` ```인터페이스```로 구현되다면 리소스를 깨끗하게 관리하는 데 사용될 수 있을 것으로 보았다.

### Step 12: Programming Puzzle Set PP_02 	
#### Puzzle-01	
* 다음 프로그램에서 발생하는 예외를 처리하는가?

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
예외는 ```NullPointerExcepton```이다. 반면 우리가 잡으려고 하는 것은 ```CurrenciesDoNotMatchException```이다.

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
예외의 ```catch```절의 순서는 보다 구체적이지 않은 것에서 더 구체적일 필요가 있따. ```CurrenciesDoNotMatchException```은 ```Exception```의 하위 클래스이다. 따라서 오류다.

#### Puzzle-03	
* 다음 코드가 컴파일되는가? 

```java	
	try {	
	} catch (IOException | SQLException ex) {	
		ex.printStackTrace();	
	}	
```	
* **_Answer : Yes_**	

#### Puzzle-03 Explained	
이 기능은 Java SE 7에 추가되었다.

## 파일 다루기	
우리는 모든 컴퓨터에 정보가 저장되는 하드 디스크가 있다는 사실을 알고 있다. 이 정보는 **files**라는 단위로 저장된다. 쉽게 엑세스 할 수 있도록 파일들이 함께 그룹화되고, **디렉토리**로 구성된다. 운영 체제에는 **file-system**이라는 하위 시스템이 있으며, 이 하위 시스템은 디스크 상의 파일 및 디렉토리와, 시스템 및 사용자 프로그램을 연결하는 역할을 한다.
Java Runtime System은 또한 네이티브 파일 시스템과 통신하며 서비스를 사용하여 Java 프로그래메어게 파일 프로그래밍 인터페이스를 제공한다.
이 섹션에서는 플랫폼 독립적인 Java 파일 APPI를 통해 프로그래머가 기본 파일 시스템과 상호 작용할 수 있는 몇 가지 기본적인 방법에 대해 알아보자.

#### Listing Directory Contents	
Eclipse IDE 환경에서 Java 소프트웨어 프로젝트를 개발하면 프로젝트의 루트 폴더에 여러 개의 흥미로운 파일들과 하위 폴더가 포함되어 있다. 이제부터 "폴더"와 "디렉토리"라는 용어는 동일한 의미를 가지기 때문에 서로 바꾸어 사용할 수 있다.
이러한 프로젝트 폴더 중 하나의 내용을 나열하는 간단한 Java 프로그램을 작성해보자.

##### Snippet-1 : Listing Directory Contents	
```java.nio.file```시스템 패키지에는 네이티브 파일 시스템을 탐색하는 데 도움이 되는 유틸리팉 ```클래스```와 ```인터페이스```가 많이 포함되어 있다.
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
**_콘솔창 출력_**	
_./.classpath_	
_./.project_	
_./.DS_Store_	
_./bin_	
_./resources_	
_./src_	

##### Snippet-1 Explained	
Java NIO Library에서 **path name**을 나타낼 때 ```Path``` ```클래스```가 사용된다. NIO는 java SE에 도입된 "New I/O"의 약자로, 초기에는 매우 어색한 File I/O Library를 대체했다.
하지만 더 이상 새로운 것은 아니지만, 그것은 또 다른 문제다!
"```.```"는 현재 디렉토리를 의미한다.
```Paths.get()``` 메소드는 ```Files.get()```메소드가 이해하는 형식으로 지정된 디렉토리의 경로 이름을 반환한다.
```Files.get()``` 메소드는 다음과 같은 의미에서 제공되는 디렉토리의 **게으른 순회**를 수행한다.
* 이 파일에는 정기적으로 발생하는 파일이 나열된다.
*  디렉토리 파일과 충돌할 경우, 해당 파일은 반복하지 않고 목록만 표시한다.
루트 디렉토리의 내용은 경로 잉름으로 나열되고 각 경로 이름은 루트 디렉토리에 상대적이다.

##### Snippet-2 : Recursive Directory Traversal	
`File.walk(currentDirectory, 2)`에서 레벨 2를 지정할 수 있다. 따라서 레벨 2까지 폴더가 검색된다.

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
**_콘솔창 출력_**	
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
**_콘솔창 출력_**	
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
Java 파일만 필터링하기 위해 `Files.walk(currentDirectory, 4.filter(predicate)`를 사용한다. 
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
**_콘솔창 출력_**	
_./src/files/DirectoryScanRunner.java_	

##### Snippet-5 : Filtered Traversal with find()	
.java extension - `(path, attributes) -> String.valueOf(path).contains(".java")`의 경로 특성을 확인하도록 구성된 `Files.find(currentDirectory, 4, matcher)`를 사용할 수 있다.

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
**_콘솔창 출력_**	
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
**_콘솔창 출력_**	
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
**_콘솔창 출력_**	
_[123.122, asdfghjkl, Apple, Bat, Cat]_	

`Files.readAllLines(pathFileToRead)` 는 파일의 내용을 문자열 값 목록으로 쉽게 읽을 수 있게 해준다.

##### Snippet-8 : Streamed File Read	
`Files.readAllLines(pathFileToRead)`는 파일의 내용을 쉽게 읽을 수 있게 한다. 그러나 대용량 파일을 읽거나 메모리를 적게 사용해야 하는 경우에는 스트리밍이 더 좋은 선택이다.

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
**_콘솔창 출력_**	
_123.122_	
_asdfghjkl_	
_Apple_	
_Bat_	
_Cat_	
`Files.lines(pathFileToRead)` returns a stream which can be consumed as needed.

##### Snippet-9 : Printing file contents in lower-case	
`map` 함수를 사용하여 `String::toLowerCase`에 매핑할 수 있다.

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

**_콘솔창 출력_**	
_123.122_	
_asdfghjkl_	
_apple_	
_bat_	
_cat_	

##### Snippet-9 : Filtering file contents	
`filter` 메소드를 사용하여 파일 내용을 필터링할 수도 있다.	
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
**_콘솔창 출력_**	
_asdfghjkl_	
_apple_	
_bat_	
_cat_	

##### Snippet-10 : Writing to a file	
`Files.write` 는 파일을 작성할 때 사용할 수 있다.
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
## 동시 실행 : 더 나아가기	
간단한 카운터를 만들어보자.

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

아주 간단하다!

### 카운터 ```increment()```메소드는 Atomic이 아니다!

코드를 보자. 이는 겉보기에는 단지 하나의 연산만을 포함한다.

```java	
	public void increment() {	
		i++;	
	}	
```	
```i++```연산은 실제로 다음과 같은 단계를 포함한다.
- Step 1. 메모리에서 CPU 레지스터로 ```i```값을 읽어온다
- Step 2. CPU 레지스터 내의 값을 증가한다.
- Step 3. 증가된 값을 ```i```의 메모리 위치에 다시 저장한다.
```i++```는 atomic 연산이 아니다.

##### `increment`이 atomic이 아니라면?	

```ConcurrencyRunner```에서 실행되어 하나의 ```Counter```객체 인스턴스에 접속하는  ```T1```과 ```T2```, 두 개의 스레드를 예를 들어 보자.

그 스레드가 `increment`와 `getI`를 동시에 호출한다고 하자.

```i```의 초기값은 ```15```라고 가정한다. 가능한 시날이오에 대해 자세히 살펴보자.
- ```T1```은 ```increment```를 호출하고 ```i++```의 첫 단계를 성공적으로 완료한다. 15의 값을 가져온다.
- ```스케줄러가 ```T2```로 스레드 전환
- ```T2```는 ```increment()```를 먼저 호출하고 ```i++```의 첫 단계를 성공적으로 완료한다. 15의 값을 가져온다.
- 스케줄러는 ```T1```로 전환한다. ```T1```은 ```increment()```의 실행을 재개하고, ```i++```의 두 번째와 세 번째 단계를 완료한다. ```i```값이 16으로 덮어 씌워지면서 ```increment()```의 실행을 완료한다.
- 스케줄러가 ```T2```로 전환한다. CPU 레지스터의 측면에서 I는 ```16```이 아니라 ```15```이다. ```T2``는 `Increment()```의 실행을 재개하고 ```i++```의 두 번째와 세 번째 단계를 완료한다. ```increment()```의 실행을 완료한다. ```Counter``` 객체의 ```i```의 값은 ```16```으로 덮어 씌워진다.

이상적으로 두 번의 ```increment```후에 ```i```의 최종 값읜 ```17```이었어야 했다. 이 오류는 작업이 차례로 연속적으로 실행될 때 발생한다.

동시 연산(연산 순서 포함)의 결과가 관련 스레드에 의한 해당 연산의 상대적 실행 순서에 따라 달라지는 이 시나리오를 *경합 조건(race-conditions)*이라고 한다.

"컵과 입술 사이에는 많은 미끄러짐이 있다(There is many a slip, between the cup and the lip)"라는 유명한 영어 속담이 있다. 이것은 우리가 차 한잔을 손에 들고 있는 시간과 실제로 차를 한 모금 마시는 시간 사이에 어떤 일이든 일어날 수 있따는 사실을 말한다.

이것은 확실히 사실처럼 들린다.

증가 연산은 실제로 보이는 것만큼 매끄럽지 않다. 왜냐하면 그것은 atomic이 아니기 때문에, 미끄러짐이 종종 발생할 수 있다. 따라서, **Thread-Safety** 의 개념을 소개한다.

*경합 조건* 없이 (독립 스레드에 의한 여러 개의 동시 호출을 포함하는) 동시 환경에서 실행 할 수 있는 메소드는 Thread Safety하다고 한다.	

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
`synchronized`키워드를 `increment` 메소드에 추가한 후에는 한 번에 한 스레드만 메소드를 실행할 수 있게 된다. 따라서 경합 조건을 피한다.

##### Snippet-3 : less concurrency	
`synchronized` 키워드는 코드를 thread safe하게 만든다. 그러나, 다른 모든 스레드가 대기하게 한다. 이로 인해 성능 문제가 발생할 수 있다. 예를 들어 보자.

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
```BiCounter``` ```클래스```의 ```incrementI()```와 ```incrementJ()```는 ```sychronized```, 즉 동기화 되었다. 따라서, 지정된 시간에 최대 하나의 스레드가 이러한 메소드 중 하나를 실행 할 수 있다! 즉, 스레드 ```T1```이 ```CocurrencyRunner.main()```내의 ```counter.incrementI()```를 실행하는 동안에는 또 다른 스레드 ```T2```이 ```counter.incrementJ```를 실행하는 것이 *허용되지 않는다*!
```counter```를 증가시키기를 원하는 ```12```개의 스레드가 있다고 상상해보라. 한 스레드가 실행 중일 때, 나머지 ```11```개의 스레드는 대기해야 한다!

#### Synchronization With Locks	
다른 동기화 옵션인 'Locks'를 살펴보자.

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

`i++`과 `j++`은 지켜야 할 코드 조각이다. 두 개의 lockForI와 lockForJ를 사용한다. 만약 스레드가 `i++`를 실행할면, 먼저 lock을 가져와야 한다. 이는 `lockForI.lock()`을 사용하여 구현된다. 연산을 수행한 후에는 `lockForI.unlock()`으로 해제할 수 있다.
```lockForI```와 ```lockForJ```는 서로 완전히 독립적이다. 따라서  ```T1```이 ```incrementI()```에서 ```i++```을 실행하는 동시에 ```T2``` 스레드는 ```incrementJ()```에서 ```j++```을 실행할 수 있다.
	
#### Atomic Classes	

```i++``` 연산은 작아 보이지만 이는 우리에게 상당한 골칫거리였다!

겉보기에 몇 분내로 수행할 연산에 많은 걱정이 필요한 경우, 연결 리스트를 여러개의 연결 리스트로 다루는 동시 데이터 구조를 작성한다고 상상해 보라!

누군가가 우리를 위해 이 작업을 처리해줄 수 있다면 정말 좋을텐데, 그렇지 않으면 우리는 어떤 코드를 확실히 잠글지, 그리고 어떤 코드가 필요하지 않은지 알아내는데 어려움을 겪을 것이다!

Java는 기본적으로 thread safety한 몇 가지 클래스를 클래스를 제공하여 기본 데이터 타입에 대해 이 문제를 해결한다. 좋은 예가 ```int```의 기본형 타입을 감싸고 있는 ```Atomic Interger```이다.

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

`incrementAndGet`는 atomic이다. 따라서, `BiCounterWithAtomicInteger`는 동기화에 대해 걱정할 필요가 없다. 

#### 동시 컬렉션

자바는 우리에게 ```AtomicInteger```와 같은 래퍼를 사용하여 thread safety 기본형 타입을 위한 기성 솔루션을 제공했다. 이러한 접근 방식이 ```int```로 작동하는 이유는 다음과 같다.
* 간단하고 작은 기본 타입
* 광범위한 잠재적 사용

컬렉션은 어떤가?

자바에서 thread safety를 제공하는 벡터(어레이리스트의 동기화 버전)와 같은 클래스를 제공한다. 그러나 동기화 사용시 발생하는 문제 또한 상속한다.

수집품들은 어때? 	

자바에서는 나사산 안전성을 제공하는 벡터(어레이리스트의 동기식 버전)와 같은 클래스를 제공한다. 그러나 동기화 사용 시 발생하는 문제를 상속합니다. 	

다른 옵션은 무엇이 있는가?

##### Snippet-6 : Need For ConcurrentMap	

```for문```내의 코드는 `get`을 한 다음 `put`을 한다. 이는 스레드 안정하지 않다.

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


동시 실행 컬렉션은 위에서 설명한 것과 같은 연산의 atomic 버전을 제공한다.
* 엔트리가 존재하지 않는 경우 생성 및 초기화
* 엔트리가 존재하는 경우 업데이트


#### ```ConcurrentMap``` ```인터페이스```	
``인터페이스" ``커런트 맵"은 복합 운영을 구현하는 방법이 있다. 이러한 작업은 다음과 같습니다.
```ConcurrentMap``` ```인터페이스```는 복합 연산을 구현하는 메소드이다. 이러한 연산은 다음과 같다.	
```	
V putIfAbsent(K key, V value);	
V computeIfPresent(K key,	
            BiFunction<? super K, ? super V, ? extends V> remappingFunction)	
```	

##### Snippet-7 : ConcurrentHashMap Logic - Stage 1	

```LongAdder```는 atomic `increment`메소드를 제공하는데, 이 메소드는 코드를 좀 더 안전하게 만들기 위해 사용한다. 그러나 서로 다른 스레드가 ```occurrences.get()```과 ```occurrences.put()```을 병렬적으로 실행할 수 있어 경합 조건은 여전히 발생할 수 있다.


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

**_콘솔창 출력_**	

_[ =2, A=3, B=3, C=3, D=2]_	


##### Snippet-8 : ConcurrentHashMap Logic - Stage 2	

우리는 ```CocurrentHashMap``` ```컬렉션```으로부터 ```computeIfAbsent()```라는 메소드를 사용하여 코드를 단일 atomic 연산으로 줄일 수 있다.

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
**_콘솔창 _**	


_[ =2, A=3, B=3, C=3, D=2]_	



#### ```ConcurrentHashMap```	


```HashTable```에서, 모든 메스다가 동기화된다.

```ConcurrentHashMap```에서는 데이터 구조가 분리된 지역으로 구성되어 있따. 접근 메소드는 지역마다 다른 ```Locks```를 사용하므로 동시 접근 시 성능에 미치는 영향은 줄어든다.

#### 동시 실행 컬렉션 : Copy-On-Write 최적화

Copy-On-Write 컬렉션의 모든 값은 내부 불변 배열에 저장된다. 컬렉션을 수정할 경우 새 배열이 만들어진다.

읽기 작업은 동기화되지 않는다. 오직 쓰기 작업만 동기화된다.

Copy on write 접근 방식은 컬렉션에서 숫자를 쓰는 것보다 읽기가 훨씬 많은 시나리오에서 사용된다.

`CopyOnWriteArrayList` & `CopyOnWriteArraySet`은 이러한 접근 방식을 구현한 것이다.

Copy On Write 컬렉션은 일반적으로 관찰자가 거의 변경되지 않는 대상-관찰자 시나리오에서 사용된다. 가장 빈번한 작업은 관찰자 주위에서 반복하여 알리는 것이다.

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

```CopyOnWriteArrayList.add()```메소드는 ```동기화된``` 메소드이다. 그리고 copy-on-write 알고리즘을 사용하면 복사(copy)작업이 별도의 복사본에서 실행되는 반면, ```get()```은 원래의 배열에서 계속 실행되는 스레드 세이프 방식으로 실행될 수 있다. ```add()```가 완료되면, 컬렉션은 새 배열을 사용하기 시작하여 이전의 배열은 버린다. 이 전략은 프로그램 수명 동안 계속된다.

```CopyWriteArrayList.get```메소드는 ```동기화된```메소드가 아니며, 읽기가 작동하기 때문에 ```add()```를 통한 직접적인 쓰기는 없을 것이다.

Copy-On-Write 컬렉션은 변화(데이터 요소 삽입/삭제/수정)에 비해 매우 많은 수의 데이터 구조 탐색(데이터 요소 읽기 전용)과 같은 특정 사용 시나리오에서만 사용해야 한다. 이러한 방식으로, 탐색에서 높은 동시성을 보인다.
