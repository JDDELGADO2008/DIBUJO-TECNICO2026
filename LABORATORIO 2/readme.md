# Ficha de registro: Laboratorio Integrador II-B

**Curso:** ICT401 – Dibujo Técnico Asistido por Computadora  
**Semana:** 16  
**Laboratorio:** Integrador II-B  
**Valor del laboratorio:** 10 %  
**Estudiante o equipo:** Picón Méndez, David; Delgado, José Daniel  
**Proyecto:** Soporte ajustable para celular  
**Fecha:** 05 de noviembre de 2026  
**Versión inicial:** `fase 2.f3z` (archivo de referencia disponible; número de versión interna de Fusion no registrado)  
**Versión evaluada:** Diseño y documentación de Fase 4 (número de versión interna de Fusion pendiente de comprobar)

## Propósito y alcance

Esta ficha registra la evidencia del Laboratorio Integrador II-B: integración del modelo, ensamblaje, documentación, exportaciones, tolerancias introductorias y control dimensional básico.

La ficha **no sustituye la entrega de la Fase 4 del Proyecto Integrador**, cuyo valor oficial es 7 % y cuyos requisitos se definen en su propia rúbrica. Algunas evidencias pueden reutilizarse si cumplen ambos propósitos, pero deben conservarse separados el registro del laboratorio y la entrega de la fase.

No se evalúan mediante esta ficha la fabricación física, la metrología avanzada, los procesos completos de manufactura ni la presentación final de la Semana 17.

## Instrucciones

1. Complete la ficha durante las cuatro lecciones.
2. Registre la versión exacta del proyecto utilizada.
3. Conserve una copia de respaldo antes de modificar o exportar.
4. Registre el propósito, formato y comprobación de cada archivo de salida.
5. No invente tolerancias cuando no estén indicadas.
6. Cada medición debe incluir característica, unidad, método y limitación.
7. Use nombres o rutas verificables para las evidencias.

Los textos que comienzan con **Ejemplo:** muestran el nivel de detalle esperado. Sustitúyalos por los datos reales de su proyecto; no los copie como resultados propios.

### Ruta general en Fusion

1. Abra el **Data Panel**, localice el proyecto y abra el diseño vigente.
2. En el **Browser**, confirme componentes, cuerpos y el componente raíz.
3. Revise **Document Settings > Units** y anote las unidades activas.
4. Para el plano, abra el **Drawing** correspondiente y revise sus hojas.
5. Para medir, utilice **Inspect > Measure** y seleccione caras, aristas, puntos o diámetros.
6. Para exportar, utilice **File > Export** cuando el formato esté disponible. Para STL, seleccione el cuerpo o componente y use **Save As Mesh**.
7. Si una orden tiene otro nombre, use el buscador de comandos y registre la orden equivalente.

## Lección 1. Auditoría del proyecto y documentación

| Elemento | Registro |
|---|---|
| Archivo o enlace principal | `fase 2.f3z`, archivo editable de referencia utilizado en el Proyecto Integrador del soporte para celular. |
| Versión revisada | Modelo y documentación de la Fase 4; el identificador exacto de revisión de Fusion está pendiente de comprobar en el Data Panel. |
| Fecha de la versión | Los planos de Fase 4 contienen fechas de 4 y 5 de noviembre de 2026; la fecha de guardado de la revisión del modelo debe confirmarse en Fusion. |
| Unidades del proyecto | Milímetros (mm), según los planos de fabricación. Debe confirmarse el ajuste activo en `Document Settings > Units`. |
| Plano o Drawing utilizado | `Drawing PROY Fase 4.pdf` y plano del ensamblaje de cuatro hojas reproducido en la documentación de Fase 4. |
| Ensamblaje utilizado, si corresponde | Ensamblaje del soporte ajustable para celular, con base inferior, soporte central regulable y marco superior inclinable. |
| Lista básica de componentes, si corresponde | Tres ítems: `Pieza 2 proyecto integrador` (montante central), `Pieza 3 proyecto integrador` (marco superior) y `Componente2` (base inferior), cantidad 1 de cada uno. |
| Ubicación del respaldo inicial | Archivo anterior `fase 2.f3z` incluido entre los archivos del proyecto; falta crear o identificar el respaldo específico de la versión evaluada en Semana 16. |
| Problema prioritario encontrado | La revisión anterior registra una referencia desactualizada en Fusion y una diferencia A2/A3 entre el Drawing y el cajetín; es necesario confirmar la versión del modelo antes de exportar. |

