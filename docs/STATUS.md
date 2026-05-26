# Estado del proyecto

**Última actualización:** 2026-05-25

## En qué estamos

App web local (un solo `index.html`, sin build, sin servidor) para comparar listas de figuritas exportadas desde [figuritas.app](https://www.figuritas.app/).

## Funcionalidad actual

- **Modo Intercambio (2 personas)** — pegas las dos listas completas (con secciones `Me faltan` y `Repetidas`) y obtienes:
  - "A le da a B" = `A.repetidas ∩ B.faltantes`
  - "B le da a A" = `B.repetidas ∩ A.faltantes`
- **Modo Tengo vs Falta** — pegas dos listas planas: una con lo que tienes (típicamente tus repetidas) y otra con lo que falta a la otra persona. Obtienes "las que te interesan" = intersección de ambas.
- Salida en mismo formato pegable (`CODIGO EMOJI: 1, 2, 3`), botón "Copiar" por bloque.
- Botón "Cargar ejemplo" con datos de prueba.
- Dark mode automático según el sistema.

## Cómo usar

```
open index.html
```

Doble click sobre el archivo también funciona. No requiere instalación de nada.

## Próximos pasos posibles

- Persistencia en `localStorage` (recordar última lista).
- Vista visual con tabla y conteos por país (además del texto plano).
- Comparación contra múltiples amigos a la vez.
- Soporte para más alias de secciones (ej. "Faltan", "Sobran").
