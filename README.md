# Planificador de materiales de Gisella Altamirano con Kardex (ET505 · Semana 9)

## Propósito
Ampliación de mi Planificador de Materiales de Semana 7 (exposición artística escolar, presupuesto de S/ 50.00). Se conservan el cálculo, el presupuesto y la validación del pedido, y se añade un pequeño kardex: materiales ficticios con código estable (M001, M002...), búsqueda por nombre o código, cambio de nombre por id, entradas y salidas enteras positivas, existencia física, inactivación o eliminación, guardado en el navegador y exportación de movimientos a CSV.

## Archivos
- index.html: estructura del planificador (S7) y sección del kardex (S9).
- styles.css: apariencia del planificador y reglas de personalización del kardex (paleta violeta rgb(107,33,168), etiqueta de 1.25rem).
- app.js: lógica del planificador (limites, calcularTotal, validarPedido y botones). Sin cambios de comportamiento respecto a S7.
- kardex.js: operaciones del kardex (saldoDe, agregarMovimiento, exportarCSV, siguienteCodigo) y su interfaz.
- README.md: esta documentación.

## Ejecutar y usar
Local: conserve los cinco archivos juntos y abra index.html en Chrome o Edge. Publicado: abra el sitio de GitHub Pages indicado abajo.
1. Escriba un nombre en el kardex y pulse Crear material.
2. Seleccione el material, elija ENTRADA o SALIDA, escriba una cantidad entera positiva y pulse Registrar movimiento.
3. Use el buscador (nombre o código), Cambiar nombre, o Eliminar sin movimientos o inactivar (pide confirmación y se puede cancelar).
4. Exportar CSV descarga movimientos-materiales.csv, que se puede abrir en Excel.

## Publicación
Repositorio: [PEGAR AQUÍ la URL de mi repositorio]
Sitio GitHub Pages: [PEGAR AQUÍ la URL que GitHub muestra]

## Aportes y ayuda recibida
Aporte propio: planificador de S7 (tres TODO, personalización), integración del kardex, personalización, pruebas y publicación. Ayuda: asistente de IA (Claude, Anthropic, 29/10/2026) para integrar los fragmentos, ajustar kardex.js (códigos M001, mensajes visibles) y preparar el borrador del informe. El detalle está en el PDF entregado en MAXEDRA.

## Límites
Los datos del kardex se guardan con localStorage: pertenecen sólo a este navegador y origen; no hay base de datos compartida ni varios usuarios. El CSV es una copia de los movimientos, no una sincronización con Excel. El saldo del pedido (dinero) y la existencia (unidades) son datos distintos. Todos los datos son ficticios.
