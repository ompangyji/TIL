# 변수

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

# 연산자
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

5. 포함연산자(`in`)
```python
print('a' in 'apple')  

output> True
```


6. 두 변수가 동일 객체인지 체크하는 연산자(`is`)
```python
a = 10
b = 10
print(a is b)

output> True
```

※ 연산자 우선순위

![사진](./assets/Order%20of%20Poerations.png)

# 형변환
1. 암시적 형변환

시스템이 자동으로 데이터 타입을 변환하는 것
```python
a = True
c = 1

output> 2
```

2. 명시적 형변환

int(), float(), str(), list(), tuple(), set(), dict() 등으로 가능

# 시퀀스(Sequence) 자료형
> 시퀀스는 데이터의 순서대로 나열된 자료구조.
> (순서대로 나열되어 있다는 것은 정렬된 것과는 다르다.)
> - list
> - tuple
> - range
> - string

1. List(배열)
- 선언 : 변수이름 = [value1, value2, value3]
- 접근 : 변수이름[index]

2. Tuple
- 선언 : 변수이름 = (value1, value2, value3)
- 접근 : 변수이름[index]
- List와 유사하지만 수정불가능(immutable)하다.

3. range
- range(n) : 0부터 n-1까지 범위
- range(n, m) : n부터 m-1까지 범위
- range(n, m, s) : n부터 m-1까지 범위, +s 만큼 증가하는 범위

4. string
- 기본 데이터 구조 참고

5. 시퀀스에서 사용 가능한 연산/함수
- indexing 
```python
my_list = [1, 2, 3, 4, 5]
print(my_list[1])
```
- slicing 
```python
print(my_list[1:3])
```
- in
```python
print(11 in my_list)
```
- not in
```python
print(11 not in my_list)
```
- concatenation
```python
print(my_list + [1, 2, 3, 4, 5])
```
- \*
```python
print(my_list * 3)
```

# 시퀀스데이터가 아닌 자료구조
1. set
수학에서 사용하는 집합과 동일하게 처리(중복된 값이 없음)
- 선언 : 변수이름 = {value1, value2, value3}

2. dictionary
- 선언 : 변수이름 = {key1: value1, key2: value2, key3: value3}
- 접근 : 변수이름[key]
- dictionary는 key와 value가 쌍으로 이루어져있다.
- key에는 immutable한 모든 값을 사용가능. (불변값 : string, integer... )
- value에는 모든데이터 가능. (list, dict도 가능)

※ 데이터 타입
-  Number
- Boolean
- String

※ 자료구조
- 시퀀스 자료형
    - [List] : mutable
    - (Tuple) : immutable
    - range() : immutable
    - 'String' : immutable

- 시퀀스가 아닌 자료형
    - {Set} : mutable
    - {Dict: ionary} : mutable

# 제어문
1. if, else
```python
if <조건식>:
    if의 조건식이 참인 경우 실행하는 코드
else:
    if의 조건식이 거짓인 경우 실행하는 코드
```
- `if`문은 반드시 참/거짓을 판단 할 수 있는 `조건식`과 함께 사용한다.
- `조건식`이 참인경우 : 이후의 문장을 실행한다.
- `조건식`이 거짓인 경우 `else` : 이후의 문장을 실행한다.

2. elif

```python
if <조건식>:
    if 조건이 참인 경우 실행
elif <조건식>:
    elif 조건이 참인 경우 실행
...
else:
    위의 조건식에 하나도 부합하지 않는 경우 실행
```

3. 조건표현식
- true_value if <조건식> else false_value

# 반복문

1. while 문
```python
while <조건식>:
    실행할 코드
```

2. for
정해진 범위 내의 반복

```python
for ariable in sequence:
    실행할 코드
```

3. dictionary 반복
- for key in dict:
- for key in dict.keys():
- for value in dict.values():
- for key, value in dict.items():

4. break
- 반복문을 종료시키는 키워드

5. continue
- continue 이후의 코드를 실행하지 않고 다음 반복을 실행

6. else
- else문은 끝까지 반복이 진행이 된 후 실행합니다.(break를 만나지 않은 경우)

7. pass 
```python
def login():
    pass

def logout():
    pass
```

8. match
```python
match value:
    case 조건:
        실행할 코드
    case 조건:
        실행할 코드
    case _:
        실행할 코드
```

# 함수(function)
1. 함수의 선언과 호출
- 함수의 선언
```python
def func_name(parameter1, parameter2):   
    code1
    code2
    ...
    return value
```

- 함수의 호출(실행)
```python
func_name(parameter1, parameter2)
```

