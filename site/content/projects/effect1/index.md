---
title: "effect1"
subtitle: "첫 이펙트 제작"
date: 2026-07-07
summary: "드라이버 + Shader"
status: none
tags: ["Blender", "3D", effect]
thumbnail: effect1 2026-11-07 184035.png
---


## 작업 소개

캐릭터명 : effect1<br>
캐릭터는 아니며 하나의 프로젝트이다<br>
처음으로 블랜더의 기능인 Driver와 Shader를 결합하여 만들 수 있는 효과를 구현하였다.


## 이미지

{{< beautifulfigure src="effect1 2026-11-07 184035.png" caption="전체 실루엣" >}}<br>
{{< beautifulfigure src="effect1_Shader 2026-11-07 184102.png" caption="사용된 Shader 노드 구조" >}}<br>


## 영상

{{< video src="effect1 2026-11-07 184158.mp4" caption="구현된 효과" >}}<br>


## 제작 과정

약 2일 동안 진행된 프로젝트로 애니메이션을 만들기 위해 추가로 포함되어야할 이펙트 효과를 처음으로 구현해보았다. 특히 블랜더에서 제공하는 함수를 이용하는 방법인 Driver를 Shader노드에 적용하여 프레임마다 상태가 변화하는 효과를 처음으로 구현하였다.

## 개선 방향

만들어진 이펙트는 방향이 아래에서 위로 올라가는 쪽으로만 구현되어 있어. 애니메이션에서는 방향을 원하는 방향으로 통제 가능하게 만들어야 한다. 그러므로 빈 오브젝트 등의 회전 값을 Driver를 통해서 제어할 수 있게 바꿀 예정이다.

## 결과

처음으로 Shader노드 안에 특정 수치가 아닌 변수를 넣었다. 이는 앞으로 여러 애니메이션 효과 또는 애니메이션을 통제하는데 있어서 있어서 매우 중요한 개념으로 Driver를 Shader 이외에 여러 고정된 수치들 대신 적용하여 더욱 다양한 효과를 구현하는 것의 시작이 될 것이다.
