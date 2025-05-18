README — Avito Recommender Experiments
======================================

Описание задачи:
----------------
Построение двухступенчатой рекомендательной системы для Avito:
1. ALS-модель (Implicit Alternating Least Squares) — формирует кандидатов на основе взаимодействий.
2. Модель ранжирования (CatBoost / LightGBM) — сортирует кандидатов по вероятности контакта.

Метрика:
--------
Основная метрика качества — Recall@40.

Содержимое:
-----------
- IM_experiments_final.ipynb — Jupyter Notebook с экспериментами и логированием в MLflow
- Функции:
    • als_predict — генерация рекомендаций
    • prepare_for_catboost — подготовка фичей для модели ранжирования
    • run_als_catboost_experiment — запуск модели CatBoost + логирование
    • run_als_lgbm_experiment — запуск модели LightGBM + логирование
    • tag_best_run — пометка лучшего run'а по метрике

Автор:
------
Igor Mozolin 
