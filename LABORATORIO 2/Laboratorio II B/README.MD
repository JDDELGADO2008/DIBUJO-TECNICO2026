# Ficha de registro del Laboratorio Integrador II-B

| Datos del laboratorio | Registro |
|---|---|
| Curso | ICT401 – Dibujo Técnico Asistido por Computadora, Universidad Nacional |
| Semana | 16 |
| Valor del laboratorio | 10 % |
| Estudiante | José Daniel Delgado |
| Proyecto | Soporte ajustable para celular |
| Fecha | 5 de noviembre de 2026 |
| Versión inicial de referencia | Ensamblaje documentado en la Fase 3. El archivo editable disponible en el paquete del proyecto es `fase 2.f3z`. |
| Versión evaluada | Documentación de Fase 4 del 4 y 5 de noviembre de 2026. Queda pendiente confirmar el número de versión del diseño en Fusion. |

## Propósito y alcance

Revisé la identificación de las tres piezas del soporte, comparé las cotas que aparecen en distintas hojas del plano y registré qué archivos se utilizaron para comunicar el diseño. La revisión se basó en el informe de Fase 4 y en los planos de su anexo A.

## Lección 1. Auditoría del proyecto y documentación

| Elemento | Registro |
|---|---|
| Archivo principal y respaldo inicial | `fase 2.f3z`, incluido como antecedente editable en el paquete de Fase 4. |
| Versión y fecha revisadas | Planos del ensamblaje de Fase 4, fechados el 4 y 5 de noviembre de 2026. |
| Unidades | Milímetros (mm). |
| Plano utilizado | PDF del ensamblaje de cuatro hojas. Las hojas 1 y 2 muestran el conjunto, la hoja 3 corresponde al marco superior y la hoja 4 a la base. `Drawing PROY Fase 4.pdf` figura como exportación adicional. |
| Ensamblaje utilizado | Base inferior, montante central y marco superior abatible. El montante sirve como referencia espacial. Las dos uniones de revolución permiten plegar el soporte y ajustar su inclinación. |
| Problema prioritario | El cajetín del PDF principal indica A3 y la captura del Drawing muestra A2. Queda pendiente confirmar el formato definitivo antes de imprimir. |

### Lista básica de componentes

| Ítem | Nombre en Fusion | Pieza del soporte | Cantidad |
|---|---|---|---:|
| 1 | Pieza 2 proyecto integrador | Montante central | 1 |
| 2 | Pieza 3 proyecto integrador | Marco superior abatible | 1 |
| 3 | Componente2 | Base inferior | 1 |
| | | **Total** | **3** |

### Revisión de coherencia

| Control | Estado | Evidencia o acción pendiente |
|---|---|---|
| Correspondencia entre la versión del modelo y el plano | Sin confirmar | Las tres piezas se reconocen en ambos registros. Falta el identificador de revisión que vincule el modelo con el PDF. |
| Vistas y cotas | Verificadas en el plano | Se identifican las vistas frontal, superior, derecha e isométrica. El ancho de 100 mm aparece tanto en el conjunto como en la base. |
| Cajetín de todas las hojas | Incompleto | El plano identifica el proyecto y los autores. Quedan campos por completar en las hojas individuales. |
| Lista y ensamblaje | Coinciden | La tabla del informe y la lista del Drawing registran una unidad de cada componente. |
| Orientación y escala | Revisión parcial | Las vistas permiten reconocer las piezas. Falta confirmar el formato de impresión y la escala de salida. |

**Evidencia del estado inicial.** Las figuras 1, 6 y 7 del informe de Fase 4 muestran el conjunto ensamblado, el Drawing general y el detalle del cajetín.

**Corrección pendiente.** Abrir en Fusion la hoja que generó el PDF, comparar su formato con el indicado en el cajetín y corregir el dato que corresponda. Después de exportar, reabrir el PDF y comprobar el tamaño de página, la escala de la vista y el número de hoja.

## Lección 2. Exportaciones y comprobación de archivos

