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

- [스프레드시트 링크](https://docs.google.com/spreadsheets/d/1tAolHvdSZUqzN1v54wQQhXsosJQsSVjXHvc1UjUMKPA/edit#gid=0)
<br>

## 🚩사용 기술 및 기능 구현
#### → Javascript, HTML, CSS, Webpack

- **바닐라 자바스크립트**로 전체 기능 구현
- **fetch API**와 **promise**를 사용하여 서버로부터 데이터 패치 
- 모바일 웹에 어울리는 **모바일 웹 UI** 구현
- **스크롤 이벤트**로 스크롤 위치 값에 있는 시간대에 따라 미세먼지 정보 렌더링 
- div 태그에 css를 적용하여 미세먼지 데이터를 막대 그래프 구현

<br>
<br>



## 🚩서비스 기능
- 현재 시간을 기준으로 24시간동안 가까운 측정소의 대기질 측정 결과를 미세먼지 등급과 함께 볼 수 있습니다.
- 미세먼지 예보 정보와, 지역별 미세먼지 등급, 대기질 예보 이미지를 확인할 수 있습니다.
- 여러장의 예보 이미지를 움직이는 애니메이션으로 볼 수 있습니다. 
<br>

## 🚩설계
- 함수형으로 진행
- 스켈레톤 코드를 짜놓고 기능 개발을 진행
- 메인 함수를 만들어 각각 만들어둔 기능을 init하도록 구성
- 각 기능은 init함수와 render함수를 가지고 있음

<br>

## 🚩회고
- 순수함수로 구현하기가 어렵다. 전역변수를 사용했는데 전역변수 없이 함수형 프로그래밍을 구현하는 방법을 더 생각해봐야겠다. 
<br>

