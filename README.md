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
~~~
k = ['a', 'b', 'c', 'd']
k. remove('d')
print(k)
~~~
~~~
k = "God is love"
print(k[:3])
print(k[6:])
print(k[-7:-2])
~~~
~~~
k = " God is love "
print(k.upper())
print(k.lower())
print(k.strip())
~~~
~~~
a = " God, is, love "
print(a. split(","))
~~~
~~~
a = ["apple", "banana", "cherry"]
a. append ("orange") #맨뒤 추가
print(a)
~~~
~~~
a = ["apple", "banana", "cherry"]
a. insert(1, "orage") #지정된 곳 삽입
print(a)
~~~
~~~
a = ["apple", "banana", "cherry"]
a. remove("banana")
print(a)
~~~
~~~
a = ["apple", "banana", "cherry"]
a. pop(0) #지정된 곳 제거
print(a)
~~~
~~~
a = ["apple", "banana", "cherry"]
a. pop() # 맨뒤 제거
print(a)
~~~
~~~
a = ["apple", "banana", "cherry"]
del a[0]
print(a)
~~~
~~~
a = ["apple", "banana", "cherry"]
a. clear() # 목록 전체 제거
print(a)
~~~
~~~
a = ["apple", "banana", "cherry"]
for x in a: # a안의 인덱스 값 정렬
  print(x)
~~~
~~~
a = ["apple", "banana", "cherry"]
for i in range (len(a)): # a안의 랭스 정렬
  print(a)
~~~
### SORT
~~~
a = [1, 3, 5, 7, 9, 0, 1, 6]
a. sort() # 순서 정렬
print(a)
a. sort(reverse=True) # 역순서 정렬
print(a)
~~~
~~~
a = ["apple", "Banana", "durian", "cherry", "Orange"]
a. sort() # 대소문자 구분 정렬
print(a)
a.sort(key=str.lower) # 대소문자 구분 x
print(a)
a. reverse() # 역순서 정렬
print(a)
~~~
~~~
a = ["apple", "Banana", "durian", "cherry", "Orange"]
mylist = a.copy() # 복사 붙이기
print(mylist)
cplist = list (a) # 복사 붙이기(함수)
print(cplist)
~~~
### Tuple
~~~
l = [1, 2, 3] # list → 대괄호
t = (1, 2, 3) # tuple → 소괄호
l[0] = 5 # 변경 가능
print(l) 
t[0] = 1 # 변경 불가능 / 프로그램 돌릴시 에러 
print(t)
~~~
~~~
a = ["apple", "Banana", "durian", "cherry", "Orange"]
print(len(a))
~~~
~~~
t = ("apple",) # tuple → 랭스안에 , 참조
print(t)
l = ("banana")
print(l)
print(type(t), type(l))
~~~
~~~
a = ("apple", "Banana", "durian", "cherry", "Orange")
print(a[:4])
print(a[3:])
~~~
~~~
a = ("apple", "Banana", "durian", "cherry", "Orange")
if "apple" in t:
  print("Yap, 'apple' is coming")
