# Практические работы № 1–6 по машинному обучению — уровень B

**Студент:** Barsbek Konurbaev  
**Дисциплина:** Машинное обучение  
**Основа заданий:** УМК Salymbekov University, Часть 3А, практические работы № 1–6, уровень B.

## Структура

```text
pr-7-ai-practices-1-6/
├── data/
│   └── README.md
├── notebooks/
│   ├── pr1_environment_and_first_notebook.ipynb
│   ├── pr2_eda.ipynb
│   ├── pr3_preprocessing_pipeline.ipynb
│   ├── pr4_regression.ipynb
│   ├── pr5_classification_threshold.ipynb
│   └── pr6_text_classification.ipynb
├── README.md
└── requirements.txt
```

## Использованные датасеты — все реальные

1. **Практика 1:** Wine Dataset из `scikit-learn` — загружается локально из библиотеки.
2. **Практики 2–3:** UCI Adult Census Income — реальные переписные данные с пропусками и числовыми/категориальными признаками. Требуется интернет.
3. **Практика 4:** Diabetes Dataset из `scikit-learn` — реальный набор для регрессии, загружается локально.
4. **Практика 5:** Breast Cancer Wisconsin (Diagnostic) из `scikit-learn` — реальный набор для бинарной классификации, загружается локально.
5. **Практика 6:** UCI SMS Spam Collection — реальный корпус текстовых сообщений, загружается с UCI; требуется интернет.

Синтетические датасеты не используются. Папка `data/` хранит пояснение об источниках; данные из `scikit-learn` берутся из установленной библиотеки, а Adult и SMS загружаются из источников в момент выполнения notebook.

## Установка

Python 3.10–3.12 рекомендуется.

```bash
python -m venv .venv
```

Windows PowerShell:
```powershell
.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
```

Linux / WSL:
```bash
source .venv/bin/activate
python -m pip install -r requirements.txt
```

Затем откройте нужный notebook в Jupyter, VS Code или Google Colab. Для практик 2, 3 и 6 требуется интернет.

## Перед сдачей

- Выполнить все ячейки сверху вниз (`Restart & Run All`).
- Проверить, что таблицы и графики сформировались.
- Вписать итоговые выводы по фактическим значениям метрик и наблюдениям.
- Сохранить результаты выполнения в notebook.
- Указать ФИО в README.

## Соответствие уровню B

- ПР-1: самостоятельный первичный анализ и минимум два графика.
- ПР-2: EDA, корреляции, редкие категории, дисбаланс и отчёт о проблемах.
- ПР-3: ColumnTransformer/Pipeline, стратегии обработки и проверка размерностей.
- ПР-4: мультиколлинеарность, полный/сокращённый набор признаков, метрики и остатки.
- ПР-5: predict_proba, ROC/PR, AUC и подбор порога по стоимости ошибок.
- ПР-6: очистка, TF-IDF, классификатор и анализ пяти ошибок.
