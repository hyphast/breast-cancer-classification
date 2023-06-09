<br />
<div align="center">
  <h2 align="center">Рак молочной железы</h2>

  <p align="center">
    Модель классификации для определения доброкачественных и злокачественных опухолей молочной железы
    <br />
    <a href="https://ru.wikipedia.org/wiki/%D0%A0%D0%B0%D0%BA_%D0%BC%D0%BE%D0%BB%D0%BE%D1%87%D0%BD%D0%BE%D0%B9_%D0%B6%D0%B5%D0%BB%D0%B5%D0%B7%D1%8B">Рак молочной железы</a>
  </p>
</div>

## Цель

Разработка модели, которая на основе измерений различных характеристик, сможет классифицировать новые образцы ткани молочной железы на злокачественные и доброкачественные опухоли.

## Задачи

1. анализ существующих решений;
2. сбор данных и их обновление;
3. обучение и оценка моделей на исходном датасете;
4. выбор двух моделей с наибольшим значением точности;
5. оценка качества и скорости работы модели на новых комментариях путем A / B тестирования;
6. выбор и развертывание наилучшей модели;
7. оптимизация выбранной модели путем квантизации и дистилляции;
8. развертывание оптимизированной модели, количественная оценка эффекта оптимизации.

## Датасет

**[Breast Cancer Wisconsin (Diagnostic) Data Set](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data?resource=download)**

Датасет "Breast Cancer Wisconsin (Diagnostic)" содержит информацию об измерениях различных характеристик клеток молочной железы, в том числе и их формы, размерах ядер и текстуре.
Особенностью данного датасета является то, что он содержит относительно небольшое количество наблюдений (569), но большое количество признаков (30).

## Проект

**[Breast Cancer Classification](https://github.com/hyphast/breast-cancer-classification)**

## Целесообразность использования датасета

Датасет Breast Cancer Wisconsin (Diagnostic) был широко использован в исследованиях и задачах классификации рака молочной железы. Его использование продолжает быть актуальным для улучшения точности диагностики и прогнозирования данного заболевания. Гистограммы, построенные по четырем параметрам, показывают, что существуют выбросы, особенно для параметра area_mean (Рис. 1). Параметры `radius_mean` и `perimeter_mean` имеют похожие распределения, с другой стороны `texture_mean` и `area_mean` отличаются, это может говорить о том, что они содержат более разнообразную информацию о данных. Диаграммы, демонстрируют целесообразность решения задачи анализа данных на выбранном датасете методами машинного обучения.

![Гистограммы](assets/gists.png 'Гистограммы для параметоров radius_mean, texture_mean, perimeter_mean, area_mean')
Рис. 1. Гистограммы для параметоров radius_mean, texture_mean, perimeter_mean и area_mean
