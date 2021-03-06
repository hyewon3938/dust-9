<h1 align="center">미세먼지 서비스</h1>
<p align="center"><strong>☁ 미세먼지 정보를 제공하는 모바일 웹 서비스입니다 ☁</strong></p>
<br>
<p align="center"><img src="https://user-images.githubusercontent.com/58355499/98921222-5e80b900-2514-11eb-8fd3-917011ce9f48.gif"/>
  <img src="https://user-images.githubusercontent.com/58355499/98921188-57f24180-2514-11eb-92ec-eb6b2d53a4bd.gif"/></p>
<br>
<br>

## 🚩프로젝트 진행 
- 개발 기간 : 2주 <br>
- 개발 인원 : FE(2) BE(1) iOS(1) <br>
- 담당 : 프론트엔드 개발 (미세먼지 탭)

<br>

## 🚩요구사항 분석 스프레드시트 
> 요구사항을 분석하여 feature 단위로 개발해야 할 기능 정리 후 코드 구현 여부, 구현 코드 반영여부를 기록

→ [스프레드시트 링크](https://docs.google.com/spreadsheets/d/1tAolHvdSZUqzN1v54wQQhXsosJQsSVjXHvc1UjUMKPA/edit#gid=0)

<br>

## 🚩사용 기술 및 기능 구현
→ ``` Javascript, HTML, CSS, Webpack ```

- **Vanilla Javascript**로 전체 기능 구현
- **fetch API**와 **promise**를 사용하여 서버로부터 데이터 패치 
- 모바일 화면에 어울리는 **모바일 웹 UI** 구현
- **스크롤 이벤트**로 스크롤 위치 값에 있는 시간대에 따라 미세먼지 데이터를 등급별 지정된 스타일로 렌더링 
- div 태그에 css를 적용하여 미세먼지 데이터를 이용한 **막대 그래프 구현**

<br>
<br>



## 🚩서비스 기능
- 현재 시간을 기준으로 24시간동안 가까운 측정소의 대기질 측정 결과를 미세먼지 등급과 함께 볼 수 있습니다.
- 미세먼지 예보 정보와, 지역별 미세먼지 등급, 대기질 예보 이미지를 확인할 수 있습니다.
- 여러장의 예보 이미지를 움직이는 애니메이션으로 볼 수 있습니다. 
<br>

## 🚩설계
- [이슈 링크](https://github.com/codesquad-member-2020/dust-9/issues?q=is%3Aopen+is%3Aissue)
- 폴더구조
```
.
├─javascript
│  ├─constants
│  ├─data
│  ├─dustCondition
│  ├─dustForecast
│  ├─navigation
│  └─util
├─page
└─style
    └─common
        └─lib
```
- 전체 화면을 상단의 navigation, 미세먼지탭 dustCondition, 미세먼지 예보 dustForecast 이렇게 총 **세가지 컴포넌트로 나누어 구성**
- 코드 전체를 **함수로 진행**
- 기능 개발에 들어가기 전 **스켈레톤 코드**를 짜놓은 후에 기능 개발을 진행
- **메인 함수**를 만들어 각각 만들어둔 **컴포넌트의 함수를 init**하도록 구성
- 각 컴포넌트 함수는 **init함수**와 **render함수**를 가지고 있음

<br>

## 🚩회고
- 클래스로만 설계하다 처음으로 함수형을 적용해보았는데 어설픈 함수형이지만 새로운 도전이었다. 순수함수로 구현하고 싶었지만 전체적으로 사용하는 데이터를 어떻게 관리해야할지 몰라 전역변수를 이용했다. 전역변수 없이 함수형 프로그래밍을 구현할 수 있도록 더 고민하고 공부해야할 것 같다.
<br>

- 이번에도 마감시간까지 시간이 부족했지만 전 프로젝트보다 비교적 계획한대로 개발을 진행한 것 같아 뿌듯하다. 
<br>

- fetch 함수에서 try-catch를 이용해 예외처리를 하지 못해서 아쉬웠다.
<br>

- 다음에는 다양한 기기에서 사용할 수 있는 반응형 모바일 웹을 위해 미디어쿼리를 더 공부해야겠다.
<br>

- 사용자 위치의 좌표값을 알아내기 위해 **geoloation API**를 사용했는데, 개발환경에서는 잘 동작했지만 배포 환경에서는 동작하지 않았다. 이유를 찾아보니 gelocation API는 localhost와 https 환경이 아니면 사용할 수 없었다. 데모 전날 배포단계에서 발견한 문제였기 때문에 좌표값을 알아내는 다른 API를 찾아 적용할 시간이 부족해 고정된 좌표값을 넣어 데모를 진행했다. 
개발 단계에서는 알 수 없었지만 배포 이후에 문제가 발생하는 변수를 항상 염두에 두고 개발을 진행하며 배포를 미리미리 해봐야한다는 걸 몸소 체험했다.   
<br>

