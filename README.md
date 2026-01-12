# SQL — Análisis de ventas del menú (Sabores del Mundo)

Proyecto de portafolio en **MySQL** para analizar transacciones de un restaurante y detectar los productos más exitosos, patrones de demanda y oportunidades para optimizar el menú.

**Repo:** https://github.com/mariafernandaglezmora-01/SQL_Restaurante_SaboresDelMundo

---

## Objetivo
Identificar cuáles productos del menú han tenido mayor demanda y cuáles han sido menos preferidos, a partir de:
- `menu_items` (catálogo)
- `order_details` (transacciones)

---

## Archivos del repositorio
- **Scripts SQL:** `queries/`
- **Reporte (resultados y conclusiones):** `docs/report/`

---

## Cómo ejecutar (rápido)
1. Abrir MySQL (Workbench).
2. Ejecutar:
   - [00_create_restaurant_db.sql](queries/00_create_restaurant_db.sql)
3. Ejecutar consultas y joins (sugerido):
   - [01_join_table.sql](queries/01_join_table.sql)
   - [02_join_menu_items.sql](queries/02_join_menu_items.sql)
   - [03_join_order_details.sql](queries/03_join_order_details.sql)

---

## Metodología (resumen)
1) Exploración del menú:
- total de artículos, precios min/max,
- conteo por categoría,
- promedio de precios.

2) Exploración de pedidos:
- pedidos únicos y órdenes con más artículos,
- primer/último pedido,
- pedidos en rango de fechas.

3) Integración:
- `LEFT JOIN` entre `order_details` y `menu_items` para analizar desempeño por producto y categoría.

4) Síntesis:
- ranking de productos más vendidos,
- comportamiento por categoría (precio promedio / ingresos),
- ventanas horarias con mayor demanda.

---

## Reporte
- Resultados y conclusiones: [Reporte_completo_SQL.docx](docs/report/Reporte_completo_SQL.docx)

---

## Herramientas
MySQL, SQL (JOINs, agregaciones, filtros temporales)

---

## Nota
Repositorio publicado con fines educativos y de portafolio.

