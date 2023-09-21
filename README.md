#include <stdio.h>

 

// Union 정의

union MyUnion {

    int intValue;

    float floatValue;

    char stringValue[20];

};

 

int main() {

    // Union 변수 선언

    union MyUnion myVar;

 

    // 데이터 할당

    myVar.intValue = 42;

    

    // 데이터 출력

    printf("정수 값: %d\n", myVar.intValue);

 

    // 다른 데이터 유형 할당

    myVar.floatValue = 3.14;

    

    // 데이터 출력

    printf("부동 소수점 값: %f\n", myVar.floatValue);

 

    // 다른 데이터 유형 할당

    strcpy(myVar.stringValue, "Hello, Union!");

    

    // 데이터 출력

    printf("문자열 값: %s\n", myVar.stringValue);

 

    return 0;

}
