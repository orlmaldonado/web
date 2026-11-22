# Bitácora de Web Personal

Contexto operativo para continuar sin buscar conversaciones anteriores. Actualizar con cada entrega. Fechas en hora de Colombia (America/Bogota). Entrega actual: **1.1.1 · 22 de noviembre de 2026**.

## Identificación

| Dato | Valor |
| --- | --- |
| Titular | José Orlando Maldonado Bautista |
| Institución | Universidad de Pamplona · Ingeniería de Sistemas |
| Página pública | https://orlmaldonado.github.io/web/ |
| Repositorio | https://github.com/orlmaldonado/web |
| Cuenta y rama | `orlmaldonado` · `main` |
| Alojamiento | GitHub Pages, archivos estáticos en la raíz |
| Recursos | https://orlmaldonado.github.io/web/recursos.html |
| Simulador | https://orlmaldonado.github.io/web/animaciones/perceptron_simple.html |
| Historial | https://github.com/orlmaldonado/web/commits/main/ |
| Despliegues | https://github.com/orlmaldonado/web/actions |

Los enlaces nuevos corresponden a 1.1. El archivo **local** `ESTADO_PUBLICACION.local.json` registra el último commit y despliegue comprobados. Se excluye del repositorio para evitar registrar un identificador de commit dentro de sí mismo. Si falta o está desactualizado, consultar `main` y Actions; no asumir éxito de Pages solo porque exista un commit.

## Historial verificado

Los números de versión son etiquetas documentales, no tags Git. Fechas e identificadores se recuperaron del historial real del repositorio.

