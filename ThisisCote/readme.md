
참고 : [한빛미디어] [이것이 취업을 위한 코딩 테스트다](https://github.com/ndb796/python-for-coding-test) , [동영상](https://www.youtube.com/watch?v=m-9pAwq1o3w)


### 출제 빈도 높은 유형
- 그리디, 구현, DFS/BFS, 정렬, 다이나믹 프로그레밍 순 알고리즘

 

### 알고리즘 성능 평가

- 코테에서 시간제한은 통상 1~5초임
    - 파이썬으로 구현시 시간초과가 나오면 Pypy로 다시 해보는 것도 권유
- 문제에서 시간제한 요구사항을 확인한후 관련 복잡도의 알고리즘을 설계해야함
    - N의 범위가 500인 경우 O(n^3)인 알고리즘
    - N의 범위가 2,000인 경우 O(n^2)인 알고리즘
    - N의 범위가 100,000인 경우 O(nlogn)인 알고리즘
    - N의 범위가 10,000,000인 경우 O(n)인 알고리즘
- 복잡도 : 알고리즘 성능을 나타내는 척도
    - 시간 복잡도 : 알고리즘 수행 시간
    - 공간 복잡도 : 알고리즘 메모리 사용량 분석
- 빅오 표기법(Big-O Notation)
    - 가장 빠르게 증가하는 항만을 고려(함수의 상한에 포커싱)
    - ex. 3n^3 + 5n^2 + 1000000000 : O(n^3)
    
    ![ddds](https://user-images.githubusercontent.com/93170871/148648284-7ee3c88f-262a-4069-a588-7ae985bff6b7.png)
    
    출처 : [https://www.bigocheatsheet.com/](https://www.bigocheatsheet.com/)
    
 

- 시간 복잡도 사례 : N개의 숫자의 곱 결과 프로그램
```python
# O(N^2) 으로 푼 경우

array = [3,5,1,2,4]

for i in array:
	for j in array:
		res = i*j
		print(res)
```

 

- 알고리즘 문제 해결 과정
    - 지문 읽기
    - 요구사항(복잡도) 분석
    - 문제 해결을 위한 아이디어 찾기 :  **핵심 아이디어를 잘 캐치하면 금방 문제 해결이 됨**
    - 소스 코드 설계 및 코딩

 

- 수행 시간 측정 코드
```python
import time
start_time = time.time()

# source code...

end_time = time.time()
print('time:', end_time - start_time #수행시간
```
