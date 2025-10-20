# Bank-Customer-Churn-Prediction
# 🏦 Bank Customer Churn Prediction

## 📘 Описание
Проект посвящён анализу поведения клиентов банка и прогнозированию их оттока с помощью моделей машинного обучения.

**Источник данных:** [Kaggle Dataset](https://www.kaggle.com/datasets/shubhammeshram579/bank-customer-churn-prediction)

## 📊 Основные этапы
- Предобработка данных
- Балансировка классов
- Анализ корреляций и визуализация признаков
- Обучение моделей: Logistic Regression, RandomForest, XGBoost
- Сравнение метрик ROC-AUC, Accuracy, R²

## 🧠 Результаты
| Модель | ROC-AUC | Accuracy |
|--------|----------|-----------|
| Logistic Regression | 0.78 | 0.79 |
| Random Forest | 0.86 | 0.85 |
| XGBoost | 0.85 | 0.84 |

## 📈 Важные графики
![Feature Importance](images/feature_importance.png)
![ROC Curve](images/roc_curve.png)
![Correlation Heatmap](images/correlation_heatmap.png)

## 💡 Выводы
- На отток клиентов влияют возраст, активность и количество продуктов.
- Сбалансированная модель RandomForest обеспечивает наилучшее качество прогноза.

# 🏦 Bank Customer Churn Prediction

## 📋 Описание
Проект по предсказанию оттока клиентов банка. 
Задача — классифицировать, покинет ли клиент банк, на основе демографических и финансовых признаков.

## 📊 Содержание
- EDA и визуализация
- Phik корреляции для категориальных и числовых признаков
- Балансировка классов (downsampling)
- Обучение моделей: Logistic Regression, RandomForest, XGBoost
- Подбор гиперпараметров через GridSearchCV
- Сравнение train/test метрик, ROC и PR кривые
- SHAP-анализ для объяснимости модели
- Сохранение артефактов и итоговые выводы

## 🧠 Основные результаты
- Лучшая модель: **XGBoost (AUC ≈ 0.87)**
- Ключевые факторы оттока:
  - `Age` — риск оттока растёт с возрастом.
  - `NumOfProducts` — клиенты с 3–4 продуктами уходят чаще.
  - `IsActiveMember` — активность клиента сильно снижает риск.
  - `BalanceGeoDiff` — отклонение баланса от среднего по стране.

## 💾 Структура проекта
