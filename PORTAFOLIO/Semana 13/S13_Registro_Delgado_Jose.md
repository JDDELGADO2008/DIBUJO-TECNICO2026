# ICT401 · Semana 13 — Registro de ensamblaje básico

12 al 17 de octubre de 2026.

- Estudiante: [Tu nombre y apellido]
- Grupo: [Tu grupo]
- Proyecto de Fusion Cloud con acceso docente: [ICT401 — Semana 13]
- Nombre del diseño de ensamblaje: [S13_Ensamblaje_Apellido_Nombre]
- Piezas base utilizadas: [Base, soporte vertical y eje o pasador]
- Fecha de trabajo de laboratorio: [Fecha de trabajo]

## Instrucciones

Utilice esta plantilla en `Portafolio/semana13/` y guárdela como `S13_Registro_Apellido_Nombre.md`. Sustituya `Apellido_Nombre` por un apellido y un nombre sin espacios ni tildes. Complete cada `[Respuesta]` durante las cuatro lecciones prácticas y agregue las imágenes solicitadas junto con la ficha.

La sesión virtual del miércoles se dedica a la revisión oral del Proyecto Integrador. Este registro corresponde únicamente a las cuatro lecciones prácticas de laboratorio. La actividad es formativa y no sustituye las evaluaciones oficiales posteriores.

Trabaje con las piezas base proporcionadas por la persona docente. Si todavía no se han distribuido, use las imágenes PNG y las dimensiones de esta ficha para construirlas. No modifique los archivos originales ni oculte un componente para evitar una interferencia. Si su versión de Fusion utiliza otro nombre de comando, escriba el nombre real utilizado y describa su función.

