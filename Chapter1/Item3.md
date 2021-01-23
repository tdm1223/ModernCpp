# 항목 3. 낌새만 보이면 const를 들이대 보자!
### const
- `const`를 붙여 선언하면 컴파일러가 사용상의 에러를 잡아내는데 도움을 준다.
- `const`는 객체, 함수 매개변수, 반환 타입, 멤버 함수 등 다양한 곳에 붙을 수있다.
- 클래스 바깥에서는 전역 혹은 네임스페이스 유효범위의 상수를 선언하는데 쓸 수 있다.
- 파일, 함수, 블록 유효범위에서 `static`으로 선언한 객체에도 붙일 수 있다.
- const 유무로 함수 오버로딩이 가능하다.

```cpp
char hello[] = "HELLO";
char testing[] = "TEST";

const char* p = hello; // 상수를 가리키는 포인터
// p[1] = 'T'; 에러

char* const p = hello; // 상수 포인터
// p = testing; 에러

const char * const p = hello // 상수를 가리키는 상수 포인터
// 위 2개 모두 에러
```

### 상수 멤버 함수
- 멤버 함수에 const가 붙으면 상수 멤버 함수가 된다.
- 상수 객체에 대해 호출되는 함수이다.

### 비트 수준 상수성
- **물리적 상수성**이라고도 한다.
- 어떤 멤버 함수가 그 객체의 어떤 데이터 멤버도 건드리지 않아야 그 멤버 함수가 `const`임을 인정하는 개념
- 객체를 수정하는 비트들 중 어떤 것도 바꾸면 안 된다.

### const로 동작하지 않는데도 비트 수중 상수성 검사를 통과하는 멤버 함수
```cpp
class TextBlock {
public:
    TextBlock(char* test)
    {
        pText = test;
    }
    // 부적절하지만 비트수준 상수성이 있어서 허용되는 operator[]의 선언
    char& operator[](size_t position) const
    {
        return pText[position];
    }
private:
    char* pText;
};

const TextBlock cctb("Hello"); // 상수 객체 선언
char* pc = &cctb[0]; // 상수 버전의 operator[]를 호출하여 cctb의 내부 데이터에 대한 포인터를 얻음
*pc = 'J'; // cctb는 "Jello"가 된다.
```

### 논리적 상수성
- 위에서 나온 특수한 상황을 보완하는 대체 개념
- **상수 멤버 함수**라고 해서 객체의 한 비트도 수정할 수 없는 것이 아니라 **일부 몇 비트** 정도는 바꿀 수 있되 그것을 사용자측에서 알아채지 못하게만 하면 **상수 멤버 자격**이 있다는 개념