~~~
### list ↔ Tuple
~~~
firm = ['Messi', 'Suarez', 'Naymar']
tdata = tuple(firm) # list ↔ tuple 변환 함수
print(tdata)
print(firm)
~~~
~~~
# 시험 출제 up up up up up up up
t = ('Messi', 'Suarez', 'Naymar', 'XAVI', 'Inesta', 'Busquets')
l = list(t)
l. append("Puyol")
t = tuple(l)
print(t)
~~~
~~~
t = ('Messi', 'Suarez', 'Naymar', 'XAVI', 'Inesta', 'Busquets')
q = ("Puyol",)
t += q
print(t)
~~~
~~~
t = ('Messi', 'Suarez', 'Naymar', 'XAVI', 'Inesta', 'Busquets')
q = list(t)
q.remove('Busquets')
t = tuple(q)
print(t)
del (t) # 제거 가능
~~~
### dict (사전자료)
~~~
d = {
    'a':1,
     'b':2,
     'c':3
}
print(d)
print(d.keys()) # 서식 지정
print(d.values()) # 값 지정
print(d.items()) # 서식, 값 지정
~~~
~~~
# 항목 추가
soccer = {
    "player":"Messi",
    "position":"foward",
    "team":"BARCELONA"
}
print(soccer)
print(len(soccer))
soccer["position"] = "midfilder" # 추가시 대괄호 사용
print(soccer)
soccer["team"]="pari saint german"
print(soccer)
soccer. update({"old":38}) # update 함수 사용 추가
print(soccer)
~~~
~~~
# 항목 제거
soccer = {
    "player":"Messi",
    "position":"foward",
    "team":"BARCELONA"
}
soccer.pop("team")
print(soccer)
~~~
~~~
soccer = {
    "player":"Messi",
    "position":"foward",
    "team":"BARCELONA"
}
soccer.popitem()
print(soccer)
~~~
~~~
soccer = {
    "player":"Messi",
    "position":"foward",
    "team":"BARCELONA"
}
soccer.clear() # 비움
del soccer
~~~
~~~
soccer = {
    "player":"Messi",
    "position":"foward",
    "team":"BARCELONA"
}
for x in soccer: # 값 출력
  print(soccer[x])
~~~
~~~
soccer = {
    "player":"Messi",
    "position":"foward",
    "team":"BARCELONA"
}
for x in soccer. values(): # 값
  print(x)
for x in soccer. keys():  # 서식
  print(x)
~~~
~~~
soccer = {
    "player":"Messi",
    "position":"foward",
    "team":"BARCELONA"
}
for x, y in soccer. items(): # 서식, 값 동시 출력 함수
  print(x, y)
~~~
~~~
soccer = {
    "player":"Messi",
    "position":"foward",
    "team":"BARCELONA"
}
myplayer = soccer.copy()
print(myplayer)
myplayer = dict(soccer)
print(myplayer)
~~~
~~~
name1 = {"name":"Messi", "team":"BARCELONA", "live":"ARGENTINA"}
name2 = {"name":"Naymar", "team":"BARCELONA", "live":"BRAZIL"}
name3 = {"name":"Suarez", "team":"BARCELONA", "live":"ARUGUI"}
family = {
    "name1":name1,
    "name2":name2,
    "name3":name3
}
print(family)
~~~
# 4. 조건문, 반복문
## 중첩 if문
~~~
score = int( input("점수를 입력해 주세요: "))

if(score > 100):
  print("0~100까지의 수를 입력하셔요") 
else:
  if(score >= 90):
    print("A")
  elif(score >= 80):
    print("B")
  elif(score >= 70):
    print("C")
  elif(score >=60):
    print("D")
  else:
    print("F")
  print ("학점입니다.")
  ~~~
  ~~~
  score = int( input("점수를 입력해 주세요: "))

if(score > 100):
  print("0~100까지의 수를 입력하셔요") 
else:
  if(score >= 90):
    print("점수: %3d A" %score)
  elif(score >= 80):
    print("점수: %3d B" %score)
  elif(score >= 70):
    print("점수: %3d C" %score)
  elif(score >=60):
    print("점수: %3d D" %score)
  else:
    print("점수: %3d F" %score)
  print ("학점입니다.")
  # print ("학점, 점수: %3d" %score)
  ~~~
  ~~~
  import random
numbers = []
for num in range(0,10):
  numbers.append(random.randrange(0,10))
print("생성된 리스트", numbers)
for num in range(0,10):
  if num not in numbers:
  #if num in numbers:
   # print("숫자 %d는 리스트에 있습니다."%num)
    print("숫지 %d는 리스트에 없습니다."%num)
  else:
    print("숫자 %d는 리스트에 있습니다."%num)
 ~~~
 ~~~
 select, answer, numStr, num1, num2 = 0,0,"",0,0
select = int(input("1.입력한 수식 계산 2. 두수의 합계:"))
if select == 1:
  numStr = input("★★★ 수식을 입력하세요 :")
  answer = eval(numStr) # 1+2, "string"+"Str"
  print("%s 결과는 %5.1f입니다."%(numStr,answer))