| Versión | Fecha en Colombia | Cambio | Commit |
| --- | --- | --- | --- |
| 0.1 | 8 nov. 2026, 19:54 | Publicación inicial | [c0c658d](https://github.com/orlmaldonado/web/commit/c0c658d88d9825c77d6d45f2a402ee2b9c389841) |
| 0.2 | 8 nov. 2026, 19:58 | Fotografía de perfil | [3646fe0](https://github.com/orlmaldonado/web/commit/3646fe0b8961520301290b9d0994c532cd5db750) |
| 1.0 | 10 nov. 2026, 11:20 | Diseño académico azul y páginas separadas de docencia, investigación y blog | [c1e7a0e](https://github.com/orlmaldonado/web/commit/c1e7a0efa7af5d70df08d8c9f6424a22e23b1279) |
| 1.1 | 22 nov. 2026 | Recursos, perceptrón y documentación de continuidad | [606dd01](https://github.com/orlmaldonado/web/commit/606dd01f39d64e68868a99e731fbe9de16d61f5b) |
| 1.1.1 | 22 nov. 2026 | Tabla compacta de Recursos, actualización de caché CSS y coordenadas del cuadrado unitario | Consultar estado local e historial de `main` |

Base anterior a 1.1: `c1e7a0efa7af5d70df08d8c9f6424a22e23b1279`. Árbol Git: `4f5acdaf6f574a0dd2a0e2ca421625994aced6b0`.

Para restaurar una versión, consultar sus archivos y crear un nuevo commit sobre la cabeza vigente. Evitar restablecimientos forzados: Git conserva las versiones publicadas.

## Correcciones de 1.1.1

- El usuario reportó que Recursos mostraba un grafo enorme y la información debajo, y pidió que el recurso apareciera en una tabla compacta. Se sustituyó la tarjeta ilustrada por una tabla semántica con columnas Recurso, Descripción y Acceso. No volver a añadir una ilustración grande al catálogo sin solicitarlo el usuario.
- Se eliminaron la ilustración SVG y sus estilos. La tabla permite desplazamiento horizontal en pantallas pequeñas y conserva colores, encabezado y pie del sitio.
- Los archivos de GitHub coincidían con los locales. Una hoja CSS anterior en caché es una posible explicación del aspecto reportado, no una causa demostrada. Todas las páginas principales ahora enlazan `styles.css?v=1.1.1`; el simulador versiona también su hoja de estilos. Al modificar CSS en próximas entregas, actualizar esta versión en todas las referencias correspondientes.
- Antes de terminar la corrección de Recursos, el usuario pidió rotular los puntos del cuadrado unitario. El plano principal ahora muestra `(0,0)`, `(0,1)`, `(1,0)` y `(1,1)` junto a los puntos, también durante el entrenamiento. Se interpretó `(1,21)` como errata por `(1,1)` y se informó al usuario.
- Las etiquetas se colocan por encima y hacia el interior del cuadrado, con contorno claro para distinguirlas del sombreado y la frontera de decisión. No cambia la distribución del simulador ni la regla de aprendizaje.
- El navegador integrado volvió a permitir visitar la web pública; se inspeccionó la versión previa a la corrección. El resultado de la comprobación posterior a publicar se registra en `ESTADO_PUBLICACION.local.json`.

## Cambios de 1.1 y autorización

- El usuario solicitó agregar **Recursos inmediatamente a la derecha de Investigación**, crear su página y enlazar el simulador, conservando su distribución.
- Después pidió revisar primero la versión local. Se detuvo la publicación y se le facilitaron los archivos. Posteriormente autorizó actualizar GitHub y solicitó esta bitácora.
- Navegación consistente: **Inicio · Docencia · Investigación · Recursos · Blog**.
- `recursos.html` permite ampliar el catálogo mediante tarjetas. Primer recurso: simulador del perceptrón simple para AND, OR y XOR.
- El simulador conserva grafo y plano a la izquierda y cálculo y tabla a la derecha. Se adaptaron colores, tipografía y enlaces de regreso sin añadir un encabezado grande.
- La tabla mantiene desplazamiento interno y el área principal usa la altura de la pantalla.
- Se corrigió el mensaje al agotar épocas: solo XOR se presenta como no separable; para AND y OR se sugiere aumentar el máximo de épocas. Cambiar parámetros reinicia el entrenamiento.
- Los atajos no interceptan entradas, enlaces, botones, menús o combinaciones con modificadores.
- Se actualizaron README y documentación de continuidad. El resultado final de publicación se registra en el estado local al terminar.

## Archivos y fuente activa

| Ruta | Uso |
| --- | --- |
| `index.html` | Portada, perfil, fotografía y acceso a secciones |
| `docencia.html` | Cursos y programas |
| `investigacion.html` | Áreas, CICOM y SIIS |
| `recursos.html` | Catálogo ampliable de enlaces |
| `blog.html` | Espacio para futuras entradas |
| `styles.css` | Diseño general y componentes |
| `assets/jose-orlando-maldonado.jpg` | Retrato aprobado |
| `animaciones/perceptron_simple.html` | Estructura, estilos base y JavaScript del simulador |
| `animaciones/perceptron.css` | Adaptación visual cargada después del estilo base |
| `.nojekyll` | Publicación sin procesamiento Jekyll |
| `README.md`, `BITACORA.md`, `AGENTS.md` | Documentación y continuidad |
| `ESTADO_PUBLICACION.local.json` | Estado de la última publicación, solo local |
| `propuesta-multipagina/` | Copia histórica de 1.0; no editar como fuente activa ni publicar |

Al iniciar 1.1, la raíz local conservaba el diseño antiguo de una sola página. Se comprobó mediante hashes Git que los cinco archivos de `propuesta-multipagina/` coincidían exactamente con la versión publicada 1.0. Se copiaron a la raíz para continuar sobre la base correcta. La carpeta histórica no se modificó.

Durante esta entrega no había `.git` inicializado localmente. La publicación se realiza mediante el conector GitHub; no asumir que `git push` esté configurado. Se creó un respaldo temporal de los archivos originales antes de adaptarlos, pero las versiones duraderas se recuperan del historial Git.

## Formato visual

Diseño académico sobrio, con fondo claro, azul marino y acentos arena, dorado y terracota. Conservar identidad y contenido aprobado.

| Elemento | Valor |
| --- | --- |
| Fondo | `#faf8f3` |
| Azul marino | `#003366` |
| Texto secundario | `#4e5d6b` |
| Bordes | `#dcdedb` |
| Dorado | `#ac8241` |
| Terracota | `#8c4d3b` |
| Superficie | `#ffffff` |
| Azul claro / arena / arcilla | `#eaf0f5` / `#f3eadb` / `#f2e6df` |
| Texto y navegación | DM Sans; alternativas sans-serif |
| Títulos editoriales | Libre Baskerville; alternativas Georgia/serif |
| Ancho máximo del sitio | 1160 px; margen interno de escritorio: 32 px |
| Adaptación | Ajustes a 800 y 650 px; tabla de Recursos con desplazamiento horizontal en pantallas pequeñas |

- HTML5, idioma español y UTF-8. Preservar tildes y símbolos matemáticos.
- Enlaces relativos porque el sitio vive bajo `/web/`; desde el simulador usar `../recursos.html` y `../index.html`.
- Mantener `aria-current="page"` en el enlace activo del menú.
- Recursos comparte encabezado y pie del sitio. Añadir nuevas filas a su tabla compacta; no se han solicitado ilustraciones, filtros ni buscador.
- Fuentes de Google Fonts con alternativas locales. No hay compilación, backend, formularios, cuentas ni base de datos.
- No añadir títulos académicos, publicaciones o datos biográficos que no haya respaldado el usuario.

## Simulador: restricciones y lógica

- **No importar `../styles.css`**: sus reglas globales podrían alterar el espacio del simulador. Usar `perceptron.css`.
- Mantener cuadrícula `minmax(300px,31%) minmax(0,1fr)`: grafo y plano a la izquierda, cálculo y tabla a la derecha.
- Evitar cabeceras altas; el usuario prioriza ver simultáneamente el grafo, el cuadrado y la tabla en escritorio.
- Área principal: `100dvh` menos el borde superior. La ampliación con capa oculta permanece debajo.
- La maquetación original apila columnas con ancho máximo 900 px o altura máxima 560 px. En móvil se priorizan legibilidad y desplazamiento vertical.
- Entradas: `(0,0)`, `(0,1)`, `(1,0)`, `(1,1)`. Activación: `y=1` cuando `z>=0`.
- Regla: `w_i = w_i + eta*(t-y)*x_i`; `b = b + eta*(t-y)`.
- Valores iniciales: `w1=0.2`, `w2=-0.4`, `b=0.1`, `eta=0.2`, máximo 20 épocas.
- AND y OR son separables linealmente; XOR no. La demostración ampliada usa OR y NAND ocultos y AND de salida con pesos fijos, sin retropropagación.
- La tabla muestra los pesos después de aplicar la actualización, como indica su encabezado.
- Conservar Paso, Época, Reproducir/Pausa, Reiniciar, velocidad, valores iniciales, Presentación y atajos de teclado.

## Comprobaciones y límites de 1.1

- Navegación, posición de Recursos y destinos locales comprobados en las cinco páginas.
- Sintaxis del JavaScript comprobada.
- Código real ejecutado en Node con DOM mínimo simulado: AND y OR convergen y clasifican las cuatro entradas; XOR completa 80 iteraciones sin converger; la red oculta resuelve las cuatro entradas XOR.
- Se verificaron Paso, Época, reproducción/pausa y reinicio; también el mensaje al agotar una sola época con AND.
- **Inspección visual pendiente:** la vista integrada no logró conectarse al servidor local y la apertura automática se detuvo porque no pudo identificar la URL del navegador con certeza. No se completó una inspección visual del diseño adaptado en distintas resoluciones. Se entregaron los archivos al usuario y después autorizó publicar.
- Comprobar despliegue de Pages en Actions y registrarlo en el estado local. Ese resultado no equivale a una inspección visual ni a una solicitud HTTP directa a la página pública.

## Procedimiento de actualización

1. Leer bitácora, README, AGENTS y el estado local de publicación.
2. Leer la cabeza actual de `main` y los archivos afectados; podrían haber cambiado desde la última sesión.
3. Editar la raíz activa. Para nuevos recursos, incorporar archivos y una fila en la tabla de `recursos.html`. Si cambia CSS, actualizar su versión en los enlaces de todas las páginas afectadas.
4. Revisar enlaces relativos, UTF-8, controles y distribución afectados; comprobar escritorio y móvil cuando sea posible.
5. Si el usuario pide revisión local, esperar su aprobación. Publicar únicamente el alcance solicitado o aprobado.
6. Crear un commit coherente sobre la cabeza vigente, conservando el árbol remoto y los archivos ajenos al cambio. No publicar copias históricas ni estado local.
7. Avanzar `main` comprobando la cabeza esperada, sin forzar. Si cambió, volver a leer y conciliar.
8. Verificar el despliegue del nuevo commit en Actions. Guardar commit, resultado, identificador, URL y fecha en `ESTADO_PUBLICACION.local.json`.
9. Actualizar esta bitácora con cambios y límites materiales de la entrega. No guardar tokens ni datos privados.

Para revisar localmente basta abrir `recursos.html`. Un intento de servidor en `127.0.0.1:4173` no fue accesible desde la vista integrada; no asumir que siga activo o funcione en otra sesión.

## Pendientes de contenido

Se incorporarán recursos progresivamente. Quedan por desarrollar materiales de clase, enlaces verificados a producción académica y primeras entradas del blog. No se ha acordado un recurso adicional concreto ni otro rediseño del simulador.
