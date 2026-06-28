# SQL_game_analytics
## Курсовая работа по модулю обучения основам SQL
____
**Цель работы** - собрать результаты технических заданий в единую структуру

**Легенда:** на протяжении нескольких месяцев я анализировала игру Zombie Revolution, ее популярность и монетезацию.
Ожидаемый результат - кратно и информативно рассказать менеджерам какие у игры метрики и какие результаты показали маркетинговые активности

*Структура курсовой:*

  *Описание количества игроков, количества сессий, средней длины сессий.
  
  *Доля проблемных записей для каждого типа устройства,процент проблемных записей Android, iOS.
  
  *Базовые метрики: MAU, DAU, WAU, Sticky Factor Weekly
  
  *Финансовые показатели в разных срезах, результаты акции.
  
  *Дополнительные монетарные расчеты.
  
  *Алгоритм нахождения лояльных пользователей, метрики по ним.

**Формат курсовой** - PowerPoint. Было необходимо представить видео с защитой, презентацию, по которой проводилась защита

Использован диалект ***PostgreSQL***:
```SQL
select count (*) as cnt
	, count (id_user) as cnt_reg
	, count (distinct id_user) as cnt_user
from skygame.users
```
[Обучение проходило на базе](https://sky.pro/?utm_source=yandex&utm_medium=cpc&utm_campaign=n_brand_search_main_ru_yandex_709604634%7Cpl_search%7Cpr_171%7Cta_cold%7Cfu_main_landing%7Cma_academtraff%7Cown_b2c%7Cchg_performance&utm_content=ai_17709664395%7Cagi_5747788104%7Cci_709604634%7Cpi_57158656976%7Cse_yandex.ru&utm_term=search%7Ckwd_skypro=&roistat=direct1_search_17709664395_skypro&roistat_referrer=yandex.ru&roistat_pos=premium_1&etext=&yclid=1072145688725553151)