elif select == 2:
  num1= int(input("★★★ 첫번쨰 숫자를 입력하세요:"))
  num2= int(input("★★★ 두번쨰 숫자를 입력하세요:"))
  for i in range(num1,num2+1):
    answer = answer+i
  print("%d+...+%d는 %d입니다."%(num1,num2,answer))
else:
  print("1또는 2만 입력해야 합니다.")
~~~
## for,while 반복문
~~~
for i in range (0,3,1):
  print("안녕!")
  # type error
#for i in range [0,3,1]: 
  #print("안녕!")
~~~
~~~
for i in range(0,3,1):
  for j in range(0,2,1):
    print("i:%d, j:%d"%(i,j))
~~~
~~~
i,j= 0,0
for i in range(2,10,1):
  for j in range(1,10,1):
    print(" %d x %d =%2d " %(i,j,i*j), end="")
  print("")
~~~
~~~
i = 0
while i < 3:
  print("%d : while문"%i)
  i = i+1
~~~
1~10 까지의 합계 구하기 while문, for문
~~~
i,hap = 0,0
i = 1
while i < 11:
  i = i + 1
  hap = hap + i
print("1~10까지의 합계: %d"%hap)
~~~
~~~
i, hap = 0,0
i = 1
for i in range(1,11,1):
  hap = hap + i
print("1~10까지의 합계: %d"%hap)
~~~
~~~
# while True:
print("무한루프", end='')
~~~
~~~
# break
for i in range(1,100):
  print("for문 %d번 실행"%i)
  break
  print("break 빠짐")
~~~
~~~
hap = 0
a,b =0,0
while True:
  a = int(input("덧셈 첫번째 수 입력:"))
  if a == 0:
    break
  b = int(input("덧셈 두번째 수 입력: "))
  if a+b:
    print("%d + %d = %d"%(a, b, hap))
print("break로 탈출")
~~~
~~~
# continue
hap, i = 0,0
for i in range(1,10):
  if i %2 == 0:
    print("i:%d"%i)
    continue
  hap += i
print("1~10까지의 합계(2의 배수 제외):%d"%hap)
~~~
~~~
fruits = ["사과","배","체리"]
for x in fruits:
  if x == "배":
    continue
  print(x)
~~~
~~~
for x in range(5):
  print(x)
else:
  print("끝")
~~~
~~~
for x in range(5):
  if x == 3:
    break
  print(x)
else:
  print("끝")
~~~
~~~
# for문 형식은 비워두기 불가능.
for x in [0,1,2]:
  pass
~~~
### 함수
~~~
# 더하기 함수
def plus (v1, v2):
  result = 0
  result = v1 + v2
  return result

hap = 0
hap = plus(10,20)
print("10+20 plus() 처리 결과: %d" %hap)
~~~
~~~
# 계산 코드
def calc (v2,v1,op):
  result = 0
  if op == '+':
    result = v1 + v2
  elif op == '-':
    result = v1 - v2
  elif op == '*':
    result = v1 * v2
  elif op == '/':
    result = v1 / v2
  return result

rst = 0
var1,var2,opr = 0,0,""
opr = input("계산코드 입력: ")
var1 = int(input("첫번째 수 입력: "))
var2 = int(input("두번째 수 입력: "))
rst = calc(var1,var2,opr)
print("계산기 %d %s %d : %d "%(var1,opr,var2,rst))
~~~
# 0 나누기= 메시지 출력
# 제곱 연산 추가
# 숫자1,숫자2,연산자 계산기 만들기
~~~
def calc (v2,v1,op):
  result = 0
  if op == '+':
    result = v1 + v2
  elif op == '-':
    result = v1 - v2
  elif op == '*':
    result = v1 * v2
  elif op == '/':
    result = v1 / v2
  elif op == '**':
    result = v1 ** v2
  return result

rst = 0
var1,var2,opr = 0,0,""
opr = input("계산코드 입력: ")
var1 = int(input("첫번째 수 입력: "))
var2 = int(input("두번째 수 입력: "))
rst = calc(var1,var2,opr)
print("계산기 %d %s %d : %d "%(var1,opr,var2,rst))
~~~
~~~
def func1():
  a = 10            # 지역변수
  print("func1()에서 값 : %d"%a)
