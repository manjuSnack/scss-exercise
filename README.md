# SCSS-EXERCISE

This repository is that I practiced about CSS/SCSS.

# 이모티콘 기호별 간단 의미

🍩 : 현재 공부 중에 있는 지식에 대한 내용을 서술한 구간이며 정확하지 않을 수 있습니다.

🍌 : 복사, 붙여넣기한 구간이며 내용에 관해 사전 지식이 부족한 내용입니다.

🍭 : 경고나 주의 혹 에러에 대한 내용을 기술한 구간입니다.

🍘 : 서적 등을 참고하여 활용 사례에 대한 내용을 기술한 구간입니다.

🍬 : 활용면에서는 '어떠한 지' 혹 '어떠할 지'에 대한 내용을 기술한 구간입니다.

🍥, 💬 : 기타 가독성이 높이고자 구분할 때 쓴 아이콘입니다.

# 🍩 CSS / SCSS 내용

🍥 2022-12-20 ~ , 아래 SCSS 익히는 과정 중 메모

- [ ] SCSS에 원하는 폰트(잘난체, 티몬체) 등을 쓰는 방법을 익혀야 할 것
- [ ] 여러 Device에 맞는 UI/UX 디자인에 맞게 고쳐야 할 것.
- [ ] div 위에 겹쳐 다른 div를 위에 얹기

# 연습 중 참조한 사이트

- [BestHorrorScenes](https://besthorrorscenes.com/)
- [PaintBox](https://paint-box.com/)
- [Tolv](https://tolv.dk/)

# 🍩 Github commit & push

git bash 혹 WSL terminal 실행

`$ git init` : github에 연결.

`$ git remote add origin https//github.com/"username/repository"` : git repository 경로로 원격 지정. "username/repository" : 인 따옴표를 지우고 안에 있는 내용은 각자의 username과 repository name을 작성하는 구간입니다.

`$ git remote -v` : git repository 원격 상태 확인

`$ git remote rm origin` : origin이라는 remote 원격 경로 삭제

`$ git add .` : github에 올릴 작업물을 cache로 임시 저장.

`$ git status` : `git add .`로 cache로 등록한 파일 등 목록을 봅니다.

`$ git rm -r --cached .` : github에 push 하기 전 미리 올린 cache를 삭제.

`$ git commit -m "내용"` : "내용" 으로 github에 commit을 하여 저장.

`$ git branch -M main` : github에 push가 가능한 main으로 branch를 변경.

`$ git push -u origin main` : github에 최종으로 작업물을 올리는 작업.

🍭 github에 push한 결과물은 수정은 못하고 새로 덮어쓰기만 가능하니 주의할 것.

# 🍌 .gitignore setting

node.js에 대한 ignore를 작성.

```
# Logs
logs
*.log
npm-debug.log*
yarn-debug.log*
yarn-error.log*
lerna-debug.log*
.pnpm-debug.log*

# Diagnostic reports (https://nodejs.org/api/report.html)
report.[0-9]*.[0-9]*.[0-9]*.[0-9]*.json

# Runtime data
pids
*.pid
*.seed
*.pid.lock

# Directory for instrumented libs generated by jscoverage/JSCover
lib-cov

# Coverage directory used by tools like istanbul
coverage
*.lcov

# nyc test coverage
.nyc_output

# Grunt intermediate storage (https://gruntjs.com/creating-plugins#storing-task-files)
.grunt

# Bower dependency directory (https://bower.io/)
bower_components

# node-waf configuration
.lock-wscript

# Compiled binary addons (https://nodejs.org/api/addons.html)
build/Release

# Dependency directories
node_modules/
jspm_packages/

# Snowpack dependency directory (https://snowpack.dev/)
web_modules/

# TypeScript cache
*.tsbuildinfo

# Optional npm cache directory
.npm

# Optional eslint cache
.eslintcache

# Optional stylelint cache
.stylelintcache

# Microbundle cache
.rpt2_cache/
.rts2_cache_cjs/
.rts2_cache_es/
.rts2_cache_umd/

# Optional REPL history
.node_repl_history

# Output of 'npm pack'
*.tgz

# Yarn Integrity file
.yarn-integrity

# dotenv environment variable files
.env
.env.development.local
.env.test.local
.env.production.local
.env.local

# parcel-bundler cache (https://parceljs.org/)
.cache
.parcel-cache

# Next.js build output
.next
out
build
.publish

# Nuxt.js build / generate output
.nuxt
dist

# Gatsby files
.cache/
# Comment in the public line in if your project uses Gatsby and not Next.js
# https://nextjs.org/blog/next-9-1#public-directory-support
# public

# vuepress build output
.vuepress/dist

# vuepress v2.x temp and cache directory
.temp
.cache

# Docusaurus cache and generated files
.docusaurus

# Serverless directories
.serverless/

# FuseBox cache
.fusebox/

# DynamoDB Local files
.dynamodb/

# TernJS port file
.tern-port

# Stores VSCode versions used for testing VSCode extensions
.vscode-test

# yarn v2
.yarn/cache
.yarn/unplugged
.yarn/build-state.yml
.yarn/install-state.gz
.pnp.*

```
