# python
## 자료형
### 숫자형
정수:123,-20,0\
실수:123.45,-432.5,6.08\
8진수:0o432,0o556\
16진수:0xff,0x00,0x0a
### 변수  
문자 또는 밑줄로 시작(beta,_kim)\
대소문자를 구분(sum,Sum,SUM)\
영문자,숫자,밑줄(A-z,0-9,_)\
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
### 문자열
큰 따옴표 : "Hello World! It's"\
작은 따옴표 : '대한민국'\
큰따옴표 3 : """Hello!"""\
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
### 여러개 변수 할당
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
### 데이터유형
텍스트\
숫자\
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
## input()함수이용한계산기
~~~
a=int(input("첫번째 숫자를 입력해주세요:"))
b=int(input("두번째 숫자를 입력해주세요:"))
result=a+b
print(a,'+',b,'=',result)
result=a-b
print(a,'-',b,'=',result)
result=a*b
print(a,'*',b,'=',result)
result=a/b
print(a,'/',b,'=',result)
~~~
~~~
a=int(input("첫번째 숫자를 입력해주세요:"))
b=int(input("두번째 숫자를 입력해주세요:"))
#제곱
result=a**b
print(a,'**',b,'=',result)
#몫
result=a//b
print(a,'//',b,'=',result)
#나머지
result=a%b
print(a,'%',b,'=',result)
~~~
~~~
num1=input("숫자입력1:")
num2=input("숫자입력2:")
result=num1+num2
print(num1,"+",num2,"=",result)
~~~
~~~
a=int(input("전화번호를입력하세요:"))
b=input("이름을입력하세요:")
c=int(input("무게를입력하세요:"))

result=c*10
print(a,"전화번호",b,"이름",c,"무게입니다")
print(c,"*10원",result)
~~~
# 2. print() 서식 출력
~~~
print("%d" % 123)
print("%5d" % 123)
print("%05d"% 123)

print("%f" % 123.45)
print("%7.1f" % 123.45)
print("%7.3f" % 123.45)

print("%s" % "대한민국")
print("%8s" % "대한민국")
~~~
# Format 함수: 순서 지정 가능
~~~
print("{0:d} {1:5d} {2:05d}".format(123,456,789))
print("{2:d} {1:5d} {0:05d}".format(123,456,789))
~~~
# 서식 출력
~~~
print("\n줄바꿈\n연습중입니다.")
~~~
~~~
print("\t탭키\t연습.")
~~~
~~~
print("글자가 \"강조\"되는 효과1")
print("글자가 \'강조\'되는 효과2")
print("역슬레시 3개출력 \\\\\\")
print(r"\n \t \"\\ \'@를 그대로 출력") #그대로 출력됨.
~~~
# 관계 연산자
~~~
a, b = 10, 20
print(a==b, a!=b, a>b, a<b, a>=b, a<=b)
~~~
# 논리 연산자
~~~
a = 99
print((a>100) and (a<200))
print((a>100) or (a<200))
print(not(a==100))
~~~
~~~
if(123):
  print("참이면 보입니다.")
if(0):
  print("거짓이면 안 보입니다.")
~~~
# 숫자 입력 동전 교환 프로그램
   ( 500원, 100원, 50원, 10원 )
~~~
bill, c500, c100, c50, c10 = 0,0,0,0,0
bill = int(input("숫자를 입력해주세요.:"))
c500 = bill // 500 
bill %= 500
c100 = bill // 100
bill %= 100
c50 = bill // 50
bill %= 50
c10 = bill // 10
bill %= 10

print("500원짜리 : %d개"%c500)
print("100원짜리 : %d개"%c100)
print("50원짜리 : %d개"%c50)
print("10원짜리 : %d개"%c10)
~~~
# 조건문
~~~
a = 10
if(a<100):
  print("100보다 작음")
  print("거짓이면 이문장은 보이지 않음")
  print("프로그램 끝")
~~~
~~~
a = 100
if(a<100):
  print("100보다 작음")
