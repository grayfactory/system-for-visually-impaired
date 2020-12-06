<a href="https://www.youtube.com/watch?v=qxElChg70Ck">
  <img src="https://user-images.githubusercontent.com/45448731/101240773-bb971580-3734-11eb-8306-26d3920e593f.png"/>
</a>

▲클릭하시면 소개 영상을 볼 수 있습니다. 
<br><br>
 

[코드 실행 방법](https://github.com/minji-o-j/system-for-visually-impaired/blob/master/How%20to%20Use(%ED%95%9C%EA%B5%AD%EC%96%B4).md)

---
![HitCount](http://hits.dwyl.com/minji-o-j/system-for-visually-impaired.svg)
[　](https://github.com/ML-DL-Study/system-for-visually-impaired/compare/master...minji-o-j:master)


## 개발기간
20/04~20/12 

## 개발자
이름|Github|비고
----|---|---
김성현|[@Seong-Hyun-0224](https://github.com/Seong-Hyun-0224)|
김한솔|[@hansol0118](https://github.com/hansol0118)| 
윤대호|[@201810788](https://github.com/201810788)|~2020/06
이혜인|[@hyeinlee725](https://github.com/hyeinlee725)|~2020/08
정민지|[@minji-o-j](https://github.com/minji-o-j)|


## 목적 및 필요성

# 그림 너무 작고 줄글 복붙하지말고 간단하게 잘 정리 (1학기 ppt에 넣었던 이미지도 넣고....)
![image](https://user-images.githubusercontent.com/61938029/101277513-586eb700-37f8-11eb-84a7-e6b07f126280.png)
<점자블록 없는 횡단보도>

![image](https://user-images.githubusercontent.com/61938029/101277552-9bc92580-37f8-11eb-933e-eefaef446cdc.png)
<고장 난 음향신호기>

올해 서울 강북구에서 시각 장애인의 보행 시 필요한 점자블록, 횡단보도 시각장애인용 음향 신호기를 점검한 결과 설치되어 있는 곳이 현저히 적고, 설치되어 있는 곳조차 법적 기준을 지키지 않아 미흡하게 설치된 곳이 많았습니다. 또한 관리가 제대로 되어있지 않아 음향 신호기의 버튼이 눌리지 않거나 소리가 작은 문제 등이 있어 많은 시각장애인들이 보행에 큰 어려움을 겪고 있습니다.

이러한 현실의 문제를 해결하기 위해 저희는 본 시스템을 구상하였습니다.
기존 시각장애인의 보행을 돕기 위한 도구로 개발된 스마트 지팡이, 내비게이션 등이 개발되고 있지만, 상용화가 되진 않았습니다. 무엇보다 지팡이라는 물체는 움직임 등의 한계로 인하여 인지 가능 범위가 제한되고, 시각 장애인을 위한 내비게이션의 경우 점자블록과 비콘이 설치된 곳에서만 이용할 수 있다는 한계가 있습니다.

저희의 시스템은 사용 장소의 한계가 없다는 점에서 기존 시스템의 상용화 되지 못한 문제점들을 보완하여 실용성을 높였습니다. 또한 카메라를 이용하여 횡단보도를 사전에 감지하고, 신호등 색을 알려주는 기능 또한 제공함으로써 기존에 음향 신호기를 이용하기 위해서 버튼을 찾아서 눌러야 하는 등의 시각 장애인들의 도보 불편을 해소하는 데 도움을 줄 것으로 예상합니다.


## 기대효과
한국장애인재활협회에서 시각 장애인을 대상으로 한 설문 조사 결과 횡단보도와 신호등 위치를 예측하기 어려움, 음향 신호기의 위치 찾기가 어려움, 신호등의 녹색 적색 여부를 알기 어려움 등의 문제들을 겪고 있다고 응답하였습니다. 저희의 도보 환경 알림이 서비스는 이러한 점들을 해결하기 위해 음향 신호기 버튼을 누르지 않아도 횡단보도, 신호등, 그리고 신호등의 색상을 검출하여 알려준다면 앞서 시각장애인이 겪는 문제들을 크게 해소할 수 있을 것이라 예상합니다.

또한 본 서비스에 보행 시 부딪힐 위험이 있는 장애물들을 검출하는 기능 등을 추가한다면 시각장애인 보행 문제 뿐 아니라 다른 문제들, 예를 들어 청와대 국민 청원에 등장한 시각 장애인들의 버스 승차를 가능하게 해달라는 것 등의 문제 해결에도 적용할 수 있을 것이라고 생각합니다. 이외에도 본 기술을 자율 주행 서비스에 적용하는 등 더 넓은 범위에도 적용할 수 있다고 생각합니다.

## 사용 프로그램
![image](https://user-images.githubusercontent.com/45448731/101232065-c5982480-36f2-11eb-894f-bb80c7f722a4.png)
---
## 사용 모델
### 1차 모델 (20/04~20/05): [YOLOv2](https://github.com/minji-o-j/system-for-visually-impaired/tree/master/v.1.0_YOLOv2(~200529))  
- 잘 안된 사진 넣기
<br>

### 2차 모델(20/08~20/12) : YOLOv4
- YOLOv4모델에 대한 설명 적는다
ppt에 있는 yolov4에 결합되었던것들 언급후적기 : 우리 모델 설명을 영상에서 자세히 안해서 여기서 좀 자세히?

---
## 알고리즘
### 신호등 색상 검출 알고리즘  
### 도보 환경 알리미 알고리즘  
---
## 시연 영상
- 유튜브 링크 이미지로바꿔서 넣기  
https://www.youtube.com/watch?v=AHQ358YE6tY  
https://youtu.be/q3KLPQ416m8  
