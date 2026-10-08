# Notas y decisiones del análisis — artículo "When animals cross the line" (2–4 oct. 2026)

Fuente: Google Doc en Drive, carpeta "Análisis Claude – ecología del movimiento (oct 2026)". Las tablas derivadas están en `data/derived/`.

## 1. Cartografía de planificación

### 1.1 Modelo urbano de conectividad del AMVA (MaterialComplementario.gdb y CONECTIVIDAD.gdb)

- Red topológica: 7 sectores (Sur; MedOcc y MedOri = Medellín a cada lado del río; CB = Copacabana y Bello; NorG = Girardota; NorB1 y NorB2 = Barbosa), 156 674 nodos y 439 528 enlaces, EPSG:3116.
- Enlaces cortos: 67 % ≤20 m y 93 % ≤50 m (del orden del error GPS). Los 7 sectores son grafos separados, sin enlaces entre sí. NorG tiene una relación costo/distancia (0,6) distinta del resto (28–41).
- CONECTIVIDAD.gdb: 194 863 polígonos de espacio verde urbano (6646 ha; Fase 1 contrato 4600067020 de 2016, Fase 2 contrato 1344 de 2018), con papel en la red, valores de circuitos y de rutas de menor costo, y régimen de manejo. Áreas de influencia ecológica 21 052 ha (88 % urbanas); zonas de restablecimiento 13 173 ha (99,9 % urbanas). No incluye superficie de resistencia.
- Red frente a jurisdicción: ~95 % de los enlaces dentro de la jurisdicción urbana, ~2 % cruza el límite, ~2 % fuera. El modelo no cubre el suelo rural.

### 1.2 Límites

- Jurisdicción ambiental del AMVA (capa entregada por el AMVA en 2019): 184,7 km², 15,9 % de los 1161 km² de los 10 municipios. Incluye el área urbana de Envigado.
- % urbano por municipio: Itagüí 71,7; Medellín 29,8; Sabaneta 25,6; Envigado 16,3; Bello 14,9; La Estrella 14,0; Copacabana 7,4; Girardota 4,9; Caldas 2,8; Barbosa 1,2.
- Suelo rural: Corantioquia. Cornare solo tiene un borde cerca de Envigado (confirmado por Adri).

### 1.3 Red Ecológica Principal de Antioquia (SIDAP 2021)

- 38 242 ha dentro del valle (32,9 %): 34 % del rural y 25 % del urbano. En su parte urbana el 61 % es construido; tramos casi rectos con patrón radial sobre Medellín.
- Método (Gobernación de Antioquia, informe contrato 4600012276): corredores de menor costo con Linkage Mapper; resistencia = inversa de la idoneidad promedio de siete mamíferos grandes (oso, jaguar, puma, guagua, nutria, manatí, churuco); pesos por expertos (Jerarquías Analíticas); coberturas 1:100 000; nodos ≥50 ha; sin validación. "Es difícil proveer cuál de ellas utilizarán los organismos para su movilidad" (p. 85). Asigna al AMVA las 318 redes del valle (38 571 ha), incluido el rural (p. 101).
- Contacto entre las dos redes: solo el 25 % del límite urbano–rural toca la red regional; 72 % está a ≤500 m. Áreas de influencia del modelo urbano solapan 25 % con la red regional.
- Áreas protegidas rurales en el valle (Corantioquia salvo la RFPN Río Nare, del Ministerio): DRMI Divisoria Aburrá–Cauca 20 751 ha; DRMI Quitasol–La Holanda 5205 ha; RFPN Río Nare 2660 ha; RFPR Alto de San Miguel 1616 ha. Urbanas (AMVA): Cerro El Volador, Nutibara, La Asomadera, El Trianón, Ditaires, Piamonte.

### 1.4 Cobertura y elevación (WorldCover 2021, Hansen GFC v1.11, Copernicus 30 m)

- Urbano: 65 % construido, 25 % árboles. Rural: 61 % árboles, 37 % pastos, 2 % construido.
- El límite coincide con el borde de lo construido (cae de 37,5 % a 16,1 % al cruzarlo), no con un borde de bosque: del lado rural hay un mosaico de árboles y pastos y la cobertura arbórea sube gradualmente (46 % a 200 m, 55 % a 1 km, 62 % a 2 km). Pico de árboles justo en el límite (53 %).
- Elevación mediana del límite: ~1310 m (Barbosa) a ~1810 m (Medellín); valle completo 1707 m. 82 % de los árboles rurales está por encima de 1800 m.
- Pérdida de bosque 2001–2023 (dosel ≥30 % en 2000): rural 8,7 %; franja rural 0–500 m 9,8 %; urbano 13,2 %.
- Advertencias: WorldCover no distingue plantaciones; el DEM es de superficie.

