# TypeScipt_Blockchain

### 타입스크립트 프로젝트에서 자바스크립트를 사용하는 방법
firstCommit => 파일 전체를 위한 타입 정의를 생성(Declaration Files), [ myPackage.js, myPackage.d.ts ] 파일 추가!
JSDoc => 타입스크립트와 같이 작업하는 방식, tsconfin.json 파일에 CompilerOptions.allowJs : "true" 추가,
그런 다음 myPackage.js 파일 상단에 @ts-check 선언, 자바스크립트가 타입스크립트의 보호를 받을 수 있게 끔 함수 위에 코멘트를 작성 [하단 코드 참고]
          
// @ts-check
/**
 * Initializes the project
 * @param {object} config
 * @param {boolean} config.debug
 * @param {string} config.url
 * @returns boolean
 */
export function init(config) {
  return true;
}
