#python\
##자료형\
###숫자형\
정수:123,-20,0\
실수:123.45,-432.5,6.08\
8진수:0o432,0o556\
16진수:0xff,0x00,0x0a
변수
문자 또는 밑줄로 시작(beta,_kim)
대소문자를 구분(sum,Sum,SUM)
영문자,숫자,밑줄(A-z,0-9,_)
파이썬 키워드는 사용불가
~~~
a=10
b=20
c=a+b
d=b-a
print(c,d)
~~~
~~~
a=10
b=3
#나눗셈
c=a/b  #나눗셈
d=a//b #몫
e=a%b #나머지
#곱셈
f=a*b #곱셈
g=a**b #제곱
print(c,d,e,f,g)
~~~
문자열
큰 따옴표 : "Hello World! It's"
작은 따옴표 : '대한민국'
큰따옴표 3 : """Hello!"""
작은 따옴표 3 : '''Life is too short, You need python'''
~~~
myName = "Seung Jun" #카멜
my_name = "이승준" #스네이크
MyName = 'jiji' #파스칼
_my_name = "korea"
MYNAME = "God is love"
my2name = "12345"
# 2myname = '9874'
# my-name = "michle"
# my name = "kiki"
myStr = '123'#Str
myNum = 123#int
print(myStr,myNum)
print(type(myStr))
print(type(myNum))
~~~
여러개 변수 할당
~~~
x,y,z = "포도","딸기","수박"
print(x)
print(y)
print(z)
~~~
~~~
a = b = c = "오렌지"
print(a)
print(b)
print(c)
~~~
~~~
fruits = ["포도","딸기","수박"]
x,y,z = fruits
print(x)
print(y)
print(z)
~~~
~~~
x = "Life"
y = "is"
z = "Beautiful"
print(x,y,z)
print(x+y+z)
~~~
~~~
a = 1
b = 2
c = 3
print(a,b,c)
print(a+b+c)
~~~
데이터유형
텍스트
숫자
불(bool)
~~~
a=100
b=200
result=a+b
print(a,'+',b,'=',result)
~~~
~~~
a=15
b=5
result=a//b
result2=a%b
print(a,'//',b,'=',result)
print(a,'%',b,'=',result2)
~~~
