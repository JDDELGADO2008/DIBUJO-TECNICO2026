# Ficha de registro: Semana 14

**Curso:** ICT401 – Dibujo Técnico Asistido por Computadora
**Semana:** 14
**Tema:** Vista explosionada, lista de componentes y documentación de conjuntos
**Estudiante:** jose daniel delgado
**Fecha:** 22 de octubre de 2026
**Archivo o enlace del conjunto:** (enlace de Fusion o ruta, p. ej. `S14_Conjunto_Apellido_Nombre_v1`)

## Propósito

Esta ficha registra las decisiones, comprobaciones, dificultades y evidencias de la documentación del conjunto. Se trabaja con el ensamblaje validado en la Semana 13. No sustituye la rúbrica oficial de la Fase 3 ni la Prueba Corta 3.

## Criterios normativos de revisión

La aplicación de estas normas es didáctica y selectiva; no constituye una certificación integral de conformidad normativa. Registre la evidencia o la limitación encontrada.

| Referencia | Criterio que se aplica | Evidencia o limitación registrada |
|---|---|---|
| INTE/ISO 128-1:2024 | La vista comunica el conjunto sin ambigüedad y conserva la identidad de sus componentes. | La vista explosionada muestra Base, Soporte y Pasador sin ocultarse entre sí; cada pieza conserva su nombre en el Browser y su globo en el Drawing. |
| INTE/ISO 128-2:2023 | Contornos, ejes, líneas ocultas y líneas de trayectoria se distinguen; las trayectorias no sustituyen los contornos. | Contornos visibles en línea continua gruesa; ejes y ocultas con su tipo de línea propio; las líneas de trayectoria (Show Trail Lines) son finas y solo apoyan la secuencia. ⚠️ Confirmar visualmente. |
| INTE/ISO 128-3:2025 / ISO 5456-2 | La orientación, las vistas y el método de proyección son coherentes. | Front, Top y Right en primer diedro (First Angle), proyectadas desde Front. La explosionada usa orientación isométrica del mismo conjunto. |
| ISO 5457 | La hoja, orientación, escala y distribución permiten leer la documentación. | ⚠️ COMPLETAR (tamaño de hoja, orientación y escala usados en cada hoja). |
| INTE/ISO 7200:2008 | El cajetín o encabezado identifica conjunto, estudiante, fecha, unidades, escala y versión cuando estén disponibles. | Cajetín completado con conjunto, estudiante, fecha, unidades y escala. ⚠️ Registrar aquí cualquier campo (p. ej. versión/revisión) que la plantilla no ofrezca. |
| ISO 7573 / ISO 6433 | La lista, las cantidades y los números de referencia corresponden a componentes reales. | Parts List generada desde el diseño (no transcrita); 3 ítems que coinciden con el Browser; cada globo aparece una sola vez. |
| ISO 16792:2021 | Modelo, Storyboard, Drawing, lista y evidencias corresponden a la misma versión. | Todo procede de la versión ⚠️ COMPLETAR (nombre/versión del archivo). |

**Alcance:** no se aplican ISO 129-1, ISO 8015 ni ISO 2768 como requisitos de esta semana porque no se solicitan cotas funcionales ni tolerancias de fabricación.

## Producto documental integrado

La entrega debe corresponder a **un único Drawing de Fusion**. Registre aquí cómo integró las representaciones:

| Elemento obligatorio | Hoja o ubicación dentro del Drawing | Comprobado |
|---|---|:---:|
| Vistas normales `Front`, `Top` y `Right` | Hoja 1 (vistas ortogonales) | [ ] |
| Proyección de primer diedro (sistema europeo) | Hoja 1; método First Angle en las propiedades del Drawing | [ ] |
| Símbolo o configuración del método de proyección | Hoja 1, símbolo de proyección (o configuración First Angle si la plantilla no lo muestra) | [ ] |
| Vista explosionada del `Storyboard` | Hoja 2 (vista base con representación del Storyboard) | [ ] |
| Lista de componentes | Hoja 2, junto a la vista explosionada | [ ] |
| Globos o números de referencia | Hoja 2, alrededor de la vista explosionada | [ ] |
| Cajetín e identificación del conjunto | Hojas 1 y 2 (misma identificación del conjunto) | [ ] |
| Nombre y versión del modelo de origen | Cajetín y esta ficha: ⚠️ COMPLETAR | [ ] |

