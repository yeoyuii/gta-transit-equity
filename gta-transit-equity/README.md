# GTA Transit Equity Dashboard

An analysis of TTC transit accessibility across Toronto's 158 neighbourhoods, with a focus on equity for underserved communities.

## 🔍 Key Finding

**34 of Toronto's officially designated Neighbourhood Improvement Areas (NIAs) — communities the city itself has flagged as underserved — also have below-average transit density.**

- Average stops/km² in NIA neighbourhoods: **16.25**
- Average stops/km² in non-NIA neighbourhoods: **17.89**
- The gap is most concentrated in **Scarborough**

## 🗺️ Maps

- `01_ttc_stops.html` — All 9,378 TTC stops across Toronto
- `02_transit_density.html` — Transit density choropleth by neighbourhood
- `03_equity_analysis.html` — NIA neighbourhoods overlaid on transit density

## 💻 Tech Stack

- **Python** — data processing
- **GeoPandas** — spatial analysis and joins
- **Folium** — interactive map visualizations
- **Pandas** — data manipulation

## 📦 Data Sources

- [TTC Routes and Schedules](https://open.toronto.ca/dataset/ttc-routes-and-schedules/) — City of Toronto Open Data
- [Toronto Neighbourhood Boundaries](https://open.toronto.ca/dataset/neighbourhoods/) — City of Toronto Open Data
- Statistics Canada Census Data

## 🚀 Run It Yourself

```bash
git clone https://github.com/yeoyuii/gta-transit-equity.git
cd gta-transit-equity
pip install pandas geopandas folium jupyter matplotlib requests
jupyter notebook
```

## 🌱 Background

This project grew out of community research on transportation access for newcomer communities in the GTA. The goal is to make transit inequity visible through data.

## 📈 Next Steps

- Add income and demographic data from Statistics Canada
- Build an interactive React dashboard
- Expand analysis to Metrolinx regional transit