### Revisión de coherencia

| Control | Sí | No | N.A. | Evidencia o corrección |
|---|:---:|:---:|:---:|---|
| El modelo y la documentación corresponden a la misma versión. | [x ] | [ ] | [ ] | Pendiente de confirmar el identificador de versión y actualizar la referencia señalada en Fusion antes de comparar modelo y plano. |
| El plano contiene las vistas, cotas y datos que corresponden. | [x] | [ ] | [ ] | Las cuatro hojas muestran el conjunto y las piezas. La hoja 2 incluye vistas del conjunto y la cota de 100 mm; falta comprobar cada cota directamente contra el modelo vigente. |
| El cajetín o identificación está completo según la plantilla. | [ ] | [x] | [ ] | Se identifican el proyecto y los autores, pero la revisión documental anterior detectó campos incompletos en hojas individuales y una diferencia de formato A2/A3. |
| La lista coincide con el ensamblaje, cuando corresponde. | [x] | [ ] | [ ] | La lista documentada contiene las mismas tres piezas principales del ensamblaje, una unidad de cada una. |
| La orientación y la escala son coherentes. | [x ] | [ ] | [ ] | Las vistas se distinguen, pero está pendiente resolver el formato A2/A3 y confirmar la escala al exportar el PDF. |

**Captura del estado inicial:** `S16_E1_Estado_Inicial.png`
**Corrección prioritaria antes de exportar:** Abrir el diseño vigente, actualizar la referencia desactualizada, guardar una revisión identificable y sincronizar el Drawing. Completar el cajetín, resolver la diferencia entre A2 y A3, verificar escala/unidades y crear una copia de respaldo con el identificador exacto de la versión.

## Lección 2. Exportaciones y comprobación de archivos

En Fusion, seleccione primero el objeto correcto en el **Browser**. No exporte todo el proyecto si solo se solicita una pieza o un componente.

| Formato | Propósito | Configuración relevante | Archivo generado | Comprobado |
|---|---|---|---|:---:|
| STL | Obtener la malla de una pieza del soporte para impresión 3D o revisión geométrica. | Seleccionar solo el cuerpo/componente requerido, usar `Save As Mesh` y unidades mm. | `Soporte_Celular_STL_vFinal.stl` (nombre propuesto; exportación pendiente). | [ ] |
| STEP | Intercambiar geometría CAD 3D del conjunto con otro programa. | `File > Export > STEP`; comprobar que se incluyan los tres componentes y las unidades correctas. | `Soporte_Celular_STEP_vFinal.step` (nombre propuesto; exportación pendiente). | [ ] |
| DXF | Intercambiar geometría bidimensional, cotas y anotaciones técnicas. | Exportación desde el Drawing o boceto; la lectura previa identificó formato DXF AC1027. | `Archivo dxf PROY.dxf` | [x] |
| PDF | Presentar las hojas de planos con vistas, cotas y cajetines. | Exportación del Drawing; cuatro hojas. Revisar tamaño de página, orientación y escala. | `Drawing PROY Fase 4.pdf` y PDF del conjunto reproducido en el informe. | [x] |
| Otro | Mantener una copia editable del diseño para modificaciones y respaldo. | Archivo de Fusion 360, componentes y ensamblaje incluidos; reapertura por comprobar. | `fase 2.f3z` (archivo previo, no respaldo final de Semana 16). | [ ] |

