
# Examen práctico - Segunda Unidad

**Nombre:** Zamora Contreras Alex Iván

**Matrícula:** 217O01834

**Materia:** Herramientas de Software en la Nube

## Objetivo del proyecto

Desarrollar y desplegar una aplicación web utilizando contenedores Docker, administrar sus servicios mediante Docker Compose y aplicar control de versiones con Git y GitHub.

## Tecnologías utilizadas

- Docker
- Docker Compose
- Git
- GitHub
- HTML5
- CSS3
- Nginx

## Imagen utilizada

La aplicación utiliza una imagen propia construida a partir de Nginx Alpine.

**Nombre de imagen:** `examen:217O01834`

## Servicios y puertos

| Servicio | Puerto local | Puerto del contenedor |
|---|---|---|
| servicio1 | 8081 | 80 |
| servicio2 | 8082 | 80 |
| servicio3 | 8083 | 80 |

## Ejecución del proyecto

Para construir la imagen:

```bash
docker build -t examen:217O01834 .
```

Para iniciar los tres servicios:

```bash
docker compose up -d
```

Para consultar el estado:

```bash
docker compose ps
```

Para detener los servicios:

```bash
docker compose down
```

## Acceso a la aplicación

- http://localhost:8081
- http://localhost:8082
- http://localhost:8083

## Recuperación de servicios

Si el segundo servicio deja de funcionar, puede recuperarse mediante:

```bash
docker compose up -d servicio2
```

## Visualización

El dashboard de datos se integrará posteriormente utilizando Excel, como herramienta de visualización perteneciente al ecosistema Microsoft.

## Visualización

Para la visualización de los datos se utilizó **Microsoft Excel**, como herramienta del ecosistema Microsoft.

Se creó un dashboard con información de ventas, clientes y pedidos correspondiente a los meses de enero a junio. Incluye una gráfica de líneas para mostrar las ventas por mes, una gráfica de barras para comparar los clientes y tres indicadores: ventas totales, promedio de pedidos y mes con mayores ventas.

El archivo del dashboard se encuentra en la carpeta `visualizacion/`.

Para consultarlo, abre el archivo `dashboard_visualizacion_217O01834.xlsx` con Microsoft Excel o una aplicación compatible.
