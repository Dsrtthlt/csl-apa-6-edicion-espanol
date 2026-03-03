# APA 6th Edition - Estilo CSL en Español

Estilo de citación APA 6ª edición (American Psychological Association) completamente localizado al español para su uso con Zotero, Pandoc, Quarto y otros procesadores CSL.

## Características

- **Totalmente en español**: Sin dependencia de babel o configuraciones adicionales
- **Conjunción "y"**: Reemplaza el ampersand (&) por "y" en referencias con múltiples autores
- **Términos localizados**: 
  - "Consultado" en lugar de "Retrieved"
  - "de" en lugar de "from"
  - "En" en lugar de "In"
  - "s.f." en lugar de "n.d."
  - "vol.", "núm.", "p.", "pp." en español
  - "Ed.", "Eds.", "Comp.", "Trads." según corresponda

## Cambios realizados respecto al original

### 1. Locale en español ampliado
Se agregó/modificó la sección `<locale xml:lang="es">` con los siguientes términos:
- Conjunciones y preposiciones
- Abreviaturas de roles editoriales
- Términos de recuperación y acceso
- Formato de páginas, volúmenes y números

### 2. Reemplazo de ampersand por "y"
- Se cambió `and="symbol"` por `and="text"` en todas las macros de autor
- Se modificó el término "and" en el locale inglés para que use "y"
- Se reemplazaron delimitadores `&amp;` por `, y `

### 3. Compatibilidad
- Funciona con Quarto/RStudio sin necesidad de `lang: es`
- Compatible con la API de Zotero
- Citekeys estándar (Apellido+Año)

## Instalación

### Opción 1: Uso local
1. Descargue el archivo `apa-6th-edition-es.csl`
2. En su documento Quarto/YAML, especifique:
```yaml
csl: apa-6th-edition-es.csl
