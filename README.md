# IASI Documentation Template

Plantilla oficial para crear repositorios de documentación del ecosistema IASI.

Incluye dos publicaciones independientes:

- `01-user-guide`: guía de usuario en HTML y PDF.
- `02-technical-guide`: guía técnica en HTML y PDF.

Cada manual es también un proyecto RStudio independiente. Ambos incluyen las páginas institucionales de `common` y la identidad visual de `resources`, incluida la franja corporativa `ants.png`. La carpeta `publish/` contiene el sitio que despliega GitHub Pages.

## Crear un repositorio de documentación

1. Crea el repositorio nuevo a partir de esta plantilla.
2. Sustituye `IASI Documentation Template` por el nombre visible del proyecto.
3. Sustituye `iasi-docs-template` por el nombre de su repositorio.
4. Reemplaza las páginas marcadas como pendientes por el contenido real.
5. Activa GitHub Pages con **GitHub Actions** como origen.

## Construcción

Desde el workspace IASI:

```text
iasi-dev build nombre-del-repositorio-docs
iasi-dev publish nombre-del-repositorio-docs
```

Para ejecutar y desplegar el ciclo completo:

```text
iasi-dev deploy --full -m "publica documentación" nombre-del-repositorio-docs
```

## Contrato de la plantilla

- Los fuentes se mantienen fuera de `publish/`.
- HTML y PDF se construyen con perfiles separados.
- `publish/` se versiona y se despliega sin reconstruir en GitHub Actions.
- La plantilla no requiere extensiones ni servicios externos para construirse.
- Cada manual puede evolucionar de forma independiente sin perder la estructura común.

Consulta también [README.en.md](README.en.md).
