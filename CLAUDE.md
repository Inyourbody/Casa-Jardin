# Proyecto Casa Jardín — Instrucciones para Claude

Migrado desde el Proyecto "Casa Jardin" de claude.ai el 20/11/2026.

## Quién soy
- Belén Suárez (en documentos formales: Ariadna Belén Suárez).
- Trabajo en Logística, en el área administrativa.
- Curso 3.er año de Técnico Superior en Logística en el Instituto Superior de Formación Técnica N.º 151 (Mar del Plata).
- Te pido sobre todo resúmenes de textos, presentaciones y ayuda con logística y estudio.

## Cómo responder
- Español de Latinoamérica (rioplatense), frases cortas, respuestas al grano.
- Si te pido una decisión, dame **una sola recomendación**, no tres opciones.
- Datos concretos antes que adjetivos. Cero lenguaje de anuncio.
- **Antes de recomendar, diferenciá la información confirmada de las suposiciones.**
- Siempre que sea posible, terminá con: **siguientes pasos**, **métricas a observar** y **datos que todavía faltan validar**.
- Podés hacerme preguntas para conocer mejor el proyecto.

## Descripción del proyecto
Casa Jardín es un local de Mar del Plata (Av. Juan B. Justo 3719) que vende y repara máquinas para cortar el pasto, vende insumos y pasa presupuestos. Tiene un técnico que hace las reparaciones y una persona que atiende el local.

La idea es armarles un ERP, sistema de información, app o página web que les sirva para optimizar y automatizar tareas diarias. La comunicación con los clientes es por WhatsApp o en persona en el local. Hoy completan ficheros en papel por cada cliente: datos, modelo de la máquina, reparación, si pagó parcial o total, presupuesto. Por eso un CRM donde se cargue la base de datos y quede registro de todo es lo indicado.

## Instrucciones originales del proyecto
Este proyecto pertenece a Casa Jardin, un local de venta y reparación de insumos y máquinas de cortar pasto; realizan reparaciones en el local. No tiene departamento de marketing ni página web; realizan todo de manera manual con ficheros para la toma de datos de los clientes, anotan presupuesto, si está pago total o parcial, y la comunicación con el cliente es por WhatsApp y físicamente en el local.

Nuestra prioridad es proponer la integración con un ERP, una aplicación o una página web, ver qué es lo mejor para implementar de manera gratuita y ofrecérselo a Casa Jardín como nuestros clientes. Esto es un proyecto mío de fin de año en donde debo dar el final de la cursada de la carrera Técnico Superior en Logística y demostrar lo aprendido en el año con una presentación y exposición oral. La idea es devolverle a alguien local y contribuirle con automatización y optimización.

## Datos confirmados del proyecto
- TP final de **EDI III: Herramientas Cuantitativas Aplicadas**, profesor **Roberto Palacios**, año 2026.
- Exposición oral: **10 minutos como máximo**. La presentación se envía antes del final; debe ser sintética y con aporte propio.
- Florencia (empleada) carga los datos y abre y cierra el local todos los días. Cuando ella no está, el local cierra.
- El técnico no anota nada en papel; solo Florencia anota y carga.
- Los dueños aceptan el cambio.
- PC del local: Windows 10 Home, Intel Core i3-7100U, 8 GB RAM, con internet; queda prendida todo el horario.
- Facturan con ARCA.
- Se eligió **Odoo** (nube, odoo.com). La app Reparaciones ya está en uso en el local; capacitación, prueba y revisión hechas.
- Deseo pendiente: que Odoo avise al cliente por WhatsApp cuando el equipo está listo e informe novedades.

## Odoo — dónde está cada cosa
- Cuenta: odoo.com > Mis bases de datos. Hay **dos bases**:
  - **reparaciones** → https://reparaciones.odoo.com — "Casa Jardin Reparaciones". **Es la que se usa.** Apps: Ventas, Inventario, Facturación, Reparaciones, Código de barras, Tableros, Conversaciones.
  - **casa-jardin** → https://casa-jardin.odoo.com — solo Conversaciones, Calendario y Contactos. No usar para productos.
- Idioma activo: Español (América Latina). Moneda ARS. IVA por defecto 21% (sin incluir en precio).
- Detalle de todo lo configurado: ver `docs/registro_odoo.md`.
- Guías paso a paso que ya se dieron: ver `docs/guias_odoo.md`.

## Mapa de la carpeta
- `README.md` — índice de todo.
- `archivos/` — archivos originales del proyecto (Excel de presupuestos, inventario, PDF del proyecto).
- `docs/TP_FINAL_SUAREZ.md` — texto completo del borrador del TP final.
- `docs/memoria_proyecto.md` — todo lo que Claude tenía guardado en memoria del proyecto.
- `docs/registro_odoo.md` — cambios hechos en Odoo, con fechas y pendientes.
- `docs/guias_odoo.md` — instructivos de uso de Odoo para el local.
- `docs/precios_y_fuentes.md` — precios de venta usados y de dónde salen.
- `odoo/` — plantilla de importación de productos (67 productos) y plantilla vacía original.
- `imagenes/` — logo, fondo y capturas de pantalla.
