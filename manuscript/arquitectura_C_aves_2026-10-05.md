# Arquitectura C — artículo de aves: "¿Conectividad para qué?" (propuesta, 2026-10-05)

## Decisiones B ya tomadas (Adri, 2026-10-05)
- **Solo aves.** Los mamíferos pasan a otro manuscrito.
- **Todas las aves marcadas como ilustración:** 40 individuos de 11 especies. Los análisis inferenciales se hacen solo con las especies focales: garza (7), coquito (8), pigua (5) y gallinazo (2, descriptivo). La guacharaca (7) es el contraste residente.
- **Marco:** conectividad según el objetivo (UICN; LaPoint; Beninde; Tischendorf & Fahrig; Nathan). El núcleo conceptual es la complementación dormidero–comedero y el forrajeo de lugar central (Dunning et al. 1992; Dennis et al.). El grafo dormidero–comedero va en la discusión.
- **Podas:** solo en la discusión, como implicación de manejo con los casos como ilustración. No es una pregunta del artículo.
- **Doble verificación:** reimplementación independiente en Python, con otras bibliotecas y sin leer el código primario. Tolerancias fijadas de antemano (matriz_opciones_analiticas_aves.md, §4b).
- **Revista:** *Landscape and Urban Planning* (se mantiene, pendiente de confirmar).

## Contribución central (propuesta)
> Connectivity in cities is planned as continuous green corridors, but what an animal needs to connect depends on how it moves. Large urban birds that commute daily need roosts and feeding grounds within flying range, not continuous corridors. In an Andean metropolis, these nodes were street trees, lake edges, institutional lawns and meat-industry grounds, and most fall outside the green-corridor networks designed for birds.

En español: las ciudades planifican la conectividad como corredores verdes continuos, pero lo que un animal necesita conectar depende de cómo se mueve. Las aves grandes que viajan cada día necesitan dormideros y comederos a su alcance, no corredores. En el Valle de Aburrá esos nodos son arbolado vial, bordes de lagos, gramas institucionales y la industria cárnica, y la mayoría queda por fuera de las redes de corredores diseñadas para aves.

**Advertencia.** La última frase ("most fall outside") es una hipótesis. Se mantiene solo si P4 la sostiene.

## Título y recuadros aprobados (Adri, 2026-10-05)
**Título:** *Connectivity for what? From a single tree to a hundred kilometres, GPS-tracked birds reveal what an Andean city must connect*

**Recuadros** (contrastantes, con el dato más llamativo):
1. **Una vida en 260 metros:** guacharacas residentes, con un solo cambio de dormidero en unas 6550 noches.
2. **De una reserva de bosque al Magdalena Medio:** piguas en la red cárnica; Pigua5, entregada al CAV y liberada en Santa Elena, pasó por las curtiembres y Zenú y llegó a Puerto Berrío.
3. **Dormir sobre la 70:** coquitos en arbolado vial y en dormideros comunales.

Las garzas van en el texto principal y en las figuras de nodos y enlaces. Las cifras son de la exploración y se recalculan con verificación doble.

## Títulos candidatos (histórico)
1. *Connectivity for what? GPS-tracked birds reveal the roost–feeding networks that urban green corridors miss*
2. *Connecting resources, not patches: roost and feeding networks of large birds in an Andean city*
3. *What do urban birds need to connect? Roosts, feeding grounds and the limits of green-corridor planning*

## Estructura

### Highlights (3–5, ≤ 85 caracteres): se escriben al final.

### Resumen (≤ 250 palabras)
Problema → pregunta "¿conectividad para qué?" → datos (40 aves de 11 especies; 29 focales) → nodos y enlaces → reconocimiento en los instrumentos → pérdida de nodos → implicación.

### 1. Introducción (4–5 párrafos)
1. **La conectividad urbana se planifica como estructura.** Corredores y redes de zonas verdes (LaPoint et al. 2015; Beninde et al. 2015). La red ecológica del AMVA se construyó con diversidad de aves y un enfoque de corredores.
2. **¿Conectividad para qué?** La conectividad es funcional y depende del objetivo y del tipo de movimiento (Taylor et al. 1993; Tischendorf & Fahrig 2000; Nathan et al. 2008; Hilty et al. 2020). Cada tipo de animal conecta cosas distintas:
   - el residente necesita calidad del parche;
   - el que viaja a diario necesita recursos complementarios a su alcance;
   - el dispersor necesita permeabilidad.
