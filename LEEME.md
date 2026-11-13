# AERIS: revisión de investigación y materiales

## Carcasa identificada como prototipo final

El usuario proporcionó «Carcasa 2do Prototipo.ipt» e indicó que es el prototipo final. El archivo original se conserva, sin modificaciones, en assets/prototipo-final.ipt. La imagen principal assets/prototipo-final.png se extrajo de la vista previa PNG integrada en ese mismo archivo: no es un dibujo recreado a partir de una fotografía ni el CAD plano de E5.

La vista previa muestra una carcasa angular con marcos y aberturas. La importación de la geometría con InventorLoader/FreeCAD no se completó debido a una incompatibilidad al leer los metadatos internos. El ejecutable de Inventor no está disponible en la instalación registrada del equipo. Por ello no se exportaron STL, STEP ni una malla verificable, y no se atribuyen dimensiones al modelo a partir de la imagen.

La simulación y el video existentes quedan identificados como representaciones anteriores, útiles para recorrer las temperaturas registradas pero no como geometría de esta carcasa final. Para sustituirlos fielmente se necesita una exportación STEP o STL del archivo original, o acceso a un lector compatible con su versión de Inventor. La imagen y el archivo fuente finales ya están incorporados a la página.

## Caracterización térmica añadida

La sección «Laboratorio» integra el informe personal de caracterización de Pyrogel XTE y XTF, actualizado el 11 de noviembre de 2026, con cuatro paneles: DFX (difusividad flash), DSC (calorimetría y capacidad calorífica), TGA (masa relativa) y densidad con cálculos derivados. Se incorporan las figuras originales extraídas del PDF sin modificar sus curvas, tablas numéricas y vínculos al documento completo. Las fotografías de preparación están disponibles dentro del panel DFX.

Se conservan los alcances documentados: tres disparos sobre el mismo espécimen; mínimos DSC sin asignación de mecanismo químico; normalizaciones A/B que no son réplicas ni incertidumbres; masa TGA aproximada leída de gráficas sin programa ni atmósfera disponibles; conductividad k* calculada y condicional. No se presenta la TGA como prueba de una superioridad de XTE ni los cálculos como mediciones directas. El informe es académico y técnico, no un certificado institucional de propiedades.

## Actualización del montaje y del resultado térmico

El equipo confirmó que el montaje final utiliza XTE adherido directamente a la base, sin cámara de aire. La propuesta separada documentada en E5 se conserva solo como antecedente histórico. El esquema de la página y el texto del montaje final representan capas adheridas; ya no hay un selector que presente la bolsa separada como configuración elegida actual.

La selección se describe como exitosa respecto al criterio térmico interior evaluado: 20 muestras entre 0 y 570 s por debajo de 93 °C, máximo de 85,5 °C a los 540 s y margen de 7,5 °C. La meta adicional de 85 °C se superó en 0,5 °C. No se atribuye a esas lecturas el cumplimiento de todos los requisitos de masa, estabilidad, batería, conservación mecánica o vuelo en incendio.

Se revisaron las fichas aportadas de XTE y XTF y las páginas oficiales de Aspen Aerogels. Ambas fichas publican la misma tabla de conductividad nominal (0,028 W/(m·K) a 200 °C de temperatura media) y la misma densidad nominal (0,20 g/cm³). La diferencia estimada en E4 pertenece a la campaña del equipo y no se presenta como una superioridad universal del XTE. Los valores comerciales, la evaluación histórica y el ensayo real quedan distinguidos y con referencias.

Las fichas se incluyen en assets/Pyrogel-XTE-ficha.pdf y assets/Pyrogel-XTF-ficha.pdf. Las referencias primarias de consulta son https://www.aerogel.com/product/pyrogel-xte/ y https://www.aerogel.com/product/pyrogel-xtf/.

Esta es una versión local preparada para sustituir el enfoque previo de electrónica y detección por la historia de selección del material, su adaptación al dron y los resultados térmicos. No se ha publicado sobre la página existente.

El sitio existente es https://aeris-esp32.nicolas15orti.chatgpt.site y su identificador verificado es `appgprj_6a95c6a42fdc8191a171e2cc501e4f68`. La apertura del código mediante Sites está bloqueada en el cliente actual: `sites_git_client_upgrade_required`. La integración y publicación deben continuar con ese mismo sitio cuando esté disponible el acceso al repositorio; no se necesita crear otra página de AERIS.

## Ver esta versión

Abre `index.html` conservando la carpeta `assets` junto a los archivos de estilo y JavaScript. El modelo 3D necesita acceso a la biblioteca Three.js de la CDN indicada en la simulación. El gráfico del ensayo funciona con los datos integrados y permite activar las seis series y recorrer las muestras.

## Fuentes y cambios de alcance

- Entrega 1: problema, especificaciones y necesidad de una protección de baja masa.
- Entrega 2: alternativas iniciales de materiales.
- Entrega 3: disponibilidad, campaña Flash/DSC y ausencia de un ganador concluyente en esa etapa.
- Entrega 4, pp. 1–4: selección de Pyrogel XTE frente a XTF y PTFE, restricciones de aislamiento y masa.
- Entrega 5, pp. 1–4: base de PLA y propuesta histórica de bolsa separada. El prototipo de ajuste documentado en esa entrega usó fomi porque el XTE no había llegado. El montaje actual confirmado posteriormente es adherido, sin espacio de aire.
- Entrega 5, anexo C: cálculos térmicos por capas. Sus predicciones para la configuración C separada no se aplican directamente a la unión adherida actual; por eso el resultado se argumenta con el ensayo real y las propiedades de las fichas.
- Excel original, Hoja1 A1:H21: 20 muestras de 0 a 570 s, cada 30 s. El equipo confirmó °C, segundos y una altura de 4,5 cm.
- Confirmación posterior del equipo: el montaje fotografiado y el Excel sí utilizaron XTE real. Su espesor exacto en ese ensayo no fue confirmado; los 10 mm se atribuyen al diseño de E5.
- Alcance actual indicado por el usuario: electrónica original del dron, sensor de temperatura, acelerómetro y batería añadida. Las cámaras, GPS y microcontroladores adicionales de las etapas anteriores no se presentan como electrónica del montaje final.
- Equipo: solo nombres y afiliación académica, sin identificaciones estudiantiles ni correo personal.

## Modelo y video

La geometría incluye un contorno central con puntas y una vista de la base con ranura central. Es una reconstrucción ilustrativa del CAD y las fotografías; no es un modelo dimensional obtenido de un archivo CAD.

El modelo térmico interior es un ajuste reducido al Excel, distinto del modelo 1D por capas de E5. El color entre sensores usa interpolación espacial. La llama es animada e ilustrativa; el ensayo original usa una resistencia eléctrica. Activar la llama no cambia los valores medidos ni el cálculo térmico.

El video conserva esa distinción. No se afirma validación de vuelo en incendio, certificación de resistencia al fuego, distancia operativa segura ni preservación mecánica a partir de las temperaturas disponibles.

Las imágenes de CAD y laboratorio se conservan con su significado original. La termografía tiene una escala en °F y no se usa para extraer temperaturas a partir de sus colores.

## Base complementaria del prototipo final
Se incluye «Base 2do Prototipo.ipt» sin modificar y su vista previa PNG original. Junto con la carcasa, documenta el diseño final proporcionado por el equipo. La vista previa no implica conversión 3D ni ensamblaje verificado. La animación y el video mantienen la representación anterior.

Aclaración del equipo: el prototipo final es el conjunto formado por la base y la carcasa; ninguna pieza por separado constituye el prototipo completo.
