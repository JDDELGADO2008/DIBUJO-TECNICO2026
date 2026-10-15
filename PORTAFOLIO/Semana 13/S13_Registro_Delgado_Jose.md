ICT401 · Semana 13 --- Registro de ensamblaje básico
12 al 17 de octubre de 2026.
- Estudiante: \(Escribe tu nombre completo\)
- Grupo: \(Escribe tu grupo\)
- Proyecto de Fusion Cloud con acceso docente: \(Escribe el nombre o
  enlace del proyecto\)
- Nombre del diseño de ensamblaje: ICT401_S13_Ensamblaje_Basico
- Piezas base utilizadas: Base maciza de 100 x 70 x 10 mm; soporte
  vertical de 60 mm de ancho, 70 mm de alto y 40 mm de fondo con
  alojamiento pasante de diámetro 16 mm; eje o pasador de diámetro 16
  x 80 mm.
- Fecha de trabajo de laboratorio: \(Escribe la fecha de trabajo\)
Instrucciones
Utilice esta plantilla en Portafolio/semana13/ y guárdela como
S13_Registro_Apellido_Nombre.md. Sustituya Apellido_Nombre por un
apellido y un nombre sin espacios ni tildes. Complete cada [Respuesta]
durante las cuatro lecciones prácticas y agregue las imágenes
solicitadas junto con la ficha.
La sesión virtual del miércoles se dedica a la revisión oral del
Proyecto Integrador. Este registro corresponde únicamente a las cuatro
lecciones prácticas de laboratorio. La actividad es formativa y no
sustituye las evaluaciones oficiales posteriores.
Trabaje con las piezas base proporcionadas por la persona docente. Si
todavía no se han distribuido, use las imágenes PNG y las dimensiones de
esta ficha para construirlas. No modifique los archivos originales ni
oculte un componente para evitar una interferencia. Si su versión de
Fusion utiliza otro nombre de comando, escriba el nombre real utilizado
y describa su función.
Ayuda oficial de Fusion: Fusion
Help, sección
Assemblies.
Conjunto de trabajo
Dimensiones nominales de referencia: base maciza 100 x 70 x 10 mm;
soporte de 60 mm de ancho, 70 mm de alto y 40 mm de fondo, con
alojamiento pasante diámetro 16 mm; pasador diámetro 16 x 80 mm.

Posicionamiento exacto
El soporte se centra sobre la base, no se coloca en una esquina:
- Margen lateral: 20 mm a cada lado, porque
  (100 - 60) / 2 = 20 mm.
- Margen frontal y posterior: 15 mm a cada lado, porque
  (70 - 40) / 2 = 15 mm.
- Cara inferior del soporte coincidente con la cara superior de la
  base.
- Relación base-soporte: Rígida (Rigid).
- Centro del alojamiento: 40 mm desde la cara inferior del soporte y
  30 mm desde cada lado del soporte.
- Pasador: coaxial con el alojamiento, centrado en el espesor de la
  pared y con relación Revolute (Revoluta).
- Si la pared mide 10 mm, el pasador de 80 mm sobresale
  aproximadamente 35 mm a cada lado.
No registre una distancia desde una esquina para ubicar el pasador. Su
posición queda definida por el centro del alojamiento.
  Componente        Nombre en Fusion  Función dentro    Observación
                                      del conjunto      inicial
  Base              Base              Sirve como        Pieza maciza de
                                      referencia y      100 x 70 x 10 mm;
                                      sostiene el       debe quedar fija.
                                      soporte.          
  Soporte vertical  Soporte vertical  Sostiene y guía   Se centra sobre
                                      el pasador        la base y se une
                                      mediante el       con una relación
                                      alojamiento.      rígida.
  Eje o pasador     Pasador           Representa el eje Cilindro de
                                      móvil del         diámetro 16 x 80
                                      conjunto.         mm; debe quedar
                                                        coaxial con el
                                                    alojamiento.
Comandos bilingües de Fusion
  Acción                  Ruta o comando                                                Resultado esperado
  Crear diseño            Archivo > Nuevo diseño (File > New Design)                  Diseño vacío y proyecto
                                                                                        confirmado en el Panel
                                                                                        de datos.
  Insertar pieza          Insertar en el diseño actual (Insert into Current Design)   Componente visible en
                                                                                        el Navegador.
  Fijar base              Clic derecho en Navegador > Fijar (Ground)                 La base no se desplaza
                                                                                        ni gira.
  Relacionar soporte      Ensamblar > Unión (Assemble > Joint) > Rígida (Rigid)    El soporte queda unido
                                                                                        a la base.
  Relacionar pasador      Ensamblar > Unión (Assemble > Joint) >                     El pasador gira
                          Revoluta (Revolute)                                         alrededor de su eje.
  Probar relación         Clic derecho en la unión > Animar unión (Drive Joint)      Se comprueba el
                                                                                        movimiento permitido.
  Revisar interferencias  Inspeccionar > Interferencia (Inspect > Interference) >    Se identifican cuerpos
                          Calcular (Compute)                                          que ocupan el mismo
                                                                                        volumen.
  Editar relación         Clic derecho en la relación > Editar (Edit)                Se corrige origen,
                                                                                        orientación, tipo o
                                                                                    desplazamiento.
