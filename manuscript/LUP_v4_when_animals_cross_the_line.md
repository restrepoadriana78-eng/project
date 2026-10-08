# When animals cross the line: GPS tracking tests urban connectivity planning in the tropical Andes

**NOTAS DE ENVÍO (eliminar antes de enviar)**

  

  - **Revista:** *Landscape and Urban Planning*, artículo de investigación.
      
      - Extensión: 4000–8000 palabras con referencias.
      - Referencias: 25–60, en APA 7.
      - Resumen: ≤ 250 palabras.
      - Highlights: 3–5, de ≤ 85 caracteres.
      - Revisión doble anónima.
  - **Versión:** v4 (cierre), 2026-10-04. Arquitectura C, aprobada por Adri (claude/arquitectura\_C\_v4.md). Incorpora los insumos verificados en claude/insumos\_pendientes\_v4.md.
  - **Lógica central:** la conectividad se planifica a tres escalas (departamental, metropolitana y municipal) y ninguna responde a cómo se mueven los animales. Lo que estructura el movimiento (cursos de agua, vías y espacios verdes) se gestiona fuera de las redes de conectividad.
  - **Cifras:** verificadas de forma independiente (claude/verificacion\_independiente.md, claude/verificacion\_independiente\_2.md y claude/vias\_barrera\_medellin.md).
  - **Convención:** cada vacío lleva la etiqueta **\[FALTA-n\]**, que remite a la tabla de faltantes de abajo. No quedan otras marcas pendientes en el texto.
  - **Glosario fijo:**
      
      - *planning instrument*: la REPA, la red metropolitana del AMVA (y su grafo) y la red del POT de Medellín;
      - *landscape element*: cursos de agua, espacios verdes, vías;
      - *potential* y *actual connectivity*;
      - *jurisdictional boundary*;
      - *movement strategy*.
  - **Faltantes (todo lo demás está verificado):**

  

|  |  |  |  |  |
| :-: | :-: | :-: | :-: | :-: |
| \*\*Código\*\* | \*\*Qué falta\*\* | \*\*Dónde\*\* | \*\*Quién / cómo se resuelve\*\* | \*\*¿Bloquea el envío?\*\* |
| FALTA-1 | Modelo exacto de los equipos CTT (GPS-GSM) y Telonics (GPS-Iridium), su peso y el porcentaje de la masa corporal; programación nominal de fijaciones | §2.2 | Adri: facturas, fichas técnicas o configuración en la plataforma del fabricante | Sí: LUP y los revisores lo exigen |
| FALTA-2 | Página de Manly et al. (2002) para las razones de selección y el diseño de tipo III | §2.7 y referencias | PDF o copia física del libro (biblioteca) | No, es referencia canónica; sí para la matriz de trazabilidad |
| FALTA-3 | Cita textual de Worton (1989) sobre el ancho de banda de referencia | §2.5 | PDF (JSTOR o biblioteca) | No |
| FALTA-4 | Cita textual de Bjørneraas et al. (2010) sobre los picos de ida y vuelta | §2.2 | PDF (Wiley o biblioteca) | No; Gupte et al. (2022) ya sostiene el método |
| FALTA-5 | Cotejar a ojo las citas del Acuerdo 48 de 2014 (arts. 24, 26 y 33), que se tomaron del normograma Astrea con un lector automático | §2.3, §4.2, §4.3 (arts. 24, 26, 33) | Adri: abrir medellin.gov.co/normograma/docs/astrea/docs/a\\\_conmed\\\_0048\\\_2014.htm y comparar | No, pero hacerlo antes de enviar |
| FALTA-6 | Cotejar la cifra de población (4.179.996 en 2024) con la tabla municipal de proyecciones del DANE | §2.1 | Adri o coautor con acceso a dane.gov.co | No |
| FALTA-7 | Repositorio de código y datos con DOI | §2.8 y Data availability | Autores: Zenodo o Movebank (conjunto ya publicado en el I2D) | Sí |
| FALTA-8 | CRediT, financiación, conflicto de intereses y página de título | Declarations | Autores | Sí |

  

  - **Mejora opcional, no necesaria:** con la capa oficial "Retiros a la red hídrica" (servicio VM\_04\_Estructura\_Ecologica\_Principal, capa 8) se podría repetir el análisis riparario con los retiros normativos en lugar de franjas fijas de 30/60 m. Hoy el texto ya usa el drenaje oficial de Medellín como validación.

  

-----

## Highlights

  - GPS tracks of 70 animals were compared with connectivity plans at three scales
  - No plan matched the extent animals used; 41% of home ranges spanned two authorities
  - Birds placed home ranges along main rivers and streams
  - Mammals crossed major urban roads less than expected (exploratory)
  - Links projected for the urban–rural edge in 2014 were still projected in 2025

  

-----

## Abstract

Cities plan ecological connectivity through instruments drawn at different administrative scales, often for purposes other than animal movement. We compared GPS tracks of 70 individuals of 18 bird and mammal species in the Aburrá Valley, Colombia, with connectivity instruments at three scales: a departmental corridor network, a metropolitan network of urban green spaces and a municipal connectivity network adopted in a land-use plan. We then asked which landscape elements structured space use and movement. No instrument matched the extent of the space animals used. The metropolitan graph stopped at the urban jurisdictional boundary, whereas 41% of home ranges spanned both sides of it and most individuals crossed it in routine daily movements. Home ranges contained less of the departmental network than was within reach of capture sites (13 of 15 species), and animals neither selected nor avoided the municipal network. Along the urban–rural boundary, the municipal network existed on 3% of its length; elements projected there in 2014 covered another 37% and were still projected in the 2025 plan revision. Instead, birds placed home ranges along main rivers and streams, consistent with official drainage data. In an exploratory analysis, mammals crossed major and collector roads 40–50% as often as expected from their home-range geometry, whereas birds were unaffected. These elements are managed outside connectivity networks, as stream buffers and road infrastructure. Connectivity planning in Andean cities should be validated against movement data and should integrate watercourses and road design across the jurisdictions that animals use as one landscape.

  

