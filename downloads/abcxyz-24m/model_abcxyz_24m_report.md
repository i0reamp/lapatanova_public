# ABC × XYZ по моделям за 24 месяца

Период: `2024-03-14 — 2026-03-14`

## Что собрано

- [abcxyz_models_24m.csv](/srv/workspaces/lapatanova/analysis/abcxyz_models_24m_2026-03-14/abcxyz_models_24m.csv)
- [action_matrix_summary_24m.csv](/srv/workspaces/lapatanova/analysis/abcxyz_models_24m_2026-03-14/action_matrix_summary_24m.csv)
- [abcxyz_matrix_summary_24m.csv](/srv/workspaces/lapatanova/analysis/abcxyz_models_24m_2026-03-14/abcxyz_matrix_summary_24m.csv)
- [scale_candidates_24m.csv](/srv/workspaces/lapatanova/analysis/abcxyz_models_24m_2026-03-14/scale_candidates_24m.csv)
- [optimize_candidates_24m.csv](/srv/workspaces/lapatanova/analysis/abcxyz_models_24m_2026-03-14/optimize_candidates_24m.csv)
- [exit_candidates_24m.csv](/srv/workspaces/lapatanova/analysis/abcxyz_models_24m_2026-03-14/exit_candidates_24m.csv)
- [summary.json](/srv/workspaces/lapatanova/analysis/abcxyz_models_24m_2026-03-14/summary.json)

## Метод

- ABC берётся из модели по выручке за 24 месяца.
- XYZ считается по месячным продажам за последние 24 календарных месяца (`2024-04` ... `2026-03`).
- Порог XYZ оставлен консистентным с предыдущим fashion-слоем: `X <= 150.0%`, `Y <= 250.0%`, `Z > 250.0%` по коэффициенту вариации.
- Модель без цвета строится по тому же правилу, что и в 24-месячном ABC-отчёте.
- Себестоимость является расчётной моделью: `30%` от фактической цены продажи.
- Stock layer агрегирован по текущему `style_master`; показатель `stock_cover_days_est_12m` считает покрытие от скорости продаж последних 12 месяцев.

## XYZ-сводка

- `X`: `78` моделей
- `Y`: `256` моделей
- `Z`: `349` моделей

## ABCXYZ-матрица

| ABCXYZ | Моделей | Выручка 24M | Доля выручки % |
| --- | --- | --- | --- |
| AX | 60 | 14153831.55 | 33.53 |
| AY | 119 | 16470142.34 | 39.01 |
| AZ | 39 | 3192194.00 | 7.56 |
| BX | 17 | 558923.68 | 1.32 |
| BY | 100 | 3182465.87 | 7.54 |
| BZ | 87 | 2554399.20 | 6.05 |
| CX | 1 | 10385.00 | 0.02 |
| CY | 37 | 396571.68 | 0.94 |
| CZ | 223 | 1696937.20 | 4.02 |

## Action Matrix

| Действие | Моделей | Выручка 24M | Доля выручки % |
| --- | --- | --- | --- |
| clearance_or_exit | 260 | 2093508.88 | 4.96 |
| optimize_colors_and_keep | 100 | 2997032.27 | 7.10 |
| keep_winner_colors | 94 | 11525964.42 | 27.30 |
| reduce_depth_keep_model | 90 | 15205076.28 | 36.02 |
| optimize_colors_and_markdown | 87 | 2739832.80 | 6.49 |
| replenish_and_scale | 30 | 4915789.34 | 11.64 |
| protect_and_repeat | 21 | 2728261.53 | 6.46 |
| keep_small_depth | 1 | 10385.00 | 0.02 |

## Top модели для роста

