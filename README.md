# Práctica 4: Integración continua

Este proyecto contiene un programa básico de JavaScript que imprime `Hola mundo`.
Además, el workflow de GitHub Actions envía una notificación al tema
`devops-itla` de ntfy cada vez que se sube código a la rama `main`.

## Ejecutar el programa

Se requiere Node.js 18 o posterior.

```bash
npm start
```

La salida esperada es:

```text
Hola mundo
```

## Integración continua

El archivo `.github/workflows/alerta.yml` se ejecuta automáticamente con cada
`push` a `main` y publica en <https://ntfy.sh/devops-itla> el repositorio y el
mensaje del último commit.