*\[Palabras: 247.\]*

  

-----

## Keywords

Urban connectivity; GPS telemetry; land-use planning; scale mismatch; roads; riparian corridors

  

-----

## 1\. Introduction

Urban areas are expanding fastest in regions that concentrate the world's biodiversity. In the tropical Andes, urban land covered about 7450 km² in 2000, and an additional 23,250 km² has a high probability of becoming urban by 2030 (Seto et al., 2012). Cities are often located in species-rich regions, and urban biotas still reflect their regional species pool (Aronson et al., 2014). Their persistence therefore depends on exchange with the surrounding landscape. To maintain that exchange, planners increasingly design ecological networks with connectivity models. Yet nearly half of urban connectivity studies validated their models with biological data, and few of them used movement data (Habrich & Fahrig, 2025). Very few studies have tested whether modelled corridors discriminate real corridors from theoretical ones (Laliberté & St-Laurent, 2020). South American cities remain particularly understudied (Habrich & Fahrig, 2025; LaPoint et al., 2015).

  

Connectivity models used in planning estimate potential rather than actual connectivity. Landscape connectivity is the degree to which a landscape facilitates or impedes movement among resource patches (Taylor et al., 1993), and it varies with the behaviour of the species considered (Calabrese & Fagan, 2004). Graph-based models address potential connectivity, whereas "data on the individual movements of organisms provide the most direct estimate of actual connectivity" (Calabrese & Fagan, 2004, p. 534). The resistance surfaces behind these models usually derive from expert opinion and tend to confound movement behaviour with resource use (Zeller et al., 2012). Models built from one kind of behaviour can misidentify the places animals actually use (Abrahms et al., 2017a). Each model is also built for a purpose, a set of species and an extent. Those choices may have little to do with the animals that live where the model is applied.

  

The extent of a connectivity instrument is usually set by the authority that commissions it. Socio-political boundaries rarely coincide with ecological boundaries and have no ecological role by themselves (Dallimer & Strange, 2015). Yet the administrative division of land into urban and non-urban areas determines which institution manages each part of an animal's range (Dallimer & Strange, 2015). When institutions operate at scales that do not match the ecosystems they manage, scale mismatches arise, and one of their most pervasive consequences is the mismanagement of ecosystems (Cumming et al., 2006). In Andean valleys, the urban–rural gradient runs laterally and upslope rather than concentrically (Garizábal-Carmona et al., 2023). Departmental, metropolitan and municipal authorities may each plan connectivity for a different part of the same valley. Whether any of these plans corresponds to the space animals actually use is an empirical question that tracking data can answer.

  

The answer may also differ among individuals and taxa. Some individuals remain within stable home ranges and leave them only during occasional excursions; others alternate among sites, shift their range or disperse (Abrahms et al., 2017b; Fleming et al., 2014). Urban edges filter forest and open-area species differently (Garizábal-Carmona et al., 2026). Elements that are not part of connectivity plans may also shape movement. Watercourses concentrate resources for wetland birds, green spaces offer habitat within the built matrix, and roads act as barriers whose effect grows with width and traffic, while their verges conduct only a few species (Forman & Alexander, 1998, pp. 207, 215); road effects on abundance also differ among birds and mammals of different sizes (Fahrig & Rytwinski, 2009). If these elements structure movement more than planned networks do, connectivity depends on instruments managed outside the environmental sector.

  

Here we compare GPS tracks of 70 individuals of 18 bird and mammal species in the Aburrá Valley, Colombia, with connectivity instruments at three scales:

  

  - a departmental network of least-cost corridors designed for large forest mammals (Gobernación de Antioquia, 2023);
  - a metropolitan network of urban green spaces built for the metropolitan environmental authority (Área Metropolitana del Valle de Aburrá & Universidad Nacional de Colombia, 2020);
  - a municipal connectivity network adopted in Medellín's land-use plan (Concejo de Medellín, 2014).

  

We asked two questions. First, do instruments at the three scales correspond to the space animals use? Second, which landscape elements (green spaces, watercourses and roads) structure space use and movement?

  

Before analysing the data we predicted:

  

  - (H1) that the urban graph would cover residents with small home ranges well and wide-ranging individuals poorly;
  - (H2) that riparian land would be selected above its availability while remaining poorly covered by planning instruments;
  - (H3) that crossings of the urban–rural jurisdictional boundary would concentrate in excursions and dispersal.

  

The analysis of roads was added after these predictions and is reported as exploratory.

  

-----

## 2\. Methods

### 2.1 Study area

The Aburrá Valley (6.0–6.5° N, 75.2–75.7° W) is a narrow valley of the Central Andes of Colombia drained by the Medellín River. Its ten municipalities cover 1161 km² (CARTOANTIOQUIA 2012, 1:25,000) between ca. 1100 and 3150 m a.s.l. (Copernicus GLO-30 surface model) and held c. 4.2 million inhabitants in 2024 (DANE, 2025) \[FALTA-6\].

  

Urban land under the metropolitan environmental authority covers 184.7 km² (15.9%), ranging from 1.2% of the municipality of Barbosa to 71.7% of Itagüí. Rural land falls under the regional autonomous corporation of central Antioquia, except a small sliver near Envigado under a second corporation. Built cover occupies 65.1% of urban land and 2.2% of rural land, where trees (60.5%) and pastures (36.7%) form a mosaic (ESA WorldCover 2021; Zanaga et al., 2022). The urban–rural boundary lies at a median elevation of 1707 m, and 82% of rural tree cover lies above 1800 m.

### 2.2 Telemetry data and screening

Between October 2022 and October 2026 we tracked wild birds and mammals fitted with GPS-GSM tags (Cellular Tracking Technologies), except two felids fitted with GPS-Iridium collars (Telonics) (Restrepo, 2026). \[FALTA-1: tag models, mass and percentage of body mass, and programmed fix schedules.\] Observed modal fix intervals were 30–60 min for wetland birds, vultures and the puma, and 2–6 h for most mammals (Table S1).

  

