# 파이썬 코딩 도장 연습

- [github site](https://github.com/DHRyu227/python_practice.git)



## 01. 파이썬 설치

## 02. 입력/출력

### 1) Input

### 2) Output



## 03. 자료 형태

### 1) List

### 2) Dictionary

### 3) Set



## 04. 조건문

### 1) if

### 2) else

### 3) elif



## 05. 반복문

### 1) for

### 2) while

### 3) break/continue



## 06. 함수

### 1) def

### 2) Lambda Expression



## 07. 객체지향

### 1) Objective

### 2) Class

```python
class Person:
    def greeting(self):
        print('hello!')

    def hello(self):
        self.greeting()

james = Person()
james.hello()

# => hello!
```



```python
# class를 만들 때 __init__ 이 속성이다.

class Person:
    def __init__(self, name, age, address):
        self.hello = "안녕하세요"
        self.name = name
        self.age = age
        self.address = address

    def greeting(self):
        print('{0} 저는 {1} 입니다.'.format(self.hello, self.name))

maria = Person('마리아', 20, '서울시 서초구 반포동')

maria.greeting()

print('이름:', maria.name)
print('나이:', maria.age)
print('주소:', maria.address)

# 안녕하세요 저는 마리아 입니다
# 이름: 마리아
# 나이: 20
# 주소: 서울시 서초구 반포구
```

 

## 08. 이터레이터/제너레이터



## 09. 데코레이터

 