## 배운점 / 확인할 점 
* C연산자(c())의 의미?!
> 데이터 벡터화 : 행렬을 세로벡터로 바꾸는 선형변환

*  model.predict 하여 실제 예측결과 확인 \
   (normalization한 데이터셋으로 예측하면 정규화된 값이 나올것, 따라서 로그씌우기 전 값으로 돌릴수 있는가)  
  그러기 위해 다시한번 확인해야하는 로그, 자연로그 등의 개념
*  train_clean 과 train_clean_nor 의 컬럼이 일치하지 않음
*  Normalization 실행한 데이터셋을 이용하여 선형회귀를 돌리는게 맞는가?
*  회원의 유무는 독립변수로 넣으면 안되는가? (회원 + 비회원 = 총 대여량(count))
*  시계열 분석은 당장 실행하지 않으므로, datetime형태의 컬럼은 파생변수를 위한 것일 뿐, int 변환하여 선형회귀의 독립변수로 작용시키면 문제가 정말 있을까?
*  QQ plot을 그려봤을때 정규화가 거의 안됐다고 볼 수 있을만큼 미세하게 정규화된것을 확인하였다. 이에대한 문제는 어떻게 풀 수 있을것인가.
*  상관분석에 독립변수는 어떤 컬럼을 채택해야하는가
## 수행결과
1. raw data => 0.38 
2. 이상치제거 => 0.39 
3. 정규화 => 0.49
4. 'hour'에 C연산자 => 0.817 
5.  weather에 '4' 삭제 => 0.817 
6.  windspeed에 '0' 삭제 => 0.819
