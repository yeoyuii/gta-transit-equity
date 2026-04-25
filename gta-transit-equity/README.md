cd gta-transit-equity
cat > README.md << 'EOF'
# GTA Transit Equity Dashboard

A spatial analysis of transit accessibility across **13,460 stops** in Toronto and Mississauga, examining equity for underserved communities.

## Key Findings

### Toronto (TTC)
- **9,378 stops** across **158 neighbourhoods**
- NIA neighbourhoods average **16.25 stops/km²**
- Non-NIA neighbourhoods average **17.89 stops/km²**
- **~34 Neighbourhood Improvement Areas** fall in low transit density zones
- Gap most concentrated in **Scarborough**

### Mississauga (MiWay)
- **4,082 stops** across **172 census tracts**
- Average **16.93 stops/km²** across the city
- Most underserved areas concentrated in outer Mississauga

### Combined GTA
- **13,460 total stops** analyzed
- **330 geographic units** mapped
- Consistent pattern: outer, lower-income areas have worse transit density across both cities

## Maps
- `01_ttc_stops.html` — All 9,378 TTC stops
- `02_transit_density.html` — Toronto transit density choropleth
- `03_equity_analysis.html` — Toronto NIA equity overlay
- `04_gta_equity_map.html` — Combined GTA equity map 🌟

## Tech Stack
- **Python** — data processing
- **GeoPandas** — spatial analysis and joins
- **Folium** — interactive map visualizations
- **Pandas** — data manipulation
- **Statistics Canada** — census tract boundaries

## Data Sources
- [TTC GTFS](https://open.toronto.ca/dataset/ttc-routes-and-schedules/) — City of Toronto
- [MiWay GTFS](https://www.mississauga.ca/miway-transit/developer-download/) — City of Mississauga
- [Toronto Neighbourhoods](https://open.toronto.ca/dataset/neighbourhoods/) — City of Toronto
- [Census Tract Boundaries](https://www12.statcan.gc.ca) — Statistics Canada

## Run It Yourself
```bash
git clone https://github.com/yeoyuii/gta-transit-equity.git
cd gta-transit-equity
pip install pandas geopandas folium jupyter matplotlib requests certifi
jupyter notebook
```

## Background
This project grew out of community research on transportation access for newcomer communities in the GTA. The goal is to make transit inequity visible through data.

## Next Steps
- Add income and demographic overlay from Statistics Canada
- Build interactive React dashboard
- Expand to Brampton (ZUM) and GO Transit
EOF
