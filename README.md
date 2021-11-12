# ☂️ **배추 가격 예측 인공지능 소프트웨어**

### 🔥 프로젝트 배경

![인플레이션](https://user-images.githubusercontent.com/56535821/141412968-44d719d2-391d-4302-9549-cf05ae2cacce.PNG)

최근 급격한 인플레이션으로 물가가 폭등하고 있다는 뉴스를 접한 경험이 있습니다. 배추 등 농식품도 예외는 아닙니다.
비록 이번 사태는 코로나라는 예기치 못한 사고로 인한 나비효과 이지만, 이러한 상황을 통해 프로젝트 아이디어를 도출해 낼 수 있었습니다. 

**바로 여러 data를 활용해서 농수산물의 가격을 예측할 수 있지 않을까? 라는 생각입니다.**

알아보니 DACON이라는 경진대회 사이트에서도 이와 비슷한 대회가 진행 중이었습니다.<br>


[따라서](https://github.com/jangsik-park/Heroku/blob/main/README.md) 이번 프로젝트를 통해 농산물의 가격을 예측하는 기본 AI 모델을 만들고
이를 발판 삼아 추후에 경진대회에 참여해보자!!<br>

라는 생각으로 해당 프로젝트를 진행하게 되었습니다.

추가적으로는 모델을 탑재한 웹페이지를 제작하고, 이를 배포해보는 것까지 진행했습니다.

<hr>

### 🔥 프로젝트 목표
1. [다중 선형회귀를 활용한 AI 모델 만들기](#)
2. [웹페이지 제작 (Flask)](#)
3. [배포 (with Heroku)](https://github.com/jangsik-park/Heroku/blob/main/README.md)
4. [경진대회 도전](#)


<hr>

### 🔥 AI모델 , 환경 , 언어

- 다중 선형회귀 모델
- EDA => ```Google Colab```
- 모델 학습 => ```VScode, GitBash, Python, tensorflow```
- 웹페이지 제작 => ```VScode, HTML, Javascript, Python```
- 배포 = > ```Heroku``` 

<hr>

### 🔥 DATA

자료는 
[기상자료개방포털 다중지점통계](https://data.kma.go.kr/climate/StatisticsDivision/selectStatisticsDivision.do?pgmNo=158)와
[농산물유통정보](https://www.kamis.or.kr/customer/price/retail/period.do?action=daily)
로부터 얻었습니다.

기간은 2010년부터 2017년까지 7년 동안으로 설정했고,<br> 
**총 2,900개**의 데이터를 수집하였습니다.

![image](https://user-images.githubusercontent.com/56535821/141423560-b3e3f423-7404-4d32-ae69-3d97e33579ce.png)
<br>

변수는 그림에서 알 수 있듯이 5개(평균 온도, 최저온도, 최고온도, 강수량, 평균 풍속)를 사용했고, <br>
target 변수는 배추의 평균 가격입니다.

[EDA](#)

### 🔥 활용 아이디어

정부에서 농수산물의 예측된 가격을 활용하여 원활한 유통을 이끌어 낼 수 있습니다. <br>
농가에서는 미리 예측된 가격을 통해 재정관리를 더 효과적으로 할 수 있을 것 같습니다. <br>


<hr>

### 🔥 참고 문헌
* [기상청 전국 기온 및 강수량](https://data.kma.go.kr/climate/StatisticsDivision/selectStatisticsDivision.do?pgmNo=158) : 기상청 정보를 토대로 채소 가격에 영향을 미치는 요인을 분석하기 위해 참고하였습니다.
* [월별 배추 가격](https://www.kamis.or.kr/customer/price/retail/period.do?action=monthly&yyyy=2018&period=10&countycode=&itemcategorycode=200&itemcode=211&kindcode=&productrankcode=&convert_kg_yn=N) : 실질적인 국내 월별 배추 가격을 분석하기 위해 참고하였습니다.
* [동빈나 유튜브](https://www.youtube.com/c/dongbinna) : 동빈나님의 유튜븡 영상을 참고 함.