| Formato | Propósito y configuración | Archivo o ubicación | Resultado documentado |
|---|---|---|---|
| PDF | Comunicar las vistas y cotas en mm. Conservar las cuatro hojas y la escala definida para cada vista. | PDF del ensamblaje reproducido en el anexo A. | Se identificaron las cuatro hojas, el ancho general de 100 mm y el formato A3 del cajetín. Queda pendiente resolver la diferencia con la captura A2. |
| DXF | Intercambiar el dibujo 2D con su geometría y anotaciones. Al importarlo, comprobar las unidades y una dimensión conocida en el espacio Modelo. | `Archivo dxf PROY.dxf`, incluido en el paquete de Fase 4. | El informe registra su apertura como AC1027, con 410 entidades, entre ellas 13 cotas. Falta verificar la escala y la orientación respecto al modelo. |
| STL | Preparar una malla para impresión 3D. Seleccionar la pieza, exportar en mm y comprobar su tamaño al importarla. | Sin archivo en la entrega revisada. | No aplica a esta revisión documental. |
| STEP | Intercambiar el ensamblaje con otro programa CAD. Exportar el conjunto y comprobar sus tres piezas al reabrirlo. | Sin archivo en la entrega revisada. | No aplica a esta revisión documental. |
| F3Z | Conservar el diseño editable con sus referencias. | `fase 2.f3z`, incluido en el paquete de Fase 4. | El informe identifica el archivo. Quedan pendientes la comprobación de apertura y la comparación con la revisión final. |

**Evidencia.** La sección 8 del informe registra el DXF y el archivo nativo. Las hojas 1 a 4 del anexo A permiten revisar el PDF.

**Discrepancia registrada.** El PDF de cuatro hojas y la exportación adicional figuran por separado. Para resolver la diferencia A2/A3 y generar un PDF definitivo se requiere el Drawing original.

## Lección 3. Tolerancias y control dimensional básico

Tomé como valor nominal la cota escrita en el plano. Para contrastarla, utilicé otra hoja o un cálculo cuando había información disponible. Las hojas revisadas no indican tolerancias numéricas para estas características. Por eso registré `N.A.` en la tolerancia y en sus límites.

| Característica | Nominal (mm) | Tolerancia | Límite inferior | Límite superior | Valor de contraste y método | Resultado |
|---|---:|---|---|---|---|---|
| Ancho exterior de la base | 100 | N.A. | N.A. | N.A. | 100 mm al sumar los tres tramos de la bisagra documentados en Fase 3. | La suma coincide con la cota de la hoja 4. |
| Ancho exterior del conjunto en la vista acotada | 100 | N.A. | N.A. | N.A. | 100 mm según la cota exterior de la base en la hoja 4. | El conjunto y la base tienen el mismo ancho en esa vista. |
| Ancho exterior del marco superior | 70 | N.A. | N.A. | N.A. | 70 mm por lectura de la hoja 3. | Cota identificada. Falta una lectura independiente para contrastarla. |
| Espesor de la base | 9,5 | N.A. | N.A. | N.A. | 9,5 mm por lectura de la hoja 4. | Cota identificada. Falta una lectura independiente para contrastarla. |

**Cálculo del ancho de la base**

- Tramo izquierdo + tramo central + tramo derecho = 25 mm + 50 mm + 25 mm = **100 mm**.
- Diferencia respecto a la cota exterior de la hoja 4 = 100 mm − 100 mm = **0 mm**.

**Alcance de la comprobación.** El cálculo confirma que las dimensiones documentadas son coherentes. Para obtener una lectura directa del modelo, queda pendiente abrir `Inspect > Measure` en Fusion, seleccionar las dos caras laterales exteriores de la base y guardar una captura del resultado en mm. Para evaluar el ajuste de la bisagra también hace falta definir una tolerancia.

**Evidencia.** Sección 6 del informe y hojas 1 a 4 del anexo A.

## Lección 4. Integración y cierre del laboratorio

### Correcciones finales

| Problema | Acción registrada | Resultado |
|---|---|---|
| Los nombres del navegador dificultan reconocer las piezas. | Relacioné cada nombre de Fusion con su función, ítem y cantidad. | Las tres piezas se pueden identificar en la lista de la lección 1 y en la sección 3 del informe. |
| El informe menciona dos PDF. | Identifiqué el plano de cuatro hojas como referencia de las lecturas dimensionales. | Las cotas del marco se localizan en la hoja 3 y las de la base en la hoja 4. |
| El formato de hoja difiere entre el PDF y el Drawing. | Registré dónde aparece cada formato. | El cajetín del PDF indica A3 y la captura muestra A2. La corrección en Fusion queda pendiente. |

### Control de cierre

