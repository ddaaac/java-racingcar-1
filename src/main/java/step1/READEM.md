[1주차] 자동차 경주 게임
Step1. 문자열 계산기
: 사용자가 입력한 문자열 값에 따라 사칙연산을 수행할 수 있는 계산기 구현
※ 메소드가 너무 많은 일을 하지 않도록 분리하기 위해 노력해 본다.

1. 사용자가 문자열을 입력한다.
2. 사칙연산을 수행한다.
3. 1과 2의 과정을 Detail하게 만든다. (Validation Check)
    1) 사칙연산 기능을 모두 구현한다.
    2) 사칙연산 우선 순위는 무시한다 → 입력한 순서대로 계산한다.
    예를 들어 "2 + 3 * 4 / 2"와 같은 문자열을 입력할 경우 2 + 3 * 4 / 2 실행 결과인 10을 출력
    3) 입력값이 NULL 이거나, 빈 공백의 문자열일 경우 Exception 처리한다.
        - 빈 공백 문자열은 String 클래스의 split(" ") 메소드를 활용한다.
        - IllegalArgumentException throw 사용
    4) 사칙연산 기호가 아닌 경우 : Exception 처리
        - IllegalArgumentException throw
    5) 반복패턴을 찾아 반복문으로 구현한다.

    - 일단 main 패키지를 구현한다. (기능별 클래스 나누기)
    - 그 다음 test 패키지를 구현한다.
    - 단계별로 수시로 깃 히스토리를 남겨두자