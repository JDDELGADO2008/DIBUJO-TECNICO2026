# ICT401 · Semana 13 — Registro de ensamblaje básico

12 al 17 de octubre de 2026.

- Estudiante: jose daniel delgado 
- Grupo: 60
- Proyecto de Fusion Cloud con acceso docente: [Nombre del proyecto compartido por el docente]
- Nombre del diseño de ensamblaje: ICT401_S13_Ensamblaje_jose_delgado
- Piezas base utilizadas: Base, soporte vertical y eje o pasador.
- Fecha de trabajo de laboratorio: [Fecha de realización]

## Instrucciones

Se emplearon las piezas base de la práctica para crear un ensamblaje sencillo en Fusion. Se reconocieron los componentes, se definieron relaciones entre ellos y se comprobaron posibles interferencias geométricas.

## Conjunto de trabajo

Las medidas nominales empleadas corresponden a una base de 100 × 70 × 10 mm, un soporte de 60 mm de ancho, 70 mm de alto y 40 mm de profundidad, con un orificio pasante de 16 mm de diámetro, y un pasador de 16 × 80 mm.

### Posicionamiento exacto

El soporte se ubica centrado encima de la base, con márgenes laterales de 20 mm y márgenes frontal y posterior de 15 mm. La superficie inferior del soporte coincide con la superficie superior de la base y ambos componentes se relacionan mediante una unión rígida.

El pasador se ajusta al centro del alojamiento, ubicado a 40 mm de la cara inferior del soporte y a 30 mm de cada lado. Se utiliza una unión revoluta para permitir el giro del pasador.

| Componente | Nombre en Fusion | Función dentro del conjunto | Observación inicial |
|---|---|---|---|
| Base | Base | Sostener y servir de referencia para el conjunto. | Placa maciza de 100 × 70 × 10 mm. |
| Soporte vertical | Soporte vertical | Sostener el pasador y mantener su posición. | Tiene un alojamiento pasante de diámetro 16 mm. |
| Eje o pasador | Pasador | Facilitar el giro alrededor de su propio eje. | Cilindro de diámetro 16 mm y longitud 80 mm. |

## Comandos bilingües de Fusion

| Acción | Ruta o comando | Resultado esperado |
|---|---|---|
| Crear diseño | Archivo > Nuevo diseño (File > New Design) | Se crea el diseño del ensamblaje. |
| Insertar pieza | Insertar en el diseño actual (Insert into Current Design) | Los componentes aparecen en el navegador. |
| Fijar base | Clic derecho > Fijar (Ground) | La base permanece inmóvil. |
| Relacionar soporte | Ensamblar > Unión (Assemble > Joint) > Rígida (Rigid) | El soporte queda unido a la base. |
| Relacionar pasador | Ensamblar > Unión (Assemble > Joint) > Revoluta (Revolute) | El pasador puede girar sobre su eje. |
| Probar relación | Clic derecho en la unión > Animar unión (Drive Joint) | Se comprueba el movimiento de giro. |
| Revisar interferencias | Inspeccionar > Interferencia (Inspect > Interference) > Calcular (Compute) | Se comprueba si existen cuerpos que ocupan el mismo volumen. |
| Editar relación | Clic derecho en la relación > Editar (Edit) | Se corrige la orientación o posición de la relación. |

## L1 — Reconocimiento de piezas y componente base

### Diagnóstico

- ¿Qué pieza funcionará como base y por qué?: La base sólida, ya que funciona como referencia fija y soporta las otras piezas.
- ¿Qué superficies de la base y del soporte podrían entrar en contacto?: La superficie superior de la base y la parte inferior del ala del soporte.
- ¿Qué eje o alojamiento utilizará el pasador?: El orificio pasante de 16 mm de diámetro del soporte vertical.
- ¿Qué movimiento estaba libre antes de aplicar relaciones?: El soporte podía desplazarse en tres direcciones y rotar alrededor de tres ejes.
- ¿Qué orientación inicial seleccionó y por qué?: Se ubicó el soporte vertical encima de la base, apoyando y centrando el ala inferior para mantener la disposición del conjunto de referencia.

