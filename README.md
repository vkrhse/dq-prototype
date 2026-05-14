# DQ Prototype — Cycle 3

Interactive hi-fi prototype for the HSE master thesis
*Прозрачность качества данных в аналитических BI-системах реального времени:
визуализация актуальности данных для поддержки принятия решений*.

Reproduces the dashboard used in cycle 3 usability testing:

- Global status bar with scenario switcher (Преим. свежий / Смешанный / Деградация)
- 4 KPI widgets with dual badges (freshness + DQ)
- Revenue Over Time chart, Conversion Funnel, Revenue by Day, Top Products
- Alert about Conversion Rate approaching staleness
- Detail tooltip on hover (latency decomposition, source, DQ, threshold)
- Sliding Data Lineage panel with bottleneck callout
- Sliding DQ panel with pass-rate trend and check list
- 4-level progressive disclosure footer

Live: <https://vkrhse.github.io/dq-prototype/>

Source code of the full prototype stack (Kafka → ClickHouse → React +
freshness scanner, FastAPI, dbt-expectations) is at
<https://gitlab.com/vkrhse/dq>.
