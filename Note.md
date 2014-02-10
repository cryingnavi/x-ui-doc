---
layout: page
title : Note
header : Post Archive
group: navigation
---
{% include JB/setup %}

## 1.0.3
+ flow, roll 애니메이션 변경
+ jquery mobile과 혼용하여 사용할 수 있도록 data-role 속성을 data-ui 형태로 변경. 
+ grunt-jsdoc 설정 변경
+ CSS3 flex box 모델 도입
+ firefox, IE 11 대응
+ carousel 버그 수정

## 1.0.2
+ jsdoc 를 이용한 문서화
+ X.View 의 toobar 생성 버그 수정
+ 그 외 자잘한 버그 수정

## 1.0.1
+ Draggable Bug 수정. 문서 최상단 부터 구하던 좌표를 부모 요소로 부터 구하도록 변경
+ LayoutView 의 Spliiter가 화면 상에 잘 못 표시되던 버그 수정서
+ LayoutView 가 여러개 생성되었을 경우 상호간에 사이즈 변경시 다른 LayoutView 에게 통지되도록 변경

## 1.0.0
+ 프로젝트 첫 릴리즈

## 문제점
+ 화면 전환을 담당하는 viewController 는 URL 과 연계하여 사용할 수 없으므로 이에 대한 보강이 필요함.