def func2():
  print("func2()에서 a값: %d"%a)
a = 20              # 전역변수
func1()
func2()
~~~
# 5. 파일 처리
"r" = read  
"a" = append  
"w" = write  
"x" = create  
"t" = text  
"b" = binary  
~~~
# w
from google.colab import files  # 파일 다운로드

f = open("a.txt",'w')
f.write("12345")
f.close()

f = open("a.txt",'w')
f.write("abcde")
f.close()

files.download('a.txt')         # 파일 다운로드
~~~
~~~
from google.colab import files  # 파일 다운로드

f = open("a.txt",'w')
f.write("12345")
f.close()

f = open("a.txt",'a')       # 추가
f.write("6789")
f.close()

files.download('a.txt')         # 파일 다운로드
~~~
~~~
from google.colab import files  # 파일 다운로드

f = open("b.txt",'x')         # 생성 파일 존재x → 정상작동
                                  # 새로운 파일시 정상작동
f.write("abcde")
f.close()

files.download('b.txt')         # 파일 다운로드
~~~
~~~
# 여러줄 내용 입력
from google.colab import files  # 파일 다운로드

f = open("a.txt",'w')
f.write("""1234
4567
890""")       # \n 역할 = """a b c"""
#f.write("123456789\n987654321\nabcde\nedcba")
f.close()

files.download('a.txt')         # 파일 다운로드
~~~
~~~
# 리스트, 튜플 내용 입력
from google.colab import files  # 파일 다운로드

t = ("1","2","3","4","5","\n")
i = ["a","b","c","d","e"]
f = open("a.txt",'w')
f.writelines(t)
f.writelines(i)
f.close

files.download('a.txt')         # 파일 다운로드
~~~
~~~
# read 모드로 파일 열기
from google.colab import files  # 파일 다운로드

f = open("a.txt",'w')
f.write("1234")
f.close()

f = open("a.txt",'r')
print(f.read())
f.close()

files.download('a.txt')         # 파일 다운로드
~~~
~~~
# readlines() 함수 = 한줄씩 가져옴
f = open("a.txt",'w')
f.write("1234\nabcd")
f.close()

f = open("a.txt",'r')
print(f.readline())
print(f.readline())
f.close()
~~~
~~~
from google.colab import files  # 파일 다운로드

import os
if os.path.exists("a.txt"):
  os.remove("a.txt") # 파일지움
# os.rmdir("a.txt")
  # os.rmdir("a.txt") 폴더 지움
else:
  print("파일이 없음")
~~~
~~~
from google.colab import files  # 파일 다운로드
import os
print(os.listdir('.'))
os.rename("b.txt","a.txt")
print(os.listdir('.'))
~~~
~~~
from google.colab import files  # 파일 다운로드
import os
print(os.path.exists('a.txt'))  # a.txt 파일 유무
print(os.path.exists('b.txt'))  # b. txt 파일 유무
~~~
~~~
# 구구단 파일로 저장
from google.colab import files  # 파일 다운로드
import sys
f = open("a.txt",'w')
sys.stdout = f
for i in range(2,10):
  for j in range(1,10):
    print("{} x {} = {}".format(i, j, i*j))
  print()
f.close()
~~~
~~~
f = open("c.txt",'w',encoding='utf8')
f.write("동해물과 백두산이 마르고 닳도록\n안녕하세요.\nHELLO WORLD")
f.close()

f.open("c.txt",'r',encoding='utf8')
lines = f.readlines()
for line in lines:
  print(line, end='')
f.close()
~~~
~~~
y = int(input("줄 수 입력하세요."))
x = int(y/2)+1

for i in range(1,2*x):
  if(i <= x):
    for j in range(x-i):
      print("",end='')
    for j in range(2*i-1):
      print("@",end='')
    for j in range(i-x):
      print("",end='')
    for j in range((2*x-i)*2-1):
      print("@", end='')
    print()