**Merging and timestamps.** Data were stored in Movebank and in a public Darwin Core dataset of the metropolitan authority. All Darwin Core locations were also present in Movebank once Darwin Core timestamps were read as UTC. Two tags had dates shifted by the GPS week-number rollover, which we corrected.

  

**Individuals.** Of 79 tagged animals, seven produced no data. Five analysed individuals came from a wildlife rehabilitation centre, were translocated or were rescued; we repeated all analyses without them. For two released individuals we removed the post-release period (20 and 7 days).

  

**Screening.** We screened each individual independently and flagged:

  

  - fixes without coordinates (8197);
  - fixes before deployment (15);
  - terminal periods without movement (447);
  - low-quality fixes (dilution of precision \> 5 or unresolved satellite fixes; 1613);
  - isolated spikes (908).

  

Spikes included out-and-back jumps \> 1 km within ≤ 6 h that returned to within max(50 m, 2% of the jump) of the previous position. These fixes had higher dilution of precision (median 1.8 vs 1.0) and implausible altitudes (Bjørneraas et al., 2010 \[FALTA-4\]; Gupte et al., 2022, pp. 294–295).

  

**Final dataset.** The analysis included 598,764 fixes of 70 individuals of 18 species (median tracking duration 421 days, range 6–1407). Median fix intervals were 1 h for birds, 5 h for terrestrial mammals and 4 h for climbing mammals. Analyses sensitive to fix rate used tracks thinned to one fix every ≥ 3.75 h (178,175 fixes).

  

**Functional groups.** Individuals were grouped into flying birds (40 individuals, 11 species), terrestrial mammals (14, 4 species) and climbing mammals (16, 3 species). The common opossum (*Didelphis marsupialis*) is described as scansorial or semi-terrestrial in forest (Arévalo-Sandi et al., 2021; Cunha & Vieira, 2002). Its use of trees varies among landscapes: it moved mostly in trees in agricultural land (Vaughan & Hawkins, 1999) but denned mostly underground in a Venezuelan savanna (Sunquist et al., 1987). Our opossums used tree cover far more than its share of urban land (median 62% of fixes vs 25%), so we grouped them with arboreal species and repeated analyses with them as terrestrial.

### 2.3 Connectivity instruments at three scales

**Departmental.** The Main Ecological Network of Antioquia was designed with Linkage Mapper (McRae & Kavanagh, 2011) as least-cost corridors between nodes of ≥ 50 ha (Gobernación de Antioquia, 2023, pp. 19, 25–29):

  

  - the resistance surface was the inverse of habitat suitability averaged across seven large mammals;
  - covariables were weighted by experts;
  - land cover was mapped at 1:100,000.

  

Within the valley it covers 382 km² (33%).

  

**Metropolitan.** The Metropolitan Ecological Connectivity Network was produced for the metropolitan environmental authority in 2019 and delivered in 2020 (Área Metropolitana del Valle de Aburrá & Universidad Nacional de Colombia, 2020). Birds were the focal group: resistance was derived from bird diversity, modelled from occupancy surveys as a function of green-space density and spectral indices of built-up land and water (p. 11). Five models were fitted, three with circuit theory and two with least-cost paths. The fifth is a planar least-cost graph with urban green spaces as connection points, split into seven overlapping sectors (pp. 17–18). Each green space was then classified into one of six network elements by combining the five models (pp. 20–21). The network rests on an inventory of 194,863 urban green-space polygons (6646 ha; mostly grass verges, front gardens and street trees), and the graph has 156,674 nodes and 439,528 links. We evaluated the classified green-space polygons and the extent of the graph; the circuit-theory surfaces were not available to us.

  

**Municipal.** Medellín's land-use plan (Acuerdo 48 of 2014) adopted an ecological connectivity network as part of the city's main ecological structure. The network comprises "structuring nodes and links (current and future)" (Concejo de Medellín, 2014, Art. 24) \[FALTA-5\]. Nodes are forest fragments \> 6400 m². Links are areas prioritized by landscape metrics, including stream corridors. Projected nodes and links are high-hazard areas to be restored, located mainly on the urban–rural edge known as the Green Belt (Art. 33).

  

The adopted layer covers 97.6 km² (26% of Medellín): 74.5 km² of existing nodes, links and fragments, and 23.0 km² of projected elements. We compared it with the layer published by the municipality for the ongoing plan revision (service "POT 2025"; queried 4 October 2026). Medellín was the main municipality of 33 of 70 individuals and contained 71% of located boundary crossings, so we restricted municipal analyses to it.

### 2.4 Landscape elements

**Green spaces.** The metropolitan green-space polygons, as above.

  

**Watercourses.** We used two drainage layers:

  

  - a drainage network derived from the 30 m elevation model by flow accumulation (channels draining ≥ 0.5 km²), for the whole valley;
  - the official drainage network of Medellín's land-use plan, which distinguishes main drainages (the Medellín River and nine major streams) from secondary drainages.

  

In Medellín, 80% of derived channels lay within 30 m of official ones, but the official network was about seven times longer because it includes minor drainages. Riparian land was a 30 m strip on each side of channels (60 m as sensitivity).

  

**Roads.** We used the road hierarchy of Medellín's land-use plan (existing roads only, railway excluded), with three classes:

  

  - major roads (urban highways, arterials, first- and second-order national roads; 528 km);
  - collector roads (260 km);
  - rural roads (345 km).

  

**Trees.** Tree cover came from WorldCover. We also used the municipal urban tree inventory (317,662 living trees), which covers public space in urban land only.

  

All layers were rasterized to a common 10 m grid (EPSG:3116).

### 2.5 Movement strategies, home ranges and excursions

**Range residency.** We classified range residency with empirical semivariograms, using the slope of log semivariance against log lag at lags ≥ 7 days (Fleming et al., 2014).

  

**Residence periods and home ranges.** We segmented tracks into residence periods (≥ 30 days without displacement beyond max(2 × r₉₀, 1 km)). For periods with ≥ 50 fixes we estimated 95% kernel utilization distributions (UD95) with half the reference bandwidth (Worton, 1989 \[FALTA-3\]); analyses were repeated with the full bandwidth.

  