### Estado inicial

| Comprobación | Resultado |
|---|---|
| Base insertada como componente | Sí, se insertó como componente de referencia. |
| Base fija o establecida como referencia | Sí, mediante el comando Ground. |
| Soporte insertado | Sí, como componente independiente. |
| Eje o pasador disponible | Sí, como tercera pieza del conjunto. |
| Nombres identificables en el navegador | Sí, Base, Soporte vertical y Pasador. |

### Evidencia L1

S13_PiezasBase_delgado_jose.png: captura del ensamblaje con la base y el soporte visibles, el navegador abierto y los nombres identificables.

## L2 — Relaciones entre componentes

### Decisiones

| Relación | Componentes o geometrías vinculadas | Movimiento que elimina | Movimiento que conserva | Resultado |
|---|---|---|---|---|
| 1 | Cara inferior del soporte y cara superior de la base. | Traslaciones y giros relativos entre ambos componentes. | Ninguno entre la base y el soporte. | El soporte queda fijo y centrado sobre la base. |
| 2 | Eje del pasador y alojamiento del soporte. | Traslaciones que separen el pasador de su eje y giros que cambien la alineación. | Giro del pasador alrededor de su propio eje. | El pasador queda alineado con el alojamiento y puede girar. |

- Comando o herramienta utilizada: Ensamblar > Unión (Joint), con los tipos Rigid y Revolute.
- ¿Por qué esa relación representa la intención del conjunto?: La relación rígida deja el soporte inmóvil sobre la base, mientras que la unión revoluta hace posible que el pasador gire sin salir de su alojamiento.
- ¿La orientación del soporte quedó correcta?: Sí, cuando el soporte está vertical, centrado y apoyado sobre la cara superior de la base.
- ¿Qué movimiento debe conservar el eje?: El giro alrededor de su propio eje.
- ¿Qué movimiento inesperado observó y cómo lo corrigió?: Si el soporte aparece al revés o el pasador no está alineado, se modifica la unión y se ajusta su orientación con Flip o cambiando su origen.

### Evidencia L2

S13_Relaciones_delgado_jose.png: captura del navegador de componentes y las uniones aplicadas, mostrando la posición del soporte y el pasador.

## L3 — Revisión de interferencias

- Herramienta utilizada: Inspeccionar > Interferencia (Inspect > Interference) > Calcular (Compute).
- Componentes comparados: Soporte vertical y pasador; también se revisa la base como parte del conjunto.
- ¿Se encontró una interferencia?: Debe registrarse según el resultado mostrado por Fusion. Si no aparece ninguna, se realiza una prueba controlada en una copia del diseño.
- Ubicación de la condición: En la zona de contacto entre el pasador y el alojamiento del soporte, si el análisis detecta una superposición.
- ¿Se trata de interferencia, contacto previsto o separación intencional?: El contacto entre las superficies de apoyo de la base y el soporte es intencional. Si un componente se introduce de forma no deseada en otro, existe una interferencia.
- Causa probable: Una ubicación equivocada, ejes desalineados o una relación configurada incorrectamente.
- ¿Qué efecto tendría sobre el funcionamiento del conjunto?: Esto podría bloquear el giro del pasador o dejar las piezas en una posición inadecuada.

| Componente A | Componente B | Zona revisada | Resultado | Evidencia |
|---|---|---|---|---|
| Soporte vertical | Pasador | Alojamiento pasante de diámetro 16 mm. | Registrar si Fusion detecta interferencia o no. | Captura del análisis en Fusion. |

### Evidencia L3

S13_Interferencia_delgado_jose.png: captura del análisis de interferencias, con los componentes involucrados identificables y el resultado visible.

## L4 — Corrección, verificación y cierre

### Registro de corrección

