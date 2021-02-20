# Effective C++

## 프리뷰
- [프리뷰](/Chapter0/Chapter0.md)

## C++에 왔으면 C++의 법을 따릅시다
- [항목 1. C++를 언어들의 연합체로 바라보는 안목은 필수](/Chapter1/Item1.md)
- [항목 2. #define을 쓰려거든 const, enum, inline을 떠올리자](/Chapter1/Item2.md)
- [항목 3. 낌새만 보이면 const를 들이대 보자!](/Chapter1/Item3.md)
- [항목 4. 객체를 사용하기 전에 반드시 그 객체를 초기화하자](/Chapter1/Item4.md)

## 생성자, 소멸자 대입 연산자
- [항목 5. C++가 은근슬쩍 만들어 호출해 버리는 함수들에 촉각을 세우자](/Chapter2/Item5.md)
- [항목 6. 컴파일러가 만들어낸 함수가 필요없다면 확실히 이들의 사용을 금해버리자](/Chapter2/Item6.md)
- [항목 7. 다형성을 가진 기본클래스에서는 소멸자를 반드시 가상 소멸자로 선언하자](/Chapter2/Item7.md)
- [항목 8. 예외가 소멸자를 떠나지 못하도록 붙들여 놓자](/Chapter2/Item8.md)
- [항목 9. 객체 생성 및 소멸 과정 중에는 절대로 가상 함수를 호출하지 말자](/Chapter2/Item9.md)
- [항목 10. 대입 연산자는 *this의 참조자를 반환하게 하자](/Chapter2/Item10.md)
- [항목 11. operator=에서는 자기대입에 대한 처리가 빠지지 않도록 하자](/Chapter2/Item11.md)
- [항목 12. 객체의 모든 부분을 빠짐없이 복사하자](/Chapter2/Item12.md)

## 자원 관리
- [항목 13. 자원 관리에는 객체가 그만!](/Chapter3/Item13.md)
- [항목 14. 자원 관리 클래스의 복사 동작에 대해 진지하게 고찰하자](/Chapter3/Item14.md)
- [항목 15. 자원 관리 클래스에서 관리되는 자원은 외부에서 접근할 수 있도록 하자](/Chapter3/Item15.md)
- [항목 16. new 및 delete를 사용할 때는 형태를 반드시 맞추자](/Chapter3/Item16.md)
- [항목 17. new로 생성한 객체를 스마트 포인터에 저장하는 코드는 별도의 한 문장으로 만들자](/Chapter3/Item17.md)

## 설계 및 선언
- [항목 18. 인터페이스 설계는 제대로 쓰기엔 쉽게, 엉터리로 쓰기엔 어렵게 하자](/Chapter4/Item18.md)
- [항목 19. 클래스 설계는 타입 설계와 똑같이 취급하자](/Chapter4/Item19.md)
- [항목 20. '값에 의한 전달' 보다는 '상수객체 참조자에 의한 전달' 방식을 택하는 편이 대개 낫다](/Chapter4/Item20.md)
- [항목 21. 함수에서 객체를 반환해야 할 경우에 참조자를 반환하려고 들지 말자](/Chapter4/Item21.md)
- [항목 22. 데이터 멤버가 선언될 곳은 private 영역임을 명심하자](/Chapter4/Item22.md)
- [항목 23. 멤버 함수보다는 비멤버 비프렌드 함수와 더 가까워지자](/Chapter4/Item23.md)
- [항목 24. 타입 변환이 모든 매개변수에 대해 적용되어야 한다면 비멤버 함수를 선언하자](/Chapter4/Item24.md)
- [항목 25. 예외를 던지지 않는 swap에 대한 지원도 생각해 보자](/Chapter4/Item25.md)

## 구현
- [항목 26. 변수 정의는 늦출 수 있는 데까지 늦추는 근성을 발휘하자](/Chapter5/Item26.md)
- [항목 27. 캐스팅은 절약, 또 절약! 잊지 말자](/Chapter5/Item27.md)
- [항목 28. 내부에서 사용하는 객체에 대한 '핸들'을 반환하는 코드는 되도록 피하자](/Chapter5/Item28.md)
- [항목 29. 예외 안정성이 확보되는 그날 위해 싸우고 또 싸우자!](/Chapter5/Item29.md)
- [항목 30. 인라인 함수는 미주알고주알 따져서 이해해 두자](/Chapter5/Item30.md)
- [항목 31. 파일 사이의 컴파일 의존성을 최대로 줄이자](/Chapter5/Item31.md)

## 상속, 그리고 객체 지향 설계
- [항목 32. public 상속 모형은 반드시 "is-a(...는 ...의 일종이다)"를 따르도록 만들자](/Chapter6/Item32.md)
- [항목 33. 상속된 이름을 숨기는 일은 피하자](/Chapter6/Item33.md)
- [항목 34. 인터페이스 상속과 구현 상속의 차이를 제대로 파악하고 구별하자](/Chapter6/Item34.md)
- [항목 35. 가상 함수 대신 쓸 것들도 생각해 두는 자세를 시시때때로 길러 두자](/Chapter6/Item35.md)
- [항목 36. 상속받은 비가상 함수를 파생 클래스에서 재정의하는 것은 절대 금물!](/Chapter6/Item36.md)
- [항목 37. 어떤 함수에 대해서도 상속받은 기본 매개변수 값은 절대로 재정의 하지 말자](/Chapter6/Item37.md)
- [항목 38. "has-a(...는...를 가짐)" 혹은 "is-implemented-in-terms-of(...는...를 써서 구현됨)"를 모형화할 때는 객체 합성을 사용하자](/Chapter6/Item38.md)
- [항목 39. private 상속은 심사숙고해서 구사하자](/Chapter6/Item39.md)
- [항목 40. 다중 상속은 심사숙고해서 사용하자](/Chapter6/Item40.md)

## 템플릿과 일반화 프로그래밍
- [항목 41. 템플릿 프로그래밍의 천릿길도 암시적 인터페이스와 컴파일 타임 다형성부터](/Chapter7/Item41.md)
- [항목 42. typename의 두 가지 의미를 제대로 파악하자](/Chapter7/Item42.md)
- [항목 43. 템플릿으로 만들어진 기본 클래스 안의 이름에 접근하는 방법을 알아두자](/Chapter7/Item43.md)
- [항목 44. 매개변수에 독립적인 코드는 템플릿으로부터 분리시키자](/Chapter7/Item44.md)
- [항목 45. "호환되는 모든 타입"을 받아들이는 데는 멤버 함수 템플릿이 직방!](/Chapter7/Item45.md)
- [항목 46. 타입 변환이 바람직할 경우에는 비멤버 함수를 클래스 템플릿 안에 정의해 두자](/Chapter7/Item46.md)
- [항목 47. 타입에 대한 정보가 필요하다면 특성정보 클래스를 사용하자](/Chapter7/Item47.md)
- [항목 48. 템플릿 메타프로그래밍, 하지 않겠는가?](/Chapter7/Item48.md)

## new와 delete를 내 맘대로
- [항목 49. new 처리자의 동작 원리를 제대로 이해하자](/Chapter8/Item49.md)
- [항목 50. new 및 delete를 언제 바꿔야 좋은 소리를 들을지를 파악해 두자](/Chapter8/Item50.md)
- [항목 51. new 및 delete를 작성할 때 따라야 할 기존의 관례를 잘 알아 두자](/Chapter8/Item51.md)