3. **Las aves grandes que viajan a diario.** Dormideros comunales, forrajeo de lugar central y complementación del paisaje (Dunning et al. 1992; Dennis et al.). En la ciudad: dormideros en arbolado, subsidios alimentarios y colonizadores recientes. Para una especie que vuela, los corredores y la complementación son objetivos distintos, no alternativas; esto responde al resultado de Beninde.
4. **Vacío.** Pocos estudios con GPS en ciudades tropicales (Eckhartt et al. 2026; Leveau et al. 2025). Ningún instrumento de planificación evalúa nodos de recurso con datos de movimiento.
5. **Objetivo y preguntas:**
   - Q1. ¿Qué conectan las aves de la ciudad? Tipos de movimiento.
   - Q2. ¿Cuáles son los nodos de recurso de las aves que viajan a diario y cómo se enlazan?
   - Q3. ¿Qué hace apto un dormidero o un comedero?
   - Q4. ¿Cuánto los reconocen los instrumentos de planificación?
   - Q5. ¿Qué tan vulnerable es la red a la pérdida de nodos?

### 2. Métodos
- **2.1 Área de estudio.** Valle de Aburrá; jurisdicciones; red de conectividad del AMVA; POT de Medellín.
- **2.2 Aves marcadas.** 40 individuos de 11 especies; collares; programación (incluido el cambio de 1 h a 4 h desde 2024); depuración; origen (silvestre, rescatado, translocado); edad. Las focales y los criterios de inclusión van en la Tabla 1.
- **2.3 Tipos de movimiento (Q1).** Métricas descriptivas comunes para las 40 aves, todas reducidas al esquema común de 4 h:
  - radio de viaje diario;
  - fidelidad al dormidero;
  - número de dormideros;
  - viajes fuera del valle;
  - actividad nocturna.

  Se ordenan en tipos: residente de parche, viajero diario con dormidero fijo, rotador entre nodos y viajero regional. Es un análisis solo descriptivo e ilustrativo.
- **2.4 Nodos de recurso (Q2).** Dormideros por individuo en dos etapas (DBSCAN/HDBSCAN con eps de 50 m) y unión entre individuos por solape. Recursión (revisitas) con el paquete recurse. Comederos agregados por día. Validación de cuatro tipos:
  - ciega en imagen satelital (Adri);
  - temporal, comparando años;
  - dejando un individuo fuera;
  - con el arbolado inventariado.
- **2.5 Enlaces diarios (Q2).** Red bipartita dormidero → comedero, distancia del viaje diario (reducida a 4 h y con AR(1)), fidelidad markoviana y horario de salida y llegada como dato censurado (solo aves horarias). No se reconstruyen rutas.
- **2.6 Aptitud de dormideros y comederos (Q3).** Elección condicional por noche o por día, con la disponibilidad dentro del radio de viaje de cada ave (no centrada en el sitio de captura) y pendientes aleatorias por individuo (Muff et al. 2020). Se suma un nulo geométrico. La iSSF en aves horarias sirve de respaldo. Covariables:
  - árboles y construido (WorldCover corregido con la verificación satelital);
  - tipos de EVU (separador, retiro de quebrada, parque…);
  - distancia al agua;
  - arbolado inventariado;
  - sitios OSM.
- **2.7 Reconocimiento por los instrumentos (Q4).** Porcentaje de noches-ave y días-ave dentro de:
  - la red de conectividad del AMVA (fragmento, enlace, nodo, zona de enlace);
  - la red ecológica del POT de Medellín;
  - la REPA;
  - las áreas protegidas;
  - los tipos de EVU.

  Se calcula una razón de reconocimiento ponderada por uso y se compara con el nulo de disponibilidad.
- **2.8 Pérdida de nodos (Q5).** Robustez de la red empírica con remoción aleatoria, por uso, por intermediación y por "no reconocido", más el índice dPC/dIIC en el lenguaje del AMVA. La validación se hace con cambios espontáneos de dormidero y con la pólvora. Los resultados son escenarios, no predicciones.
- **2.9 Extensión regional.** Estudios de caso: Garza2, Gallinazo2, Garza4 y Pigua4.
- **2.10 Inferencia, sensibilidad y doble verificación.** La especie entra como efecto fijo. El bootstrap es por individuo. Para el sitio de captura se hacen dos controles: excluir los primeros 7 y 20 días y excluir lo que está a ≤ 1 km de la captura. Se aplican las 18 pruebas de sensibilidad y la verificación independiente con tolerancias (Tabla S).

