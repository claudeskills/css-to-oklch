# ![css2oklch](./assets/css-to-oklch.png)

# CSS to OKLCH Skill

Skill de Claude para convertir colores CSS al espacio de color OKLCH.

## Características

- 🎨 **Convierte todos los formatos**: hex, rgb, rgba, hsl, hsla
- 📁 **Procesamiento por lotes**: Procesa proyectos enteros de una vez
- 💬 **Preserva originales**: Añade el color original como comentario
- 🔍 **Modo dry run**: Previsualiza cambios antes de aplicarlos
- 📦 **Múltiples tipos de archivo**: CSS, SCSS, SASS, Less, PostCSS

## ¿Por qué OKLCH?

OKLCH es un espacio de color perceptualmente uniforme que hace la manipulación de colores más intuitiva:
- Ajustes de luminosidad predecibles
- Saturación consistente entre tonos
- Mejor para design systems y theming

## Instalación

1. Descarga `css-to-oklch.skill`
2. Abre Claude.ai → Settings → Skills
3. Sube el archivo `.skill`

## Ejemplos de Uso

**Convertir un archivo:**
```
Convierte los colores de styles.css a OKLCH
```

**Procesar proyecto entero:**
```
Convierte todos los archivos CSS en /src a OKLCH
```

**Previsualizar cambios:**
```
Muéstrame qué colores cambiarían en /styles (dry run)
```

## Ejemplo de Salida

```css
/* Antes */
:root {
  --primary: #ff0000;
  --background: rgb(255, 255, 255);
}

/* Después */
:root {
  --primary: oklch(62.79% 0.257 29.23) /* #ff0000 */;
  --background: oklch(100% 0 0) /* rgb(255, 255, 255) */;
}
```

## Tipos de Archivo Soportados

- `.css`
- `.scss` / `.sass`
- `.less`
- `.styl`
- `.pcss` / `.postcss`

## Requisitos

- Claude Desktop o Claude.ai con Skills habilitadas
- Python con coloraide (`pip install coloraide`)

## Licencia

MIT License - Ver archivo LICENSE para detalles

## Autor

Creado por Daniel Serrano para Griddo
