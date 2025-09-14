# Interactive Map of the Komi Republic

A web application for visualizing socio-economic indicators and infrastructure objects in the Komi Republic. The map is implemented in **JavaScript** using **D3.js**, **Chart.js**, and the **Canvas API**.

## Features
- Display of municipal boundaries and infrastructure objects:
  - settlements, roads, railways, buildings, churches, terminals, beaches, parking lots, wetlands, rivers, etc.;
- Two display themes: **day** and **night**;
- Loading and rendering of GeoJSON maps for each district;
- Object highlighting on mouse hover with tooltips showing names;
- Clicking on an object opens an **information box** with data from **Wikidata** (type, population, area, foundation date, flag, coat of arms, etc.);
- Integration with **Overpass API** to obtain Wikidata IDs from OSM IDs;
- Connection to local socio-economic datasets (JSON files in `data/sorted/`), including:
  - education, housing, agriculture, culture, sports, budget, employment, and more;
- Building **tables and charts** (Chart.js) for selected regions with available indicators.

## Controls
- 🔍 **Zoom & Pan**: mouse wheel and drag-and-drop (implemented with `d3.zoom`);
- 🌓 **Theme switch**: button in the top-right corner (day/night);
- ☰ **Menu controls**:  
  - text buttons to toggle individual layers (e.g. roads, buildings, rivers);  
  - icon-based buttons as an alternative way to control layers;  
  - “enable all maps” button to show all layers at once;
- 🖱 **Left click on object**: opens an info box with Wikidata data and the social indicators tab;  
- 🖱 **Right click on map**: shows author information;  
- 📊 **Social indicators**:  
  - list of available files (education, healthcare, culture, etc.);  
  - year-by-year tables;  
  - dynamic charts of selected metrics.

## Technologies
- **D3.js** — projections, GeoJSON handling, zoom & pan;
- **Canvas API** — custom map and object rendering;
- **Chart.js** — visualization of socio-economic indicators;
- **Overpass API, Wikidata API** — retrieving object metadata;
- **Vanilla JS + CSS** — custom UI (tooltips, menus, switches, icons).

------------------------------------------------------------

# Интерактивная карта Республики Коми

Веб-приложение для визуализации социально-экономических показателей и объектов инфраструктуры на карте Республики Коми. Карта реализована на **JavaScript** с использованием **D3.js**, **Chart.js** и **Canvas API**.

## Возможности
- Отображение границ муниципальных образований и объектов инфраструктуры:
  - населённые пункты, дороги, железные дороги, здания, церкви, терминалы, пляжи, парковки, болота, реки и др.;
- Две темы отображения: **дневная** и **ночная**;
- Загрузка и отрисовка карт из GeoJSON для каждого района;
- Подсветка объектов при наведении мыши, всплывающие подсказки с названием;
- Клик по объекту открывает **информационное окно** с данными из **Wikidata** (тип, население, площадь, дата основания, флаг, герб и др.);
- Подключение к **Overpass API** для получения Wikidata ID по OSM ID;
- Интеграция с локальными социально-экономическими данными (JSON-файлы в папке `data/sorted/`), включая:
  - образование, жильё, сельское хозяйство, культура, спорт, бюджет, занятость и др.;
- Построение **таблиц и графиков** (Chart.js) для выбранного региона по доступным показателям.

## Управление
- 🔍 **Масштабирование и перемещение карты**: колесо мыши и drag-and-drop (реализовано через `d3.zoom`);
- 🌓 **Переключение темы**: кнопка в правом верхнем углу (день/ночь);
- ☰ **Боковое меню**:  
  - текстовые кнопки для включения/выключения отдельных слоёв (например, дороги, здания, реки);  
  - иконки для управления слоями (альтернативный режим);  
  - кнопка «включить все карты» для отображения всех слоёв;
- 🖱 **ЛКМ по объекту**: открытие информационного окна с данными из Wikidata и вкладкой социальных показателей;  
- 🖱 **ПКМ по карте**: отображение информации об авторе;  
- 📊 **Социальные показатели**:  
  - список доступных файлов (образование, здравоохранение, культура и т. д.);  
  - таблица по годам;  
  - графики динамики показателей.

## Технологии
- **D3.js** — проекции, работа с GeoJSON, масштабирование/перемещение;
- **Canvas API** — отрисовка карты и объектов;
- **Chart.js** — визуализация показателей в графиках;
- **Overpass API, Wikidata API** — получение данных об объектах;
- **Vanilla JS + CSS** — кастомный UI (тултипы, меню, переключатели, иконки).
