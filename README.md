# CAwithC
computer architecture with c

# C 언어를 통해 배우는 컴퓨터 구조와 운영체제.
강의당 20~30분 짧은 분량

### 0. main 함수, stdio
#include, stdio.h, main함수 소개
printf, scanf 표준입출력 소개
함수 구조 소개

### 1. 자료형 
각 자료형마다 몇비트로, 어떻게 구성되어 있는지.
sizeof()
int
char : ascii code 상에서 각 문자,숫자가 어떤 숫자로 대응되는지
float : IEEE754 format
double
포인터
void
etc.. 

### 1.2 ascii
escape sequence
non printable들
\n 이런 거
윈도우는 \n\r

### 1.5 연산자
+, -, *, /, %, ++, --, ,

### 2. 배열
배열의 기본개념과 선언
2중 배열, 더 큰 차원의 배열
행, 열

### 3. 포인터(배열먼저? 포인터먼저?)
파이썬과 C의 차이
포인터를 통한 메모리 접근
배열의 이름이 의미하는 것
포인터 연산과 배열 접근 비교 *(ptr + i)
#include <stdio.h>

int main() {
    int array[5] = {1, 2, 3, 4, 5};
    int *ptr = array;

    for (int i = 0; i < 5; i++) {
        printf("%d ", *(ptr + i));
    }

    return 0;
}

### 4. 구조체
구조체를 통해 자료구조 만들기. linked list, tree ...

### 5. 조건문
if, switch, for, while

### 6. 배열 메모리 로컬리티
캐시 소개
배열을 사용할 때 메모리 접근 패턴(행, 열) -> 퍼포먼스 비교 (어떤 방식으로?)
psuedo LRU 구현

### 7. 조건문과 분기예측
assembly -> branch 
분기예측
간단한 해시테이블 (모듈러로)
psuedo LRU(트리로, 파이프라인 얘기해야해서 뒤로 미뤄도 될듯)

### 8. 함수와 스택프레임
함수의 기본 개념
스택 프레임과 함수 호출
함수 호출의 어셈블리 코드

### 9. 하드웨어 구현
RTL
기본 boolean function (and, or ...)
드모르간
truth table, 카르노맵
combinational logic vs sequential logic

### 11. Adder 구현

### 12. ALU 구현
// 간단한 ALU 시뮬레이션
int ALU(int a, int b, char op) {
    switch(op) {
        case '+': return a + b;
        case '-': return a - b;
        case '*': return a * b;
        case '/': return a / b;
        default: return 0;
    }
}

### 13. 메모리 구현
래치, 플립플랍

### 14. SC

### 15. MC

### 16. pipelined

### 17. superscalar 

### 18. MMU, page table
컴구 + 운체
가상메모리 주소 어떻게 사용되는지


### GPU computing

### vector processor

### cuda

### 베릴로그 하드웨어 설계

### 파이썬 인공지능 쪽, 뉴로모픽

### 하드웨어 가속기
