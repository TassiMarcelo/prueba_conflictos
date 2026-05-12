# prueba_conflictos

La idea es que cada integrante del equipo de Alentapp entienda cómo resolver conflictos, dado que vamos a trabajar en paralelo y pueden surgir conflictos si las ramas no están actualizadas.

---

## Ejercicio

1. Crear dos ramas desde main
2. Pararse en la primera rama y modificar `conflictos.md`
3. Hacer push y aprobar el PR — se mergea a main
4. Cambiarse a la segunda rama y modificar el **mismo archivo**
5. Hacer push y abrir el PR — como la segunda rama no tiene los cambios del main, va a aparecer el conflicto

---

## Cómo resolverlo

### Opción 1 — Desde GitHub

En el mismo PR aparece un botón para resolver el conflicto. Se puede elegir qué cambios dejar.

> ⚠️ **Importante:** "Mantener ambos cambios" no siempre da el resultado esperado. Revisar que el archivo quede como realmente se quiere antes de confirmar.

### Opción 2 — Desde local (VS Code)

Estando en la rama con conflicto, ejecutar:

\```bash
git pull origin main
\```

VS Code muestra visualmente qué cambió y permite elegir qué dejar. Una vez resuelto:

\```bash
git add .
git commit -m "merge: resolve conflicts with main"
git push
\```

Esto actualiza el PR automáticamente.

> ⚠️ **Importante:** No mezclar las dos opciones — elegir una y completarla.

---

