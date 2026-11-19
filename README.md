# Mi despensa V13 — Nutrición (versión inicial)

Actualiza los archivos del repositorio GitHub Pages. Haz antes una copia de seguridad desde Ajustes. No desinstales la PWA.

- Sustituye Comparar por Nutrición; permite seleccionar días, ver promedios y detalle por comida.
- Objetivos individuales guardados localmente por identificador de cuenta (todavía NO sincronizados en Supabase).
- Añade recetas precargadas sin cambiar los identificadores de las recetas existentes.
- Valores nutricionales orientativos por ingredientes de una tabla genérica local. Las preparaciones comerciales requieren valores de etiqueta.
- No calcula todavía vitaminas/minerales, grasas mono/poliinsaturadas ni azúcares añadidos: no se inventan.
- Por ahora cada plato planificado se interpreta como una ración para el análisis personal, aunque el menú permita varios comensales. Para hogares con raciones diferentes será necesario un plan por persona.

IMPORTANTE: No usar los datos como asesoramiento dietético ni como medición exacta.

## Corrección V13.1
- Al abrir Nutrición se selecciona el día actual, según el día de la semana local.
- El día seleccionado muestra su total por persona; varios días muestran la media diaria por persona.
- Se respeta el día exacto de cada plato del menú. El número de comensales del menú no multiplica los nutrientes individuales: los ingredientes de la receta se dividen entre las raciones base de la receta.
- El total de toda la receta y la cantidad que se compra para varias personas siguen siendo conceptos distintos.