| Модель | Категория | ABCXYZ | Stock | Выручка 24M | Действие |
| --- | --- | --- | --- | --- | --- |
| Джемпер чешуйки оверсайз | knitwear | AX | stockout | 576574.00 | replenish_and_scale |
| Рубашка джинсовая женская | tops_blouses | AY | stockout | 518723.90 | keep_winner_colors |
| Бомбер женский | outerwear | AY | stockout | 491816.00 | keep_winner_colors |
| Свитер кострома | knitwear | AX | balanced | 462492.41 | protect_and_repeat |
| Тренч женский | outerwear | AY | stockout | 432514.00 | keep_winner_colors |
| Палантин трикотажный листочки | accessories | AX | balanced | 426183.99 | protect_and_repeat |
| Джемпер сердечки | knitwear | AX | stockout | 415268.00 | replenish_and_scale |
| Джемпер грибочки мужской | knitwear | AX | understock | 402266.00 | replenish_and_scale |
| Джинсы-бананы | pants | AX | understock | 364242.60 | replenish_and_scale |
| Рубашка из тенсела женская | tops_blouses | AY | stockout | 310482.00 | keep_winner_colors |
| Брюки классика вискоза | pants | AX | balanced | 297988.00 | protect_and_repeat |
| Кардиган чешуйки жаккард | knitwear | AX | stockout | 289640.00 | replenish_and_scale |
| Пальто женское оверсайз | outerwear | AY | stockout | 288832.00 | keep_winner_colors |
| Джемпер чешуйки двусторонний | knitwear | AX | stockout | 281731.50 | replenish_and_scale |
| Джемпер джаред оверсайз | knitwear | AX | stockout | 266742.00 | replenish_and_scale |
| Пальто шерстяное двубортное с поясом | outerwear | AX | stockout | 259175.00 | replenish_and_scale |
| Брюки палаццо вискоза | pants | AX | stockout | 242164.36 | replenish_and_scale |
| Юбка трикотажная в рубчик макси | skirts | AX | balanced | 231753.00 | protect_and_repeat |
| Бомбер женский изумрудный в клетку | outerwear | AY | stockout | 226055.00 | keep_winner_colors |
| Пальто шерсятное двубортное с поясом | outerwear | AY | stockout | 223125.00 | keep_winner_colors |

## Top модели для оптимизации и выхода

| Модель | Категория | ABCXYZ | Stock | Выручка 24M | Действие |
| --- | --- | --- | --- | --- | --- |
| Шапка взрослая | accessories | AX | overstock | 1212108.60 | reduce_depth_keep_model |
| Рубашка женская из тенсела | tops_blouses | AX | overstock | 1002936.00 | reduce_depth_keep_model |
| Джемпер женский грибочки | knitwear | AX | overstock | 572722.00 | reduce_depth_keep_model |
| Футболка трикотажная косичка | tshirts_longsleeves | AX | overstock | 560170.00 | reduce_depth_keep_model |
| Шапка взрослая шерсть | accessories | AX | overstock | 446831.98 | reduce_depth_keep_model |
| Шарф взрослый | accessories | AX | overstock | 446327.00 | reduce_depth_keep_model |
| Юбка мерилин из тенсела | skirts | AY | overstock | 430882.00 | reduce_depth_keep_model |
| Юбка трикотажная ажур листочки | skirts | AY | overstock | 415562.00 | reduce_depth_keep_model |
| Брюки трикотаж | pants | AX | overstock | 396082.00 | reduce_depth_keep_model |
| Джемпер в рубчик укороченный | knitwear | AX | overstock | 281514.10 | reduce_depth_keep_model |
| Шорты льняные | pants | AY | overstock | 278926.00 | reduce_depth_keep_model |
| Блуза с воротом стойка из тенсела | tops_blouses | AZ | overstock | 278065.00 | reduce_depth_keep_model |
| Жилет льняной | knitwear | AY | overstock | 240758.00 | reduce_depth_keep_model |
| Брюки палаццо льняные | pants | AY | overstock | 238460.00 | reduce_depth_keep_model |
| Джемпер джеки интерлок | knitwear | AX | overstock | 232356.00 | reduce_depth_keep_model |
| Жакет прямого кроя с карманами | jackets_blazers | AX | overstock | 228836.00 | reduce_depth_keep_model |
| Джемпер чешуйки двусторонний морская волна | knitwear | AX | overstock | 218624.00 | reduce_depth_keep_model |
| Джемпер авангард жаккард | knitwear | AY | overstock | 217630.00 | reduce_depth_keep_model |
| Платье ариэль макси искусственный шелк | dresses | AY | overstock | 204824.00 | reduce_depth_keep_model |
| Платье трикотажное ажур колоски макси | dresses | AY | overstock | 199960.00 | reduce_depth_keep_model |

## Краткий стратегический вывод

- Ядро бизнеса сейчас лучше всего читать через слой `AX/AY/BX`: именно там сидит repeat-core и второй эшелон для масштабирования.
- Модели с действием `replenish_and_scale` и `protect_and_repeat` формируют `28.84%` выручки в верхнем списке кандидатов на рост.
- Слой `AZ/BZ/CZ` нельзя вести как базу: это fashion-хвост и волатильные модели, которые нужно держать малой глубиной и через winner-based подход.
- Для развития бизнеса дальше логика должна быть такой: расширять `AX/BX`, аккуратно развивать `AY`, жёстко оптимизировать цвета в `BY/BZ`, выводить `CY/CZ`.