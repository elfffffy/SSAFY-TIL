# 🤓 Preview
1. 프로그래밍
2. python
3. 변수
4. 데이터 타입

# 🖥️ 프로그래밍

### 프로그램

문제를 해결하기 위한 명령어들의 집합

### 프로그래밍

명령어 묶음을 만드는 과정

### 프로그래밍 언어

컴퓨터에게 작업을 지시하고 문제를 해결하는 도구

# 🐍 Python

## Python을 배우는 이유

1. 쉽고 간결한 문법
2. 강력한 커뮤니티 지원
3. 광범위한 응용 분야
4. 전세계적으로 많이 사용되는 언어 (JavaScript > Python)
5. 프로그래밍과 **인공지능**에서 기본 언어로 가장 많이 사용되는 언어

## Python 프로그램 실행 과정

프로그램 - **인터프리터** - 운영체제

인터프리터가 사용자의 명령어를 운영체제가 이해하는 언어로 바꾼다.

### shell

터미널을 켜고 `python -i` 를 입력하면 파이썬 인터프리터 환경이 실행된다.

### 확장자가 .py인 파일

```bash
$ python 파일명.py
```


## 표현식과 값

하나의 값으로 **평가**될 수 있는 모든 코드

*평가 : 표현식을 계산하여 그 결과인 값을 만들어내는 과정

`3 + 5` 는 **표현식**이지만, 그 자체로 값은 아니며, **평가**를 거쳐야 **값** `8`이 된다.


# 🪣 변수

값을 **나중에 다시 사용하기 위해**, 그 값에 붙여주는 고유한 이름

### 변수 할당 `=`

표현식이 만들어 낸 값에 이름을 붙이는 과정

```python
# 값 36.5을 변수 degrees에 할당
degrees = 36.5 
```

### 재할당

이미 값이 할당된 변수에 새로운 값을 다시 할당하는 것

```python
# 값 "hello"를 변수 degrees에 재할당
degrees = "hello"
```

### 변수명 규칙

사람이 데이터를 쉽게 다루기 위해 만드는 인간 친화적인 이름

1. 영문 알파벳, 언더스코어, 숫자로 구성
2. 숫자로 시작할 수 없다.
3. 대소문자를 구분한다.
4. 파이썬의 내부 예약어를 사용할 수 없다.

## 메모리

컴퓨터가 특정 데이터 값을 정확히 찾아가기 위해 사용하는 기계적인 숫자 주소

구성 요소 :

- 고유한 ID = 메모리 주소
- 타입
- 값

값 + 타입 + 주소 정보를 묶은 것을 **객체**라고 부른다.

> 💡 **객체**
>
> 값, 타입, 그리고 관련된 행동까지 하나로 묶인 개념

</aside>

⭐ 변수는 특정 **객체를 가리키는 것(point to)**이지 가지지(contain) 않는다.

# 🎁 Data Types

### 타입

변수나 값이 가질 수 있는 데이터의 종류를 의미한다.


### 데이터 타입

값의 종류와 그 값으로 할 수 있는 동작을 결정하는 속성

## ✅ 숫자형 데이터 numeric types

### **정수형 int**

소수점이 없는 숫자를 표현한다.

```python
student_count = 30
temperature = -5
balance = 0
```

### **실수형 float**

소수점이 있는 정밀한 숫자를 표현한다.

```python
pi = 3.14
weight = 65.5
tax_rate = 0.1
```

### **지수 표현법 e, E**

아주 크거나 아주 작은 실수를 간결하게 표현하기 위해 사용하는 방식

```python
# 1,230,000,000 (1.23 * 10^9)
big_number = 1.23e9
# 0.00314 (3.14 * 10^-3)
small_number = 3.14e-3
```

### 산술 연산자

⭐ 우선순위:  `**` > `-` > `*`, `/`, `//`, `%` > `+`, `-` 



## ✅ 시퀀스 타입 sequence types

여러 개의 값들을 **순서**대로 **나열**하여 저장하는 자료

### 공통 특징

순서 / 인덱싱 / 슬라이싱 / 길이 / 반복

### 문자열 str

문자들의 **순서가 있는** **변경 불가능한** 시퀀스 자료형

```python
print('Hello, World!')
```

### 이스케이프 시퀀스

역슬래시(\)와 문자를 조합해 특별한 기능을 수행한다.

```python
# 따옴표 앞에 \를 붙여 문자로 인식시킴
print('He\'s a boy.')
# \n 은 줄바꿈(엔터)을 의미함
print('첫째 줄\n둘째 줄')
```

### ⭐ f-string

문자열 내에 변수나 표현식의 결과를 손쉽게 삽입하는 강력한 방법

```python
name = '홍길동'
age = 25
greeting = f'안녕하세요, 제 이름은 {name}이고 나이는 {age}살입니다.'
```

### 인덱스

시퀀스 자료형에서 각 값의 위치를 식별하기 위해 부여된 고유한 번호

인덱스는 **0부터 시작**한다. (시작점으로부터 얼마나 떨어져 있는가)

> 💡 **음수 인덱스 지원**
>
> 시퀀스의 끝에서부터 값에 접근할 수 있다.

```python
word = "hello"
word[0] # h
word[-1] # o
```

</aside>

### 슬라이싱

시퀀스의 일부분을 잘라내어 새로운 시퀀스를 만드는 작업

```python
word = "hello"
word[2:4] # ll
word[:3] # hel
word[::2] # hlo
word[::-1] # olleh
```


# 🔦 참고

### python tutor

[Online Python compiler with AI assistants](https://pythontutor.com/python-compiler.html#mode=edit)


# 🎩 추가 설명

### print (python 내장 함수)

`sep` :  공백(default)

`end` : 줄바꿈(default)

```python
print('Hello', end=' ')
print('World')
```

```
Hello World

```

```python
print('Hello', 'World')
```

```
Hello World
```

### 대소문자

서로 다른 유니코드 값을 가지고 있다.

```python
print(ord('A'))
print(ord('a'))
```

```
65
97
```

### 지수 표현식을 활용한 1억

```python
number = 1e8
print(number) #100000000.0
```

### 공백

```python
print(ord(' ')) #32
```

### f-string 소수점 표현

`:.nf` : 소수 n자리까지 반올림

```python
height = 185.76
print(f'키: {height:.1f}') # 키: 185.8cm
```

### 슬라이싱

> **char[start:end:step]**
> 
step이 양수일 때 : start 부터 end - 1 까지

step이 음수일 때: start 부터 end + 1 까지

▶️ **핵심은 항상 end를  포함하지 않는다.**


### 포맷팅

```python
sum = 3.14

#1. 포맷팅
print("%.1f" % sum)

#2. .format() 메서드
print("{:.1f}" %sum)

#3. f-string
print(f'{sum:.1f}')
```

### 단축키

`ctrl` + `/` : 주석

`ctrl` + ``` : 터미널 열고 닫기

`ctrl` + `b` : 사이드바 열고 닫기

`ctrl` + `a` : 전체 블록 지정

`ctrl` + `w` : 창 닫기 

`shift` + `tab` : 들여쓰기 취소 

`home`, `end` 키 

`ctrl` + `,` :  settings 

`ctrl` + `shift` + `f` : 전체 파일에서 찾기 

`ctrl` + `h` : 바꾸기  

`alt` + `shift` + 방향키 : 한 줄 복사 붙여 넣기

`ctrl` + `alt` + 방향키 : 커서 여러 개

`alt` + 마우스 좌클릭 : 커서 여러 개