
## 2단계: 개략적 설계안 제시 및 동의 구하기

다음과 같은 내용을 다룬다.

- API 설계
- 개략적 설계안
- 주변 사업장 검색 알고리즘
- 데이터 모델

### 데이터 모델 

읽기/쓰기 비율(read/write ratio)에 대한 고려가 필요하다. 읽기 연산이 더 자주 사용되기 때문이다.

- 주변 사업장 검색
- 사업장 정보 확인

읽기 연산은 빈도가 낮다. 사업장 정보를 추가하거나 삭제, 편집은 빈번하지 않기 때문이다. 읽기 연산이 압도적인 시스템은 MySQL 같은 관계형 데이터베이스가 바람직할 수 있다.
