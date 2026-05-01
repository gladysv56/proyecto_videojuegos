# 🎮 Análisis de Ventas de Videojuegos – Ice Store

## Contexto
Análisis realizado para Ice, una tienda online de videojuegos a nivel mundial. 
El objetivo fue identificar patrones que determinan el éxito de un videojuego 
para detectar proyectos prometedores y planificar campañas publicitarias para 2017, 
basándose en datos históricos hasta 2016.

## Proceso de análisis

### 1. Exploración y limpieza de datos
- Dataset de 16,715 registros con 11 columnas
- Conversión de tipos de datos (year_of_release a Int64, user_score a float)
- Tratamiento de valores ausentes: se mantuvieron en critic_score y user_score 
  por representar un porcentaje considerable; rating se rellenó como 'Unrated'
- Identificación y análisis de valores TBD en user_score
- Revisión de duplicados explícitos e implícitos por nombre, plataforma y género
- Cálculo de ventas totales globales por juego

### 2. Análisis de plataformas
- Identificación del ciclo de vida de plataformas (~9-11 años)
- Las plataformas con mayores ventas históricas: PS2, X360, PS3, Wii, DS
- Plataformas activas más rentables para 2017: **PS4 y XOne**
- Análisis de distribución de ventas por plataforma con diagramas de caja
- Comparación de eficiencia: ventas por juego vs cantidad de juegos por plataforma

### 3. Impacto de reseñas en ventas
- Correlación débil-moderada entre reseñas de críticos/usuarios y ventas
- Las buenas reseñas no garantizan altas ventas

### 4. Análisis por género
- Géneros más rentables globalmente: **Action, Sports y Shooter**
- Los géneros de alta emoción e instinto competitivo generan mayores ingresos

### 5. Perfil por región
- **NA y EU**: comportamiento similar, dominan Action y Sports
- **JP**: tendencia diferente, prioriza Role-Playing
- Las clasificaciones ESRB no afectan significativamente las ventas por región

### 6. Pruebas de hipótesis
- ✅ Las calificaciones promedio de usuarios para Xbox One y PC **son iguales** 
  (no se rechaza H0)
- ✅ Las calificaciones promedio para géneros Action y Sports **son diferentes** 
  (se rechaza H0)

## Conclusiones principales
- **PS4 y XOne** son las plataformas más rentables con ciclo de vida aún activo
- **Action, Sports y Shooter** lideran ventas globales; **Role-Playing** es 
  prioritario en Japón
- Estrategia recomendada: **calidad sobre cantidad** (~98 juegos por plataforma 
  para maximizar retorno)
- Los datos de 2016 pueden estar incompletos, lo que puede afectar el análisis 
  del último año

## Herramientas utilizadas
`Python` `Pandas` `Matplotlib` `Seaborn` `Scipy` `Pruebas de hipótesis` `EDA`

## Estado
✅ Proyecto aprobado por revisor TripleTen