else :  
  print("100보다 큼")
  print("프로그램 끝")
~~~
~~~
a = int(input("정수를 입력하세요.:"))
if(a%2==0):
  print("짝수입니다.")
else:
  print("홀수입니다.")
~~~
~~~
a=50
if(a>50):
  if(a<100):
    print("50<a<100")
  else:
    print("a>100")
else:
    print("a<50")
~~~
~~~
fruit = ['사과','배','감','포도']
fruit.append('딸기')
if '딸기' in fruit:        #if '딸기' not in fruit:
  print("딸기가 있습니다.")  # print("딸기가 없습니다.")
print(fruit)
~~~
~~~
import random

number = []
for num in range (0,6) :
  number.append(random.randrange(1,46))
print("생성된 리스트",number)
~~~
# 반복문
~~~
for i in range(0,3,1):#시작값,끝값+1
  print("안녕하세요.")   #print("%d 안녕하세요."%i)
                         #print(i)
print("반갑습니다.")
~~~
~~~
for i in range(1,9,1):
  print("%d " %i, end = "")
print("\n")
for i in range(1,9,1):
  print("%d" %i, end = " ")
~~~
~~~
sum=0
for i in range(1,11,1):
  sum = sum + i
print("1~10까지 합계 :%d" %sum)
~~~
# 숫자입력 1부터 입력된 수까지의 합 출력 프로그램
~~~
sum,a=0,0
a=int(input("숫자를 입력하세요:"))
for i in range(1,a+1,1):
  sum=sum+i
print("1~a까지의 합계:%d"%sum)
~~~
#중첩  for문
~~~
i,j,k=0,0,0
k = int(input("단수를 입력하세요.:"))
for i in range(1,10,1):
  print("%d * %d = %2d"%(k,i,k*i))
  print(" ")
~~~
~~~
i,j,k=0,0,0
for i in range(2,10,1):
  for j in range(1,10,1):
    print("%d*%d =%2d"%(i,j,i*j))
    print("")
~~~
## 2,3,4,5단 줄바꿔서 출력
~~~
i,j,=0,0
for i in range(2,3,1):
  for j in range(1,10,1):
    print("%d*%d =%2d" %(i,j,i*j))
    print("")
print("\t")
i,j,=0,0
for i in range(3,4,1):
  for j in range(1,10,1):
    print("%d*%d =%2d" %(i,j,i*j))
    print("")
print("\t")
i,j,=0,0
for i in range(4,5,1):
  for j in range(1,10,1):
    print("%d*%d =%2d" %(i,j,i*j))
    print("")
print("\t")
i,j,=0,0
for i in range(5,6,1):
  for j in range(1,10,1):
    print("%d*%d =%2d" %(i,j,i*j))
    print("")
~~~
# 3. 자료형
## 1) 인덱스와 슬라이딩
~~~
L = [0, 1, 2, 3, 4, 5, 6, 7, 8 , 9]
print(L[1])
~~~
~~~
L = [0, 1, 2, 3, 4, 5, 6, 7, 8 , 9]
print(L[-1])
~~~
~~~
L = [0, 1, 2, 3, 4, 5, 6, 7, 8 , 9]
print(L[0:9:2])
~~~
~~~
L = [0, 1, 2, 3, 4, 5, 6, 7, 8 , 9]
print(len(L))
print(L[len(L)-1])
~~~
~~~
L = [0, 1, 2, 3, 4, 5, 6, 7, 8 , 9]
L[0] = 99
L[9] = '가나다'
L[1]=[1,2,3]
print(L)
print(L[9])
~~~
~~~
a = [1, 2, 3]
b = [4, 5, 6]
c = a+b
print(a+b)
print(c)
print(a*3)
~~~
~~~
L = [1,2 ,3 ,4 ,5]
print(L)
L. append(6) #리스트 뒤 추가
print(L)
L. remove(3) #해당 요소값 삭제
print(L)
~~~
