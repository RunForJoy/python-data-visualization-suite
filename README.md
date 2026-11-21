# Data Visualization with Matplotlib, Seaborn & Plotly

[English](#english) | [Русский](#русский)

---

## English

A comprehensive data visualization project analyzing user behavior on an educational platform by querying **SQLite** databases via **Pandas** and building static, statistical, and animated charts across **Matplotlib**, **Seaborn**, and **Plotly**.

### Tech Stack & Tools
* **Visualization Libraries:** `matplotlib`, `seaborn`, `plotly` (`graph_objects`), `pandas.plotting`
* **Data Processing & Storage:** `pandas`, `numpy`, `sqlite3` (SQL queries)
* **Environment:** Jupyter Notebook

### Project Structure (`src/`)

* **`ex00/00_line_chart.ipynb`** — **Basic Line Chart:** Querying daily pageview counts from SQLite and plotting time-series dynamics with custom figure sizing, font styling, and rotated axis ticks.
* **`ex01/01_line_chart_styles.ipynb`** — **Styled Multi-Series Line Chart:** Overlaying daily pageviews and code submission commits on shared active dates with custom line styles, markers, and grid formatting.
* **`ex02/02_bar_chart.ipynb`** — **Stacked Bar Chart by Time of Day:** Categorizing user commits into four daily intervals (`night`, `morning`, `afternoon`, `evening`) and visualizing temporal shifts across dates.
* **`ex03/03_bar_charts.ipynb`** — **Grouped Bar Charts (Weekdays vs. Weekends):** Aggregating average hourly commit activity on working days versus weekends to uncover behavioral patterns.
* **`ex04/04_histogram.ipynb`** — **Overlapping Histograms:** Comparing absolute hourly commit distributions between weekdays and weekends with transparency (`alpha=0.7`) and custom palettes.
* **`ex05/05_boxplot.ipynb`** — **Boxplot & Variance Analysis:** Visualizing distribution spread, medians, Interquartile Range (`IQR`), and outliers for `test` and `control` cohorts before and after the Newsfeed rollout.
* **`ex06/06_scatter_matrix.ipynb`** — **Scatter Matrix & KDE:** Exploring non-linear relationships and distributions across pageviews, commit counts, and average deadline deltas using `scatter_matrix` with Kernel Density Estimation diagonals.
* **`ex07/07_heatmap.ipynb`** — **Activity Heatmaps:** Building multi-panel user activity heatmaps across days of the week and hours of the day using `mpl_toolkits.axes_grid1` colorbars.
* **`ex08/08_seaborn.ipynb`** — **Cumulative Line Plot with Seaborn:** Tracking cumulative project commit trajectories per user over time using styled `seaborn` line plots.
* **`ex09/09_plotly.ipynb`** — **Animated Line Race with Plotly:** Creating an interactive animated line chart (`plotly.graph_objects`) illustrating user commit progression frame by frame.

### Usage
* Place the SQLite database inside `src/data/` and open any notebook in Jupyter Lab / Jupyter Notebook or VS Code: `jupyter notebook src/ex09/09_plotly.ipynb`

---

## Русский

Комплексный проект по визуализации данных, посвящённый анализу поведения пользователей образовательной платформы на основе запросов к базе данных **SQLite** через **Pandas** и построения статических, статистических и анимированных графиков в **Matplotlib**, **Seaborn** и **Plotly**.

### Стек и инструменты
* **Библиотеки визуализации:** `matplotlib`, `seaborn`, `plotly` (`graph_objects`), `pandas.plotting`
* **Обработка данных и БД:** `pandas`, `numpy`, `sqlite3` (SQL-запросы)
* **Среда разработки:** Jupyter Notebook

### Структура проекта (`src/`)

* **`ex00/00_line_chart.ipynb`** — **Базовый линейный график:** Выгрузка ежедневных посещений из SQLite и построение временного ряда с настройкой размеров графика, шрифтов и поворота подписей оси X.
* **`ex01/01_line_chart_styles.ipynb`** — **Стилизованный многорядный линейный график:** Совмещение динамики просмотров ленты и коммитов на общих датах с настройкой стилей линий, маркеров и сетки.
* **`ex02/02_bar_chart.ipynb`** — **Столбчатая диаграмма с накоплением по времени суток:** Разбиение коммитов на четыре временных интервала (`night`, `morning`, `afternoon`, `evening`) и анализ изменения активности по дням.
* **`ex03/03_bar_charts.ipynb`** — **Сгруппированные столбчатые диаграммы (будни и выходные):** Сравнение среднего почасового числа коммитов в рабочие и выходные дни для выявления паттернов активности.
* **`ex04/04_histogram.ipynb`** — **Наложенные гистограммы:** Сопоставление абсолютного распределения коммитов по часам в будни и выходные с настройкой прозрачности (`alpha=0.7`) и цветовой палитры.
* **`ex05/05_boxplot.ipynb`** — **Диаграмма размаха (Boxplot):** Анализ разброса значений, медиан, межквартильного размаха (`IQR`) и выбросов в группах `test` и `control` до и после запуска ленты новостей.
* **`ex06/06_scatter_matrix.ipynb`** — **Матрица диаграмм рассеяния (Scatter Matrix):** Исследование нелинейных зависимостей и плотностей распределения (`KDE`) между числом просмотров, количеством коммитов и средней дельтой до дедлайна.
* **`ex07/07_heatmap.ipynb`** — **Тепловые карты активности (Heatmap):** Построение парных тепловых карт коммитов по дням недели и часам суток с настройкой цветовых шкал через `mpl_toolkits.axes_grid1`.
* **`ex08/08_seaborn.ipynb`** — **Накопительный линейный график в Seaborn:** Визуализация динамики роста числа коммитов по пользователям в ходе командного проекта с помощью `seaborn`.
* **`ex09/09_plotly.ipynb`** — **Анимированный график в Plotly:** Создание интерактивной анимации гонки коммитов (`plotly.graph_objects`) с покадровым отображением прогресса пользователей.

### Запуск
* Поместите файл базы данных SQLite в директорию `src/data/` и откройте нужный ноутбук в Jupyter Notebook / Jupyter Lab или VS Code: `jupyter notebook src/ex09/09_plotly.ipynb`
