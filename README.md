# Proyecto Grupo 8 — MCDI500

Análisis de la relación entre los patrones de uso de tecnología (pantallas, redes
sociales, videojuegos) y los indicadores de salud mental, estrés y calidad del
sueño, mediante un flujo de trabajo reproducible, documentado y colaborativo.

## Integrantes
- Abigail Roblez Chavez (@abda-abigail-github)
- Daniel Pérez Ramirez (@danielramirezdr114-dev-github)
- Matias Manriquez Ortiz (@matiasIMO98-github)
- Roberto Sánchez Saldivia (@quiltroconiphone-github)

## Datos
- **Fuente:** Kaggle — *Mental Health and Technology Usage Dataset* (autor: waqi786).
  `https://www.kaggle.com/datasets/waqi786/mental-health-and-technology-usage-dataset`
- **Licencia:** verificar términos del autor en Kaggle antes de una redistribución pública.
- **Dimensiones:** 10.000 registros × 14 variables originales.
- **Variables:** `User_ID`, `Age`, `Gender`, `Technology_Usage_Hours`,
  `Social_Media_Usage_Hours`, `Gaming_Hours`, `Screen_Time_Hours`,
  `Mental_Health_Status`, `Stress_Level`, `Sleep_Hours`,
  `Physical_Activity_Hours`, `Support_Systems_Access`,
  `Work_Environment_Impact`, `Online_Support_Usage`.

## Estructura del repositorio
```
proyecto-grupo8-mcdi500/
├─ F1/
│  └─ notebooks/
│     └─ S1_F1_Definicion.ipynb        Fase 1 — definición del problema y entorno
├─ F2/
│  └─ S1_F2_Preprocesamiento.ipynb     Fase 2 — obtención, limpieza y transformación
├─ docs/
│  ├─ Mapa Conceptual Proyecto/
│  ├─ Informe/
│  └─ Referencias/                     (crear cuando corresponda)
├─ requirements.txt                    dependencias del proyecto (único, en la raíz)
└─ README.md                           este archivo
```

## Requisitos y ejecución
Python 3.11 o superior.

```bash
python -m venv .venv
source .venv/Scripts/activate      # Windows, Git Bash
# .venv\Scripts\Activate.ps1       # Windows, PowerShell
python -m pip install -r requirements.txt
python -m ipykernel install --user --name grupo8_mcdi500 --display-name "Python (grupo8-mcdi500)"
```

Ejecutar los notebooks en orden, desde la raíz del proyecto, seleccionando el
kernel `Python (grupo8-mcdi500)`:
1. `F1/notebooks/S1_F1_Definicion.ipynb`
2. `F2/S1_F2_Preprocesamiento.ipynb`

## Documentación (docs/)
Cada tipo de documento va en su propia subcarpeta, para no mezclar archivos:
- `docs/Mapa Conceptual Proyecto/`
- `docs/Informe/`
- `docs/Referencias/` (crear si se necesita)

## Convención de commits
Prefijos usados: `docs`, `data`, `feat`, `fix`, `test`.
Ejemplos:
- `docs: agrega mapa conceptual v1 y v2`
- `data: incorpora dataset mental_health_and_technology_usage_2024.csv`
- `feat: implementa funciones de preprocesamiento`
- `test: valida nulos, duplicados y rangos del dataset procesado`

## Decisiones técnicas
- **Limpieza:** [completar: qué encontraron al revisar nulos/duplicados/rangos]
- **Transformación:** [completar: qué transformaciones aplicaron y por qué]
- **Reproducibilidad:** entorno virtual `.venv` + `requirements.txt` (un solo archivo en la raíz).