| Criterio | Estado al 5 de noviembre de 2026 |
|---|---|
| Coincidencia entre la versión del modelo y la documentación | Pendiente de comparar el identificador de revisión en Fusion. |
| Plano revisado e identificado | Se revisaron las cuatro hojas. Quedan campos del cajetín por completar. |
| Lista coherente con el ensamblaje | Sí. Se identificaron tres ítems y una unidad de cada uno. |
| Propósito de cada formato | Registrado en la lección 2. |
| Revisión de las exportaciones | Documentada para el PDF principal y el DXF. |
| Unidades, escala, orientación y versión | Se identificaron las unidades en mm y las vistas del plano. Quedan pendientes la escala de salida y la revisión del modelo. |
| Comprobación dimensional | Se contrastó el ancho de la base mediante la suma de tres tramos. Falta la lectura directa en Fusion. |
| Interpretación de tolerancias | Las hojas revisadas carecen de tolerancias numéricas para las cotas seleccionadas. La conformidad dimensional queda sin evaluar. |
| Discrepancias y correcciones | Registradas en la tabla de correcciones finales. |
| Respaldo de la versión evaluada | Se identificó `fase 2.f3z` como antecedente editable. Falta acreditar una copia de la revisión final. |
| Ficha y evidencias | Registro escrito completo. Quedan pendientes la captura de medición directa y la evidencia del respaldo final. |
| Entrega de Fase 4 | Revisada por separado mediante la matriz de cumplimiento de la sección 9 del informe. |

### Evidencias finales

| Evidencia | Ubicación | Qué permite comprobar |
|---|---|---|
| Estado inicial y auditoría | Informe de Fase 4, figuras 1, 6 y 7 | Ensamblaje, plano general y cajetín. |
| Exportaciones | Sección 8 y anexo A | Registro de apertura del DXF y reproducción del PDF. |
| Control dimensional | Sección 6 y anexo A, hoja 4 | Suma de los tres tramos y cota exterior de la base. |
| Plano revisado | Anexo A, hojas 1 a 4 | Vistas del conjunto, marco superior y base. |
| Lista de componentes | Sección 3 y figura 6 | Identificación y cantidad de los tres componentes. |
| Respaldo | `fase 2.f3z` | Existencia de un antecedente editable. El respaldo final de semana 16 queda pendiente de acreditar. |
| Ficha de registro | `registro.md` | Cuatro lecciones, resultados, evidencias y comprobaciones pendientes. |

## Separación de la Fase 4

**¿Qué producto adicional exige la Fase 4?**  
La entrega del proyecto vale 7 % y comprende el modelo editable, la documentación técnica del conjunto y de sus piezas, la lista de componentes y las salidas solicitadas por la rúbrica. El laboratorio vale 10 % y registra las comprobaciones realizadas.

**¿Qué evidencia se puede reutilizar?**  
El plano de cuatro hojas, la lista de tres componentes, las vistas del conjunto y el DXF, siempre que correspondan a la versión que se va a entregar.

**¿Qué requisito sigue abierto?**  
Falta acreditar que el plano definitivo y las exportaciones provienen de la revisión aprobada. También queda pendiente resolver la diferencia de formato A2/A3 y completar los campos del cajetín.

## Cierre reflexivo

**¿Qué exportación requirió más comprobación y por qué?**  
El PDF. Tuve que identificar cuál de los dos archivos contenía las cuatro hojas y comparar el tamaño indicado en el cajetín con el de la captura del Drawing.

**¿Qué diferencia hay entre nominal, tolerancia y valor observado?**  
El ancho nominal de la base es 100 mm. La tolerancia indicaría cuánto puede variar ese ancho. Al sumar los tres tramos obtuve 100 mm. Para registrar un valor observado directamente en el modelo, necesito medir la distancia entre las caras exteriores de la base en Fusion.

**¿Qué corrección mejoró la confiabilidad del producto técnico?**  
Vincular cada cota con su hoja y cada nombre de Fusion con su pieza. Así puedo localizar el espesor de 9,5 mm en la hoja 4 y distinguirlo de las dimensiones del marco superior, que aparecen en la hoja 3.

**¿Qué limitación debe comunicarse antes de cerrar la Fase 4?**  
Las cotas revisadas permiten describir el diseño. Para confirmar el funcionamiento de la bisagra, queda pendiente comprobar el giro en Fusion, revisar las interferencias y definir el criterio de ajuste si se va a fabricar el soporte.

## Documentos consultados

- Guía de ejercicios de ICT401, semana 16, *Laboratorio Integrador II-B*, lecciones 1 a 4.
- David Picón Méndez y José Daniel Delgado, *Documentación y archivos finales del soporte ajustable para celular*, Fase 4, secciones 3 y 6 a 9, y anexo A.