Las vistas pueden distribuirse en varias hojas, pero deben permanecer dentro del mismo Drawing. No entregue la vista explosionada y las vistas ortogonales como documentos independientes.

### Distribución de la hoja

| Control de distribución | Registro o evidencia |
|---|---|
| Vista principal utilizada como referencia | `Front` es la vista principal; `Top` y `Right` se proyectan desde ella. |
| `Top` colocado debajo de `Front` | Sí, en Hoja 1, alineado verticalmente con `Front`. |
| `Right` colocado a la izquierda de `Front` | Sí, en Hoja 1, alineado horizontalmente con `Front` (primer diedro). |
| Alineación y separación entre vistas ortogonales | Vistas proyectadas desde `Front` (no movidas de forma independiente); separación suficiente para no tocarse. |
| Zona reservada para la vista explosionada | Hoja 2, zona central/derecha, sin romper las alineaciones de la Hoja 1. |
| Ubicación de la lista y los globos | Lista cerca de la vista explosionada, sin cubrir piezas ni trayectorias; globos alrededor con líneas de referencia cortas. |
| Cajetín libre de superposiciones | Ninguna vista, lista, globo o texto invade el cajetín. |
| Hoja adicional utilizada dentro del mismo Drawing, si corresponde | Sí: Hoja 2 para explosionada, lista y globos (mismo Drawing). ⚠️ Cambiar si todo cupo en una hoja. |

## Lección 1. Análisis del ensamblaje y planificación

### 1. Estado inicial

| Elemento | Registro |
|---|---|
| Nombre del archivo original | ⚠️ COMPLETAR (archivo validado de la Semana 13) |
| Nombre de la copia de trabajo | ⚠️ COMPLETAR (p. ej. `S14_Conjunto_Apellido_Nombre_v1`, creada con Save As) |
| Versión o fecha de respaldo | Respaldo guardado el 22 de octubre de 2026 antes de iniciar la representación. |
| Número de componentes | 3 |
| Componente de referencia | Base |
| Estado inicial del ensamblaje | Ensamblaje validado en Semana 13, completo y en posición original; el Browser muestra componentes (no cuerpos sueltos). |

**Captura del conjunto antes de crear la vista explosionada:**
![Conjunto inicial de la Semana 13](evidencias/S14_E1_Conjunto_Inicial.png)

| Análisis de referencia | Registro |
|---|---|
| ¿Por qué se mantiene ese componente como referencia? | La Base sostiene y recibe al Soporte, por lo que permite interpretar la posición de las demás piezas. Si todas se desplazaran al mismo tiempo se perdería el punto de comparación y no se leería la relación de montaje. |

### 2. Componentes del conjunto

| ID | Nombre del componente | Función | Cantidad | Referencia o archivo | Observaciones |
|---|---|---|---:|---|---|
| 1 | Base | Sostener el conjunto y recibir al Soporte; sirve de referencia. | 1 | ⚠️ COMPLETAR (archivo/componente en Fusion) | Permanece fija en la explosionada. |
| 2 | Soporte | Apoyarse sobre la Base y alojar al Pasador. | 1 | ⚠️ COMPLETAR | Se separa verticalmente. |
| 3 | Pasador | Unir/guiar la relación entre piezas siguiendo su eje. | 1 | ⚠️ COMPLETAR | Se separa siguiendo su eje. |

### 3. Plan de montaje y separación

**Orden previsto de montaje y desmontaje:**

| Orden | Acción | Componente | Referencia o contacto | Dirección | Función comunicada | Comprobado |
|---:|---|---|---|---|---|:---:|
| 1 | Montar / retirar | Base (se coloca primero) | Superficie de apoyo | — (referencia fija) | Soporte y referencia del conjunto | [ ] |
| 2 | Montar / retirar | Soporte (se monta sobre la Base) | Cara de contacto Soporte–Base | Vertical (eje Z) | Apoyo del Soporte sobre la Base | [ ] |
| 3 | Montar / retirar | Pasador (se inserta al final) | Alojamiento del Soporte | Siguiendo el eje del pasador | Unión/guía del Pasador en el alojamiento | [ ] |
| 4 | Montar / retirar | Pasador (se retira primero al desmontar) | Alojamiento del Soporte | Sentido inverso del eje | Confirma el orden inverso de desmontaje | [ ] |

