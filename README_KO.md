# 도쿄도 코로나19 감역대책 사이트

![](https://github.com/tokyo-metropolitan-gov/covid19/workflows/production%20deploy/badge.svg)

[![도쿄도 코로나19 감역대책 사이트](https://user-images.githubusercontent.com/1301149/75629392-1d19d900-5c25-11ea-843d-2d4376e3a560.png)](https://stopcovid19.metro.tokyo.lg.jp/)

### [日本語](./README.md) | [English](./README_EN.md) | [Spanish](./README_ES.md) | Korean

## 기여방법
오픈중의 이슈를에대해 협력해주신다면 대단히 감사하겠습니다.

자세히는 [기여방법](./.github/CONTRIBUTING.md)를 참고해주세요.


## 행동강령
자세히는 [사이트 구축 행동강령](./.github/CODE_OF_CONDUCT.md)를 참고해주세요.


## 라이선스
본 소프트웨어는 [MIT라이선스](./LICENSE.txt)를 따르고 있습니다.

## 개발자 정보

### 개환경 구축순서

- 필요한 Node.js 버젼: 10.19.0이상

**yarn을 사용하는 겨우**
``` bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn dev
```

**docker compose를 사용하는경우**
```bash
# serve with hot reload at localhost:3000
$ docker-compose up --build
```

### 스테이징환경/운영환경에의 반영

`master` 브랜치가 업데이트되면, 자동적으로  `production` 브랜치의 HTML파일들이 빌드됩니다. 그후 운영환경 사이트 https://stopcovid19.metro.tokyo.lg.jp/ 가 갱신됩니다.

`staging` 브랜치가 업데이트되면, 자동적으로  `gh-pages` 브랜치의 HTML파일들이 빌드됩니다. 그후 스테이징환경 사이트 https://stg-covid19-tokyo.netlify.com/ 가 갱신됩니다.

`development` 브랜치가 업데이트되면, 자동적으로  `dev-pages` 브랜치의 HTML파일들이 빌드됩니다. 그후 개발용 사이트 https://dev-covid19-tokyo.netlify.com/ 가 갱신됩니다.