Marque `N.A.` cuando un formato no corresponda al proyecto y justifique la decisión.

### Comprobación de cada salida

| Archivo | Geometría | Unidades | Escala/orientación | Versión | Ubicación | Resultado |
|---|:---:|:---:|:---:|:---:|---|---|
| PDF del conjunto, cuatro hojas | [x] | [x] | [ ] | [ ] | Informe de Fase 4, anexo de planos. | Se reconocen vistas y cotas en mm. Está pendiente confirmar tamaño de página, escala y versión exacta. |
| `Archivo dxf PROY.dxf` | [x] | [ ] | [ ] | [ ] | Archivos de Fase 4. | La inspección anterior registró 410 entidades, incluidas 13 cotas; deben verificarse unidades y coincidencia dimensional al abrirlo. |
| `Drawing PROY Fase 4.pdf` | [ x] | [ ] | [ ] | [ ] | Archivos de Fase 4. | Archivo identificado; falta cotejarlo de forma independiente con el Drawing actualizado. |
| `fase 2.f3z`, STL y STEP | [ ] | [x ] | [ ] | [ ] | Archivo F3Z previo disponible; salidas STL/STEP pendientes. | Reabrir el F3Z y generar/comprobar STL y STEP desde la versión evaluada si se requieren. |

**Archivo o captura de comprobación:** `evidencias/S16_E2_Exportaciones.png` (captura de los archivos y de su comprobación, pendiente). Se dispone de evidencia documental del PDF y de la lectura del DXF en la Fase 4.  
**Discrepancia encontrada:** La revisión de los planos registra una diferencia entre el formato A2 del Drawing y el A3 señalado en el cajetín. No se ha confirmado que DXF y PDF procedan de la misma revisión exacta del modelo; tampoco se han aportado STL y STEP de esta versión.  
**Corrección aplicada:** Se identificaron por nombre los archivos existentes y se separaron de los pendientes. Para completar la corrección técnica se deberá actualizar el Drawing, unificar formato/escala, exportar de nuevo si corresponde y abrir cada salida para verificarla.

## Lección 3. Tolerancias y control dimensional básico

En Fusion, la ruta de comprobación es **Design > Inspect > Measure**. En el resultado de la medición deben poder reconocerse la geometría seleccionada y la unidad.

No agregue una tolerancia que no esté indicada en el plano, la rúbrica o la instrucción correspondiente.

| Característica | Dimensión nominal | Tolerancia | Límite inferior | Límite superior | Valor observado | Unidad |
|---|---:|---:|---:|---:|---:|---|
| Ancho exterior de la base inferior | 100 | No indicada | N.A. | N.A. | 100 (lectura/cálculo documental; falta medir en Fusion) | mm |
| Ancho exterior del conjunto en vista acotada | 100 | No indicada | N.A. | N.A. | 100 (lectura del plano; no es medición independiente) | mm |
| Ancho exterior del marco superior | 70 | No indicada | N.A. | N.A. | 70 (lectura de cota del plano; falta medir en Fusion) | mm |
| Espesor de la base inferior | 9,5 | No indicada | N.A. | N.A. | 9,5 (lectura de cota del plano; falta medir en Fusion) | mm |

### Método y resultado

| Característica | Herramienta o método | Resultado | Limitación de la comprobación |
|---|---|---|---|
| Ancho exterior de la base inferior | Suma documental de tramos `25 + 50 + 25` y cotejo con la hoja de la base; medición directa prevista con `Inspect > Measure`. | Coincidencia documental de 100 mm; conformidad dimensional pendiente. | No se dispone de captura de medición entre caras externas ni de tolerancia indicada. |
| Ancho exterior del conjunto en vista acotada | Comparación de la cota del conjunto con la de la base en las hojas del Drawing. | Coincidencia documental de 100 mm; pendiente de medición 3D. | La comparación de cotas no verifica físicamente un producto ni el estado del CAD actual. |
| Ancho exterior del marco superior | Lectura de la cota de ancho en el plano de la pieza superior; medición 3D prevista. | Cota nominal identificada: 70 mm; pendiente de comprobar. | Sin lectura independiente de `Measure` ni tolerancia que permita declarar conformidad. |
| Espesor de la base inferior | Lectura de la cota de espesor de la base; medición 3D prevista entre caras paralelas. | Cota nominal identificada: 9,5 mm; pendiente de comprobar. | No se cuenta aún con lectura de `Measure`; el plano tampoco establece tolerancia. |

