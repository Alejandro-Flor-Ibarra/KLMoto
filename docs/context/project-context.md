# Contexto confirmado del proyecto

## Producto

- KLMoto ayuda a gestionar el mantenimiento de una motocicleta y sus recorridos.
- La pantalla de cuidados mostrará una tabla de mantenimientos pendientes, por ejemplo, cambio de discos de clutch, cambio de pastillas de freno y lubricación de guayas.
- Un agente de IA buscará y analizará el manual de taller correspondiente a la moto para recomendar mantenimientos según el documento.
- Si no se encuentra el manual correcto, la app ofrecerá alternativas: pedir al usuario una foto del manual o mostrar recomendaciones genéricas claramente marcadas como orientativas.
- La pantalla de talleres consultará Google Maps y listará los talleres encontrados, mostrando distancia y calificación. El usuario podrá ajustar el peso relativo de esos criterios en el orden.
- Habrá una actividad inicial de registro que solicitará el nombre del usuario y los datos de su moto. Para identificarla, el usuario podrá elegir entre un catálogo de motos o aportar una foto del manual.
- Para buscar el manual desde el catálogo, se pedirán marca, modelo, año, cilindrada y versión exacta de la moto.

## Estado de implementación confirmado

- La aplicación es Android nativa y usa Kotlin, layouts XML, Material 3 y `ConstraintLayout`.
- La pantalla principal contiene un título, un panel de kilometraje, un bloque informativo de registro automático y una navegación inferior.
- El bloque de registro automático incluye un `SwitchMaterial`; la pantalla muestra una explicación relacionada con el uso de ubicación GPS.
- La navegación inferior usa `BottomNavigationView` y un menú de recursos en `res/menu`.
- Los iconos SVG deben convertirse a Vector Drawable XML para usarse como recursos Android. La tintura automática de los iconos se desactivó para conservar los colores de vectores multicolor.
- `MainActivity` configura el layout y los insets del sistema. La selección de destinos de navegación y el registro GPS todavía no están implementados.

## Pendiente

- Definir cómo se valida la foto del manual y cómo el usuario confirma que la IA identificó correctamente la moto.
- Definir las fuentes y el proceso de verificación del manual de taller usado por el agente de IA.
- Definir cómo se ponderan distancia y calificación al ordenar talleres y cómo se ajustan esos pesos en la interfaz.
- Definir si una cuenta podrá administrar varias motos.
- Definir los permisos y el alcance del uso de ubicación GPS.
- Conectar las opciones de navegación inferior con sus pantallas y comportamientos.