2. 함수의 return
- 함수가 return을 만나면 해당 값을 반환하고 함수를 종료
- 만약 return이 없다면 None을 자동으로 반환
- return은 오직 하나의 객체만 반환한다.

3. 함수의 인수
- 위치인수
    - 기본적으로 함수는 인수의 위치로 판단합니다.

- 기본값
```python
def func(p1=v1):
    code...
    return p1
```

- 키워드 인자
    - 함수를 호출(실행)할 때 내가 원하는 위치에 직접적으로 특정인자를 전달 가능

4. 가변 인자 리스트
```python
def func(*parms):
    code
    ...
```
5. 정의되지 않은 키워드 인자 처리하기
```python
def func(**kwargs):
    code 
    ...
```
6. dictionary를 인자로 넣기(unpacking)
```python
a, b, c = {'key1': 1, 'key2': 2, 'key3': 3}
```
7. lambda 표현식
```python
lambda parameter: expression
```
8. 타입힌트
```python
def my_sum(a: int, b: int) -> int:
    return a + b
```

9. 이름공간(scope)
>python에서 사용되는 이름들은 이름공간(namespace)에 저장되어있습니다.
>- Local scope : 정의된 함수 내부
>- Enclosed scope : 상위 함수
>- Global scope : 함수 밖의 변수 혹은 import된 모듈
>- Built-in scope : python이 기본적으로 가지고 있는 함수 혹은 변수

10. 재귀(recursive)
- 재귀 함수는 함수 내부에서 자기 자신을 호출하는 함수를 의미한다.

# 문자열 메소드(객체 안에 들어있는 함수)
```python
my_list = [1, 2, 3, 4, 5]
```
- capitalize()
    - 문장의 시작을 대문자로 바꿈
- title()
    - 단어의 시작을 대문자로 바꿈
- upper()
    - 전체 대문자로 바꿈
- lower()
    - 전체 소문자로 바꿈;ㅔ
- '?'.join()
    - 문자열 리스트 중간을 문자(?)로 대체해서 합쳐줌 
- .strip([chars])
    - 좌우에서 문자열을 삭제
    - .lstrip() : 왼쪽
    - .rstrip() : 오른쪽 
- .replace(old, new[, count])
    - old를 new로 변경
    - count만큼 변경한다.
- .find()
    - 문자열에서 찾고 싶은 문자의 index를 반환
    - 없다면 -1을 반환
- .index()
    - 문자열에서 찾고 싶은 문자의 index를 반환
    - 없으면 find랑 다르게 에러발생
- .split()
    - 문자를 기준으로 자른다.
- .count()
    - 문자열에서 특정 문자의 개수를 반환한다.

# 리스트 메소드
- .append(x)
    - 리스트에 x요소 추가
- .extend(iterable)
    - 리스트랑 리스트 합침
- .inster(idx, x)
    - idx위치에 x요소 추가
- .remove(x)
    - x요소를 리스트에서 삭제
- .pop(idx)
    - numbers.pop() : 마지막 요소 추출, numbers를 호출해보면 마지막 요소가 삭제됨
    - numbers.pop(0) : 0번째 index 요소 추출
- .sort()
    - 정렬
    - numbers.sort(reverse=True) : 역정렬
- .reverse()
    - 반대로 나열

# list copy
```python
a = [1, 2, 3]
b = a[:]

import copy
a = [1, 2, [99, 100]]
b = copy.deepcopy(a)
```

# list comprehension
```python
#for
result = []

for number in numbers:
    result.append(number ** 3)
    
print(result)
#comprehension
result2 = [number **3 for number in numbers]
print(result2)
```

# 딕셔너리 메소드
```python
info = {
    'name' : 'ompang',
    'location' : 'seoul',
}
```
- .pop(key[, default])
    - key에 해당하는 {key : value}가 삭제
- .update(key=value)
    - {key : value} 추가
- .get(key[, default])
    - key에 해당하는 value 추출

# dict comprehension
```python
#for
# {1 :1, 2: 8, 3: 9, ...}
result  = {}
numbers = range(1, 11)
for number in numbers:
    result[number] = number ** 3
print(result)

#comp
result = {number: number **3 for number in range(1, 11)}
print(result)
```

# 세트 메소드
```python
fruits = {'apple', 'anna', 'melon'}
```
- .add(x)
    - 순서와 상관없이 요소
- .update(x)
    - 조각내서 각 요소를 추가
    - .update({'apple', 'orange'}) : 단어로 추가
- .remove(x)
    - 요소 삭제
- .pop()
    - 요소 삭제
