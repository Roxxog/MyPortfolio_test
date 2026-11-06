---
title: "Yoonsea"
subtitle: "두 번째 모델"
date: 2025-07-01
summary: "완벽한 모델에 대한 집착"
status: complete
tags: ["Blender", "3D"]
# thumbnail: cover.png
---


## 작업 소개

캐릭터명 : 마법고 윤세아<br>
두 번째 캐릭터<br>
사용된 원본 아트의 소스 링크 : https://www.youtube.com/watch?v=xIcxxcdKIyU (제작사인 어썸피스의 제작자의 개인 블로그에 올라온 마법고 제작 비하인드에 대해 정리한 영상에서 사진을 참고자료로 사용함, 사진의 라이선스는 확인할 수 없음)

## 이미지

{{< beautifulfigure src="윤세아 원본 일러스트.png" caption="원본 캐릭터를 만든 게임 회사의 초기 아트 모습" >}}<br>
{{< beautifulfigure src="yoonsea2.png" caption="얼굴 토폴로지 수정 중 사진" >}}<br>
{{< beautifulfigure src="yoonsea3.png" caption="전체 실루엣" >}}<br>
{{< beautifulfigure src="yoonsea1.png" caption="Shader 적용 전" >}}<br>
{{< beautifulfigure src="yoonsea.png" caption="Shader 적용 후" >}}<br>
{{< beautifulfigure src="yoonseaShaderTest.png" caption="Shader 테스트" >}}<br>
{{< beautifulfigure src="yoonseaShaderTest1.png" caption="Shader 테스트" >}}<br>


## 제작 과정
제작 기간 : 약 2개월 (시작일은 date 참고)<br>
기존의 문제였던 최적화되지 않은 폴리곤, 애니메이션에 적합하지 않은 토폴로지 등을 수정한 새로운 모델을 만들고자 하였다.<br>
그 결과 얼굴, 무릅 등의 근육이 움직이는 부분들의 모델링을 공부하여 개선하고 기존의 Shader를 공부하며 새로운 Shader노드들의 결합을 시도하였다.<br>
학업과 블랜더를 병행하며 2개월 정도의 기간 동안 제작하였다.


## 개선 방향
폴리곤 수를 감축한 것은 좋지만 얼굴 실루엣 등의 중요 부위에서 부드럽지 않고 각지는 문제가 있다. 이 문제는 최적화가 중요한 게임, VRChat 등에서 쓰이는 캐릭터를 만드는 전문가들이 만드는 모델과 비교하여 얼굴의 윤곽과 같이 캐릭터에게 있어서 중요한 부분과 몸통과 같이 비교적 덜 중요한 부분을 확인하고 적절히 폴리곤의 수를 할당하는 방법에 대해서 배운 후 수정할 계획이다.


## 결과

모델링을 할 때 애니메이션을 고려하여 적은 폴리곤으로 모델을 최적화하고 움직일 때 캐릭터가 뭉개지지 않은 토폴로지를 구성하는 법을 본격적으로 배우고 특히 Shader에 대해 관심을 가지기 시작한 계기가 되었다.<br>
하지만 이 때부터 최적화가 완벽한 모델의 집착이 시작되었으며 현재 까지 이어지는 정체기의 시작이라고 할 수 있다.
