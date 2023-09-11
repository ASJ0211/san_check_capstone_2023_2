# san_check_capstone
#산 CHECK

## 날씨를 통한 산악사고 위험도 예측
- 2023 데이터 활용 부산관광 아이디어 공모전 출품작
- 기간: ‘23년 4월 ~ ‘23년 06월(3개월)
- 성과: 117팀 중 동상(3등) 수상 
- Tools: R, Qgis
- 활용 데이터
  - 소방청 산악사고 데이터 (2010~2021)
  - 기상청 종관 기상 관측 정보 데이터(2010~2021)
<br>


## 1️⃣ 개요
날씨에 따른 산악사고 위험도를 예측하고 수치화 하는 플랫폼을 만들어 산악사고를 예방하고, 피해를 줄이고자 한다.

<br>

## 2️⃣ 문제 재정의
날씨에 따른 산악사고 위험도를 산별로 예측하고 학습된 모델과 날씨 데이터를 결합해 당일의 각 산들의 위험도를 수치화하여 지도상에 표시하는 플랫폼을 개발해, 산악사고의 발생을 예측, 피해를 줄이고자 한다.

<br>

## 3️⃣ 과정 

❶문제정의 ❷데이터 수집 및 가공 ❸데이터 분석 ❹모델학습 ❺플랫폼 개발 ❻사업화


### 👤역할
기획, 데이터 수집,데이터 전처리, API 연동 , 모델 개발, 뉴스 크롤링
<br>

### 🧐 Main Issues
2010~2021년까지의 데이터를 활용했는데 날씨데이터, 산악 사고 데이터 모두 기간이 길어서 중간에 데이터의 저장 형식이 바뀌는 경우가 있어 그러한 부분을 통일시키는 과정에 어려움이 있었습니다.
전처리 과정에서 데이터들을 형식을 통일하는데 많은 시간을 사용했습니다. 
날씨 데이터의 변수들이 많고 결측치의 비율이 높아 전처리 과정에 많은 시간을 사용하였습니다.
또한 날씨 데이터 변수들 중 실제로 연관성이 있는 변수들을 골라내는 것이 어려웠습니다. 

### 🛠️ Resolved
데이터 EDA를 통해 기타산악, 산악기타가 동일한 사고 코드임을 확인 후 테이터 통합을 진행하였음. 
데이터 EDA를 통해 날씨 데이터 결측치 비율을 확인하고 결측치가 높은 column을 드랍하였음.
관측지점명, 관측지역을 통해 날씨데이터와 산악사고 데이터를 결합하여 사용하였음.

<br>

### 🎯 Result
비가오면 산악사고 발생이 증가할것이라는 예측과 달리 오히려 산행인구가 감소하여 산악사고 발생이 감소하는 경향이 발견되었습니다.
비가오면 산악사고 발생이 증가할 것이라는 가설이 틀렸다는 것을 확인하였음.
<br>
### ⭐ Learnd Lessons
날씨 API를 활용하여 실시간 날씨를 불러와 지도에 맵핑하는 것을 경험해 보았고,
tensorflow를 활용해 학습시킨 모델을 저장해 활용해 보는 방식을 배웠음.
keras를 활용해 웹페이지를 개발하고 데이터들을 시각화 하는 것을 경험하였음.
빅데이터를 전처리하고 결측치를 제거하는 것을 경험하였음.

<br>
<br>

<div class="image-container">
  <img src="https://user-images.githubusercontent.com/93497667/232216526-99e27c85-daac-4a25-b49a-73c3848aaf25.jpg" alt="image"  width="400"/>
  <img src="https://user-images.githubusercontent.com/93497667/232216651-c00ad08b-0d94-43ef-998b-8851b734d169.jpg" alt="image"  width="400"/>
</div>


- [커널밀도분석(KDE)](https://www.notion.so/TMP-e977f66c09ee453b9e2c05d3869ff5e9?pvs=4)


산악사고 예방을 위한
![image](https://github.com/ASJ0211/san_check_capstone/assets/118821779/e617747e-76be-4533-9875-a5dbb964a96d)
![image](https://github.com/ASJ0211/san_check_capstone/assets/118821779/a49ed31c-329a-42d2-bca2-648c467538ae)
![image](https://github.com/ASJ0211/san_check_capstone/assets/118821779/5092e90a-588d-4f8c-a467-b0935fc458e6)

![image](https://github.com/ASJ0211/san_check_capstone/assets/118821779/2678fc3a-7858-4d7f-9e90-f203e8d4f1b7)
![image](https://github.com/ASJ0211/san_check_capstone/assets/118821779/ebc56223-912c-45f4-aa8b-85fb19f808f4)
![image](https://github.com/ASJ0211/san_check_capstone/assets/118821779/a44165aa-76c3-4704-a4da-c3a0535d06f6)

