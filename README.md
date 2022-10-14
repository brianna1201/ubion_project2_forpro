# FORPRO 'KOSDAQ 시장 대상 관리종목 지정예측모델을 활용한 Factor 투자 전략 검증'
:trophy: 2022 Ubion 프로젝트2 우수상
## 프로젝트 소개
 본연구는관리종목을기업부실로삼고관리종목지정을예측하여,투자유니버스에서부실한기업을 제외함으로써안정성을높인수익률검증을목적으로한다. 관리종목으로 지정되었다는 사실 자체는 그 기업의 경영상태가 건실하지 못하다는 점을 의미하기 때문에 관리종목 지정은 주가 하락으로 연결되며, 나아가 상장폐지의 위험에 노출되어 있다는 신호로 작용하게 된다.<br>
 
 따라서 상장폐지 이전에 관리종목 지정기업을 예측함으로써, 사전에 주가 하락을 방지하고 안정성을 높이고자 하였다. 예측방법으로는 연도 기준 train:test(8:2) 로 데이터셋을 구분하여 머신러닝(LR, DT, SVM, RF, LGBM, XGB, SV, Stacking Ensemble) 과 딥러닝(DNN) 을 활용하였다. 이를 통해 예측된 관리종목으로 지정될 기업을 투자 유니버스에서 제거한 후, 이어 데이터를 활용하여 퀀트 투자전략을 통해 수익성 개선을 검증하였다.<br>
 
 관리종목 지정예측 기업을 포함한 투자와 제외한 투자의 수익률을 비교하여, 투자유니버스에서 관리종목 기업을 제외하는 것이 안정성과 동시에 수익성이 보다 개선되는 것을 확인하고자 하였다. 검증방법으로는 기업 가치와 관련된 퀀트의 팩터 전략을 활용하였다. 이를 통해 관리종목 지정예측기업을 제외하였을 때 CAGR과 MDD값은 유지되는 반면 수익성이 향상되는 것을 검증하였다.

## 구조
### 1. 데이터 전처리 
### 2.1. Feature Selection
- T-TEST
- Lasso
- Stepwise
### 2.2. Feature Selection_over sampling version
- SMOTENC
- T-TEST
- Lasso
- Stepwise
### 3.1. Modeling
- 머신러닝(LR, DT, SVM, RF, LGBM, XGB, SV, Stacking Ensemble)
- 딥러닝(DNN)
### 3.2. Modeling_over sampling version
- SMOTENC
- 머신러닝(LR, DT, SVM, RF, LGBM, XGB, SV, Stacking Ensemble)
- 딥러닝(DNN)
### 4. Quant factor modeling
- Size factor
- Value factor
- Quality factor
- Value & Quality factor
- Momentum factor
- Low vol factor<br>
(코스닥은 10년동안 배당주는 기업 73개에 불과, 2012,2013년에는 배당주 없음 → 제외)

## Team members
- [강동화](https://github.com/Donghwaa)
- [박해완](https://github.com/parkhaewan)
- [이민재](https://github.com/mzaeee)