**Excursions.** Following Burt's (1943, p. 351) distinction between the home range and "occasional sallies outside the area", and distance and duration criteria (Karns et al., 2011), an excursion was a run of ≥ 2 fixes that met three conditions:

  

  - it lay outside the UD95;
  - it reached a distance from its edge greater than the radius of a circle of equal area;
  - it included the species' resting period or lasted ≥ 24 h, and returned within 30 days.

  

**Strategies.** We assigned one strategy to each individual:

  

  - resident;
  - resident with excursions;
  - multisite: ≥ 1 return to a site used for ≥ 30 days, with sites separated by more than twice the home-range diameter;
  - range shift: displacement of an adult without return, which abandons "the old home range" and sets up "a new one" (Burt, 1943, p. 351);
  - dispersal: the same displacement in a juvenile or subadult (Howard, 1960, p. 152).

### 2.6 Question 1: correspondence between instruments and space use

**Home ranges split between authorities.** We calculated the proportion of each individual's main UD95 within the urban jurisdiction. A home range was split if 5–95% of it lay on each side.

  

**Coverage.** We calculated the proportion of fixes and of the UD95 within each instrument.

  

**Boundary crossings.** A crossing was a change between consecutive fixes in whether the animal was inside the urban jurisdiction. Fixes within 20 m of the boundary (|d| \< 20 m) inherited the previous state. Each crossing was classified as routine (within a residence period), excursion, or range shift or dispersal.

  

To check whether crossing frequency simply reflects where home ranges lie, we rotated each thinned track 199 times around its median position. We compared observed and expected days with a crossing per 100 tracking days. This is a geometric control: a line with no ecological counterpart should be crossed as often as the geometry of home ranges predicts.

  

**Second-order selection** (Johnson, 1980, p. 69). We compared the composition of each individual's largest home range with ≥ 90% of its area in the valley against the area reachable from its capture site. The reachable area was a disc around the first valid fix, whose radius was the species' median 95th-percentile distance from the capture site (minimum 1 km).

  

We used this reachable area rather than the whole valley because capture sites were mostly urban. With the whole valley as availability, rural instruments would appear avoided by design. For the municipal network, use and availability were restricted to Medellín.

### 2.7 Question 2: landscape elements that structure space use and movement

**Selection.** We estimated:

  

  - second-order selection of green spaces and riparian land, as above, using the derived drainage for the valley and the official drainage (main and all drainages) in Medellín;
  - third-order selection with Manly selection ratios: fixes within the UD95 against the composition of the UD95, using each individual's main residence period (Manly et al., 2002 \[FALTA-2\]);
  - third-order selection of urban tree density (inventory trees per hectare within 50 m), within the inventoried urban part of each home range.

  

**Roads (exploratory).** For individuals with ≥ 25% of thinned fixes in Medellín and ≥ 20 steps with both ends in Medellín, we computed:

  

  - the proportion of steps whose straight segment crossed each road class;
  - the same proportion for 199 rotated tracks, counting only steps with both ends in Medellín in each rotation.

  

We also split major and collector roads into 50 m pieces with and without tree cover (≥ 20%, 30% or 50% of WorldCover pixels within 20 m).

### 2.8 Inference and verification

The individual was the sampling unit (Hebblewhite & Haydon, 2010, p. 2304). We tested log ratios against zero with Wilcoxon signed-rank tests within functional groups. Because a few species contributed many individuals, we also:

  

  - used species as the unit (mean log ratio per species);
  - repeated each test leaving out one species at a time;
  - applied Benjamini–Hochberg corrections within families of tests.

  

Sensitivity analyses excluded rehabilitated, translocated and rescued individuals, used the full kernel bandwidth, a 60 m riparian strip and the opossum as terrestrial. An analyst who had not taken part in the analyses reproduced the main results with separate code. Analyses used Python (NumPy, SciPy, GeoPandas, Shapely, Rasterio, pysheds, statsmodels). Code and data are available at \[FALTA-7\].

  

-----

## 3\. Results

### 3.1 Three planning scales, three footprints

The three instruments covered different parts of the valley (Fig. 1):

  

  - **Metropolitan graph.** Confined to the urban jurisdiction: 95% of its links lay within it, and its seven sectors formed disconnected graphs.
  - **Departmental network.** Covered 33% of the valley, mostly rural land, with largely straight corridors that crossed the city.
  - **Municipal network (Medellín).** Spanned both sides of the boundary (12% of urban and 32% of rural land). Where the two jurisdictions meet, however, its existing nodes and links lay along only 2.9% of the boundary, and projected elements along another 36.8% (Fig. 5).

  

The layer published for the 2025 plan revision was identical to the 2014 layer: the same 776 polygons, with the same area by type. None of the projected nodes or links had been reclassified as existing.

### 3.2 Individuals followed five movement strategies

Among the 70 individuals (Fig. 2):

  

|  |  |
| :-: | :-: |
| \*\*Strategy\*\* | \*\*Individuals\*\* |
| Resident | 35 |
| Resident with excursions | 19 |
| Multisite | 6 |
| Range shift | 1 |
| Dispersal | 4 |
| Insufficient data | 5 |

  

Median home-range size (main residence period) differed among groups: 0.05 km² for climbing mammals, 0.89 km² for terrestrial mammals and 4.25 km² for birds. We identified 111 excursions by 28 individuals, with a median duration of 24 h and a median distance of 3.6 km beyond the home-range edge.

### 3.3 Home ranges spanned jurisdictions and instruments

Twenty-six of 64 home ranges (41%) were split between the urban and rural jurisdictions (Fig. 3):

  

  - 20 of 37 birds;
  - 4 of 13 terrestrial mammals;
  - 2 of 14 climbing mammals.

  

Forty-three of 70 individuals (61%) crossed the jurisdictional boundary. Crossings were part of routine movement: the median individual made 100% of its crossings within residence periods. Across all crossings, 99.5% were routine and 0.4% occurred during excursions; this did not change with thinned tracks (42 individuals). H3 was therefore not supported.

  