| Decisión | Respuesta |
|---|---|
| Componente que se colocaría primero | Base |
| Componente que se retiraría al final | Base |
| Criterio utilizado para definir el orden | Secuencia funcional de montaje: se parte de la pieza que sostiene (Base), luego la que se apoya (Soporte) y por último la que une (Pasador); el desmontaje es el orden inverso. Las direcciones se definieron con caras, ejes y superficies de contacto. |

| Orden | Componente | Dirección o referencia de separación | Razón funcional | Distancia aproximada | Comprobado |
|---:|---|---|---|---:|---|
| 1 | Pasador | Siguiendo su eje, hacia afuera del alojamiento | Es lo primero que se retira y hace visible su relación con el alojamiento | ≈ 40 mm ⚠️ ajustar | [ ] |
| 2 | Soporte | Vertical, hacia arriba respecto a la Base | Muestra las superficies de contacto con la Base | ≈ 60 mm ⚠️ ajustar | [ ] |
| 3 | Base | Sin desplazamiento (referencia) | Mantiene la lectura de posición de las demás piezas | 0 mm | [ ] |
| 4 | — | — | — | — | [ ] |

| Pregunta de análisis | Respuesta |
|---|---|
| ¿Qué relación de montaje comunica la secuencia? | Que el Soporte se apoya verticalmente sobre la Base y que el Pasador se inserta, a lo largo de su eje, en el alojamiento del Soporte para unir el conjunto. |
| ¿Qué dificultad o duda debe comprobarse durante la Lección 2? | Que las trayectorias del Pasador y del Soporte no se crucen ni oculten piezas, y que la distancia elegida permita ver el alojamiento sin romper la relación visual entre componentes. |

## Lección 2. Construcción de la vista explosionada

### 4. Construcción en Fusion

**Herramienta utilizada:** `Animation > Transform > Move` ⚠️ (o `Auto Explode`, según lo que haya usado) <br>
**Storyboard:** ⚠️ COMPLETAR (nombre del Storyboard, p. ej. `Storyboard1_Explosionada`) <br>
**Vista u orientación principal:** Isométrica, para ver las tres piezas y sus trayectorias sin ocultamientos. <br>
**Criterio para separar los componentes:** Secuencia funcional de montaje con la Base como referencia fija; distancias proporcionales y suficientes para interpretar el conjunto, siguiendo caras y ejes de contacto.

**Captura de la vista explosionada:**
![Vista explosionada inicial](evidencias/S14_E2_Vista_Explosionada.png)

**Captura de la posición o versión intermedia, si corresponde:**
![Posición o storyboard intermedio](evidencias/S14_E2_Posicion_Intermedia.png)

**Decisiones realizadas en Fusion:**

| Decisión | Acción realizada | Resultado observado | Evidencia |
|---|---|---|---|
| Orientación principal | Cambié al espacio Animation y orienté el conjunto en vista isométrica con el cubo de navegación. | Se ven los tres componentes y sus relaciones. | `S14_E2_Vista_Explosionada.png` |
| Dirección de separación | Con Transform > Move, seleccioné el componente completo y el eje correspondiente: vertical para el Soporte y el eje propio para el Pasador. | Las piezas se separan siguiendo su dirección de montaje. | `S14_E2_Vista_Explosionada.png` |
| Distancia o posición | Escribí la distancia en el cuadro de transformación (≈ 60 mm Soporte, ≈ 40 mm Pasador ⚠️ ajustar) y activé Show Trail Lines. | Separación suficiente y proporcional, sin ocultar piezas. | `S14_E2_Vista_Explosionada.png` |
| Captura de posición / storyboard | Guardé el Storyboard y capturé la pantalla tras revisar desde otra orientación. | Posición final y posición intermedia registradas. | `S14_E2_Posicion_Intermedia.png` |

**¿Se modificó alguna geometría?** Sí [ ] No [x] <br>
**¿Se capturó la posición o el storyboard?** Sí [x] No [ ]

