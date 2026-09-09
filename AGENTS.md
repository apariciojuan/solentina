# Repository Guidelines

## Estructura del proyecto

Este repositorio es una web estática de yoga. `index.html` contiene el marcado, los estilos y el comportamiento de la página. La imagen principal vive en `img/`. Consulta `DESIGN.md` antes de cambiar la interfaz: define la identidad mediterránea, tokens de color, tipografías, espaciado y reglas adaptables. `README.md` solo ofrece una descripción breve del proyecto.

## Desarrollo y vista previa

No hay gestor de paquetes, compilación ni servidor de desarrollo configurados. Para revisar cambios, abre `index.html` en un navegador o sírvelo localmente con una herramienta disponible en tu equipo, por ejemplo:

```bash
python3 -m http.server 8000
```

Después visita `http://localhost:8000`. No añadas dependencias, herramientas de construcción ni archivos generados sin una necesidad explícita.

## Estilo y convenciones

Usa HTML semántico (`header`, `main`, `section`, `footer`) y conserva la indentación existente, de dos espacios. Escribe clases CSS en minúsculas con palabras separadas por guiones, por ejemplo, `.class-card` o `.hero-content`. Mantén las variables, colores, radios, sombras y escalas tipográficas coherentes con `DESIGN.md`; prioriza la legibilidad, el contraste y una composición espaciosa. Añade texto alternativo descriptivo a las imágenes y evita estilos en línea salvo que el archivo ya use ese patrón.

## Pruebas y revisión visual

No existe una suite automatizada. Antes de enviar cambios, revisa la página en un navegador y comprueba al menos los anchos móvil (320–767 px), tableta (768–1023 px) y escritorio (1024 px o más). Verifica enlaces, carga de imágenes, legibilidad, navegación por teclado y que no aparezcan desbordamientos horizontales.

## Commits y pull requests

El historial usa mensajes breves e imperativos, como `Add web`. Sigue ese formato: `Add booking section` o `Adjust mobile spacing`. Mantén cada commit centrado en un cambio. Las pull requests deben explicar qué cambió, enlazar la incidencia si existe y adjuntar capturas antes/después cuando alteren la interfaz. Indica también qué tamaños de pantalla revisaste.
