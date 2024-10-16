## 정보처리기사 Python 기출 문제 모음

### 목차 
- [20년 기출](#year20)
- [21년 기출](#year21)
- [22년 기출](#year22)
- [23년 기출](#year23)
- [24년 기출](#year24)
  
### <h3 id="year20">📋20년 기출</h3>

**20년 2회**

```python
a={'한국','중국','일본'}
a.add('베트남')
a.add('중국')
a.remove('일본')
a.update(['한국','홍콩','태국'])
print(a)
```
<details>
<summary>✅ 정답</summary>
{'한국', '중국', '베트남', '홍콩', '태국'}
</details>
<br>

🖋 **문제 풀이** <br>
1. 초기 집합 생성: a는 '한국', '중국', '일본'을 포함하는 집합.
2. 요소 추가: a.add('베트남')으로 '베트남'을 추가.
3. 중복 추가 무시: a.add('중국')은 이미 존재하는 '중국'을 추가하려고 하지만, 집합에서는 중복을 허용하지 않음.
4. 요소 제거: a.remove('일본')으로 '일본'을 제거.
5. 여러 요소 추가: a.update(['한국','홍콩','태국'])으로 '한국', '홍콩', '태국'을 추가. '한국'은 이미 존재하므로 무시.

<hr> 

**20년 4회**

```python
	lol = [[1,2,3],[4,5],[6,7,8,9]]
print(lol[0])
print(lol[2][1])
for sub in lol:
  for item in sub:
    print(item, end = '')
  print()
```
<details>
<summary>✅ 정답</summary>
[1, 2, 3]
7
1 2 3
4 5
6 7 8 9
</details>
<br>

🖋 **문제 풀이** <br>
```python
# 리스트 생성
lol = [[1, 2, 3], [4, 5], [6, 7, 8, 9]]

# 첫 번째 서브 리스트 출력
print(lol[0])  # [1, 2, 3]

# 세 번째 서브 리스트의 두 번째 요소 출력
print(lol[2][1])  # 7

# 중첩 루프를 통해 모든 요소 출력
for sub in lol:
    for item in sub:
        print(item, end=' ')  # 요소를 한 줄에 출력
    print()  # 서브 리스트마다 줄 바꿈

```

<hr> 

### <h3 id="year20">📋20년 기출</h3>

**21년 1회**

```python
class good :
	li = ["seoul", "kyeonggi","inchon","daejeon","daegu","pusan"]
 
g = good()
str01 = ''
for i in g.li:
	str01 = str01 + i[0]
    
print(str01)
```
<details>
<summary>✅ 정답</summary>
skiddp
</details>
<br>

🖋 **문제 풀이** <br>
```python
1. 초기값 설정: a에 100을 할당하고, result를 0으로 초기화.<br>
2. 반복문: for i in range(1, 3)는 i가 1과 2일 때 반복.<br>
3. 첫 번째 반복 (i = 1)<br>
- result = a >> 1: 100을 오른쪽으로 1비트 시프트.<br>
    - 100의 이진수 표현: 110010<br>
    - 1비트 시프트: 011001 (즉, 50)<br>
result = result + 1: 50에 1을 더하여 result = 51<br>
4. 두 번째 반복 (i = 2)<br>
    - result = a >> 2: 100을 오른쪽으로 2비트 시프트.<br>
    - 2비트 시프트: 001100 (즉, 25)<br>
5. result = result + 1: 25에 1을 더하여 result = 26<br>
6. 결과 출력: 최종적으로 print(result)를 통해 26이 출력.

```
<hr> 

**21년 3회**

```python
a,b = 100, 200 
print(a==b)
```
<details>
<summary>✅ 정답</summary>
False
</details>
<br>

🖋 **문제 풀이** <br>
- 파이썬에서는 True와 False가 대문자로 구분되는 불리언 값 (주의할것)
<hr> 

### <h3 id="year22">📋22년 기출</h3>

**22년 1회**

```python
def exam(num1, num2=2):
  print('a=', num1, 'b=', num2)
exam(20)
```
<details>
<summary>✅ 정답</summary>
a=20 b=2
</details>
<br>

🖋 **문제 풀이** <br>
```python
def exam(num1, num2=2):  # num2의 기본값을 2로 설정
    print('a=', num1, 'b=', num2)  # num1과 num2를 출력

exam(20)  # num1에 20을 전달, num2는 기본값인 2 사용
```
<hr> 

**22년 2회**

```python
	a="REMEMBER NOVEMBER"
b=a[:3]+a[12:16]
c="R AND %s" % "STR";
print(b+c)
```
<details>
<summary>✅ 정답</summary>
REMEMBER AND STR
</details>
<br>

🖋 **문제 풀이** <br>
1. 슬라이싱: b = a[:3] + a[12:16]<br>
- a[:3]: 문자열 a의 인덱스 0부터 2까지의 문자, 즉 "REM"을 가져옴.<br>
- a[12:16]: 문자열 a의 인덱스 12부터 15까지의 문자, 즉 "EMBE"를 가져옴.<br>
따라서 b는 "REM" + "BER"가 되어 "REMEMBER".<br>

2. 문자열 포맷팅: c = "R AND %s" % "STR"<br>
- %s는 문자열 포맷팅에서 사용되며, 뒤에 오는 "STR"로 교체.<br>
- 결과적으로 c는 "R AND STR".<br>

3. 출력: print(b + c)는 b와 c를 합쳐서 출력.<br>
<hr> 

**22년 3회**

```python
TestList = [1,2,3,4,5]
TestList = list(map(lambda num : num + 100, TestList)))
 
print(TestList)
```
<details>
<summary>✅ 정답</summary>
[101,102,103,104,105]
</details>
<br>

🖋 **문제 풀이** <br>
 map 함수와 lambda 함수를 사용하여 리스트의 각 요소에 100을 더하는 예제<br>
1. 초기 리스트: TestList에 [1, 2, 3, 4, 5]를 할당합니다.<br>
2. map과 lambda 사용<br>
- map 함수는 주어진 함수를 리스트의 각 요소에 적용합니다.<br>
- lambda num: num + 100는 익명 함수로, 입력된 num에 100을 더하는 기능을 합니다.<br>
- map 함수는 TestList의 각 요소에 이 lambda 함수를 적용하여 새로운 값을 생성합니다.<br>
- 리스트 변환: list(...)를 사용하여 map의 결과를 리스트로 변환합니다.<br>
3. 결과 출력: print(TestList)를 통해 최종 결과인 [101, 102, 103, 104, 105]를 출력합니다.

<hr> 

### <h3 id="year23">📋21년 기출</h3>

**23년 1회17번 출력 결과(20년 2회 기출문제와 동일)**

```python
a={'한국','중국','일본'}
a.add('베트남')
a.add('중국')
a.remove('일본')
a.update(['한국','홍콩','태국'])
print(a)
```
<details>
<summary>✅ 정답</summary>
{'한국', '중국', '베트남', '홍콩', '태국'}
</details>
<br>

🖋 **문제 풀이** <br>
1. 초기 집합 생성: a는 '한국', '중국', '일본'을 포함하는 집합.
2. 요소 추가: a.add('베트남')으로 '베트남'을 추가.
3. 중복 추가 무시: a.add('중국')은 이미 존재하는 '중국'을 추가하려고 하지만, 집합에서는 중복을 허용하지 않음.
4. 요소 제거: a.remove('일본')으로 '일본'을 제거.
5. 여러 요소 추가: a.update(['한국','홍콩','태국'])으로 '한국', '홍콩', '태국'을 추가. '한국'은 이미 존재하므로 무시.

<hr> 

**23년 2회**<br>
출력 결과는?

```python
a = "engineer information processing"
b = a[:3]
c = a[4:6]
d = a[28:]
e=b+c+d
 
print(e)
```
<details>
<summary>✅ 정답</summary>
engneing
</details>
<br>

🖋 **문제 풀이** <br>
```python
a = "engineer information processing"  # 문자열 a 정의
b = a[:3]  # b는 a의 인덱스 0부터 2까지의 문자 -> eng
c = a[4:6]  # c는 a의 인덱스 4부터 5까지의 문자 -> ne
d = a[28:]  # d는 a의 인덱스 28부터 끝까지의 문자 -> ing

e = b + c + d  # b, c, d를 합침 eng + ne + ing
print(e)  # 결과 출력

```
<hr> 

**23년 3회**<br>
한 번에 2개를 입력받아서 분리문자로 분리해서 각각 다른 변수에 저장하려고 한다.

```python
num1, num2 = input(). ( 가 )(분리문자)
```
<details>
<summary>✅ 정답</summary>
split
</details>
<br>

🖋 **문제 풀이** <br>
## 문자열 관련 함수

| 함수      | 설명                                       | 예제                                         |
|-----------|------------------------------------------|--------------------------------------------|
| `split()` | 문자열을 분리하여 리스트로 반환          | `num1, num2 = input().split(',')`        |
| `join()`  | 리스트의 요소를 연결하여 문자열로 만듦   | `result = ', '.join(['apple', 'banana'])` |
| `strip()` | 문자열의 양쪽 공백을 제거                | `cleaned = user_input.strip()`           |
| `replace()` | 특정 문자열을 다른 문자열로 교체       | `new_string = original_string.replace('old', 'new')` |
| `find()`  | 특정 문자열의 인덱스를 반환              | `index = string.find('substring')`       |

###  리스트 관련 함수

| 함수      | 설명                                       | 예제                                         |
|-----------|------------------------------------------|--------------------------------------------|
| `append()`| 리스트의 끝에 요소를 추가                | `my_list.append('new_item')`              |
| `extend()`| 리스트에 다른 리스트의 요소를 추가      | `my_list.extend(['item1', 'item2'])`     |
| `insert()`| 특정 인덱스에 요소를 추가               | `my_list.insert(1, 'new_item')`           |
| `remove()`| 특정 값을 가진 첫 번째 요소를 제거      | `my_list.remove('item_to_remove')`        |
| `pop()`   | 특정 인덱스의 요소를 제거하고 반환      | `item = my_list.pop(0)`                    |

### 수학 관련 함수

| 함수      | 설명                                       | 예제                                         |
|-----------|------------------------------------------|--------------------------------------------|
| `max()`   | 주어진 iterable의 최대값을 반환         | `largest = max([1, 2, 3, 4])`            |
| `min()`   | 주어진 iterable의 최소값을 반환         | `smallest = min([1, 2, 3, 4])`           |
| `sum()`   | 주어진 iterable의 합계를 반환           | `total = sum([1, 2, 3, 4])`              |
| `sorted()`| 주어진 iterable을 정렬하여 리스트로 반환| `sorted_list = sorted([3, 1, 4, 2])`     |

### 기타 유용한 함수

| 함수      | 설명                                       | 예제                                         |
|-----------|------------------------------------------|--------------------------------------------|
| `len()`   | 객체의 길이를 반환                      | `length = len(my_list)`                   |
| `type()`  | 객체의 타입을 반환                      | `obj_type = type(my_variable)`            |
| `range()` | 숫자의 범위를 생성                     | `for i in range(5): print(i)`            |

<hr> 

### <h3 id="year24">📋24년 기출</h3>

**24년 1회**<br>
출력 결과는?

```python
a = ["Seoul", "Kyeonggi", "Incheon", "Daejun", "Daegu", "Pusan"] 
str = "S"
 
for i in a:
    str = str + i[1]
 
print(str)
Colored
```
<details>
<summary>✅ 정답</summary>
Seynaau
</details>
<br>

🖋 **문제 풀이** <br>
```python
a = ["Seoul", "Kyeonggi", "Incheon", "Daejun", "Daegu", "Pusan"]  # 도시 이름 리스트
str = "S"  # 초기 문자열

for i in a:  # 리스트 a의 각 도시를 순회
    str = str + i[1]  # 각 도시의 인덱스 1 문자를 str에 추가

print(str)  # 최종 결과 출력
# 최종 출력: "Seynaau"
```
<hr> 

**24년 2회😿**<br>
출력 결과는?

```python
def fnCalculation(x,y):
    result = 0;
    for i in range(len(x)):
     temp = x[i:i+len(y)] 
     if temp == y:
       result += 1;
    return result
 
a = "abdcabcabca"
p1 = "ab";
p2 = "ca";
 
out = f"ab{fnCalculation(a,p1)}ca{fnCalculation(a,p2)}"
print(out)
```
<details>
<summary>✅ 정답</summary>
ab3ca3
</details>
<br>

🖋 **문제 풀이** <br>
```python
def fnCalculation(x, y):
    result = 0  # 결과를 저장할 변수 초기화
    for i in range(len(x)):  # x의 길이만큼 반복
        temp = x[i:i+len(y)]  # x의 i번째 인덱스부터 y의 길이만큼 슬라이스
        if temp == y:  # 슬라이스한 부분이 y와 같으면
            result += 1  # 결과를 1 증가
    return result  # 최종 결과 반환

a = "abdcabcabca"  # 검색할 문자열
p1 = "ab"  # 찾을 첫 번째 패턴
p2 = "ca"  # 찾을 두 번째 패턴

out = f"ab{fnCalculation(a, p1)}ca{fnCalculation(a, p2)}"  # 결과 문자열 생성
print(out)  # 결과 출력
```
<hr> 
