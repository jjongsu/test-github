# gh-pages 사용

1. github settings pages 
branch main 생성
2. gh-pages 설치
```
npm install gh-pages --save-dev
```
3. file 수정
- package scripts
```
"predeploy": "npm run build",
"deploy": "gh-pages -d dist"
```
- package hompages
```
  "homepage": "https://jjongsu.github.io/RxJS-study/",
```
- vite.config.ts
```
export default defineConfig({
    base: '/RxJS-study/',
    plugins: [react()]
});
```
4. deploy
```
npm run predeploy
npm run deploy
```
5. github setting pages
branch gh-pages 변경