Registre en cada lección qué componente seleccionó, qué comando utilizó
y qué resultado observó. No se considera suficiente escribir solo el
nombre de la herramienta.
L1 --- Reconocimiento de piezas y componente base
Diagnóstico
- ¿Qué pieza funcionará como base y por qué?: La base maciza de 100 x
  70 x 10 mm, porque sostiene el conjunto y sirve como referencia fija
  para posicionar los demás componentes.
- ¿Qué superficies de la base y del soporte podrían entrar en
  contacto?: La cara superior de la base y la cara inferior del
  soporte vertical.
- ¿Qué eje o alojamiento utilizará el pasador?: El alojamiento pasante
  de diámetro 16 mm situado en el soporte vertical.
- ¿Qué movimiento estaba libre antes de aplicar relaciones?: Antes de
  fijar y relacionar los componentes, las piezas insertadas podían
  tener movimientos de traslación y rotación. La base se fija para
  establecer la referencia.
- ¿Qué orientación inicial seleccionó y por qué?: Una orientación en
  la que la base quede horizontal, el soporte vertical sobre ella y el
  eje del alojamiento visible para facilitar el posicionamiento y la
  revisión.
Estado inicial
  Comprobación                        Resultado
  Base insertada como componente      \(Sí/No + explicación según lo
                                      observado en Fusion\)
  Base fija o establecida como        \(Sí/No + comando utilizado\)
  referencia                          
  Soporte insertado                   \(Sí/No\)
  Eje o pasador disponible            \(Sí/No\)
  Nombres identificables en el        \(Sí/No\)
  navegador                           
Evidencia L1
S13_PiezasBase_Apellido_Nombre.png: captura del ensamblaje con la base
y el soporte visibles, el navegador de componentes abierto y los nombres
identificables.

L2 --- Relaciones entre componentes
Decisiones
  Relación       Componentes o  Movimiento que Movimiento que Resultado
                 geometrías     elimina        conserva
                 vinculadas                                   
  1              Base y soporte La unión       Ninguno entre  El soporte
                 vertical; cara rígida elimina esas dos       permanece fijo
                 inferior del   los            piezas.        respecto de la
                 soporte y cara movimientos                   base.
                 superior de la relativos de
                 base           traslación y
                                rotación entre
                                la base y el
                                soporte.                      
  2              Pasador y      La relación    Rotación       El pasador
                 alojamiento    revoluta       alrededor del  puede girar
                 del soporte;   restringe los  eje del        alrededor de
                 ejes           movimientos    pasador.       su eje.
                 cilíndricos    relativos que
                 coaxiales      no
                                corresponden
                                al giro
                                alrededor del
                            eje.                          
- Comando o herramienta utilizada: Ground para fijar la base y
  Assemble > Joint para crear una unión Rigid entre la base y el
  soporte y una unión Revolute entre el soporte y el pasador.
- ¿Por qué esa relación representa la intención del conjunto?: La
  unión rígida evita que el soporte se mueva respecto de la base; la
  unión revoluta permite el giro del pasador alrededor de su propio
  eje.
- ¿La orientación del soporte quedó correcta?: \(Sí/No + explicación
  después de comprobar que el soporte está centrado y su cara inferior
  coincide con la cara superior de la base\).
- ¿Qué movimiento debe conservar el eje?: La rotación alrededor de su
  eje longitudinal.
