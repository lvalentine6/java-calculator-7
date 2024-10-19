# java-calculator-precourse

## 미션 소개
이 프로젝트는 우아한테크코스 프리코스 1주차 미션으로, 문자열로 입력받은 숫자들을 더하는 계산기를 구현한다.

## 미션 목표
- 객체 지향 프로그래밍 원칙을 적용한 계산기를 구현한다.
- 기능별 커밋을 원칙으로 한다.
- TDD를 적용한다.
  - 각 기능별로 테스트 케이스를 작성한다.
  - 기능별로 해피 케이스, 예외 케이스를 나누어 작성한다.
  - 실패 테스트 작성 -> 테스트 통과 -> 리팩토링
- 클린 코드를 지향하며 의미 있는 변수명과 메서드명을 사용한다.

## 주요 클래스 설명
- `Application`: 프로그램의 진입점으로, CalculatorController를 초기화하고 실행을 위임한다.
- `CalculatorController`: 사용자 입력, 계산 처리, 결과 출력 등 계산기 프로그램의 전체 흐름을 제어하고 각 구성 요소를 조정한다.
- `Calculator`: 문자열 파싱 및 계산 로직을 담당한다.
- `InputHandler`: 사용자 입력 처리를 담당한다.
- `ValidatingParser`: 사용자 입력에 대한 파싱과 검증을 담당한다.
- `OutputHandler`: 결과 출력을 담당한다.

## 기능 목록
- [x] 쉼표(,) 또는 콜론(:)을 구분자로 가지는 문자열을 입력받아 숫자의 합을 반환
- [x] 커스텀 구분자 지원 ("//"와 "\n" 사이의 문자를 구분자로 사용)
- [x] 잘못된 입력에 대한 예외 처리 (IllegalArgumentException 발생)
- [x] 음수 입력에 대한 예외 처리
- [x] 계산 결과가 int 범위를 초과할 경우 예외 처리

## 테스트 목록
- [x] Calculator 테스트
  - [x] 여러 숫자 리스트의 합계를 계산한다.
  - [x] 단일 숫자 리스트의 합계를 계산한다.
  - [x] 0이 하나인 숫자 리스트의 합계를 계산한다.
  - [x] 빈 리스트 입력 시 0을 반환한다.
  - [x] 음수가 포함된 리스트에 대해 예외를 발생시킨다.
  - [x] 합계가 int의 최댓값을 초과할 경우 예외를 발생시킨다.

- [x] ValidatingParser 테스트
  - [x] 커스텀 구분자가 포함된 문자열을 파싱한다.
  - [x] 커스텀 구분자 뒤에 빈 문자열이 오면 [0]을 반환한다.
  - [x] 기본 구분자(쉼표, 콜론)가 포함된 문자열을 파싱한다.
  - [x] 빈 문자열 입력 시 [0]을 반환한다.
  - [x] 잘못된 커스텀 구분자 형식에 대해 예외를 발생시킨다.
  - [x] 음수 입력 시 예외를 발생시킨다.
  - [x] 숫자가 아닌 입력에 대해 예외를 발생시킨다.

## 작성자
lvalentine6 (이승로)