~~~
~~~
for i in range(5):
  print('@', end='')
print("")

for i in range(i+1):
  print('@', end='')
print("")
~~~
~~~
x = int(input("줄수 입력:"))
for i in range(1,x+1):
  for j in range(i):
    print("@",end='')
  print()

def starw(i):
  if i == 6:
    return
  print("@"*i)
  i = i+1
  starw(i)
starw(1)
~~~
~~~
def add(a,b):
  print("a+b")        # 정상 작동
x=add(10,20)
print(x)              # none

def addr(a,b):
  return a+b
y=addr(10,20)
print(y)              # 정상 작동
~~~
~~~
from tkinter import *
window = Tk()
window.title("윈도우 창 연습")     # 제목 정의
window.geometry("400x400")         # 사이즈 정의
window.resizable(width=FALSE, height=FALSE) # 마우스 지정 X
window.resizable(width=TRUE, height=TRUE) # 마우스 지정 O
window.mainloop()
~~~
~~~
from tkinter import*
window = Tk()
Label1 = Label(window,text="안녕하세요")
Label2 = Label(window,text="파이썬", front=("궁서체",10),fg = "blue")
Label3 = Label(window,text="Love is ",bg="red",width=10, height=5, anchor=2)
Label1.pack()
Label2.pack()
Label3,pack()

window.mainloop()
~~~
~~~
# 사진 올리기
from tkinter import*
window = Tk()
photo = photoImage(file=파일저장위치)   # 사진 저장 퍼오기
Label1 = Label(window,image=photo)   # 사진
Label.pack(side=LEFT) #좌우 배치
Label.pack(side=RIGHT) # 좌우 배치
window.mainloop()
~~~
~~~
 # 버튼 만들기
from tkinter import*
window = Tk()
button1 = button(tk, text = "파이썬 종료", fg = "red", command = quit) 
button1.pack()
tk.mainloop()
~~~
~~~
# 버튼과 사진 동시 만들기
from tkinter import
from tkinter import messagebox
def myfunc():
  messagebox.showinfo("개 버튼","개가 짖어요")
tk = Tk()
photo = photoimage(file="파일저장위치")
# button = button(tk, text = "파이썬 종료", fg = "blue", command = quit)
button1 = button(tk, image=photo, command = myfunc)
button.pack()
tk.mainloop()
~~~
# 기말
~~~
< !DOCTYPE html>
<html>
 <head> HTML basic </head>
 <body>
   <h1>헤딩 h1</h1>
   <h2>헤딩 h2</h2>
   <h3>헤딩 h3</h3>
   <h4>헤딩 h4</h4>
   <p>선언 !DOCTYPE은 문서 유형을 나타내며 브라우저가 <br/>을 사용하여 나타냄
 </body>
</heml>
~~~
~~~
<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge"
  <meta name="viewport" content="wudth=device=width,
  <title>Style</title>
</head>
<body>
  <h1 style = "color: red;>" red color</h1>
  <p style="background-color: yellow;>"css color</p>
  <p style="font-size: 100%;>문장 나타내는 p태그</p>
  <!--      여러줄
  -->       주석 처리
</body>
</html>
~~~
~~~
<h1 style="background-color: rgb(255,0,0);>rgh(255,0,0)</h1>         red
<h2 style="background-color: rgb(255,255,0);>rgh(255,255,0)</h2>     yellow
<h3 style="background-color: rgb(0,255,0);>rgh(0,255,0)</h3>          green
<h4 style="background-color: rgb(0,0,255);>rgh(0,0,255)</h4>         blue
<h5 style="background-color: rgb(255,255,255);>rgh(255,255,255)</h5>   white
<h6 style="background-color: rgb(0,0,0);>rgh(0,0,0)</h6>              black
<h7 style="background-color: #ee82ee);">#ee82ee</h7>                  pink
~~~
~~~
<h1>과일</h1>
  <ul>
    <li>과일</li>
    <li>과일</li>
    <li>과일</li>
  </ul>