Ayuda oficial de Fusion: [Fusion Help](https://help.autodesk.com/view/fusion360/ENU/), sección `Assemblies`.

## Conjunto de trabajo

Dimensiones nominales de referencia: base maciza `100 x 70 x 10 mm`; soporte de `60 mm` de ancho, `70 mm` de alto y `40 mm` de fondo, con alojamiento pasante `diámetro 16 mm`; pasador `diámetro 16 x 80 mm`.

![Ensamblaje básico de referencia](ICT401_S13_Ensamblaje_Basico.png)

### Posicionamiento exacto

El soporte se centra sobre la base, no se coloca en una esquina:

- Margen lateral: `20 mm` a cada lado, porque `(100 - 60) / 2 = 20 mm`.
- Margen frontal y posterior: `15 mm` a cada lado, porque `(70 - 40) / 2 = 15 mm`.
- Cara inferior del soporte coincidente con la cara superior de la base.
- Relación base-soporte: `Rígida (Rigid)`.
- Centro del alojamiento: `40 mm` desde la cara inferior del soporte y `30 mm` desde cada lado del soporte.
- Pasador: coaxial con el alojamiento, centrado en el espesor de la pared y con relación `Revolute (Revoluta)`.
- Si la pared mide `10 mm`, el pasador de `80 mm` sobresale aproximadamente `35 mm` a cada lado.

No registre una distancia desde una esquina para ubicar el pasador. Su posición queda definida por el centro del alojamiento.

| Componente | Nombre en Fusion | Función dentro del conjunto | Observación inicial |
|---|---|---|---|
| Base | [BASE_100x70x10] | [Referencia fija del conjunto y soporte de las demás piezas] | [Placa rectangular que debe permanecer estable] |
| Soporte vertical | [SOPORTE_60x70x40] | [Sostiene el pasador y contiene el alojamiento] | [Debe quedar centrado sobre la base] |
| Eje o pasador | [PASADOR_D16x80] | [Permite el movimiento de rotación] | [Debe quedar alineado con el alojamiento] |

## Comandos bilingües de Fusion

| Acción | Ruta o comando | Resultado esperado |
|---|---|---|
| Crear diseño | `Archivo > Nuevo diseño (File > New Design)` | Diseño vacío y proyecto confirmado en el Panel de datos. |
| Insertar pieza | `Insertar en el diseño actual (Insert into Current Design)` | Componente visible en el Navegador. |
| Fijar base | Clic derecho en Navegador > `Fijar (Ground)` | La base no se desplaza ni gira. |
| Relacionar soporte | `Ensamblar > Unión (Assemble > Joint)` > `Rígida (Rigid)` | El soporte queda unido a la base. |
| Relacionar pasador | `Ensamblar > Unión (Assemble > Joint)` > `Revoluta (Revolute)` | El pasador gira alrededor de su eje. |
| Probar relación | Clic derecho en la unión > `Animar unión (Drive Joint)` | Se comprueba el movimiento permitido. |
| Revisar interferencias | `Inspeccionar > Interferencia (Inspect > Interference)` > `Calcular (Compute)` | Se identifican cuerpos que ocupan el mismo volumen. |
| Editar relación | Clic derecho en la relación > `Editar (Edit)` | Se corrige origen, orientación, tipo o desplazamiento. |

Registre en cada lección qué componente seleccionó, qué comando utilizó y qué resultado observó. No se considera suficiente escribir solo el nombre de la herramienta.

## L1 — Reconocimiento de piezas y componente base

### Diagnóstico

- ¿Qué pieza funcionará como base y por qué?: [La base de 100 x 70 x 10 mm, porque sirve como referencia fija y sostiene los demás componentes.]
- ¿Qué superficies de la base y del soporte podrían entrar en contacto?: [La cara superior de la base y la cara inferior del ala del soporte vertical.]
- ¿Qué eje o alojamiento utilizará el pasador?: [El alojamiento pasante de diámetro 16 mm del soporte vertical.]
- ¿Qué movimiento estaba libre antes de aplicar relaciones?: [El soporte podía trasladarse en tres direcciones y girar alrededor de tres ejes, con seis grados de libertad si estaba completamente libre.]
- ¿Qué orientación inicial seleccionó y por qué?: [Coloqué el soporte vertical con el ala inferior orientada hacia la base para hacer coincidir las caras de apoyo.]

### Estado inicial

| Comprobación | Resultado |
|---|---|
| Base insertada como componente | [Sí/No + explicación] |
| Base fija o establecida como referencia | [Sí/No + comando utilizado] |
| Soporte insertado | [Sí/No] |
| Eje o pasador disponible | [Sí/No] |
| Nombres identificables en el navegador | [Sí/No] |

### Evidencia L1

`S13_PiezasBase_Apellido_Nombre.png`: captura del ensamblaje con la base y el soporte visibles, el navegador de componentes abierto y los nombres identificables.

![L1: piezas base](S13_PiezasBase_Apellido_Nombre.png)

## L2 — Relaciones entre componentes

### Decisiones

| Relación | Componentes o geometrías vinculadas | Movimiento que elimina | Movimiento que conserva | Resultado |
|---|---|---|---|---|
| 1 | [Base y soporte vertical] | [Elimina las traslaciones y rotaciones relativas] | [Ningún movimiento relativo] | [El soporte queda fijo respecto de la base] |
| 2 | [Pasador y alojamiento circular del soporte] | [Elimina las traslaciones relativas y los giros distintos del eje de giro] | [Rotación alrededor del eje del alojamiento] | [El pasador gira sin trasladarse] |

- Comando o herramienta utilizada: [Ensamblar > Unión (Assemble > Joint), seleccionando las geometrías correspondientes.]
- ¿Por qué esa relación representa la intención del conjunto?: [La unión rígida mantiene el soporte unido a la base y la unión revoluta permite que el pasador gire alrededor de su eje.]
- ¿La orientación del soporte quedó correcta?: [Sí/No + explicación]
- ¿Qué movimiento debe conservar el eje?: [La rotación alrededor de su eje longitudinal, sin trasladarse.]
- ¿Qué movimiento inesperado observó y cómo lo corrigió?: [Si el soporte queda invertido, editar la unión rígida y corregir la orientación. Si el pasador se desplaza, revisar el origen y la alineación de la unión revoluta.]

### Evidencia L2

`S13_Relaciones_Apellido_Nombre.png`: captura del navegador de componentes y de la relación aplicada, con el conjunto orientado para leer la posición del soporte y del eje.

![L2: relaciones](S13_Relaciones_Apellido_Nombre.png)

## L3 — Revisión de interferencias

- Herramienta utilizada: [Inspeccionar > Interferencia (Inspect > Interference) > Calcular (Compute).]
- Componentes comparados: [Soporte vertical y pasador; después, la base y el conjunto completo.]
- ¿Se encontró una interferencia?: [Sí/No, según el resultado real de Fusion.]
- Ubicación de la condición: [Indicar la zona identificada en el análisis.]
- ¿Se trata de interferencia, contacto previsto o separación intencional?: [Interpretar según el análisis y la función de las piezas.]
- Causa probable: [Posición incorrecta, desalineación o solapamiento no previsto, si corresponde.]
- ¿Qué efecto tendría sobre el funcionamiento del conjunto?: [Una interferencia no deseada podría impedir el montaje o el giro correcto del pasador.]

| Componente A | Componente B | Zona revisada | Resultado | Evidencia |
|---|---|---|---|---|
| [Soporte vertical] | [Pasador] | [Alojamiento de diámetro 16 mm] | [Resultado real de Compute] | [Captura del análisis] |
| [Soporte vertical] | [Base] | [Caras de apoyo] | [Contacto previsto o condición observada] | [Captura de la zona revisada] |

### Evidencia L3

`S13_Interferencia_Apellido_Nombre.png`: captura del análisis o de la zona problemática, con los componentes involucrados identificables.

![L3: interferencia](S13_Interferencia_Apellido_Nombre.png)

## L4 — Corrección, verificación y cierre

### Registro de corrección

- Problema seleccionado: [Describir el problema observado o la condición revisada.]
- Corrección prevista antes de modificar: [Revisar la posición, el origen y la orientación de la relación responsable.]
- Componente o relación modificada: [Indicar el componente o la relación realmente modificada.]
- Cambio aplicado: [Describir el cambio realizado en Fusion.]
- Resultado del segundo análisis: [Indicar el resultado real después de volver a ejecutar Compute.]
- ¿La base continúa estable?: [Sí/No + evidencia]
- ¿El soporte conserva su orientación?: [Sí/No + explicación]
- ¿El eje conserva el movimiento esperado?: [Sí/No + resultado de Drive Joint]
- Versión o nombre final en Fusion Cloud: [Nombre real del diseño guardado.]

### Comprobación final

| Comprobación final | Resultado | Evidencia o explicación |
|---|---|---|
| Componentes visibles y nombrados | [Conforme/No conforme] | [Los tres componentes deben tener nombres identificables.] |
| Relaciones comprensibles | [Conforme/No conforme] | [La unión rígida fija el soporte y la revoluta permite el giro del pasador.] |
| Movimiento esperado | [Conforme/No conforme] | [Resultado observado al ejecutar Drive Joint.] |
| Interferencia revisada | [Conforme/No conforme] | [Resultado real de Compute.] |
| Corrección documentada | [Conforme/No conforme] | [Problema, cambio y resultado posterior.] |

### Evidencia L4

`S13_Correccion_Apellido_Nombre.png`: captura comparativa o lámina con el estado problemático y el estado corregido, ambos etiquetados.

![L4: corrección](S13_Correccion_Apellido_Nombre.png)

## Checklist de cierre

- [ ] Las tres piezas base corresponden al conjunto indicado.
- [ ] La base está fija o definida como referencia.
- [ ] Los componentes tienen nombres identificables.
- [ ] Cada relación aplicada tiene una intención explicable.
- [ ] El movimiento permitido corresponde a la función del conjunto.
- [ ] Se ejecutó una revisión de interferencias.
- [ ] La interferencia o ausencia de interferencia quedó interpretada.
- [ ] La corrección quedó registrada antes y después.
- [ ] El ensamblaje fue guardado en Fusion Cloud.
- [ ] La ficha y las imágenes utilizan la nomenclatura solicitada.
- [ ] No se adelantaron vistas explosionadas ni listas de componentes.

## Reflexión final

1. ¿Qué diferencia encontró entre insertar piezas y construir un ensamblaje con relaciones?: [Insertar piezas permite colocarlas en el diseño, mientras que las relaciones definen cómo se mantienen unidas y qué movimientos pueden realizar.]

2. ¿Qué relación fue más difícil de definir y por qué?: [La unión revoluta, porque requiere alinear el eje del pasador con el centro del alojamiento y permitir únicamente el giro alrededor de ese eje.]

3. ¿Cómo distinguió una interferencia de un contacto previsto?: [Utilicé la herramienta Interferencia de Fusion y revisé la función de las piezas. El apoyo entre la base y el soporte es intencional, mientras que una penetración no prevista puede indicar un problema de posición o alineación.]

4. ¿Qué comprobará en Semana 14 antes de generar una vista explosionada o una lista de componentes?: [Comprobaré que las tres piezas estén identificadas, que la base permanezca fija, que las relaciones estén bien definidas, que el pasador tenga el movimiento esperado y que se haya revisado cualquier interferencia.]

## Revisión docente

- Observación sobre componentes y nombres: [Respuesta de la persona docente]
- Observación sobre relaciones: [Respuesta de la persona docente]
- Observación sobre interferencias: [Respuesta de la persona docente]
- Corrección sugerida: [Respuesta de la persona docente]
- Estado del registro: [Pendiente/Completo]