Crossing frequency matched the geometry of home ranges. Days with a crossing per 100 tracking days did not differ from rotated tracks (median observed/expected 0.95, p = 0.07, n = 51), and no individual crossed less than expected.

  

Coverage by the metropolitan graph declined from residents to wide-ranging strategies, descriptively consistent with H1. The graph footprint contained a median 98.5% of fixes of residents, 91% of residents with excursions, 84% of the range-shifting individual, 68% of dispersers and 53% of multisite individuals. Climbing mammals lay almost entirely within it.

### 3.4 Animals settled away from the regional network and showed no selection for the municipal one

Home ranges contained less of the departmental network than was reachable from capture sites (median ratio 0.76, n = 59, p = 0.0001, q = 0.002; Fig. 4). The result held with species as the unit (13 of 15 species, p = 0.002) and when any one species was excluded.

  

In Medellín, home ranges contained the municipal network in proportion to its availability (ratio 1.33, n = 28, p = 0.19; 5 species above, 6 below).

  

Protected areas were absent within reach of about a third of capture sites (median ratio 1.00; signed-rank p = 0.046). Their strong apparent avoidance when the whole valley was used as availability (ratio 0.02) was an artefact of urban capture sites.

### 3.5 Main watercourses structured where birds settled

Birds placed home ranges where riparian land was more frequent than within reach of their capture sites:

  

  - derived drainage: ratio 1.52 (n = 34, p = 0.005; 60 m strip 1.50, p = 0.001; both q ≤ 0.026);
  - 8 of 10 species in the same direction;
  - with species as the unit, the pattern was not significant (p = 0.28); excluding one species at a time, the 60 m result held (maximum p = 0.020) but the 30 m result did not (maximum p = 0.062).

  

The official drainage of Medellín refined this result (Fig. 4):

  

  - **Main watercourses:** birds settled along them (ratio 1.66, n = 19, p = 0.002; all seven species ≥ 1.0).
  - **Full drainage network, including minor channels:** no selection by birds (0.94, p = 0.44). Climbing mammals placed home ranges along it (1.68, n = 7, p = 0.03), but the sample was small.

  

Within home ranges, no group selected riparian land (birds w = 1.00, p = 0.91). H2 was therefore supported only for the placement of home ranges and only for main watercourses.

  

Evidence for green spaces was weak:

  

  - Home ranges did not contain more green space than was reachable (ratio 1.33, p = 0.82).
  - Within home ranges, mammals used green-space polygons more than available (w = 1.21, n = 17, p = 0.006), but this did not survive correction within the family of third-order tests (q = 0.13) or the exclusion of single species.
  - Urban tree density from the inventory was not selected within home ranges (use/availability 0.95, n = 44, p = 0.48).

### 3.6 Mammals crossed major and collector roads less than expected (exploratory)

Thirty-three individuals had enough steps in Medellín for the road analysis (20 birds and 13 mammals; Fig. 6). Tests included individuals with observed or expected crossings of each road class (11 mammals for major roads, 10 for collector roads).

  

**Birds.** They crossed all road classes as often as their home-range geometry predicted (median ratios 0.83–1.06 for the three classes, all p ≥ 0.09).

  

**Mammals.** They crossed:

  

  - major roads at 39% of the expected rate (9 of 11 individuals below expectation, p = 0.019);
  - collector roads at 51% (8 of 10, p = 0.020).

  

Robustness of the mammal result:

  

  - The collector-road result held when any single species was excluded (maximum p = 0.039).
  - The major-road result depended on foxes and opossums (maximum p = 0.11).
  - Neither survived correction across 29 road tests (q = 0.07).
  - An independent analysis reproduced the direction and magnitude.

  

Whether road pieces had tree cover made no consistent difference. Major roads with tree cover were crossed less than expected at all thresholds (ratios 0.37–0.56), but the comparison with treeless pieces changed with the threshold and with the definition of road pieces in the independent analysis.

  

-----

## 4\. Discussion

### 4.1 Planning scales and movement do not meet

GPS tracking showed that connectivity is planned at three scales that do not correspond to how animals in the Aburrá Valley use space:

  

  - **Departmental network:** animals settled away from it.
  - **Metropolitan graph:** stopped where 41% of home ranges continued.
  - **Municipal network:** spans both jurisdictions, but along the boundary its links were projected in 2014 and are still recorded as projected in 2025.

  

Meanwhile, the elements associated with space use and movement lie largely outside these networks: main watercourses for birds and, tentatively, roads for mammals. Answering our two questions together: actual connectivity in the valley depends on elements that connectivity plans do not target, across a boundary that the plans divide.

### 4.2 Instruments built for other purposes

Each instrument reflects the purpose for which it was built:

  

  - **Departmental network:** designed for seven large forest mammals, with resistance weighted by experts and land cover at 1:100,000 (Gobernación de Antioquia, 2023, pp. 19, 25–29). That animals in a metropolitan valley settled away from it does not make the network wrong for its target species. It shows that it cannot be read as connectivity for urban wildlife, consistent with evidence that resistance surfaces built from expert opinion confound resource use with movement (Zeller et al., 2012). The regional study itself acknowledges that it is difficult to anticipate which corridor organisms will use (Gobernación de Antioquia, 2023, p. 85).
  - **Metropolitan network:** an inventory of urban green space classified with resistance surfaces derived from bird diversity, not from movement (Área Metropolitana del Valle de Aburrá & Universidad Nacional de Colombia, 2020, pp. 11, 20–21). Its extent is the jurisdiction of the authority that commissioned it.
  - **Municipal network:** combines forest fragments, stream corridors and the restoration of high-hazard land on the urban edge. Its projected links are defined by hazard and restoration criteria rather than by wildlife movement (Concejo de Medellín, 2014, Art. 33).

  

None of these purposes is illegitimate, and graph models may offer the greatest benefit-to-effort ratio at metropolitan scales (Calabrese & Fagan, 2004, p. 535). But more than 70% of urban graph-based studies remain unvalidated (Habrich & Fahrig, 2025). Our comparison suggests that the mismatch lies less in the routes predicted than in the species, extents and purposes for which instruments are built.

