# Legibilidad de codigos antiguos

## 1. Elige nombres descriptivos
- **Código:** RetoCccf  
- **Error:** `caja1`, `caja2`, `caja3`, `caja4`, `caja5`  
- **Problema:** No son descriptivos y no indican claramente qué representan.  
- **Solución:** Cambiar a nombres como: `cajaActiva1`, `cajaActiva2`, etc.

## 2. Elige nombres al nivel de abstracción apropiado
- **Código:** WhacAMole  
- **Error:** `golpeHorizontalJugador`, `golpeVerticalJugador`  
- **Problema:** Son demasiado específicos y no están al nivel de abstracción adecuado.  
- **Solución:** Refactorizar por: `filaGolpe` y `columnaGolpe`.

## 3. Usa nomenclatura estándar donde sea posible
- **Código:** RetoCaracol  
- **Error:** `caracolVivo`  
- **Problema:** No sigue la convención de nombres booleanos en Java (prefijo `is`).  
- **Solución:** Cambiar a: `isCaracolVivo`.

## 4. Nombres no ambiguos
- **Código:** RetoCaracol  
- **Error:** `coche`  
- **Problema:** Es ambiguo. No está claro si se refiere a un coche o a un evento relacionado.  
- **Solución:** Cambiar a: `eventoCoche` o `cocheAparcado`.

## 5. Usa nombres largos para ámbitos largos
- **Código:** RetoCccf  
- **Error:** `i` en el bucle `for`  
- **Problema:** Demasiado corto para un ámbito largo (todo el bucle principal).  
- **Solución:** Cambiar a: `minutoActual`.

## 6. Evita codificaciones
- **Código:** RetoCccf  
- **Error:** `cantidadItems1`, `cantidadItems2`, etc.  
- **Problema:** Usa sufijos numéricos (`1`, `2`, etc.) que no aportan claridad.  
- **Solución:** Cambiar a: `itemsEnCaja1`, `itemsEnCaja2`, etc.

## 7. Los nombres deberían describir los efectos laterales
- **Código:** WhacAMole  
- **Error:** `posicionTopoHorizontal`, `posicionTopoVertical`  
- **Problema:** No indican que su valor cambia aleatoriamente en cada iteración.  
- **Solución:** Cambiar a: `posicionTopoFila`, `posicionTopoColumna`.

## 8. Los nombres deben revelar su intención
- **Código:** RetoCaracol  
- **Error:** `caida`  
- **Problema:** No revela claramente que representa la profundidad del pozo.  
- **Solución:** Cambiar a: `profundidadPozo`.

## 9. La elección de buenos nombres lleva tiempo, pero ahorra más de lo que toma
- **Código:** RetoCccf  
- **Error:** `tiempoTotal`  
- **Problema:** No es claro si se refiere al tiempo total del día, de la simulación, etc.  
- **Solución:** Cambiar a: `minutosTotalesSimulacion`.

## 10. Nombres pronunciables que permitan mantener una conversación
- **Código:** RetoCccf  
- **Error:** `RetoCccf`  
- **Problema:** No es pronunciable ni sigue una convención clara.  
- **Solución:** Cambiar a: `SimulacionSupermercado`.

## 11. Mayúsculas en los caracteres inicio de palabra (CamelCase)
- **Código:** RetoCaracol  
- **Error:** `profAgua`  
- **Problema:** No sigue la convención CamelCase.  
- **Solución:** Cambiar a `nivelAguaPozo`.

## 12. Nombres del dominio del problema y de la solución
- **Código:** WhacAMole  
- **Error:** `contadorTurnos`  
- **Problema:** No refleja claramente el dominio del problema (un juego de golpear topos).  
- **Solución:** Cambiar a: `turnosJugados`.

## 13. Elige una palabra para un concepto abstracto y aférrate a él
- **Código:** RetoCaracol  
- **Error:** `caida` y `salida`  
- **Problema:** Usa dos términos diferentes para la profundidad del pozo.  
- **Solución:** Unificar con: `profundidadPozo`.

## 14. Nombres de paquetes deben ser sustantivos y comenzar en minúsculas
- **Código:** No aplica directamente.  
- **Error:** Un paquete mal nombrado podría ser `RetoCaracol`.  
- **Solución:** Usar un sustantivo en minúsculas, como: `simulacion`.

## 15. Nombres de clases deben ser sustantivos y comenzar en mayúsculas
- **Código:** RetoCccf  
- **Error:** `RetoCccf`  
- **Problema:** No es un sustantivo claro ni sigue la convención de nombres de clases.  
- **Solución:** Cambiar a `SimulacionSupermercado`.

## 16. Nombres de métodos deben ser verbos o una frase con verbo y comenzar en minúsculas
- **Código:** No aplica directamente.  
- **Error:** Un mal nombre de método sería `totalItems()`.  
- **Solución:** Usar un verbo, como `calcularTotalItems()`.

## 17. Nombres de métodos de acceso deben anteponer `get` (`is` para booleanos), `set` o `put`
- **Código:** No aplica directamente.  
- **Error:** Si hubiera un método booleano mal nombrado, sería `caracolVivo()`.  
- **Solución:** Cambiar a: `isCaracolVivo()`.

## 18. Si un nombre requiere un comentario, el nombre no revela su intención
- **Código:** RetoCaracol  
- **Error:** `coche`  
- **Problema:** Requiere un comentario para explicar que representa un evento de aparcamiento.  
- **Solución:** Cambiar a: `eventoCoche`.

## 19. Nombres de una letra y, en particular, `O` y `l`, que se confunden con `0` y `1`
- **Código:** RetoCccf  
- **Error:** `i` en el bucle `for`  
- **Problema:** Es un nombre de una sola letra que no es descriptivo.  
- **Solución:** Cambiar a: `minutoActual`.
