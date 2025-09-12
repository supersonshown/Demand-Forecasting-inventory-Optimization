# Demand-Forecasting-inventory-Optimization
---

## 2. 유통판매량 예측 및 재고 최적화
```markdown
# 📊 Demand Forecasting & Inventory Optimization
> LSTM 기반 시계열 분석을 통한 유통업체 재고 관리 효율화

![Time Series Analysis](./images/demand_forecast.png)

## 📌 프로젝트 개요
LSTM 모델을 활용하여 유통업체의 판매량을 예측하고 재고를 최적화하는 시계열 분석 프로젝트입니다.

## 🎯 주요 성과
- **RMSE**: 16.6 달성 (우수한 예측 성능)
- **R² Score**: 0.49 (CNN 대비 향상)
- **패턴 발견**: 금/토요일, 12월 방문 피크 패턴 식별

## 🛠 기술 스택
- **Model**: LSTM, CNN (비교 분석)
- **Framework**: TensorFlow, Scikit-learn
- **Analysis**: Pandas, NumPy
- **Visualization**: Matplotlib

## 📊 데이터 분석

### 시기별 패턴 분석
![Seasonal Pattern](./images/seasonal_pattern.png)

- **요일별 패턴**: 금요일, 토요일 방문자 수 증가
- **월별 패턴**: 12월 판매량 급증
- **연도별 추세**: 지속적인 성장세

## 🔬 모델 비교

| Model | RMSE | R² Score | 특징 |
|-------|------|----------|------|
| LSTM | 16.6 | 0.49 | 장기 의존성 학습 우수 |
| CNN | 높음 | 낮음 | 지역적 패턴만 추출 |

![Model Comparison](./images/model_comparison.png)

## 💻 코드 예시

### 데이터 전처리
```python
def preprocess_data(df):
    # 시계열 데이터 정규화
    # 요일, 월별 특성 추출
    # 트레인/테스트 분할
    return X_train, X_test, y_train, y_test
