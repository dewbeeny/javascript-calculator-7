# javascript-calculator-precourse

## 필수 구현 기능 목록

1. **쉼표(,) 또는 콜론(:)을 구분자로 사용하여 숫자 더하기**

   - 입력 문자열에 쉼표(,) 또는 콜론(:)이 있을 경우, 해당 구분자를 기준으로 숫자를 분리한 후 그 합을 계산한다.
   - 예시: `"1,2,3"` → `6`, `"1:2:3"` → `6`

2. **커스텀 구분자 사용**

   - 커스텀 구분자는 문자열 앞부분의 `"//[구분자]\n"` 형식으로 정의한다.
   - 해당 구분자를 기준으로 숫자를 분리한 후 합을 계산한다.
   - 예시: `"//;\n1;2;3"` → `6`

3. **숫자가 아닌 잘못된 값 입력 시 예외 처리**
   - 입력 문자열에 숫자가 아닌 값이 포함되면, `[ERROR]` 메시지와 함께 예외를 발생시킨다.
   - 예시: `"1,X,3"` → `[ERROR]`

## 추가 구현 기능 목록 (시간이 남을 경우)

4. **빈 문자열 또는 null 입력 시 0 반환**

   - 입력이 빈 문자열 또는 `null`인 경우, 결과로 0을 반환한다.
   - 예시: `""` → `0`, `null` → `0`

5. **음수 입력 시 예외 처리**

   - 음수가 포함된 입력 문자열이 주어지면, `[ERROR]` 메시지와 함께 예외를 발생시킨다.
   - 예시: `"//;\n-1;2;3"` → `[ERROR]`

6. **구분자와 숫자가 모두 없는 입력 시 0 반환**
   - 입력 문자열에 숫자가 없거나, 구분자만 있을 경우 0을 반환한다.
   - 예시: `"//;\n"` → `0`
