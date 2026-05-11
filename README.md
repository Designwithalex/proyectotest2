# sillasylamparas — CMS

## Cómo actualizar el contenido de la web

Todo el contenido de la web se administra desde este Google Sheet:
[Abrir Google Sheet](https://docs.google.com/spreadsheets/d/1sHjjT-nMbwAa1tHKczegBedw3VN3M9bEHFtveCS5rxo)

Los cambios se ven en la web **en segundos**, sin tocar código.

---

## Pestaña "Sheet1" — Productos

Cada fila es un producto. Columnas:

| Columna | Qué poner |
|---------|-----------|
| id | Número único (1, 2, 3...) |
| name | Nombre del producto |
| description | Descripción corta (máximo 2 líneas) |
| category | "silla" o "lampara" |
| image_url | URL de Google Drive (ver abajo) |
| whatsapp_message | Ej: "Me interesa la Silla Calma" |
| active | TRUE para mostrar, FALSE para ocultar |

---

## Pestaña "config" — Configuración general

Columnas: `key` y `value`

| key | qué controla |
|-----|-------------|
| hero_imagen | Foto principal del hero |
| hero_titulo | Título grande del hero |
| hero_subtitulo | Texto debajo del título |
| hero_cta_texto | Texto del botón del hero |
| whatsapp_numero | Número de WhatsApp (ej: 5491155556666) |
| productos_titulo | Título de la sección de productos |
| featured_nombre | Nombre del producto destacado |
| featured_imagen | Foto del producto destacado |
| featured_bullet1 | Primer beneficio del destacado |
| featured_bullet2 | Segundo beneficio del destacado |
| featured_bullet3 | Tercer beneficio del destacado |
| footer_tagline | Texto debajo del logo en el footer |
| instagram_url | Link al perfil de Instagram |

---

## Cómo subir imágenes desde Google Drive

1. Subí la imagen a Google Drive
2. Clic derecho → **Compartir** → "Cualquier persona con el enlace"
3. Copiá el link. Va a tener este formato:
   `https://drive.google.com/file/d/XXXXXXXX/view`
4. En el Sheet pegá este formato reemplazando el ID:
   `https://drive.google.com/uc?export=view&id=XXXXXXXX`
   
   El ID es la parte larga entre `/d/` y `/view`.

---

## El Sheet tiene que estar compartido como "Cualquier persona con el enlace puede ver"
De lo contrario la web no puede leer los datos.
