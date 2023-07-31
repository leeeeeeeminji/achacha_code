# 🚌 Achacha!
![image](https://github.com/leeeeeeeminji/achacha_code/assets/87288893/ddba97de-6975-4b41-9177-091fe1c99b0c)

<br>

##  📘 프로그램 소개
<p>
<b>"achacha!"</b> 는 <b>어린이 승합차량 갇힘 사고를 예방하기 위해 제작</b>된 서비스입니다. 
</p>
<p>
승합차량의 문이 열릴 때, 아이의 얼굴을 인식하고 각 어린이의 승/하차 여부를 확인합니다 <br>
실시간으로 진행되는 승/하차 인원 체크는 운전자에게 각 인원의 수를 빠르게 알려주어, 인원 관리에 큰 편의를 제공합니다. <br>
또한, 차량에 남아 있는 인원 수를 마지막으로 비교하면서, 만약 차량 안에 사람이 남아 있는 경우, <br>
자동으로 비상벨을 울려 다른 보호자들과 운전자에게 즉각적인 대응을 도와줍니다. <br>
이를 통해 차량 갇힘 사고를 예방하고 어린이들의 안전을 도모합니다. <br>
뿐만 아니라, 텔레그램 서비스를 통해 안전함을 높이고 불안함을 줄일 수 있습니다. 
</p>
<br>
<p>
  <b>어린이 승합차량 갇힘사고 웹 서비스 코드</b><br>
  https://github.com/leeeeeeeminji/achacha_web
</p>
<br>

## 📌 문제 인식 & 기획 의도
- #### 어린이 승합차량 관련 사고 증가
  <img width="800" alt="image" src="https://github.com/leeeeeeeminji/achacha_code/assets/87288893/99e57511-50f2-4251-b67e-6086b00c4fb8">

- #### 기존 정책의 한계점
  <img width="800" alt="image" src="https://github.com/leeeeeeeminji/achacha_code/assets/87288893/fd28dea6-258e-4a18-a231-65788d6ad15c">

- #### 어린이 안전 사고 예방의 필요성
  <img width="800" alt="image" src="https://github.com/leeeeeeeminji/achacha_code/assets/87288893/33a0e887-0efd-4e03-826e-e096712e709b">
<br>

## 📅 개발 기간
### 2021.08.01 - 2021.09.10

<br>

## ⚙ 개발 환경
#### ✔ 사용 언어
<div>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=Python&logoColor=white" />
  <img src="https://img.shields.io/badge/R-276DC3?style=flat&logo=R&logoColor=white" />
</div>

#### ✔ 사용 툴
<div>
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=Jupyter&logoColor=white"/>
  <img src="https://img.shields.io/badge/VisualStudio-5C2D91?style=flat&logo=VisualStudio&logoColor=white"/>
</div>

<br>

## 🖋 개발 과정
#### 1️⃣ 실험 설계 - 배경
<img width="500" alt="image" src="https://github.com/leeeeeeeminji/achacha_code/assets/87288893/1c4d2426-9a2d-4bbc-bd35-f30cfdcc2481">
  <div>
    본격적인 실험 설계를 하기에 앞서 차량 갇힘 사고의 주된 대상자인 어린이의 특성에 대해 알아보았습니다. <br>
    이 특성 중, 아직 정신적으로 성숙하지 않은 어린이는 보이지 않는 것은 없다고 생각하며, <br>
    구석진 곳에서 노는 경향이 강하게 나타난다는 특성에 주목하여 실험을 설계하였습니다. 
  </div>
<br><br>

#### 2️⃣ 실험 설계 - 사각지대 비교, 방법 선정
![image](https://github.com/leeeeeeeminji/achacha_code/assets/87288893/3652d982-39d5-4a5f-afac-9170acaf06b6)
<div>
  사각지대 비교를 위해 고정된 6대의 카메라를 이용하여 다양한 각도로 조원들을 촬영하였습니다.<br>
  가운데 그림에서 빨간색 점은 카메라의 위치이고, 노란색 점은 어린이라고 가정하였습니다. <br>
  각각 사진은 사람이 4명이 앉아있으나 파란색 동그라미로 볼 수 있듯 사람이 있으나 카메라에 잡히지 않는 사각지대가 존재하였습니다. <br>
  사각지대를 없애기 위해서는 최소 6대의 카메라가 필요하다는 것을 알 수 있었고, 비용 문제로 현실적인 해결책으로 사용하기 어렵다고 판단하였습니다.
</div>
<br>

![image](https://github.com/leeeeeeeminji/achacha_code/assets/87288893/0161ea04-91cd-4dbf-9729-f3f86cff1a92)
<div>
  따라서, 모바일 기기에 내장된 카메라를 이용해 차량 입구에서 승/하차 인식을 통해 명확하게 인원을 파악하는 방법을 선정했습니다. <br>
</div>
<br>

#### 3️⃣ 분석 흐름도
![image](https://github.com/leeeeeeeminji/achacha_code/assets/87288893/1fa0e3e0-55af-4d59-aba7-40d4f5129c7e)
<br>

#### 4️⃣ 데이터
#### 4️⃣-1️⃣ 데이터 수집
![image](https://github.com/leeeeeeeminji/achacha_code/assets/87288893/85ecb6ef-e18d-4a57-95c8-53375c3523c4)
<div>
 얼굴 인식에 필요한 이미지를 학습히기 위해 약 400여장의 조원들의 얼굴 데이터를 수집하였습니다. <br>
얼굴 인식의 정확도를 높이기위해 다양한 각도에서 촬영하였습니다.
</div>
<br>

#### 4️⃣-2️⃣ 데이터 전처리
![image](https://github.com/leeeeeeeminji/achacha_code/assets/87288893/1e5845ba-5de4-4f24-80f2-6956ca84741b)
<div>
  정확한 얼굴 인식을 위해 머신러닝 기반의 얼굴 검출 알고리즘인 'harr casecade'를 통해 얼굴 부분만 크롭하였습니다. <br>
  그 다음, 노이즈 제거를 위해 양방향 필터를 적용하였습니다. 양방향 필터는 수식을 사용해 기준 픽셀과 이웃 픽셀과의 거리 그리고 픽셀 값의 차이를 함께 고려하여 블러링 정도를 조정합니다.
</div>

![image](https://github.com/leeeeeeeminji/achacha_code/assets/87288893/0e942cb0-1dff-4472-8f8e-a3d3af27ead9)
<div>
  마지막으로 이상치 제거 과정을 거쳐 약 100장의 Train Data 를 얻었습니다.
</div>
<br>

#### 5️⃣ 얼굴 인식
![image](https://github.com/leeeeeeeminji/achacha_code/assets/87288893/4e0c4bb3-80dc-4586-bd67-17f61d4d5d15)
<div>
  python의 OpenCV 라이브러리와 Face Recognition, Dlib 패키지를 사용하여 얼굴 인식 코드를 작성하였습니다. <br>
  1) 먼저 인식된 얼굴을 흑백으로 변환한 후, 주변 픽셀들과 비교한 다음에 16*16 크기 픽셀로 분해합니다.
</div>
<br>

![image](https://github.com/leeeeeeeminji/achacha_code/assets/87288893/501968a1-3b96-4249-bfad-14849527a8d9)
<div>
  2) 분해한 픽셀을 이용해 얼굴에 존재하는 68개의 특정 포인트를 찾아내고 기계학습 알고리즘을 충분히 훈련시켜 어떤 얼굴에서든 68개의 특정 포인트를 찾아낼 수 있게 합니다.
</div>
<br>

![image](https://github.com/leeeeeeeminji/achacha_code/assets/87288893/999065b9-e2f0-4cb9-99b2-cd7c81fed278)
<div>
  3) 찾아낸 68개의 특정 포인트를 사용해 얼굴 이미지로부터 128개의 측정값을 얻습니다. <br><br>
이 측정값을 이용해 특정 인물로 분류할 수 있습니다.<br>
배경이나 각도가 다른 사진일지라도, 같은 인물이라면 거의 동일한 측정값을 가졌기에 동일한 사람으로 인식합니다.

</div>
<br>

#### 분석 결과
![image](https://github.com/leeeeeeeminji/achacha_code/assets/87288893/c48c59b4-2060-42d6-a935-7dadf857844a)
<br>

#### 6️⃣ 서비스
![image](https://github.com/leeeeeeeminji/achacha_code/assets/87288893/76b65584-0511-4aab-a713-e42b098db400)
<div>
  얼굴 인식이 성공적으로 될 경우, 승하차 인원을 카운트하고, 승하차 음성 알림, 동시에 텔레그램으로 학부모님께 메시지 전송까지 되도록 구현하였습니다. 
</div>


## 💬 소감