**Ejemplo de cálculo, si corresponde:** Ancho de base por suma de tramos documentados: `25 mm + 50 mm + 25 mm = 100 mm`. Diferencia entre el cálculo documental y la cota indicada: `100 mm − 100 mm = 0 mm`. **Esta diferencia no representa un error de fabricación ni una medición observada independiente.** No es posible calcular límites superior e inferior sin una tolerancia especificada.

**Captura o referencia de la medición:** `evidencias/S16_E3_Control_Dimensional.png` (pendiente: abrir `Inspect > Measure`, seleccionar las caras exteriores de la base y mostrar el resultado en mm). Como referencia documental están las cotas de las hojas de Fase 4.  
**¿Qué valor o criterio no pudo comprobarse?** No se pudo determinar si el ajuste de las bisagras es conforme porque el plano no muestra una tolerancia aplicable. También quedan pendientes los valores medidos directamente en la versión vigente de Fusion y la comprobación de una pieza fabricada, que está fuera del alcance de este laboratorio.

## Lección 4. Integración y cierre del laboratorio

Después de corregir, guarde la versión evaluada desde **File > Save** o la orden equivalente. Compruebe que el archivo exportado y la ficha se refieran a esa misma versión.

### Correcciones finales

| Problema | Acción aplicada | Resultado | Evidencia |
|---|---|---|---|
| Nombres internos poco descriptivos de las piezas. | Se relacionaron los nombres del Browser con las piezas y cantidades de la lista básica. | Se identificaron base, montante y marco superior, cada uno con cantidad 1. | Lista de componentes y planos de Fase 4. |
| Existencia de varios PDF sin correspondencia de versión confirmada. | Se distinguió el PDF de cuatro hojas usado como referencia y el archivo `Drawing PROY Fase 4.pdf`. | Quedó establecido qué plano se empleó para las comparaciones documentales; falta cotejar la revisión exacta. | Anexo de planos de Fase 4 y tabla de la Lección 2. |
| Diferencia A2/A3 y referencia desactualizada en Fusion. | Se documentó la discrepancia y la secuencia para resolverla: actualizar la referencia, completar cajetín y volver a exportar. | Incidencia identificada; corrección dentro de Fusion y nueva exportación pendientes. | Registro de Lección 1 y captura de pantalla de la referencia. |

### Checklist del Laboratorio II-B

- [ ] La versión del modelo y la documentación coincide.
- [x] El plano final fue revisado.
- [x] La lista básica coincide con el ensamblaje, cuando corresponde.
- [x] Cada archivo exportado tiene un propósito registrado.
- [ ] Las salidas fueron revisadas fuera del comando de exportación.
- [ ] Se registraron unidades, escala, orientación y versión.
- [ ] Se realizó al menos una comprobación dimensional básica.
- [x] Las tolerancias introductorias fueron interpretadas sin inventar valores.
- [x] Se registraron discrepancias y correcciones.
- [ ] La versión evaluada fue respaldada.
- [x] La ficha está completa.

### Evidencias finales del laboratorio

