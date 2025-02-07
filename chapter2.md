2장. 실행 컨텍스트

실행 컨텍스트는 실행할 코드 환경을 말합니다. 실행 컨텍스트는 전역 컨텍스트와 eval(이벨:평가-문자열로 된 자바스크립트 코드 실행) 및 함수 실행에 의한 컨텍스트 등이 있습니다. 실행 컨텍스트 객체는 활성화되는 시점에 VariableEnvironment, LexicalEnvironment, ThisBinding의 세 가지 정보를 수집합니다.
variableEnvironment는 실행 컨텍스트가 생성될 때 선언된 변수와 함수의 초기 상태(초기화 단계)를 저장하는 저장소입니다.
LexicalEnvironment는 현재 실행 중인 코드의 실행 범위(스코프) 내에서 변수와 함수, 그리고 블록 스코프를 포함한 식별자 정보를 저장하는 환경입니다.
실행 컨텍스트를 생성할 때는 LexicalEnvironment는 변경 사항이 즉시 반영되는 반면 VariableEnvironment는 변경 사항을 반영하지 않습니다. 
ThisBinding은 this 식별자가 바라봐야 할 대상 객체입니다.