### 3. Resultados
- **3.1 Cada ave conecta cosas distintas.** Galería de las 40 aves: residentes de parche (guacharacas, pavas, búhos), viajeros diarios con dormidero comunal (garzas, coquitos, cormorán, garza real, guaco), rotadores entre nodos (piguas, gallinazos) y viajeros regionales. → **Fig. 1**
- **3.2 Los nodos de recurso.** Dormideros y comederos: tipo, uso compartido entre individuos y especies, y validación. → **Fig. 2** (mapa de nodos)
- **3.3 Cómo se enlazan.** Red bipartita, distancia y horario de los viajes, fidelidad. → **Fig. 3**
- **3.4 Qué hace apto un dormidero o un comedero.** Coeficientes de selección y comparación con el nulo. → **Fig. 4**
- **3.5 Lo que reconocen los instrumentos.** Brecha ponderada por uso entre las redes y los nodos. → **Fig. 5**
- **3.6 Vulnerabilidad a la pérdida de nodos.** Curvas de robustez y nodos críticos. → **Fig. 6**
- **3.7 Extensión regional.** Breve, como casos.

**Recuadros** (2–3; Adri elige):
1. El garcero: San Antonio de Prado, el guadual de El Rodeo y el lago de Parque Norte.
2. Coquitos que duermen en el arbolado vial (la 70, la Bolivariana, canalizaciones).
3. Piguas y la industria cárnica: el tulipán africano junto a Zenú y la rotación entre nodos.

### 4. Discusión
1. **¿Conectividad para qué?** La respuesta depende del tipo de movimiento. Para aves que viajan a diario, lo que hay que conectar son recursos, no parches.
2. **Nodos que nadie planifica.** Arbolado vial, bordes de lagos y gramas institucionales.
3. **El manejo del arbolado como palanca.** Podas en árboles de dormidero, con los casos como ilustración (la decisión B dejó las podas en la discusión).
4. **Subsidios y conflicto.** Industria cárnica, aeropuerto y riesgo aviario (Oro et al. 2013).
5. **Corredores y complementación son complementarios, no alternativos.** Beninde; los dispersores.
6. **Limitaciones:**
   - n por especie;
   - garzas de una sola colonia;
   - esquema de fijación confundido con el año;
   - WorldCover marca el arbolado vial como construido;
   - la red está muestreada por 29 aves;
   - no hay catastro.

### 5. Implicaciones para la planificación (sección obligatoria en LUP)
**Tabla 2:** tipo de nodo × instrumento que hoy lo ignora × actor responsable × acción. Ejemplos:
- protocolo de poda en árboles de dormidero (Secretaría de Medio Ambiente);
- dormideros comunales como nodos de la red del AMVA;
- manejo de la grama en el aeropuerto y los campus;
- subsidios de la industria cárnica.

### Figuras y tablas
| # | Contenido |
|---|---|
| Fig. 1 | Galería de tipos de movimiento: 40 aves de 11 especies, con un panel pequeño por ave o tipo y sus métricas |
| Fig. 2 | Mapa de nodos de dormidero y comedero y su tipo |
| Fig. 3 | Red bipartita, distancia y horario de los viajes |
| Fig. 4 | Selección de dormideros y comederos (coeficientes con su incertidumbre) |
| Fig. 5 | Reconocimiento por los instrumentos (brecha) |
| Fig. 6 | Robustez de la red ante la pérdida de nodos |
| Tabla 1 | Aves marcadas: especie, n, origen, edad, esquema, días y rol (focal o ilustrativa) |
| Tabla 2 | Implicaciones para la planificación |
| Suplementario | Atlas por individuo; Tabla S de sensibilidad (18 pruebas); Tabla S de verificación doble; lista de dormideros verificados |

## Orden de trabajo propuesto (después de validar C y D)
1. Congelar los datos con hash y escribir las fichas de especificación de cada análisis.
2. Hacer Q1 (galería) y Q2 (nodos y enlaces), con su verificación doble.
3. Hacer Q3, luego Q4 y luego Q5, cada uno con su verificación doble y su sensibilidad.
4. Redacción (E) y verificación final con agentes independientes (F).

## Lo que necesito de Adri
1. Elegir el título o proponer otro, y confirmar la revista (LUP).
2. Elegir los recuadros.
3. Subir los PDF de Dunning 1992, Dennis 2003, Nathan 2008, Hilty 2020 (UICN), Baguette 2013, Saura & Pascual-Hortal 2007 y Orians & Pearson 1979 para tener las citas textuales con página.
4. Garza1 y Garza2: su dormidero principal está a unos 20 km de El Rodeo. ¿Es el garcero de San Antonio de Prado (nodo 27) o un sitio fuera de Medellín?
