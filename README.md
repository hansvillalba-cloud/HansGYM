# HansFit Casa

Aplicación de entrenamiento en español para personalizar una rutina, revisar las demostraciones y registrar el progreso en el navegador.

## Archivos

- `index.html`: aplicación completa, con sus estilos, funciones y demostraciones incluidas.
- `README.md`: esta guía de uso e instalación.

## Subir a GitHub y publicar con GitHub Pages

1. Descomprime el paquete ZIP en tu computador.
2. En GitHub, crea un repositorio nuevo; por ejemplo, `hansfit-casa`.
3. En el repositorio, entra a **Add file → Upload files** y sube los archivos `index.html` y `README.md` que están dentro del paquete. Déjalos en la carpeta principal del repositorio, no dentro de otra carpeta.
4. Confirma los cambios con **Commit changes**.
5. Ve a **Settings → Pages**. En **Build and deployment**, selecciona **Deploy from a branch**; elige la rama `main` y la carpeta `/(root)` y guarda.
6. Espera a que GitHub termine la publicación. En **Settings → Pages** aparecerá la dirección del sitio. Ábrela desde el celular usando HTTPS.

Revisa la visibilidad del repositorio y del sitio antes de publicarlos. GitHub Pages puede hacer que el sitio sea público. No incluyas contraseñas, información privada ni datos de entrenamiento personales en el repositorio.

## Uso

1. Abre la aplicación y crea el perfil: objetivo, nivel, días y uno o varios equipos disponibles. Las horas de ciclismo son opcionales.
2. Elige una sesión A, B o C; si programas cuatro o cinco días también aparecen D y E. Selecciona cada día en **Tu semana** para revisar su rutina.
3. Despliega **Ver movimiento animado y pasos**. Puedes pausar o reproducir la demostración; las imágenes ilustran el patrón de movimiento y no siempre muestran el implemento exacto.
4. Inicia la sesión. Incluye calentamiento y estiramientos. Usa el cronómetro o el contador manual y registra la actividad al terminar.
5. Consulta el progreso por día, semana o mes. Las calorías son estimaciones basadas en peso, duración y tipo de actividad, no mediciones exactas.

## Cámara y pulsaciones

- Abre el sitio desde una dirección HTTPS y concede permiso para usar la cámara. También puede funcionar desde `localhost`; al abrir el archivo directamente, el acceso depende del navegador.
- La primera carga del seguimiento necesita internet para descargar MediaPipe y su modelo. La aplicación muestra cómo ubicar el teléfono y puede contar repeticiones en los movimientos compatibles. En las demás actividades usa el contador manual o el cronómetro. El seguimiento y las indicaciones son orientativos: no certifican la técnica ni sustituyen a un entrenador.
- Para oír el conteo activa **Conteo por voz**. La disponibilidad y el idioma de la voz dependen del dispositivo.
- La conexión de pulso usa Web Bluetooth y un dispositivo que exponga el servicio estándar de frecuencia cardiaca. La compatibilidad depende del dispositivo, el sistema operativo y el navegador; si no está disponible, registra el pulso manualmente.
- La cámara, el reloj o la banda deben probarse en el propio teléfono y navegador de destino.

## Datos y funcionamiento

Los perfiles y el historial se guardan en el almacenamiento local del navegador. No se sincronizan automáticamente entre teléfonos, computadoras, navegadores o direcciones web distintas. Exporta una copia desde el perfil antes de borrar los datos del navegador o cambiar de dispositivo.

Las demostraciones están incluidas en el archivo y no requieren descargar imágenes. La detección de postura necesita la primera descarga de componentes externos; sin ella puedes seguir usando las rutinas y el registro manual. Para mayor privacidad, no incluyas exportaciones con datos personales en un repositorio público.
