# TypeScipt_Blockchain

### 타입스크립트 프로젝트에서 자바스크립트를 사용하는 방법

Declaration Files => 파일 전체를 위한 타입 정의를 생성(Declaration Files), [ myPackage.js, myPackage.d.ts ] 파일 추가! <br/>

JSDoc => 타입스크립트와 같이 작업하는 방식, tsconfin.json 파일에 CompilerOptions.allowJs : "true" 추가,
그런 다음 myPackage.js 파일 상단에 @ts-check 선언, 자바스크립트가 타입스크립트의 보호를 받을 수 있게 끔 함수 위에 코멘트를 작성 [하단 코드 참고] <br/>

Block => DefinitelyTyped : TypeScript 정의를 위한 레포지토리 https://github.com/DefinitelyTyped/DefinitelyTyped [npm i -D @types/node] 설치한 라이브러리를 타입스크립트에서 사용할 때 모듈 인식이 안되는 에러가 발생할 경우 유용함

Chain => 간단한 crypto를 사용한 해쉬 값 생성과 nodemon을 사용한 빌드 과정과 실행 과정을 단축, 블록으로 연결된 간단한 코인 생성까지 실행

// @ts-check

- Initializes the project
- @param {object} config
- @param {boolean} config.debug
- @param {string} config.url
- @returns boolean
  export function init(config) {
  return true;
  }
