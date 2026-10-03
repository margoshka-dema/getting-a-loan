# Credit Scoring: Default Risk Prediction

Проект по прогнозированию риска кредитного дефолта с использованием методов машинного обучения.

## О проекте

Цель проекта — определить вероятность дефолта заёмщика на основе его финансовых и кредитных характеристик.

**Датасет:** 2000 записей, 11 признаков.

### Основные признаки

* возраст;
* доход;
* существующая задолженность;
* сумма кредита;
* кредитная история;
* количество просроченных платежей;
* количество кредитных линий;
* стаж работы;
* отношение долга к доходу;
* отношение суммы кредита к доходу.

**Целевая переменная:** `default_risk`

## Что сделано

* проведён первичный анализ и EDA;
* изучены распределения и корреляции признаков;
* выполнено разбиение данных на обучающую и тестовую выборки с сохранением баланса классов;
* проведено масштабирование признаков для Logistic Regression;
* обучены и сравнены несколько моделей классификации;
* рассчитаны основные метрики качества;
* построены Confusion Matrix и ROC-кривые;
* проведено сравнение моделей по Accuracy, Precision, Recall, F1-score и ROC-AUC.

## Модели

* Logistic Regression;
* Decision Tree;
* Random Forest.

## Результаты

| Модель              | Accuracy | Precision | Recall |     F1 | ROC-AUC |
| ------------------- | -------: | --------: | -----: | -----: | ------: |
| Logistic Regression |   0.9450 |    0.9298 | 0.8833 | 0.9060 |  0.9857 |
| Decision Tree       |   0.9000 |    0.8390 | 0.8250 | 0.8319 |  0.9050 |
| Random Forest       |   0.9275 |    0.9027 | 0.8500 | 0.8755 |  0.9748 |

В рамках проведённого эксперимента наилучшие значения метрик показала **Logistic Regression**.

## Технологии

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Plotly
* Scikit-learn
* Jupyter Notebook

## Структура проекта

```text
getting-a-loan/
├── getting_a_loan.ipynb
├── credit_data.csv
├── .gitignore
└── README.md
```

## Запуск

Клонировать репозиторий:

```bash
git clone https://github.com/margoshka-dema/getting-a-loan.git
cd getting-a-loan
```

Установить зависимости:

```bash
pip install pandas numpy matplotlib seaborn plotly scikit-learn
```

Открыть `getting_a_loan.ipynb` в Jupyter Notebook или JupyterLab и выполнить ячейки последовательно.
