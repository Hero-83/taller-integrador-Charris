# TALLER INTEGRADOR
**Eissan Libardo Charris Meriño**

## Sitio publicado
https://taller-integrador-charris.netlify.app/

---

## Tabla de hallazgos de la auditoría

| Defecto encontrado | Por qué era un problema | Cómo lo corrigió |
|---|---|---|
| Variable llamada `x` | No indica qué almacena; obliga a leer todo el código para entenderlo | Se renombró a `cantidadNotas` |
| Variable llamada `TempValue2` | Nombre no descriptivo y con formato inconsistente | Se renombró a `promedio` |
| Variable llamada `data1` | Arreglo declarado pero nunca usado (código muerto) | Se eliminó |
| Parámetros `a`, `b`, `c` | Nombres de una sola letra sin significado semántico | Se renombraron a `nota1`, `nota2`, `nota3` |
| Función llamada `calc()` | Nombre demasiado abreviado, no describe lo que hace | Se renombró a `calcularPromedio()` |
| `id="r"` e `id="r2"` | Identificadores sin significado, dificultan el mantenimiento | Se renombraron a `resultado-promedio` y `resultado-estado` |
| `class="cont1"` | Nombre sin significado semántico | Se renombró a `contenedor` |
| `<title>pagina</title>` | Título genérico y en minúscula, no describe la página | Se cambió a `Calculadora de Promedio` |
| `Mi Pagina De Notas.HTML` | Espacios en el nombre y extensión en mayúsculas | Se renombró a `index.html` |
| `Estilos Del Sitio.CSS` | Espacios en el nombre y extensión en mayúsculas | Se renombró a `styles.css` |
| Función comentada `calcularAntiguo` | Código muerto que genera ruido y confusión | Se eliminó |
| `console.log` de depuración | Logs que no deben estar en producción | Se eliminaron |
| Indentación inconsistente en `<script>` | El bloque no seguía la indentación del resto del HTML | Se corrigió la indentación |
