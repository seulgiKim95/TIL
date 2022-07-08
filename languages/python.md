# python

생성일: 2022년 3월 7일 오후 5:05
최종수정일: 2022년 7월 8일 오전 9:39



### anaconda

- Spyder
    
    F9 : 한줄 수행
    
    블럭지정 후 ctrl+enter : 블럭 수행 (이때 # %%으로 블럭 구분하면 그 안의 내용 수행)
    
    F5 : 전체 수행
    
    ```bash
    reset -sf # 사용중인 객체 전부 지우기
    clear # console 창 지우기
    ```
    

### 8진수 / 16진수

```bash
var_8B = 0o101 # 8진수는 0o 문법
var_16B = 0x56 # 16진수는 0x 문법 
```

### 연산자

```bash
a // b # a/b 의 정수값만 리턴
```

### 입출력

```bash
f'문자열문자열{변수}' # 이러면 print가 없더라도 변수에 변수가 들어가서 출력됨

```

### 문자열 함수

```python
# join
a = ','; b = a.join('abcd') # b = 'a,b,c,d' 

# upper / lower 대 / 소문자 만들기
b = a.upper; c = a.lower

# strip 소문자로 바꾸고 양쪽의 공백지우기, 각 왼쪽/오른쪽 공백 지우기는 lstrip / rstrip
b = a.strip()

# count 글자 수 세기
n = a.count() 

# find, index
n = a.find('a') # a 라는 문자를 찾아서 위치 반환. 만약 없으면 -1 리턴
m = a.find('a') # a 라는 문자를 찾아 위치 반환. 없으면 ValueError

# replace
a.replace(oldstr, newstr)
```

### list

```python
a = [1,2,3]
b = a*3 # [1,2,3,1,2,3,1,2,3]
a[1:1] = ['a','b','c'] # [1,'a','b','c',2,3], 리스트 추가
a[1:4] = [] # [1,2,3], 리스트 삭제

a.append(n) # 리스트 끝에 요소 n 추가
a.reverse() # 리스트 뒤집기. or [::-1] => 끝에서부터 읽기
a.index(n) # n의 위치 반환, 없으면 valueerror
a.insert(idx, n) # idx의 위치에 n 삽입
a.remove(n) # 첫번째로나온 n을 삭제
a.pop(idx) # idx 위치의 원소를 반환하고 삭제. idx를 주지 않으면 가장 마지막 요소 삭제
a.count(n) # a 안에 n이 몇번 나오는지
a.extend([4,5]) # 마지막 위치에 [4,5] 삽입
```

*** 배열과의 차이점 : 배열은 같은 자료형만 삽입할 수 있지만, 리스트는 다른 자료형도 삽입 가능.

---