| Evidencia | Nombre o ruta | Completa | Observaciones |
|---|---|:---:|---|
| Estado inicial y auditoría | `evidencias/S16_E1_Estado_Inicial.png` | [x ] | Pendiente de guardar con este nombre. Existe una captura de referencia del ensamblaje y Browser en la documentación previa. |
| Exportaciones y comprobación | `evidencias/S16_E2_Exportaciones.png` | [x ] | Pendiente de adjuntar captura que permita identificar salidas y comprobaciones; DXF y PDF figuran en Fase 4. |
| Control dimensional | `evidencias/S16_E3_Control_Dimensional.png` | [x ] | Falta captura de una medición directa con la herramienta `Measure` en mm. |
| Plano final o documentación | `Drawing PROY Fase 4.pdf` y PDF de cuatro hojas del conjunto, anexo de Fase 4. | [x] | La documentación está disponible; queda pendiente cerrar la escala, el formato A2/A3 y la versión. |
| Lista básica, si corresponde | Informe de Fase 4, lista de tres componentes. | [x] | Base inferior, montante central y marco superior, uno de cada tipo. |
| Archivo de respaldo | `fase 2.f3z` (antecedente editable); respaldo de versión evaluada pendiente. | [ ] | Se debe guardar un respaldo identificado de la versión final de Semana 16. |
| Ficha completa | `Ficha_Laboratorio_Integrador_IIB_David_Jose.md` | [x] | Todos los apartados escritos; las verificaciones pendientes están identificadas expresamente. |

## Separación de la Fase 4

**¿Qué producto o archivo adicional exige la rúbrica de la Fase 4?**

La Fase 4 requiere la entrega del proyecto editable y su documentación técnica final: planos del conjunto y de las piezas, vistas pertinentes, lista de componentes y archivos de salida especificados en su rúbrica. La ficha de Semana 16 registra la auditoría, pero no sustituye dichos productos.

**¿Qué evidencia de esta ficha puede reutilizarse en la Fase 4?**

Se pueden reutilizar los planos de cuatro hojas, la lista de tres componentes, la vista del conjunto y el DXF, siempre que se confirme que corresponden a la misma revisión evaluada. Las capturas de auditoría y medición también pueden servir como respaldo técnico cuando estén terminadas.

**¿Qué requisito de la Fase 4 todavía no está cubierto por esta ficha?**

Falta confirmar en Fusion la versión exacta del conjunto y su enlace con el Drawing, completar los campos de identificación del plano, resolver la discrepancia A2/A3 y verificar las exportaciones finales. También debe comprobarse el funcionamiento de las uniones y la ausencia de interferencias según lo exigido para el proyecto.

## Cierre reflexivo

**¿Qué exportación requirió más comprobación y por qué?**

El PDF del Drawing, porque contiene varias hojas y fue necesario distinguir los archivos disponibles, revisar la legibilidad de sus cotas y detectar la diferencia entre el tamaño de hoja indicado en el cajetín y el mostrado en Fusion. La verificación de su escala y versión todavía debe cerrarse.

**¿Qué diferencia encontró entre el valor nominal, la tolerancia y el valor observado?**

El valor nominal es la medida prevista en el plano, por ejemplo 100 mm para el ancho de la base. La tolerancia sería la variación máxima permitida, pero en el plano revisado no aparece una para esa característica. La lectura documental también es de 100 mm; no debe confundirse con un valor observado de manera independiente, que todavía debe obtenerse con `Inspect > Measure`.

**¿Qué corrección mejoró la confiabilidad del producto técnico?**

Relacionar cada pieza con su nombre en el ensamblaje, su cantidad en la lista y sus cotas en el plano permitió detectar con mayor claridad posibles discrepancias. La identificación de la diferencia A2/A3 también evita dar por válida una exportación cuyo formato final aún debe comprobarse.

**¿Qué limitación debe comunicar antes de considerar terminada la Fase 4?**

Aunque se cuenta con el modelo y documentación del soporte, falta comprobar la actualización de referencias y la coincidencia exacta entre el diseño, sus planos y las salidas. También falta registrar mediciones directas, revisar el movimiento de las uniones y verificar posibles interferencias. La comprobación digital no acredita la fabricación física del soporte.