~~~
# css
## 전체 선택자
~~~
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Wildcard selector</title>
    <style>*{color: red;}</style>                     # 전체 빨간색
</head>
<body>
    <h1>로렘임숨이란?</h1>
    <h2>https://ko.wikipedia.org/wiki/%EB%A1%9C%EB%A0%98_%EC%9E%85%EC%88%A8</h2>
    <p>Lorem Ipsum은 단순히 인쇄 및 조판 업계의 더미 텍</p>
</body>
</html>
~~~
~~~
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Wildcard selector</title>
    <style>*{background-color: gainsboro;}       # 바탕은 회색
     h1{color: red;}                             # h1은 빨간색 
     p{color:yellow;}</style>                    # p는 노란색
             
</head>
<body>
    <h1>로렘임숨이란?</h1>
    <h2>https://ko.wikipedia.org/wiki/%EB%A1%9C%EB%A0%98_%EC%9E%85%EC%88%A8</h2>
    <p>Lorem Ipsum은 단순히 인쇄 및 조판 업계의 더미 텍</p>
</body>
</html>
~~~
~~~
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Wildcard selector</title>
    <style>*{background-color: gainsboro;}
     h1{color: red;}
     p{color:yellow;}
     body,h1,p,h3{margin: 50; padding: 0;}</style>     # 결과창 문장과 문장 사이의 거리 표시
             
</head>
<body>
    <h1>로렘임숨이란?</h1>
    <p>https://ko.wikipedia.org/wiki/%EB%A1%9C%EB%A0%98_%EC%9E%85%EC%88%A8</p>
    <br>                              # 한칸 띄는 결과 표시
    <h3>게 어디서 났니?</h3>
    <p>Lorem Ipsum은 단순히 인쇄 및 조판 업계의 더미 텍</p>
</body>
</html>
~~~
~~~
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS ID selector</title>
    <style>
        #header{
            width: 800px; margin: 0 auto;
            background-color: green;
        }
        #wrap{
            width: 800px; margin: 0 auto;
            overflow: hidden;
        }
        #aside{
            width: 200px; float: left;
            background-color: aqua;
        }
        #content{
            width: 600px; float: left;
            background-color: chartreuse;
        }
    </style>
</head>
<body>
  <div id="header">
    <h1>#header 태그</h1>
  </div>
  <div id="wrap">
    <div id="aside">  
    <h1>#aside 태그</h1>
    </div>
    <div id="content">
    <h1>#content 태그</h1>
    </div>
</body>
</html>
~~~
~~~
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS ID selector</title>
    <style>
        .select{
            color: cyan;
        }
        .select1{
            color: blue;
        }
        .select2{
            color: red;
        }
                .item{color:green;}
        .header{background-color:yellow;}
        #.header{background-color:rgb(250,10,20);}
    </style>
</head>
<body>
    <h1 class="item header">좋아하는 과일은?</h1>
    <u1>
        <li class="select">배</li>
        <li class="select1">포도</li>
        <li class="select2">감</li>
    </u1>
</body>
</html>
~~~
~~~
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>descendent css selectro</title>
    <style>
        #header h1, h2{color: aqua;}
        #section h1,#section h2{color: red;}
        
    </style>
</head>
<body>
    <div id="header">
        <h1 class="title">타이틀</h1>
        <div id="nav">
           <h1>네비게이션</h1>
           <h2>후손적용가능?</h2>
        </div>
    </div>
    <div id="section">
        <h1 class="title">컨텐츠</h1>
        <h2>후손적용가능?</h2>
        <p>로렘 입숨 사이트 정보</p>
    </div>
</body>
</html>
~~~
~~~
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>desc Table</title>
    <style>
      .color_r{ color: red;}
      .color_b{ color: balck;}
</head>
<body>
   <table border = "1">                                      # table → 태그에 style 적용 x
        <tr>
            <th class="color_r">이름</th>
            <th class="color_b">나라</th>
        </tr>
        <tr>
            <td>지뉴</td>
            <td>브라질</td>
        </tr>
        <tr>
            <td>피를로</td>
            <td>이탈리아</td>
        </tr>
    </table>
