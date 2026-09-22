# Calculadora de Promedio — Auditoría y Corrección

## Descripción
Página web que calcula el promedio de tres notas e indica si el estudiante aprueba o reprueba.

---

## Auditoría de defectos encontrados

### Nombres de archivos
1. `Mi Pagina De Notas.HTML` — espacios en el nombre y extensión en mayúsculas. Deberia ser `index.html`
2. `Estilos Del Sitio.CSS` — espacios en el nombre y extensión en mayúsculas. Deberia ser `styles.css`

### Variables en JavaScript
3. `data1` — arreglo nunca usado y sin nombre descriptivo (código muerto). Lo ideal sería eliminarlo.
4. `TempValue2` — nombre no descriptivo. Una mejor opción sería `promedio`
5. `x` — nombre sin significado semántico, representa la cantidad de notas. Estaría mejor usar el literal `3` directamente

### Nombre de función
6. `calc()` — nombre demasiado abreviado y sin significado claro. Sería mucho mejor `calcularPromedio()`

### Identificadores HTML
7. `id="r"` — nombre sin significado. Una opción más clara sería `id="resultado-promedio"`
8. `id="r2"` — nombre sin significado. Una opción más clara sería `id="resultado-estado"`
9. `class="cont1"` — nombre sin significado semántico. Estaría mejor como `class="contenedor"`

### Título de la pestaña
10. `<title>pagina</title>` — título genérico y en minúscula. Lo ideal sería algo como `<title>Calculadora de Promedio</title>`

### Código muerto e innecesario
11. `console.log("valores capturados:", a, b, c)` — log de depuración que no debería estar en producción
12. `console.log("promedio calculado")` — log de depuración que no debería estar en producción
13. `console.log("pagina cargada")` — log de depuración que no debería estar en producción
14. Función comentada `// function calcularAntiguo(...)` — código muerto comentado, lo mejor sería eliminarlo

### Indentación y formato
15. El bloque `<script>` no tenía indentación consistente con el resto del HTML
16. Líneas en blanco sobrantes dentro de la función y al inicio y final del `<script>`

---

## Correcciones realizadas

### refactor: Renombrar variables y función
- `data1`, `TempValue2`, `x` → eliminadas/renombradas a `promedio` y `cantidadNotas`
- `a`, `b`, `c` → `nota1`, `nota2`, `nota3`
- `calc()` → `calcularPromedio()`

### style: Formato e indentación
- Corregida indentación del bloque `<script>` para que sea consistente con el HTML
- Eliminadas líneas en blanco sobrantes

### chore: Renombrar archivos y eliminar código muerto
- `Mi Pagina De Notas.HTML` → `index.html`
- `Estilos Del Sitio.CSS` → `styles.css`
- Eliminada función comentada `calcularAntiguo`
- Eliminados todos los `console.log` de depuración

### refactor: Renombrar identificadores HTML
- `id="r"` → `id="resultado-promedio"`
- `id="r2"` → `id="resultado-estado"`
- `class="cont1"` → `class="contenedor"`
- `<title>pagina</title>` → `<title>Calculadora de Promedio</title>`