**¿Las líneas de trayectoria se distinguen de contornos, ejes y líneas ocultas?** Sí [ ] No [ ] ⚠️ marcar tras revisar

## Lección 3. Lista de componentes y rotulación

### 5. Lista básica de componentes

| Ítem | Identificador visible | Nombre en la lista | Cantidad | Componente correspondiente | Verificado |
|---:|---|---|---:|---|---|
| 1 | Globo 1 | Base | 1 | Base | [ ] |
| 2 | Globo 2 | Soporte | 1 | Soporte | [ ] |
| 3 | Globo 3 | Pasador | 1 | Pasador | [ ] |

![Lista básica de componentes e identificadores](evidencias/S14_E3_Lista_Componentes.png)

| Comparación | Resultado |
|---|---|
| Diferencia encontrada entre el Browser, la vista y la lista | ⚠️ COMPLETAR (p. ej. nombre genérico tipo `Component1` en el Browser, o cantidad incorrecta; si no hubo diferencias, escribir "Ninguna: 3 componentes en Browser, vista y lista"). |
| Corrección aplicada | ⚠️ COMPLETAR (p. ej. renombré los componentes con Rename a `Base`, `Soporte` y `Pasador`). |
| ¿Cada globo o número de referencia corresponde una sola vez a un componente? | Sí: 3 globos para 3 componentes, sin repetidos ni globos sin componente. ⚠️ Confirmar. |

## Lección 4. Documentación y evaluación

### 6. Documentación del conjunto

| Criterio | Sí | No | Corrección necesaria |
|---|:---:|:---:|---|
| La vista muestra todos los componentes importantes | [ ] | [ ] | |
| La separación sigue una lógica de montaje | [ ] | [ ] | |
| El mismo Drawing contiene Front, Top y Right del ensamble normal | [ ] | [ ] | |
| Las vistas ortogonales están organizadas en primer diedro europeo | [ ] | [ ] | |
| El mismo Drawing contiene también la vista explosionada | [ ] | [ ] | |
| `Top` está debajo de `Front` y `Right` a la izquierda de `Front` | [ ] | [ ] | |
| Las vistas relacionadas están alineadas y suficientemente separadas | [ ] | [ ] | |
| La vista explosionada, lista y globos tienen una zona propia | [ ] | [ ] | |
| Ningún elemento invade el cajetín | [ ] | [ ] | |
| Se comprobó el símbolo o configuración de primer diedro | [ ] | [ ] | |
| Los identificadores se leen con claridad | [ ] | [ ] | |
| La lista coincide con el modelo | [ ] | [ ] | |
| Los contornos, ejes, ocultas y trayectorias se distinguen | [ ] | [ ] | |
| Los globos o identificadores coinciden una sola vez con la lista | [ ] | [ ] | |
| La hoja, escala, orientación e identificación son coherentes | [ ] | [ ] | |
| El modelo, Storyboard y Drawing corresponden a la misma versión | [ ] | [ ] | |
| La orientación facilita la interpretación | [ ] | [ ] | |
| La escala permite leer textos y componentes | [ ] | [ ] | |
| No hay superposiciones innecesarias | [ ] | [ ] | |
| El título y los datos del conjunto están completos | [ ] | [ ] | |
| La versión del modelo, Storyboard, Drawing y evidencias coincide | [ ] | [ ] | |

> ⚠️ Marque **Sí** o **No** en cada fila según lo que vea en su Drawing; si marca **No**, anote la corrección.

**Archivo o captura de la documentación final:** ⚠️ COMPLETAR (nombre del Drawing) <br>
![Documentación final del conjunto](evidencias/S14_E4_Documentacion_Final.png)

| Resultado de la revisión con la rúbrica | Registro |
|---|---|
| Criterio que cumple mejor | ⚠️ COMPLETAR (p. ej. la lista coincide con el modelo y los globos son únicos) |
| Criterio que requiere corrección | ⚠️ COMPLETAR (p. ej. legibilidad de globos o escala) |
| Corrección prioritaria | ⚠️ COMPLETAR (la que más afecte la lectura de la documentación) |

### 7. Problemas y correcciones

