# Retroalimentación — Taller evaluativo 03 (NumPy)

**Estudiante:** Sebastian Rincon Rodriguez · **Taller:** Taller evaluativo 03 — NumPy
**Fecha límite:** 2026-10-26 23:59 · **Versión revisada:** commit `374cf29`

Excelente trabajo: todos los ejercicios dan los resultados esperados.

## Nota

| Criterio | Puntos |
|---|---|
| Creación y atributos de arreglos (Ej. 1) | 10 / 10 |
| Indexación y slicing (Ej. 2) | 10 / 10 |
| Máscaras booleanas (Ej. 3) | 15 / 15 |
| Vectorización y broadcasting (Ej. 4) | 15 / 15 |
| Estadística por eje y funciones universales (Ej. 5 y 6) | 20 / 20 |
| Integración (Ej. 7) | 10 / 10 |
| Ejecución sin errores | 10 / 10 |
| Documentación | 4 / 5 |
| Entrega correcta | 2 / 5 |
| **Total** | **96 / 100** |
| **Nota (0–5)** | **4.80** |

Este taller aporta **14.4 %** de los 15 % del momento evaluativo.

## 1. Creación y atributos de arreglos (10 / 10)
**Lo que hizo bien:**
- Creó la tabla con `np.array` a partir de una lista de listas y leyó forma, dimensiones, tamaño y tipo de sus atributos.
- `dias`, `pendientes` e `interceptos` son correctos.

## 2. Indexación y slicing (10 / 10)
**Lo que hizo bien:**
- Cada resultado sale de una sola expresión, con el índice negativo y el bloque de forma (3, 4) bien recortado.

## 3. Máscaras booleanas (15 / 15)
**Lo que hizo bien:**
- `es_util` une las dos comparaciones con `&` y paréntesis; quedan 5 lecturas útiles, 2 faltantes y promedio 27.0.

## 4. Vectorización y broadcasting (15 / 15)
**Lo que hizo bien:**
- Convirtió pendientes e intercepto en columnas (5, 1) y calibró sin bucles.
- Explicó con claridad por qué falla la multiplicación de formas (5, 7) y (5,).
- El promedio calibrado de SBC-A da 31.9.

## 5. Estadística por eje y funciones universales (20 / 20)
**Lo que hizo bien:**
- Los promedios por sensor y por día, el máximo y la media sobre el límite son correctos.
- Usó `np.maximum`, `np.abs` y `np.round`, y `en_alerta` se hizo sobre una copia sin alterar `calibradas` (8 celdas mayores que 0).

## 6. Integración (10 / 10)
**Lo que hizo bien:**
- Los conteos (9, 18, 7 y 1) suman 35, el día pico es 5 y las dos líneas de salida coinciden con lo pedido.

## 7. Ejecución sin errores (10 / 10)
**Lo que hizo bien:**
- El notebook corre completo sin errores y la verificación final imprime el mensaje esperado.

## 8. Documentación (4 / 5)
**Lo que hizo bien:**
- Cada ejercicio tiene su celda de texto previa y los nombres de variables están bien.

**Lo que puede mejorar:**
- La primera celda solo tiene el título: faltan su nombre completo y la fecha.

**Cómo corregirlo:**
- Edite la primera celda de texto y escriba debajo del título su nombre completo y la fecha de entrega.

## 9. Entrega correcta (2 / 5)
**Lo que hizo bien:**
- Subió el notebook a la carpeta `ejercicios/` de la rama `main`, antes del plazo.

**Lo que puede mejorar:**
- No siguió la estructura acordada: el archivo se llama `taller_evaluativo_03_numpy.ipynb` y debe llamarse exactamente `taller-evaluativo-03-numpy.ipynb` (con guiones medios, no bajos).

**Cómo corregirlo:**
- En la carpeta `ejercicios/` de su repositorio, cambie el nombre del archivo a `taller-evaluativo-03-numpy.ipynb`, reemplazando cada guion bajo por un guion medio, y verifique en GitHub que quede en la rama `main`.

## ¿El notebook funciona?
Sí. Corre completo sin errores, la celda de verificación imprime "Verificación completada sin errores." y todos los resultados coinciden con los esperados.

## Para el próximo taller
- Use el nombre de archivo exacto que pide la guía, con guiones medios, y revíselo en GitHub antes de entregar.
- Complete la primera celda con título, nombre completo y fecha.
- Siga con el mismo cuidado de revisar la forma de los resultados.
