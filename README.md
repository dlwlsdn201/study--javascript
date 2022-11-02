# Javascript 의 모든 것
---

## 배열

### 두 배열 비교하기

> **배열 합집합**
  - 전개 연산자 spread operator(...) 과 `Set()` 을 사용하여 두 배열을 병합하고 모든 중복된 요소를 제거할 수 있다.
    ```jsx
      let arrA = [1, 4, 3, 2];
    let arrB = [5, 2, 6, 7, 1];

    [...new Set([...arrA, ...arrB])]; // returns [1, 4, 3, 2, 5, 6, 7]
    ```
  
> **배열 교집합**
  - `filter` 와 `includes` 을 사용하여 두 배열에 포함된 동일한 요소를 확인할 수 있다.
  `includes()` 함수의 return 형식은 **boolean** 이다.
    ```jsx
      let arrA = [1, 4, 3, 2];
      let arrB = [5, 2, 6, 7, 1];

      arrA.filter(it => arrB.includes(it)); // returns [1, 2]
    ```
