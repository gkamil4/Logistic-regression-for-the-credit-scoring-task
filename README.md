# Проект по Кредитному Скорингу с использованием Логистической Регрессии

## 🎯 Задача
Целью данного проекта является разработка и подготовка модели **логистической регрессии** для задачи кредитного скоринга. Ключевая задача модели - эффективное предсказание вероятности дефолта по кредиту, обозначенного как `d4p12`.

## 💡 Реализованные Решения

В ходе работы над проектом были реализованы следующие ключевые компоненты и достигнуты результаты:

1. **Функция `woe_line` и сопутствующие инструменты**:
   - Разбиение значений признака на интервалы (бакеты).
   - Расчет WOE (Weight of Evidence) и доверительных интервалов для каждого бакета.
   - Вычисление Information Value (IV) и коэффициента R² для анализируемых признаков.

2. **Линеаризация признаков и очистка от шума**:
   - Преобразование фичей посредством линеаризации по WOE.
   - Исключение шумовых фичей из модели.

📈 Эти преобразования позволили **улучшить показатель ROC AUC модели** на тестовой выборке с `0.7` до `0.9`. Такое значительное улучшение делает модель особенно ценной для предсказания вероятности дефолта.

## 🛠 Использованные Библиотеки

Для реализации проекта были использованы следующие библиотеки:

- **`Pandas`**, **`Numpy`** для обработки и анализа данных.
- **`Sklearn`** для модели логистической регрессии.
- **`Scipy`** для logita.
- **`Plotly`**, **`Matplotlib`**, **`Seaborn`** для визуализации данных.
