# 2단계. 문자열 계산기 

## TODO (개발 초기)

- [X] 사용자 입력 받기
  - [X] 자동차 수
  - [X] 시도 횟수
- [X] 자동차 구현
  - [X] 움직임 : 전진 or 멈춤
    - [X] random 값이 4이상일 경우 전진
  - [X] 현재 위치값
- [X] 랜덤 넘버 생성 클래스
- [X] 자동차 경주 클래스
-[X] 결과 값 출력

## TODO (리팩터링중 추가됨)
- [X] 랜덤 넘버 생성 클래스에 대한 테스트 만들기 
- [X] Round 클래스 분리
- [X] position 일급 컬렉션으로 분리
- [X] position 테스트 클래스 추가
- [X] position은 0 이상의 정수이다. 
- [X] cars 일급 컬렉션으로 분리
- [X] rounds 일큽 컬렉션으로 분리
- [X] cars 테스트 코드 추가
- [X] round 테스트 코드 추가
- [X] rounds 테스트 코드 추가
- [X] MoveRule 클래스 추가 (자동차의 움직임 결정)
- [X] Cars에서 car의 수는 1이상이다.
- [X] roundNum(시도횟수)는 0 이상의 정수이다. 
- [X] ResultView 리팩토링

## 피드백 반영 
- [X] 하이픈 리턴 대신 Position 리턴. 
- [ ] 전략 패턴 테스트 변경
   - [ ] RandomNumber Test 제거
   - [ ] carMoveTest 변경 (포지션 대신 strategy 주입)
- [ ] 테스트를 위한 생성자 제거
- [ ] position increase 변경
  - [ ] int position을 final로 변경 (Position return은 유지)
  

## 꼭 기억할 것 
- Getter를 올바르게 이해하자. 🐣  
  **객체에서 값을 꺼내서 처리할 로직은 (예. 값 비교, 유효성 검사) 객체에게 메시지를 통해 시킨다.**   
  단 이외의 경우에 값이 다른 클래스에서 리턴 될 필요가 있을때는 (예. view에서 값 얻기)  
  getter를 쓰는것이 바람직하다.   
  
## slack으로 질문할 것
- [ ] 랜덤하게 움직이는게 아니라 특정 규칙이 있다면 이것은 테스트가 필요한가?  
  - [ ] 랜덤을 테스트하는 방법이 없기 때문에 테스트를 스킵하는걸까?
- [ ] 테스트를 위해 production 코드를 수정하는 것은 지양되지만,  
  생성자 생성은 괜찮다고 라이브 강의 때 들었는데,   
  생성자 생성이 괜찮은 경우가 따로 있는 걸까?