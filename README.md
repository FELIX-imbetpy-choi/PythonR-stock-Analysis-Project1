# 주가 지수 현황 분석 및 예측

주가 DATA 출처 : http://www.krx.co.kr   
환율 DATA 출처 : http://www.smbs.biz    
라면가격 DATA 출처 : http://www.price.go.kr    
재무제표 DATA 출처 : http://comp.fnguide.com¶     


## 1) 연도별 각 기업 주가 및 환율 분석
### ① 종가 히스토그램 및 분위수 그림
<img src="https://github.com/FELIX-imbetpy-choi/Python-stock-Analysis-Project1/blob/master/project-1.png?raw=true" width="500" height="500"> 

> 히스토그램으로 확인한 결과 종가 데이터가 정규분포가 아닌 것을 확인  
분위수 그림 확인 결과 마찬가지로 정규분포가 아닌 것을 확인  

`※분위수 그림이란?`  
대각선(qqline())을 기준으로 산점도 점들이  
가깝게 선형을 이루며 붙어 있으면 정규성을 보인다고 평가하고  
그렇지 않으면 정규성을 띠지 않는다고 보는 것  

### ② 종가 / 시가총액 추세 비교

<img src="https://github.com/FELIX-imbetpy-choi/Python-stock-Analysis-Project1/blob/master/project-2.png?raw=true" width="500" height="500"> 

> 농심은 종가와 시가총액 모두 감소하는 추세를 보여주는 반면 오뚜기와 삼양은 증가하는 추세

### ③ 환율과 거래량 추세 비교
<img src="https://github.com/FELIX-imbetpy-choi/Python-stock-Analysis-Project1/blob/master/project-3.png?raw=true" width="500" height="500"> 

> 환율이 증가(원화가치 약세)하게 되면 외국인 투자자들은 대부분 주식을 매도 할 것이다.
반대로 환율이 감소(원화가치 강세)하게 되면 외국인 투자자들은 주식을 매수 할 것이다.
매도/매수 가 얼마나 됐는지는 거래량을 보고 알 수 있는데,
2014 ~ 2016년간 달러화 환율이 점차 증가 -> 주식의 거래량 또한 증가 하는것을 알 수 있다.
즉 환율이 증가해 원화가치가 떨어져 많은 외국인 투자자들이 주식을 매도하기 시작 한 것이다.

> 하지만 환율이 하락하는 구간인 2016 ~ 2017년에 삼양의 거래량이 높게 올랐다. 이 구간은 위안화 환율과 연관이 있는데
2017년 삼양식품은 중국 업체와 중국 총판에 대한 업무협약을 맺었으며, 엄청난 양의 신제품을 쏟아내기 시작하였다.
그 신제품은 삼양의 대표 판매제품이라고 할 수 있는 불닭볶음면의 여러가지 시리즈 제품이였다.
이미 성공을 맛 본 제품이기 때문에 그에 따른 시리즈 제품들 또한 성공할 확률이 높았다고 판단 한 것이다.
이러한 소식에 많은 투자자들이 주식을 매수 한 것이다.

### ④ 각 기업의 주가는 서로에게 영향을 미칠까
<img src="https://github.com/FELIX-imbetpy-choi/Python-stock-Analysis-Project1/blob/master/project-4.png?raw=true" width="500" height="500"> 
추세 역시 오뚜기와 농심은 비슷한 형태의 추세를 보여주고 있다.
<img src="https://github.com/FELIX-imbetpy-choi/Python-stock-Analysis-Project1/blob/master/project-5.png?raw=true" width="500" height="500"> 

....

## 중간생략

....

## 3) 삼양 데이터 추론 및 예측

<img src="https://github.com/FELIX-imbetpy-choi/Python-stock-Analysis-Project1/blob/master/project-7.PNG?raw=true" width="500" height="500"> 


<img src="https://github.com/FELIX-imbetpy-choi/Python-stock-Analysis-Project1/blob/master/project-6.png?raw=true" width="500" height="500"> 


<img src="https://github.com/FELIX-imbetpy-choi/Python-stock-Analysis-Project1/blob/master/project-8.PNG?raw=true" width="500" height="500"> 


## 분석 후기 및 한계점
> 약 일주일에 걸친 주가 분석을 해보았다. 현황 분석은 어느 정도 할 수 있었지만  
회귀분석을 하는 과정에서 많은 어려움을 겪었는데. 종속변수가 되는 종가 데이터가 정규분포를 이루지 않았기 때문이다.  
물론 로그변환 등 다른 방법을 통하여 정규화 시킬 수 있었지만 주가 데이터를 정규화 시킨다는 것은 데이터의 오류라고 판단  
따라서 샘플링을 통해 정규분포를 맞추고 회귀분석을 실시하였는데 데이터의 수가 너무 작았기 때문에  
이 분석 결과가 높은 신뢰도를 가진다고 말할 수는 없다.  
결론적으로 내가 하고자 싶은 정확한 예측은 불가능했지만, 현황 분석을 통해  
내가 선택한 세 기업의 전반적인 주식 흐름을 알 수 있었고 분석에 대한 지식을 더 높일 수 있는 계기가 되는 프로젝트였다.  
다음 주가 분석을 할때는 외국 기업을 대상으로 주가 분석을 해보고 싶다.  

