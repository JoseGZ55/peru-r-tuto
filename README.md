# Mapas Electorales del Perú con R — Elecciones 2026

Tutorial de elaboración de mapas temáticos en R usando los resultados oficiales de la primera vuelta de las **Elecciones Presidenciales del Perú 2026** (Fuente: ONPE).

## Contenido del repositorio

| Archivo | Descripción |
|---------|-------------|
| `tutorial_mapas_peru_2026.Rmd` | Tutorial completo en R Markdown |
| `tutorial_mapas_peru_2026.html` | Versión renderizada del tutorial (para ver en el navegador) |
| `elecciones_2026.csv` | Datos electorales por departamento (ONPE, >94% actas) |

## Requisitos

- R ≥ 4.0
- RStudio (recomendado)
- Shapefile de departamentos del Perú: descargarlo desde [GEO GPS PERÚ](https://www.geogpsperu.com/)

## Paquetes de R necesarios

```r
install.packages(c("sf", "tidyverse", "ggplot2", "ggrepel", "readr"))
```

## Mapas generados

1. **% de votos de Keiko Fujimori** por departamento (escala continua).
2. **Candidato ganador** en cada departamento (mapa categórico).
3. **Diferencia entre Sánchez y Fujimori** (escala divergente).

## Fuente de datos

- ONPE: https://resultadoelectoral.onpe.gob.pe/main/presidenciales  
- Tutorial de referencia: https://rpubs.com/rcondor/619184

## Resultados nacionales (>94% actas procesadas)

| Candidato | Partido | % Votos válidos |
|-----------|---------|-----------------|
| Keiko Fujimori | Fuerza Popular | ~17.1% |
| Roberto Sánchez | Juntos por el Perú | ~12.0% |
| Rafael López Aliaga | Renovación Popular | ~11.9% |
| Jorge Nieto | Partido del Buen Gobierno | ~11.0% |
| Ricardo Belmont | Partido Cívico Obras | ~10.2% |

---
*Elaborado para el curso de Métodos Cuantitativos — UTEC, 2026.*
