# Wind- und FF-PV-Potenziale im Landkreis Passau

Details siehe Jupyter Notebook 

## Ordnerstruktur

- Jupyter Notebook: `Wind_und_FF_PV-Potenziale_LK_Passau.ipynb`
- Jupyter Notebook (Version für den Export als HTML-Präsentation): `Wind_und_FF_PV-Potenziale_LK_Passau_presentation.ipynb`
- Eingangsgeodaten: `./geodata_raw/`
- Ergebnisse (HTML): `./html_export/` - 
  - Notebook: `2023-07-17_Wind_und_FF_PV-Potenziale_LK_Passau.html`
  - Folien: `2023-07-17_Wind_und_FF_PV-Potenziale_LK_Passau_presentation.slides.html`
- Ergebnisse (Geodaten, CSV, JSON): `./results/` 

## Installation (Linux)

Zum Bearbeiten Repository ins aktuelle Verzeichnis klonen

    git clone git@github.com:rl-institut/ee_potenziale_lk_passau.git .
    cd ee_potenziale_lk_passau

Virtualenv anlegen und aktivieren (hier mit Python 3.8)

    virtualenv --python=python3.8 venv
    source venv/bin/activate

Benötigte Pakete installieren

    pip install -r requirements.txt

Jupyter im Browser öffnen

    jupyter notebook

## Datenquellen

| Datei                                                           | Quelle Originaldaten |
|-----------------------------------------------------------------|---------------------|
| `./geodata_raw/DEU_wind_speed_100m.tif`                         | [1]                 |
| `./geodata_raw/DEU_wind_speed_150m.tif`                         | [1]                 |
| `./geodata_raw/district.gpkg`                                   | [2]                 |
| `./geodata_raw/potentialarea_pv_agriculture.gpkg`               | [3]                 |
| `./geodata_raw/potentialarea_pv_agriculture_lfa-on.gpkg`        | [3]                 |
| `./geodata_raw/potentialarea_pv_road_railway.gpkg`              | [3]                 |
| `./geodata_raw/potentialarea_pv_road_railway_200m.gpkg`         | [3]                 |
| `./geodata_raw/potentialarea_pv_road_railway_500m.gpkg`         | [3]                 |
| `./geodata_raw/potentialarea_wind.gpkg`                         | [3]                 |
| `./geodata_raw/potentialarea_wind_settlement-1000m.gpkg`        | [3]                 |
| `./geodata_raw/potentialarea_wind_settlement-1000m_forest.gpkg` | [3]                 |
| `./geodata_raw/potentialarea_wind_settlement-1000m_lpa.gpkg`    | [3]                 |

[1] Technical University of Denmark (DTU) - Global Wind Atlas 3.0, Stand 01.02.2021, https://globalwindatlas.info, Lizenz: CC BY 4.0

[2] Dienstleistungszentrum des Bundes für Geoinformation und Geodäsie (DLZ) - Verwaltungsgebiete 1:250 000 VG250 (Ebenen), Stand 01.01.2020, https://gdz.bkg.bund.de/index.php/default/open-data/digitales-landschaftsmodell-1-250-000-ebenen-dlm250-ebenen.html, Lizenz: dl-de/by-2-0

[3] Amme, J. (2022). Der Photovoltaik- und Windflächenrechner - Geodaten Potenzialflächen (v1.0) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.6728382, Lizenz: ODbL-1.0 

## Lizenz

- Quellcode: AGPL, siehe [LICENSE](LICENSE)
- Eingangsdaten: Siehe Datenquellen oben
- Ergebnisdaten: ODbL-1.0
