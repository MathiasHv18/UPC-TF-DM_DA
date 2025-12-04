# UPC-TF-DM_DA

Proyecto de EDA y minería de patrones sobre el dataset de retail online (2010-2011).

## Contenido
- `eda.ipynb`: carga reproducible (local/Kaggle), análisis de faltantes y calidad, pipeline de limpieza, exploración estacional y top productos, exporta `data/processed/cleaned_online_retail.csv`.
- `data_mining.ipynb`: one-hot con espacio único, itemsets frecuentes (FP-Growth), reglas de asociación, patrones emergentes H2 vs H1 y exportes de resultados.

## Requisitos
- Python 3.10+ recomendado.
- Instalar dependencias: `pip install -r requirements.txt`

## Datos
- Coloca `online_retail.csv` en `data/raw/`. Alternativamente, con credenciales de Kaggle configuradas el notebook lo descarga vía `kagglehub` (`ulrikthygepedersen/online-retail-dataset`).

## Ejecución
1. Abrir y ejecutar `eda.ipynb` completo (genera `data/processed/cleaned_online_retail.csv` y visualizaciones de calidad/estacionalidad).
2. Abrir y ejecutar `data_mining.ipynb` (reutiliza el CSV procesado, genera itemsets/reglas/patrones y los guarda en `data/processed/`).

## Recursos
- Dataset: https://www.kaggle.com/datasets/ulrikthygepedersen/online-retail-dataset
- Informe (Drive): https://docs.google.com/document/d/1il2bpjSq5bJBttwviHi70vrwbnkTc0Z-dujMvQz3pbE/edit?usp=sharing