### 4.3 What structures movement is managed elsewhere

**Watercourses.** Birds settled along the Medellín River and main streams. This is consistent with the recent colonization of the valley by the bare-faced ibis, which began along the river and urban lakes (Gómez-Londoño & Pulgarín-R., 2024). Watercourses are already protected by stream buffers under national law, up to 30 m on each side (Decreto-Ley 2811 de 1974, Art. 83; Decreto 2245 de 2017), and Medellín's plan sets buffers of 30 m in rural land and 10–60 m in urban land (Concejo de Medellín, 2014, Art. 26). Several stream corridors are also links of the municipal network (Art. 33). The gap is therefore one of implementation and integration rather than of designation.

  

**Roads.** Mammals crossed major and collector roads less than expected from the geometry of their home ranges. Road width and traffic are major determinants of the barrier effect, and roads are a major source of mortality (Forman & Alexander, 1998, pp. 207, 215); mid-sized and large mammals tend to decline near roads (Fahrig & Rytwinski, 2009). They are planned by the mobility sector, not as part of ecological networks. Tree cover along roads did not consistently increase crossing; whether canopy bridges or underpasses would help climbing and terrestrial mammals remains to be tested. This result is exploratory and based on 13 mammals, mostly foxes and opossums.

  

**Green spaces.** Evidence was weak, which is consistent with green-space polygons that are mostly small verges and gardens.

### 4.4 The boundary as a gap in implementation

The jurisdictional boundary has no ecological role by itself (Dallimer & Strange, 2015). In our rotation analysis, crossing frequency did not differ from that expected from home-range geometry, although two individuals (a disperser and a range-shifting fox) crossed more often. The boundary matters because it divides the management of space that animals use as a unit. Medellín's plan recognized this: it projected restoration along the urban–rural edge. Eleven years later the official layer still lists those elements as projected. Monitoring of the city's ecological network has been reported as lacking targets and indicators (Jaramillo & Montoya González, 2018, p. 27). The scale mismatch described by Cumming et al. (2006) here takes the form of a plan that diagnoses the right place but does not reach it.

### 4.5 Limitations

  - **Sample.** Few individuals per species, and an assemblage dominated by open-area and wetland birds, limit inference to functional groups. Forest specialists are under-represented.
  - **Fix intervals.** Intervals of 1–8 h prevent path-level tests of links and approximate crossing locations.
  - **Home ranges.** Kernel home ranges ignore autocorrelation.
  - **Municipal and road layers.** They exist only for Medellín. The road analysis was exploratory and added after our predictions.
  - **What the 2025 comparison shows.** It shows the state of the official record, not of the ground.
  - **Metropolitan network.** We evaluated its classified green spaces and graph extent, not its circuit-theory surfaces.
  - **Confounding.** Urbanization and elevation are confounded along the valley (Garizábal-Carmona et al., 2023).

  

-----

## 5\. Conclusions and implications for planning

Connectivity planned at departmental, metropolitan and municipal scales did not correspond to how urban wildlife moved in an Andean valley. The elements that did structure movement are managed by other instruments. For each actor:

  

1.  **Departmental authority.** Departmental networks should state the species and extents for which they are valid and add urban and peri-urban species when applied to metropolitan areas.
2.  **Metropolitan authority.** Metropolitan green-space graphs should extend beyond the jurisdictional boundary, where 41% of tracked home ranges continued.
3.  **Municipalities.** Projected links on the urban–rural edge need funding, deadlines and monitoring. Movement data can prioritize where to build them first.
4.  **Water and mobility authorities.** Main watercourses and road crossings for fauna should be integrated into connectivity planning across jurisdictions.
5.  **All plans.** Connectivity plans should be validated with movement data before they guide investment (Laliberté & St-Laurent, 2020).

  

-----

## Figures

  - **Fig. 1.** Connectivity is planned at three scales with different footprints (Fig1\_instrumentos.png).
  - **Fig. 2.** Individuals followed five movement strategies (Fig2\_estrategias.png).
  - **Fig. 3.** Home ranges spanned jurisdictions and instruments (Fig3\_area\_vida\_partida.png).
  - **Fig. 4.** Home ranges contained less of the regional network and, for birds, more main watercourses than was reachable (Fig4\_seleccion\_segundo\_orden.png).
  - **Fig. 5.** Along the urban–rural boundary, Medellín's network is mostly projected, and most crossings fall outside it (Fig5\_pot\_limite.png).
  - **Fig. 6.** Mammals crossed major and collector roads less than expected; birds did not (exploratory) (Fig6\_vias.png).
  - **Fig. S1.** Land cover across the jurisdictional boundary (FigS1\_cobertura\_limite.png).
  - **Table S1.** Observed fix intervals by species (TablaS1\_intervalos\_fijacion.csv).

  

-----

## Declarations

**CRediT authorship contribution statement.** \[FALTA-8\]

  

**Declaration of generative AI and AI-assisted technologies in the manuscript preparation process.** During the preparation of this work the authors used Claude (Anthropic) to structure the manuscript, organize the literature, write analysis code and draft text. After using this tool, the authors reviewed and edited the content as needed and take full responsibility for the content of the published article.

  

**Data availability.** Telemetry locations to March 2024 are published as a Darwin Core dataset (Restrepo, 2026). Full tracks, layers and code: \[FALTA-7\].

  

**Funding.** \[FALTA-8\]

  

**Declaration of competing interest.** \[FALTA-8\]

  

-----

## References

Abrahms, B., Sawyer, S. C., Jordan, N. R., McNutt, J. W., Wilson, A. M., & Brashares, J. S. (2017a). Does wildlife resource selection accurately inform corridor conservation? *Journal of Applied Ecology, 54*(2), 412–422. <https://doi.org/10.1111/1365-2664.12714>

  

