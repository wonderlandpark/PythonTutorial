# 3강 기본 입출력 함수
이번 강의에서는 파이썬의 기본 입출력 함수에 대해 이야기해보려고 합니다.

## 입출력이란 무엇인가?
입출력이란, 말 그대로 입력과 출력이에요. 프로그래밍을 하면서, 만들어낸 프로그램이 외부로부터 데이터를 **입력** 받고, 프로그램이 외부에 데이터를 **출력** 하게 될거에요.
이 입력과 출력은 프로그램이 실행중인 콘솔에서 이루어질 수도 있고, 프로그램과 통신하는 외부 서버 사이에서 이루어질 수도 있습니다.

오늘은, 가장 기본적인 콘솔과의 입출력에 대해 배워보려고 해요.

## 콘솔이란 무엇인가?
![imaage01](01-console.png)
프로그램을 실행할 때, 검정색 배경에 흰색으로 글씨가 적혀있는 창이 나타날거에요. 이 창을 **콘솔(console)** 이라고 불러요.
우리는 이 창에 데이터를 출력할 수도 있고, 반대로 이 창에서 프로그램으로 데이터를 입력할 수도 있어요.

우선, 이 창에 데이터를 입력하는 과정부터 진행해볼게요.
파이썬에서는 콘솔에 데이터를 출력하는 가장 기본적인 함수로 **print** 를 제공해요.
이 print 함수의 괄호 안에 출력하고자 하는 데이터를 전달해, 콘솔에 데이터를 출력할 수 있어요.
[ code ]
```python
print(100)
print(True)
print("Hello World!")
print(3.14)
```
[ result ]
```
100
True
Hello World!
3.14
```
print 함수에 여러개의 데이터를 쉼표(,) 로 구분해서 입력해주면, 입력한 데이터들을 공백 한 칸(띄어쓰기)으로 구분해서 출력해줘요.
[ code ]
```python
print(100, True, "Hello!", 3.14)
```
[ result ]
```
100 True Hello! 3.14
```

앞서 2강에서 여러가지 자료형의 데이터들을 변수에 저장했었죠? 파이썬에서는 변수가 담고있는 데이터의 자료형을 반환하는 **type** 이라는 함수가 있어요.
[ code ]
```python
print(type(100))
print(type(True))
print(type("Hello World!"))
print(type(3.14))
``` 
[ result ]
```
<class 'int'>
<class 'bool'>
<class 'str'>
<class 'float'>
```

콘솔에 데이터를 출력했다면, 이제는 콘솔에서 데이터를 입력할 차례겠죠.
파이썬은 콘솔에서 데이터를 입력받는 가장 기본적인 함수로 **input**을 제공해요.
이 input 함수의 괄호 안에는 데이터 입력을 받기 전에 출력할 문자열을 전달하고, input 함수는 입력받은 데이터를 문자열로 반환해요.
[ code ]
```python
answer = input("정답을 입력해주세요! : ")
print("입력하신 정답은", answer, "입니다.")
```
[ resuit]
```
정답을 입력해주세요! : 안녕
입력하신 정답은 안녕 입니다.
```