- ¿Qué movimiento inesperado observó y cómo lo corrigió?: \(Si
  ocurrió, describe el movimiento y cómo editaste la unión. Si no
  ocurrió, escribe: "No observé movimientos inesperados después de
  revisar las uniones".\)
Evidencia L2
S13_Relaciones_Apellido_Nombre.png: captura del navegador de
componentes y de la relación aplicada, con el conjunto orientado para
leer la posición del soporte y del eje.

L3 --- Revisión de interferencias
- Herramienta utilizada:
  Inspeccionar > Interferencia (Inspect > Interference) > Calcular (Compute),
  si está disponible en la versión de Fusion utilizada.
- Componentes comparados: Base, soporte vertical y pasador.
- ¿Se encontró una interferencia?: \(Sí/No; escribe el resultado real
  que muestra Fusion\).
- Ubicación de la condición: \(Indica la zona que Fusion resalta, o
  escribe "No se detectó ninguna interferencia" si ese fue el
  resultado\).
- ¿Se trata de interferencia, contacto previsto o separación
  intencional?: \(Interpreta el resultado observado. El contacto entre
  la base y el soporte es previsto; una interferencia debe verificarse
  con el análisis real\).
- Causa probable: \(Describe la causa según la zona identificada; por
  ejemplo, posición incorrecta, dimensiones incompatibles o contacto
  previsto\).
- ¿Qué efecto tendría sobre el funcionamiento del conjunto?: Una
  interferencia no prevista puede impedir el ensamblaje o el
  movimiento correcto. El contacto previsto entre las caras de la base
  y el soporte forma parte del posicionamiento del conjunto.
  Componente A   Componente B   Zona revisada  Resultado        Evidencia
  Base           Soporte        Cara superior  Contacto         \(Captura o
                 vertical       de la base y   previsto si las  descripción
                                cara inferior  caras coinciden  del
                                del soporte    correctamente.   resultado\)
  Soporte        Pasador        Alojamiento    \(Escribe el     \[Captura o
  vertical                      pasante de     resultado real   descripción
                                diámetro 16 mm de Fusion\)      del
                                                            resultado]
Evidencia L3
S13_Interferencia_Apellido_Nombre.png: captura del análisis o de la
zona problemática, con los componentes involucrados identificables.

L4 --- Corrección, verificación y cierre
Registro de corrección
- Problema seleccionado: \(Escribe el problema real detectado en L3.
  Si no se detectó ninguno, indica que se verificó el conjunto y no se
  requirió corrección\).
- Corrección prevista antes de modificar: \(Describe la corrección
  planeada; si no fue necesaria, escribe "No fue necesaria una
  corrección"\).
- Componente o relación modificada: \(Nombre del componente o unión
  editada; si no se modificó nada, escribe "Ninguno"\).
- Cambio aplicado: \(Describe el cambio realizado o indica que no hubo
  cambios\).
- Resultado del segundo análisis: \(Escribe el resultado real después
  de corregir o volver a comprobar\).
- ¿La base continúa estable?: \(Sí/No; comprobar en Fusion\).
- ¿El soporte conserva su orientación?: \(Sí/No; comprobar que está
  centrado y apoyado correctamente\).
- ¿El eje conserva el movimiento esperado?: \(Sí/No; comprobar que
  gira alrededor de su eje\).
- Versión o nombre final en Fusion Cloud: \(Escribe el nombre real del
  diseño guardado\).
  Comprobación final      Resultado               Evidencia o explicación
  Componentes visibles y  \(Conforme/No           \[Verificar los tres
  nombrados               conforme\)              componentes en el
                                                  Navegador]
  Relaciones              \(Conforme/No           \[Confirmar las uniones
  comprensibles           conforme\)              rígida y revoluta]
  Movimiento esperado     \(Conforme/No           \[Probar el giro del
                          conforme\)              pasador con Drive
                                                  Joint, si está
                                                  disponible]
  Interferencia revisada  \(Conforme/No           \[Registrar el
                          conforme\)              resultado real de
                                                  Inspect >
                                                  Interference]
  Corrección documentada  \(Conforme/No           \[Anotar el problema,
                          conforme\)              el cambio y el
                                                  resultado; si no hubo
                                              corrección, indicarlo]
Evidencia L4
S13_Correccion_Apellido_Nombre.png: captura comparativa o lámina con
el estado problemático y el estado corregido, ambos etiquetados. Si no
hubo un problema que corregir, muestra el estado final y explica en la
ficha que no fue necesaria una corrección.

Checklist de cierre
- [ ] Las tres piezas base corresponden al conjunto indicado.
- [ ] La base está fija o definida como referencia.
- [ ] Los componentes tienen nombres identificables.
- [ ] Cada relación aplicada tiene una intención explicable.
- [ ] El movimiento permitido corresponde a la función del conjunto.
- [ ] Se ejecutó una revisión de interferencias.
- [ ] La interferencia o ausencia de interferencia quedó interpretada.
- [ ] La corrección quedó registrada antes y después, o se indicó que
  no fue necesaria.
- [ ] El ensamblaje fue guardado en Fusion Cloud.
- [ ] La ficha y las imágenes utilizan la nomenclatura solicitada.
- [ ] No se adelantaron vistas explosionadas ni listas de componentes.
Reflexión final
1. ¿Qué diferencia encontró entre insertar piezas y construir un
   ensamblaje con relaciones?: Insertar piezas las incorpora al diseño;
   construir el ensamblaje con relaciones define cómo se posicionan,
   qué movimientos se restringen y qué movimientos se permiten entre
   los componentes.
2. ¿Qué relación fue más difícil de definir y por qué?: \(Describe la
   relación que te resultó más difícil y explica por qué. Por ejemplo,
   la unión revoluta puede requerir seleccionar correctamente el eje
   cilíndrico del pasador y el del alojamiento\).
3. ¿Cómo distinguió una interferencia de un contacto previsto?: Comparé
   la zona señalada por la herramienta de interferencias con la función
   y la geometría del conjunto. El contacto entre la base y el soporte
   es previsto; cualquier otra condición debe verificarse con el
   resultado de Fusion.
4. ¿Qué comprobará en Semana 14 antes de generar una vista explosionada
   o una lista de componentes?: Comprobaré que el ensamblaje esté
   guardado, que los componentes tengan nombres claros, que las
   relaciones estén correctamente definidas y que el movimiento y las
   interferencias se hayan revisado.