Abrahms, B., Seidel, D. P., Dougherty, E., Hazen, E. L., Bograd, S. J., Wilson, A. M., McNutt, J. W., Costa, D. P., Blake, S., Brashares, J. S., & Getz, W. M. (2017b). Suite of simple metrics reveals common movement syndromes across vertebrate taxa. *Movement Ecology, 5*, 12. <https://doi.org/10.1186/s40462-017-0104-2>

  

Área Metropolitana del Valle de Aburrá & Universidad Nacional de Colombia. (2020). *Análisis de la conectividad ecológica funcional y estructural en el Área Metropolitana del Valle de Aburrá: Informe final, análisis de conectividad ecológica* (Contrato interadministrativo 1344 de 2018) \[Technical report\]. Área Metropolitana del Valle de Aburrá.

  

Arévalo-Sandi, A. R., Gonçalves, A. L. S., Onizawa, K., Yabe, T., & Spironello, W. R. (2021). Mammal diversity among vertical strata and the evaluation of a survey technique in a central Amazonian forest. *Papéis Avulsos de Zoologia, 61*, e20216133. <https://doi.org/10.11606/1807-0205/2021.61.33>

  

Aronson, M. F. J., La Sorte, F. A., Nilon, C. H., Katti, M., Goddard, M. A., Lepczyk, C. A., Warren, P. S., Williams, N. S. G., Cilliers, S., Clarkson, B., Dobbs, C., Dolan, R., Hedblom, M., Klotz, S., Kooijmans, J. L., Kühn, I., MacGregor-Fors, I., McDonnell, M., Mörtberg, U., … Winter, M. (2014). A global analysis of the impacts of urbanization on bird and plant diversity reveals key anthropogenic drivers. *Proceedings of the Royal Society B: Biological Sciences, 281*(1780), 20133330. <https://doi.org/10.1098/rspb.2013.3330>

  

Bjørneraas, K., Van Moorter, B., Rolandsen, C. M., & Herfindal, I. (2010). Screening Global Positioning System location data for errors using animal movement characteristics. *Journal of Wildlife Management, 74*(6), 1361–1366. <https://doi.org/10.2193/2009-405>

  

Burt, W. H. (1943). Territoriality and home range concepts as applied to mammals. *Journal of Mammalogy, 24*(3), 346–352. <https://doi.org/10.2307/1374834>

  

Calabrese, J. M., & Fagan, W. F. (2004). A comparison-shopper's guide to connectivity metrics. *Frontiers in Ecology and the Environment, 2*(10), 529–536.

  

Concejo de Medellín. (2014, December 17). *Acuerdo 48 de 2014, por medio del cual se adopta la revisión y ajuste de largo plazo del Plan de Ordenamiento Territorial del Municipio de Medellín y se dictan otras disposiciones complementarias*. Gaceta Oficial No. 4267. <https://www.medellin.gov.co/normograma/docs/astrea/docs/a_conmed_0048_2014.htm>

  

Cumming, G. S., Cumming, D. H. M., & Redman, C. L. (2006). Scale mismatches in social-ecological systems: Causes, consequences, and solutions. *Ecology and Society, 11*(1), 14. <https://doi.org/10.5751/ES-01569-110114>

  

Cunha, A. A., & Vieira, M. V. (2002). Support diameter, incline, and vertical movements of four didelphid marsupials in the Atlantic forest of Brazil. *Journal of Zoology, 258*(4), 419–426. <https://doi.org/10.1017/S0952836902001565>

  

Dallimer, M., & Strange, N. (2015). Why socio-political borders and boundaries matter in conservation. *Trends in Ecology & Evolution, 30*(3), 132–139. <https://doi.org/10.1016/j.tree.2014.12.004>

  

DANE. (2025). *Proyecciones de población municipal 2020–2035* \[Data set\]. Departamento Administrativo Nacional de Estadística. <https://www.dane.gov.co/index.php/estadisticas-por-tema/demografia-y-poblacion/proyecciones-de-poblacion> \[FALTA-6\]

  

Decreto 2245 de 2017. (2017, December 29). *Por el cual se reglamenta el artículo 206 de la Ley 1450 de 2011 y se adiciona una sección al Decreto 1076 de 2015, en lo relacionado con el acotamiento de rondas hídricas*. Ministerio de Ambiente y Desarrollo Sostenible, Colombia.

  

Decreto-Ley 2811 de 1974. (1974, December 18). *Código Nacional de Recursos Naturales Renovables y de Protección al Medio Ambiente* (Art. 83). Presidencia de la República de Colombia.

  

Fahrig, L., & Rytwinski, T. (2009). Effects of roads on animal abundance: An empirical review and synthesis. *Ecology and Society, 14*(1), Article 21. <https://doi.org/10.5751/ES-02815-140121>

  

Fleming, C. H., Calabrese, J. M., Mueller, T., Olson, K. A., Leimgruber, P., & Fagan, W. F. (2014). From fine-scale foraging to home ranges: A semivariance approach to identifying movement modes across spatiotemporal scales. *The American Naturalist, 183*(5), E154–E167. <https://doi.org/10.1086/675504>

  

Forman, R. T. T., & Alexander, L. E. (1998). Roads and their major ecological effects. *Annual Review of Ecology and Systematics, 29*, 207–231. <https://doi.org/10.1146/annurev.ecolsys.29.1.207>

  

Garizábal-Carmona, J. A., Betancur, J. S., Montoya-Arango, S., Franco-Espinosa, L., Ruíz-Giraldo, N., & Mancera-Rodríguez, N. J. (2023). Bird diversity across an Andean city: The limitation of species richness values and watershed scales. *Acta Biológica Colombiana, 28*(3), 506–516. <https://doi.org/10.15446/abc.v28n3.101974>

  

Garizábal-Carmona, J. A., Cáceres-López, H. D., Mancera-Rodríguez, N. J., & MacGregor-Fors, I. (2026). Urban landscapes as ecological filters: Insights from a Neotropical bird assemblage. *Ecology, 107*(2), e70277. <https://doi.org/10.1002/ecy.70277>

  

