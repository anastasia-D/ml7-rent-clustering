# Кластеризация объявлений об аренде

Учебный проект по кластеризации RentHop. Ноутбук применяет K-Means, DBSCAN, агломеративную кластеризацию и Gaussian Mixture к координатам и характеристикам объявлений.

Собственные K-Means и DBSCAN сравниваются с библиотечными алгоритмами. Метки кластеров используются как признаки для Lasso. Ноутбук сопоставляет время работы, силуэт и ошибку прогноза арендной платы.

[Открыть ноутбук](src/ml7_clustering_algorithms.ipynb)

## Данные

Распакуйте файл с обучающими объявлениями и положите его в `src/data/train.json`. Данные собраны площадкой RentHop и опубликованы в конкурсе [Two Sigma Connect: Rental Listing Inquiries](https://www.kaggle.com/competitions/two-sigma-connect-rental-listing-inquiries/data).

## Запуск в Linux или WSL

Используйте Python 3.12. Подготовьте файлы данных по указанным выше путям и выполните команды из папки проекта.

```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
cd src
jupyter lab ml7_clustering_algorithms.ipynb
```

В ноутбуке сохранены примеры данных и результаты расчётов. Чтобы повторить эксперимент, выполните ячейки по порядку в Jupyter.

Обучение на полных данных может занять несколько минут. Время зависит от процессора и настроек моделей.