</body>
</html>
~~~
~~~
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>document</title>
    <style>
        div{                                        # 박스모양 꽉참
            width: 100px; height: 100px; 
            background-color: aqua;
            border: 20px solid blue;
            margin: 0 10px; padding: 0 30px;
        }
        .box{border-width: thick;                  # 박스 모양 점밖이
             border-style: dashed;
             border-color: red;
             margin: 20px; padding: 20px;
             border-radius: 20px 20px;              # 모따기
            }
    </style>
</head>
<body>
    <div class="box"><p>아쿠아리움에 오신걸 환영합니다.~</p></div>
</body>
</html>
~~~
~~~
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>css font size</title>
    <style>
        .a{font-size: large;}
        .b{font-size: small;}
        .c{font-size: 18px;}
        .d{font-size: 2em; font-style: italic;}
    </style>
</head>
<body>
    <h1>Lorem Ipsum</h1>
    <p class="a">Lorem Ipsum</p>
    <p class="b">Lorem Ipsum</p>
    <p class="c">Lorem Ipsum</p>
    <p class="d">Lorem Ipsum</p>
</body>
</html>
~~~
~~~
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>button</title>
    <style>
        .f_big{font-size: 2em;}
        .f_italic{font-style: italic;}
        .f_bold{font-weight: bold;}
        .f_center{text-align: center;}
        .button{
            width:160px; height: 80px;
            background-color: aqua;
            border: 10px solid black;
            border-radius: 30px;
            box-shadow: 5px 5px 5px #a9a9a9;
        }
        .button > a{ display: block; line-height: 80px}
    </style>
</head>
<body>
    <div class="button">
        <a href="https://www.naver.com/" class="f_big f_italic f_bold f_center">click</a>
    </div>
</body>
</html>
~~~
~~~
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>position</title>
    <style>
        .box{
            width: 200px; height: 200px;
            position: absolute;
        }
        .box:nth-child(1){
            background-color: aqua;
            left: 10px; top: 10px;
            z-index: 10;}
        .box:nth-child(2){
            background-color: blue;
            left: 20px; top: 20px;
            z-index: 5;}
        .box:nth-child(3){
            background-color: green;
            left: 30px; top: 30px;
            z-index:1;}
    </style>
</head>
<body>
    <div class="box"></div>
    <div class="box"></div>
    <div class="box"></div>
</body>
</html>
~~~
~~~
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>position</title>
    <style>
        img{float: left; width: 20px; height: 20px;}
    </style>
</head>
<body>
    <img src="logo.png" alt="logo">
    <p>로렘입솜정보1</p>
    <p>로렘입솜정보2</p>
</body>
</html>
~~~
~~~
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>float</title>
    <style>
        .box{
            width:200px; height: 200px;
            background-color: aqua;
            margin: 10px; padding:10px;
            float :left;                     #세로 정렬(1,2) 
           #float :light                     #세로 정렬(2,1)
        }
    </style>
</head>
<body>
    <div class="box">1</div>
    <div class="box">2</div>
</body>
</html>
~~~
#엑셀 파일 만들고 저장
~~~
f = open("저장위치")
s = f.readline()
print(s,end="")
s = f.readline()
print(s,end="")
f.close()
~~~
~~~
def printlist(plist):
    for data in plist:
        print(data,end="\t")
    print()
with open("저장위치",'r') as f:
    header = f.readline()
    header = header.strip()
    for s in f:
        s = s.strip() 
        rowlist = s.split(',')
        printlist(rowlist)
~~~
~~~
with open("저장위치",'r') as f:
    with open("저장위치",'w') as fs:
        h = f.readline()
        h = h.strip()
        hlist = h.split(',')
        idx1 = hlist.index('id')
        idx2 = hlist.index('passwoed')
        hlist = [hlist[idx1],hlist[idx2]]
        hstr = ','.join(map(str,hlist))
        fs.write (hstr +'\n')
        for s in f:
            s = s.strip()
            rstr = s.split(',')
            if int(rlist[idx1]) >= 165:
                rlist = [rlist[idx2],rlist[idx1]]
                rstr = ','.join(map(str,rlist))
                fs.write(rstr+'\n')
