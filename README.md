# react-plain-setting

## 설명
쌩 바닥에서부터 세팅한 React

## 구성
### dependencies
- react: React 컴포넌트 생성
- react-dom: DOM에 컴포넌트 내용을 적용

### devDependencies
- webpack: 바벨을 이용해 빌드 + html에 적용
- webpack-cli: webpack 커맨드 사용
- webpack-dev-server: 개발서버 작동
- html-webpack-plugin: html에 번들을 삽입
- babel-loader: webpack에서 사용하는 로더
- @babel/preset-react: React용 플러그인 프리셋

### 실행 방식
빌드: npm run build 실행. /dist 폴더에 결과물 출력
개발서버 실행: npm run dev 실행. 파일이 변경되면 자동으로 적용.

### 작동 플로우 (npm run build 시)
1. webpack 커맨드를 실행
2. webpack이 public/index.html과 src/index.jsx를 가져옴.
3. babel이 @babel/preset-react를 근거로 es5 코드로 변환
4. html-webpack-plugin이 index.html에 변환된 코드 삽입
5. webpack이 /dist 폴더에 결과물 출력
