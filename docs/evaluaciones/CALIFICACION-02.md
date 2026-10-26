# Retroalimentación — Taller evaluativo 02: Funciones y POO

**Estudiante:** Sebastian Rincon Rodriguez · **Taller:** Taller evaluativo 02 — Funciones y POO
**Fecha límite:** 2026-10-26 23:59 · **Versión revisada:** commit `2d75652`

Muy buen trabajo: el código funciona y los resultados coinciden con los esperados.

## Nota

| Criterio | Puntos |
|---|---|
| Funciones: parámetros, valores por defecto y retorno (Ej. 1 a 3) | 19 / 20 |
| `map`, `filter` y `lambda` (Ej. 4) | 10 / 10 |
| Clases, atributos y métodos (Ej. 5 y 7) | 15 / 15 |
| Encapsulamiento y validación (Ej. 6) | 15 / 15 |
| `__repr__` y `__str__` (Ej. 6 a 8) | 10 / 10 |
| Integración de funciones y clases (Ej. 8) | 10 / 10 |
| Ejecución sin errores | 10 / 10 |
| Documentación | 2 / 5 |
| Entrega correcta | 2 / 5 |
| **Total** | **93 / 100** |
| **Nota (0–5)** | **4.65** |

Este taller aporta **14.0 %** de los 15 % del momento evaluativo.

## 1. Funciones: parámetros, valores por defecto y retorno (19 / 20)
**Lo que hizo bien:**
- `calibrar_lectura` tiene los valores por defecto en la firma, usa `return` y da 11.5 y 12.0 donde corresponde.
- `es_lectura_valida` rechaza -999.0 y 600.0 y acepta 25.0 y 0.0.
- `promedio_valido` reutiliza `es_lectura_valida`, da 27.0 y devuelve `None` si no hay lecturas válidas.

**Lo que puede mejorar:**
- En el Ejercicio 2 la primera prueba usa 25.5 y la guía pedía 25.0.

## 2. `map`, `filter` y `lambda` (10 / 10)
**Lo que hizo bien:**
- Usó `filter`, `map` y `lambda` sin bucles. Obtuvo 5 lecturas calibradas (de 11.5 a 61.9) y 2 excedencias.

## 3. Clases, atributos y métodos (15 / 15)
**Lo que hizo bien:**
- `Lectura` guarda sus tres datos con valores por defecto y convierte mg/m3 a ug/m3 (25.2).
- `Estacion` guarda objetos `Lectura` y `valores()` entrega los ocho valores usando `a_microgramos()`.

## 4. Encapsulamiento y validación (15 / 15)
**Lo que hizo bien:**
- `Sensor` lanza `ValueError` con código vacío o pendiente menor o igual a cero, antes de guardar datos.
- `_pendiente` e `_intercepto` son internos y `calibrar` reutiliza `calibrar_lectura`.
- No dejó celdas de prueba que fallen.

## 5. `__repr__` y `__str__` (10 / 10)
**Lo que hizo bien:**
- Los textos de `Sensor`, `Estacion` e `InformeEstacion` coinciden exactamente con lo pedido.

## 6. Integración de funciones y clases (10 / 10)
**Lo que hizo bien:**
- `InformeEstacion` da 31.9 y "Moderada" reutilizando las funciones y el método `calibrar` del sensor.
- `categoria_pm25` usa una sola cadena `if` / `elif` / `else`.
- También hizo el reto opcional de `excedencias` (da 2).

## 7. Ejecución sin errores (10 / 10)
**Lo que hizo bien:**
- El notebook corre completo sin errores y la celda de verificación imprime el mensaje final.

## 8. Documentación (2 / 5)
**Lo que hizo bien:**
- Cada ejercicio tiene una celda de texto previa y los nombres siguen las convenciones.

**Lo que puede mejorar:**
- Ninguna función, clase ni método tiene docstring (la frase corta entre triples comillas al inicio).
- La celda inicial solo trae el título: faltan su nombre completo y la fecha.

## 9. Entrega correcta (2 / 5)
**Lo que puede mejorar:**
- No siguió la estructura acordada: el nombre del archivo debe ser exactamente `taller-evaluativo-02-funciones-y-poo.ipynb` (con guiones medios) y se entregó como `taller_evaluativo_02_funciones_y_poo.ipynb` (con guiones bajos). Sí está en `ejercicios/`.

## ¿El notebook funciona?
Sí. Corre completo sin errores, la celda de verificación imprime "Verificación completada sin errores." y todos los resultados coinciden con los esperados.

## Para el próximo taller
- Copie el nombre del archivo tal cual lo indica la guía.
- Agregue un docstring de una línea a cada función, clase y método.
- Escriba en la primera celda el título, su nombre completo y la fecha.
- Pruebe cada ejercicio con los valores exactos que pide la guía.
