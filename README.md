🎧 Spotify Streaming Audit & Playlist Optimization
Rol: Data Analyst | Contexto: Colaboración en Equipo (4 integrantes)

🎯 El Desafío de Negocio (Business Case)
El catálogo de Spotify cuenta con millones de canciones, pero la selección manual o intuitiva para las playlists premium genera ineficiencias: menor engagement de los oyentes y pérdida de oportunidades de descubrimiento de contenido.

El objetivo: Construir un marco basado en datos para responder: ¿Qué canciones garantizan un alto rendimiento y cómo segmentar la música de forma inteligente para maximizar la retención del usuario?

🛠️ Mi Enfoque Analítico (Workflow)
Calidad de Datos: Limpieza y normalización de un dataset de ~2,000 tracks con algoritmos de detección de outliers (Isolation Forest).

Análisis Macroeconómico/Temporal: Evaluación de la evolución del perfil acústico (1958–2019) detectando el fenómeno de la "Loudness War" (caída de la acousticness y subida de la energy desde los 90s).

Segmentación Avanzada (Clustering): Implementación de K-Means en Python para agrupar canciones por "vibra" (Energy vs. Valence).

Inteligencia de Negocio: Consultas avanzadas en SQL (DuckDB) para extraer cuartiles de popularidad, análisis de géneros por década y filtrado de anomalías de mercado (Grammy vs. Popularidad).
📊 Visualización de Datos (Interactive Dashboard)
Diseñé e integré un dashboard interactivo utilizando Plotly estructurado en 4 pilares estratégicos:
Evolución Acústica: Establece el estándar sonoro moderno para calificar a una playlist ($Energy > 0.60$, $Acousticness < 0.30$).
Mapa de Clústeres: Identificación visual de la "Premium Zone" (High Energy + High Valence).
Top 10 Géneros por Década: Filtro interactivo para curación histórica y nostálgica
Hidden Gems Detector: Cruce de datos de crítica (Grammys) vs. éxito comercial para descubrir oportunidades editoriales.

🔗 Explorar el Dashboard en Vivo de este Proyecto
https://17juan08.github.io/Spotify_Streaming_Audit/dashboard_spotify.html
💡 Recomendaciones Estratégicas para el Negocio
Regla del Primer Filtro: Utilizar el cuartil superior de popularidad ($Q4$) como screening automatizado antes de la curación humana.
Estrategia Editorial 70/30: Asignar un 70% de la playlist a géneros comerciales validados y un 30% a "Hidden Gems" (Joyas Ocultas) para sofisticar el algoritmo de recomendación y retener audiencias específicas.
Estandarización de Audio: Automatizar el rechazo de canciones en playlists de alta energía que no cumplan con el umbral de $-8\text{ dB}$ de loudness.
