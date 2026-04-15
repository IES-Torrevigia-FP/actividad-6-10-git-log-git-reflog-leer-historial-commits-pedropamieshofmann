## Diferencia entre git log y git reflog

git log muestra el historial de commits del repositorio.

git reflog muestra todos los movimientos de HEAD, incluyendo cambios de rama, resets y commits recientes, incluso si ya no están en el historial visible.

---

## Situación donde reflog salva la vida

Por ejemplo, si haces un git reset --hard y pierdes commits importantes, puedes usar git reflog para encontrar el estado anterior y recuperarlo.

También si borras una rama por error, puedes recuperar sus commits con reflog.

---

## Por qué tener cuidado con reset --hard

Aunque reflog permite recuperar cambios, no es una garantía permanente.

- Los datos pueden borrarse con el tiempo.
- Puede ser difícil encontrar el estado correcto.
- En repositorios compartidos, puede causar problemas graves.

Por eso, reset --hard debe usarse con cuidado.