print('save ok!')
~~~
~~~
from tkinter import *
tk = Tk()
counter = 0
def clicked():
    global counter
    counter += 1
    label1['text'] = 'button click num' + str(counter)
def reset():
    global counter
    counter = 0
    label1['text'] = 'butoon go'
tk.tktitle('gul 카운터')
label1 = Label(tk, text ='button go', fg = 'blue', font =20)
label1.pack( side = LEFT, padx =10, pady =10)
button1 = Button(tk, text = 'go to click',
                       bg = 'green', font=15, width=30, height=5, command=clicked)
button1.pack( side = LEFT, padx =10, pady =10)
button2 = Button(tk, text = 'reset', 
                      bg = 'red', font=15, width=30, height=5, command=reset)
button2.pack( side = LEFT, padx =10, pady =10)
tk.mainloop()
~~~
~~~
import urllib.request
url = "https://www.naver.com"
res = urllib.request.urlopen(url)
html = res.read()
print(html)
~~~
~~~
import urllib.request
import bs4
url = "https://www.naver.com"
res = urllib.request.urlopen(url)
bsobject = bs4.beautifulsoup(res,'html.parser')
print(bsobject)
~~~
~~~
import urllib.request
import bs4
url = "https://www.naver.com"
res = urllib.request.urlopen(url)
bsobject = bs4.beautifulsoup(res,'html.parser')
tag_div = bsobject.find('div')
print(tag_div)
~~~
~~~
import urllib.request
import bs4
url = "https://www.naver.com"
res = urllib.request.urlopen(url)
bsobject = bs4.beautifulsoup(res,'html.parser')
tag_div = bsobject.find('div')
print(tag_div)
tag_id = tag_div.findALL('news-area')
print(tag_id)
~~~
~~~
import urllib.request
import bs4
url = "https://www.naver.com"
res = urllib.request.urlopen(url)
html = res.read()
bsobject = bs4.beautifulsoup(res,'html.parser')
tag = bsobject.find('div', {'id':'naverci'})
print(tag, '\n')
a_tag = tag.find("a")
print(a_tag,'\n')
href = a_tag['href']
print(href,'\n')
text = a_tag.text
print(text)
~~~
# 인구 통계 자료
~~~
import pandas as pd
url = "http://stat.paju.go.kr/index.do"
~~~
~~~
table = pd.read_html(url)  # 자료에 표 존재시 작성
len(table)
~~~
~~~
import seaborn as sb
import matplotlib.font_manager as fm
sb.set( font="nanumgothic")
#sb.set(font="applegothic")
~~~
~~~
# 한글 다운로드(런타임 다시 시작)
! sudo apt-get install -y fonts0nanum
!sudo fc-cache -fv
!rm ~/.cache/matplotlib -rf
~~~
~~~
sys_font=fm.findSystemFonts()
print(f"sys_font number: {len(sys_font)}")
nanum_font = { f for f in sys_font if 'nanum' in f}
print(f"nanum_font number:{len(nanum_font)}")
~~~
~~~
fontbath='복사주소'
font = fm.Fontproperties(fname=fontbath,size=10)
~~~
~~~
import matplotlib.font_manager as fm
fontpath = '복사주소'
font = fm.fontproperties(fname=fontpath,size=10)
~~~
~~~
# 기본글꼴 변경
import matplotlib as mp
#mp.font_manager.rebuild()
mp.pyplot.rc('font',family='nanumgothic')
~~~
~~~
# 시각화
import seaborn as sb
import matplotlib.font_manager as fm
fontpath = '복사 주소'
font = fm.FontProproperties( fname=fontpath,size=10).get_name()
#plt.rc('font',family=font)
sb.set(font="NanumGothic")
~~~
#기상청 데이터 가져오기
~~~
# 디코딩 키 사용
import requests
url = '복사 주소'# 기상청 데이터 주소
params = {'serviceKey':'복사 주소'} #값 주소
response = requests.get(url, params=params)
print(response.content)
~~~