- Problema seleccionado: Posible desalineación del pasador respecto al alojamiento.
- Corrección prevista antes de modificar: Revisar el origen, la orientación y el eje de la unión revoluta.
- Componente o relación modificada: Unión revoluta entre el soporte y el pasador, si el diagnóstico confirma que es la causa.
- Cambio aplicado: Ajustar la posición del pasador para que su eje coincida con el centro del alojamiento y corregir la orientación de la unión.
- Resultado del segundo análisis: Registrar si la interferencia desaparece después de corregir la relación. Si no existía interferencia, documentar el resultado real de la segunda comprobación.
- ¿La base continúa estable?: Sí, si permanece fijada mediante Ground.
- ¿El soporte conserva su orientación?: Sí, si permanece centrado y unido rígidamente a la base.
- ¿El eje conserva el movimiento esperado?: Sí, si gira alrededor de su eje sin trasladarse.
- Versión o nombre final en Fusion Cloud: ICT401_S13_Ensamblaje_jose_delgado.

| Comprobación final | Resultado | Evidencia o explicación |
|---|---|---|
| Componentes visibles y nombrados | Conforme, si se verifica en Fusion. | Base, soporte vertical y pasador identificados en el navegador. |
| Relaciones comprensibles | Conforme, si se verifica en Fusion. | Unión rígida para la base y el soporte; unión revoluta para el pasador. |
| Movimiento esperado | Conforme, si se verifica con Drive Joint. | El pasador gira sin trasladarse. |
| Interferencia revisada | Conforme, si se ejecuta Compute. | Se registra el resultado real del análisis. |
| Corrección documentada | Conforme, si se incluyen ambas evidencias. | Se comparan el estado inicial y el estado final. |

### Evidencia L4

S13_Correccion_delgado_jose.png: captura comparativa del estado problemático y el corregido, ambos etiquetados.

## Checklist de cierre

- [x] Las tres piezas base están identificadas según el conjunto indicado.
- [x] La base se establece como referencia fija mediante Ground.
- [x] Se definieron nombres identificables para los componentes.
- [x] Se estableció la intención de cada relación aplicada.
- [x] Se identificó el movimiento permitido para el pasador.
- [ ] Se ejecutó una revisión de interferencias y se registró el resultado real.
- [ ] La interferencia o ausencia de interferencia quedó interpretada.
- [ ] La corrección quedó registrada antes y después.
- [ ] El ensamblaje fue guardado en Fusion Cloud.
- [ ] La ficha y las imágenes utilizan la nomenclatura solicitada.
- [x] No se adelantaron vistas explosionadas ni listas de componentes.

## Reflexión final

1. ¿Qué diferencia encontró entre insertar piezas y construir un ensamblaje con relaciones?

Insertar piezas sirve para agregarlas al diseño, mientras que las relaciones determinan cómo se unen y cuáles movimientos pueden efectuar.

2. ¿Qué relación fue más difícil de definir y por qué?

La unión revoluta, ya que hay que hacer coincidir el eje del pasador con el centro del alojamiento y dejar libre solamente el giro previsto.

3. ¿Cómo distinguió una interferencia de un contacto previsto?

Usé la herramienta Interference de Fusion y revisé las superficies. El contacto previsto ocurre cuando las piezas se apoyan entre sí; una interferencia, en cambio, significa que sus volúmenes se superponen de manera no deseada.

4. ¿Qué comprobará en Semana 14 antes de generar una vista explosionada o una lista de componentes?

Verificaré que las piezas estén identificadas, que las relaciones funcionen bien, que el pasador mantenga su movimiento, que no haya interferencias injustificadas y que el ensamblaje se encuentre guardado.

## Revisión docente

- Observación sobre componentes y nombres: Pendiente de revisión docente.
- Observación sobre relaciones: Pendiente de revisión docente.
- Observación sobre interferencias: Pendiente de revisión docente.
- Corrección sugerida: Pendiente de revisión docente.
- Estado del registro: Pendiente.