### 1.5 Red de drenaje provisional

- Derivada del DEM (pysheds; quebradas ≥0,5 km² de cuenca, ríos ≥50 km²) porque no hay red hídrica oficial disponible (decisión de Adri).
- Casi todas las especies están más cerca de quebradas de lo esperado (1,3–3,6 veces la línea base de 13,9 % del valle a ≤60 m). Río principal (línea base 2,6 % a ≤150 m): ñeque 18×, garza bueyera 13×, cormorán 10×, garza blanca 9×, ibis 5×. El río Medellín es la única estructura continua que cruza la jurisdicción urbana de sur a norte.

## 2. Telemetría

### 2.1 Conciliación de fuentes

- Base: Movebank (610 504 filas, 72 individuos, oct. 2022 – oct. 2026). Las 236 928 fijaciones del Darwin Core están todas en Movebank; no se agregó nada.
- El Darwin Core tiene la hora en UTC aunque dice "Colombia time".
- 6 individuos sin especie en Movebank (Buho1, Buho2, Cormoran1, Gallinazo1, Guacharaca02, Guacharaca03): especie completada desde el marcaje.
- 7 marcados sin datos, excluidos: Asio3, Zorro1, Zorro10, Pigua7, Phimosus9–11.
- Fechas corregidas por reinicio del contador de semanas del GPS: Phimosus7 (2084 → dic. 2025) y Phimosus1 (2062 → jul. 2023).
- Zorro5 y Zorro9 usaron el mismo collar (reutilizado).

### 2.2 Origen y cortes posliberación (opción B aprobada)

- 65 silvestres in situ; CAV: Ñeque2, Zorro12, Asio2; translocados: Pigua5, Perezoso1; rescatados: Asio1, Guacharaca4.
- Cortes: Asio2 20 días; Pigua5 7 días (resto = posible dispersión); Perezoso1 excluido de área de vida y excursiones; los demás sin corte. Análisis de sensibilidad sin estos individuos.
- Edad al marcaje como covariable (53 adultos, 12 subadultos, 7 juveniles). Confundida con especie: todas las piguas son juveniles o subadultas; solo los zorros permiten contraste (5 y 5).

### 2.3 Limpieza por individuo (aprobada)

Orden: coordenadas 0 (8197) → antes del marcaje (15) → cola final inmóvil, solo si el animal no se vuelve a mover (447; Ñeque2 completo, colas de Zarigueya2, 3 y 7, Pava1, Ardea1) → calidad: HDOP >5 en GSM; en Iridium "Unresolved QFP", "Resolved QFP (Uncertain)", QFP con HDOP >5 y "Succeeded" con error >50 m (1613) → picos de ida y vuelta (36) → velocidad alta de una sola vía, marcada y conservada (7). Resultado: 600 196 fijaciones válidas; 71 individuos. Errores concentrados cerca de las 23:00 y 10:30 UTC.

## 3. Estrategias de movimiento (variogramas empíricos, Python)

- Criterio: pendiente del variograma en desfases ≥7 días (<0,3 residente; 0,3–0,6 intermedio; ≥0,6 no residente). Resultado: 50 residentes, 9 intermedios, 7 no residentes, 5 con datos insuficientes.
- Tipología aprobada: (1) residente estricto; (2) residente con excursiones (Zorro12, Pigua2, Phimosus4, Garza5; Zorro9 con una excursión de ~27 km y dos meses); (3) multisitio (Garza2, Pava1); (4) cambio de área (Zorro8, Zorro4, Phimosus6, Cormorán1, Zorro3); (5) dispersión escalonada (Pigua5 y Pigua6, juveniles, hasta 90–100 km).
- Supuestos aprobados para el siguiente paso: área de vida en periodos residentes (por sitio en los tipos 3–5) con el contorno del 95 % de un estimador de núcleo, declarando la subestimación por autocorrelación; excursión = fijaciones consecutivas fuera del 95 % que regresan; sin regreso en 30 días = cambio de área.

## 4. Decisiones sobre el manuscrito (v2 en Drive)

- Párrafo 4 de la introducción reescrito: el límite sigue el borde de lo construido, con un mosaico de transición del lado rural.
- Pregunta 1 con hipótesis alternativas: grafo urbano, corredores regionales, (propuesto) red hídrica, frente a un modelo nulo en línea recta.
- Pendientes: año del modelo urbano (2019 o 2020) y cita formal del informe técnico del AMVA y del informe del SIDAP.