Gobernación de Antioquia. (2023). *Informe contrato No. 4600012276* \[Technical report by R. J. Pérez Montalvo on the Main Ecological Network of Antioquia\]. Secretaría de Ambiente y Sostenibilidad. <https://www.antioquia.gov.co/images/PDF2/MedioAmbiente/SIDAP/DocumentoTecnicoRED_Conectividad_SIDAP_2021_CONTRATO_4600012276.pdf>

  

Gómez-Londoño, D. M., & Pulgarín-R., P. C. (2024). Colonización, patrones de distribución y uso de hábitat del ibis negro *Phimosus infuscatus* en la zona urbana del Valle de Aburrá, Colombia. *Ornitología Neotropical, 35*(2), 70–79. <https://doi.org/10.58843/ornneo.v35i2.873>

  

Gupte, P. R., Beardsworth, C. E., Spiegel, O., Lourie, E., Toledo, S., Nathan, R., & Bijleveld, A. I. (2022). A guide to pre-processing high-throughput animal tracking data. *Journal of Animal Ecology, 91*(2), 287–307. <https://doi.org/10.1111/1365-2656.13610>

  

Habrich, A. K., & Fahrig, L. (2025). Systematic map of urban connectivity research reveals a dearth of validation of connectivity estimates. *Current Landscape Ecology Reports, 10*, 5. <https://doi.org/10.1007/s40823-025-00106-y>

  

Hebblewhite, M., & Haydon, D. T. (2010). Distinguishing technology from biology: A critical review of the use of GPS telemetry data in ecology. *Philosophical Transactions of the Royal Society B: Biological Sciences, 365*(1550), 2303–2312. <https://doi.org/10.1098/rstb.2010.0087>

  

Howard, W. E. (1960). Innate and environmental dispersal of individual vertebrates. *The American Midland Naturalist, 63*(1), 152–161. <https://doi.org/10.2307/2422936>

  

Jaramillo, C. H., & Montoya González, S. (2018). *Estado del arte de la red ecológica de Medellín, en el contexto metropolitano* \[Technical report\]. Observatorio de Políticas Públicas del Concejo de Medellín. <https://www.concejodemedellin.gov.co/wp-content/uploads/files/2019-08/red-edologica-2018.pdf>

  

Johnson, D. H. (1980). The comparison of usage and availability measurements for evaluating resource preference. *Ecology, 61*(1), 65–71. <https://doi.org/10.2307/1937156>

  

Karns, G. R., Lancia, R. A., DePerno, C. S., & Conner, M. C. (2011). Investigation of adult male white-tailed deer excursions outside their home range. *Southeastern Naturalist, 10*(1), 39–52. <https://doi.org/10.1656/058.010.0104>

  

Laliberté, J., & St-Laurent, M.-H. (2020). Validation of functional connectivity modeling: The Achilles' heel of landscape connectivity mapping. *Landscape and Urban Planning, 202*, 103878. <https://doi.org/10.1016/j.landurbplan.2020.103878>

  

LaPoint, S., Balkenhol, N., Hale, J., Sadler, J., & van der Ree, R. (2015). Ecological connectivity research in urban areas. *Functional Ecology, 29*(7), 868–878. <https://doi.org/10.1111/1365-2435.12489>

  

Manly, B. F. J., McDonald, L. L., Thomas, D. L., McDonald, T. L., & Erickson, W. P. (2002). *Resource selection by animals: Statistical design and analysis for field studies* (2nd ed.). Kluwer Academic Publishers. <https://doi.org/10.1007/0-306-48151-0> \[FALTA-2\]

  

McRae, B. H., & Kavanagh, D. M. (2011). *Linkage Mapper connectivity analysis software* \[Computer software\]. The Nature Conservancy. <https://linkagemapper.org>

  

Restrepo, A. (2026). *GPS/GSM and GPS/Iridium telemetry data of mammals and birds present in urban areas of Valle de Aburrá, Antioquia, Colombia* (Version 1.3) \[Data set\]. Instituto de Investigación de Recursos Biológicos Alexander von Humboldt. <https://i2d.humboldt.org.co/ceiba/resource?r=rrbb_aves_amva_2022&v=1.3>

  

Seto, K. C., Güneralp, B., & Hutyra, L. R. (2012). Global forecasts of urban expansion to 2030 and direct impacts on biodiversity and carbon pools. *Proceedings of the National Academy of Sciences, 109*(40), 16083–16088. <https://doi.org/10.1073/pnas.1211658109>

  

Sunquist, M. E., Austad, S. N., & Sunquist, F. (1987). Movement patterns and home range in the common opossum (*Didelphis marsupialis*). *Journal of Mammalogy, 68*(1), 173–176. <https://doi.org/10.2307/1381069>

  

Taylor, P. D., Fahrig, L., Henein, K., & Merriam, G. (1993). Connectivity is a vital element of landscape structure. *Oikos, 68*(3), 571–573. <https://doi.org/10.2307/3544927>

  

Vaughan, C., & Hawkins, L. F. (1999). Late dry season habitat use of common opossum, *Didelphis marsupialis* (Marsupialia: Didelphidae) in neotropical lower montane agricultural areas. *Revista de Biología Tropical, 47*(1–2), 263–269.

  

Worton, B. J. (1989). Kernel methods for estimating the utilization distribution in home-range studies. *Ecology, 70*(1), 164–168. <https://doi.org/10.2307/1938423>

  

Zanaga, D., Van De Kerchove, R., Daems, D., De Keersmaecker, W., Brockmann, C., Kirches, G., Wevers, J., Cartus, O., Santoro, M., Fritz, S., Lesiv, M., Herold, M., Tsendbazar, N.-E., Xu, P., Ramoino, F., & Arino, O. (2022). *ESA WorldCover 10 m 2021 v200* \[Data set\]. Zenodo. <https://doi.org/10.5281/zenodo.7254221>

  

Zeller, K. A., McGarigal, K., & Whiteley, A. R. (2012). Estimating landscape resistance to movement: A review. *Landscape Ecology, 27*(6), 777–797. <https://doi.org/10.1007/s10980-012-9737-0>

  

*\[41 referencias.\]*