| Problema observado | Causa probable | Corrección aplicada | Evidencia |
|---|---|---|---|
| ⚠️ Ej.: Líneas de trayectoria cruzadas entre Soporte y Pasador | Direcciones de separación demasiado cercanas | Ajusté la distancia y la orientación de la vista | `S14_E2_Vista_Explosionada.png` |
| ⚠️ Ej.: Nombres genéricos (`Component1`) en la lista | Componentes sin renombrar en el Browser | Rename a `Base`, `Soporte`, `Pasador` y actualización de la Parts List | `S14_E3_Lista_Componentes.png` |
| ⚠️ Ej.: Globos que cruzaban líneas principales | Colocación automática de Auto Balloon | Reubiqué los globos con líneas de referencia cortas | `S14_E4_Documentacion_Final.png` |

> Reemplace los ejemplos por los problemas reales que tuvo.

### 8. Autoevaluación

| Pregunta | Respuesta |
|---|---|
| ¿Qué componente funcionó como referencia y por qué? | La Base: sostiene y recibe al Soporte, y al mantenerse fija permite leer la posición de las demás piezas. |
| ¿Qué criterio utilizó para definir el orden de separación? | La secuencia funcional de montaje en sentido inverso: primero se retira el Pasador, luego el Soporte, y la Base queda como referencia; las direcciones salen de caras, ejes y superficies de contacto. |
| ¿Qué diferencia existe entre mover una pieza y documentar una vista explosionada? | Mover una pieza solo cambia su posición de representación. Documentar una vista explosionada exige una secuencia con lógica de montaje, trayectorias legibles, lista, globos, escala y cajetín coherentes, de modo que otra persona entienda el conjunto. |
| ¿Cómo comprobó que la lista coincide con el conjunto? | Generé la Parts List desde el diseño (no de memoria) y comparé uno por uno nombre, cantidad, identificador y componente contra el Browser y la vista explosionada. |
| ¿Qué corrección mejoró más la legibilidad de la documentación? | ⚠️ COMPLETAR (p. ej. reubicar globos y ajustar la escala de la vista explosionada). |

## Cierre de las cuatro lecciones

### 9. Evidencias finales

| Evidencia | Nombre o ruta del archivo | Completa | Observaciones |
|---|---|:---:|---|
| Archivo o enlace verificable del conjunto en Fusion | ⚠️ COMPLETAR (enlace/nombre) | [ ] | |
| Vista explosionada | `evidencias/S14_E2_Vista_Explosionada.png` | [ ] | |
| Lista básica de componentes | `evidencias/S14_E3_Lista_Componentes.png` | [ ] | |
| Documentación del conjunto | `evidencias/S14_E4_Documentacion_Final.png` | [ ] | |
| Captura del estado inicial | `evidencias/S14_E1_Conjunto_Inicial.png` | [ ] | |
| Tabla y justificación del componente de referencia | Sección "Lección 1, 1. Estado inicial" de esta ficha | [ ] | |
| Plan de montaje y separación de la Lección 1 | Sección "Lección 1, 3. Plan de montaje y separación" de esta ficha | [ ] | |
| Registro de la dificultad o duda comprobada | Sección "Lección 1, 3" y sección 7 de esta ficha | [ ] | |
| Capturas del proceso o de las correcciones | `evidencias/` ⚠️ COMPLETAR | [ ] | |
| Registro de la posición o storyboard | `evidencias/S14_E2_Posicion_Intermedia.png` | [ ] | |
| Ficha completa y nombrada correctamente | `S14_Registro_Apellido_Nombre.md` | [ ] | |
| Revisión de la rúbrica de la Fase 3 | Sección 6 de esta ficha | [ ] | |

### 10. Cierre

| Cierre | Registro |
|---|---|
| Dificultad principal | ⚠️ COMPLETAR |
| Decisión técnica más importante | Mantener la Base como referencia fija y separar las demás piezas siguiendo la secuencia funcional de montaje, sin modificar la geometría. |
| Pendiente antes de entregar | ⚠️ COMPLETAR (p. ej. revisar la rúbrica de la Fase 3 y confirmar nombres de archivo) |
| Nombre final de la versión entregada | ⚠️ COMPLETAR (p. ej. `S14_Registro_Apellido_Nombre.md` y nombre del Drawing) |
