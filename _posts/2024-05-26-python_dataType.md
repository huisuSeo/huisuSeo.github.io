---
layout: single
title:  "파이썬 빌트인 데이터타입"
---

# 빌트인 데이터 타입.

빌트인 데이터 타입은 언어 자체에서 제공하는 **데이터 타입**과 **컬렉션 테이터 타입**이 있습니다.


- 앱실론을 포함한 연산에 주의하라

```python
import sys

# 앱실론 출력
print(sys.float_info.episilon)
# 부동소수점 수의 오차 검사
a = 0.1 + 0.1 + 0.1
b = 0.3
print(a - b)
if abs(a - b) < sys.float_info.epsilon:
  print("a와 b는 같은 값입니다.") # 이 코드가 출력됨
else:
  print("a와 b는 다른 값입니다.")
```

