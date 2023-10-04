# 1. 변수

>변수이름 `=` 값
>- 변수이름은 어떤 이름이든 상관 없음
>- 영어, 숫자, `_` 를 이용하여 선언
>- 키워드는 사용불가

1. number
- int
   - a = 100
- float 
    - a = 1.1
- complex 
    - a = 1 - 4j

2. Boolean
- True, False로 이루어진 타입

3. None
- 데이터가 없음을 의미

4. String
- 문자열은 `'`, `"`를 이용하여 표현

※ string interpolation
- %-formatting
- str.format()
- f-string

# 2. 연산자.
1. 산술연산자
- a + b
- a - b
- a * b
- a / b
- a ** b
- a // b
- a % b 

2. 비교연산자
- a > b
- a < b
- a >= b
- a <= b
- a == b
- a != b

3. 논리연산자
- and : 양쪽 모두 True 일 때, True를 변환
- or : 양쪽 모두 False 일 때, False를 반환
- not : 값을 반대로 전환

4. 복합연산자

|문법|의미|
|----|----|
|a += b | a = a + b|
|a -= b|a = a - b|
|a *= b|a = a * b|
|a /= b|a = a / b|
|a //= b|a = a // b|
|a %= b|a = a % b|
|a **= b|a = a ** b|

5. 포함연산자
- print('a' `in` 'apple')  
output> True

6. 두 변수가 동일 객체인지 체크하는 연산자(`is`)
```python
a = 10
b = 10
print(a is b)
```

※ 연산자 우선순위

![사진](./assets/Order%20of%20Poerations.png)

# 3. 형변환



