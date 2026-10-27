# Peluditos Pet Chile

Trabajo de la semana 3 de Integración de Plataformas. Esta carpeta contiene los diagramas BPMN y una prueba del proceso en Flowable OSS 6.8.1.

## Para ejecutarlo

Se necesita Windows, Java 21 JDK, Python 3 y conexión a internet en el primer inicio. Los pasos están en `GUIA-DEMOSTRACION.md`.

Flowable se descarga automáticamente la primera vez que se ejecuta `iniciar-flowable-rest.cmd`. Los archivos descargados quedan en `flowable-6.8.1/` y no se suben al repositorio.

## Contenido

- `bpmn/`: proceso actual y dos procesos propuestos.
- `despliegue-proceso-681.bar`: proceso de prueba para Flowable.
- `formularios/`: formularios de Flowable y panel local.
- `servicio-java/`: servicio que propone un mensaje.
- `worker/`: programa que conecta Flowable con el servicio Java.
- `docs/servicios.md`: servicios actuales y propuestos.
- `evidencias/`: imágenes y resultados de las pruebas.

## Qué hace la prueba

Desde el panel se inicia una oportunidad para el cumpleaños de una mascota. El servicio Java genera un mensaje sugerido. La dueña lo revisa y registra si hubo venta. El envío del correo es simulado.

Esta prueba todavía no guarda clientes de forma permanente ni se conecta con redes sociales. Al cerrar Flowable REST se pierden los casos iniciados; para volver a probar hay que ejecutar de nuevo `desplegar-demo-flowable.cmd`.
