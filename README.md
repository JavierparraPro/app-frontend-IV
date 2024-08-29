# Frontend del Sistema Móvil de Navegación y Asistencia de Rutas en Entornos Cerrados

## Descripción General

Este repositorio contiene el código fuente del frontend para la aplicación móvil de navegación y asistencia de rutas en entornos cerrados. La aplicación permite a los usuarios crear mapas en 3D y generar guías de rutas a partir de imágenes. El frontend está desarrollado utilizando **Flutter**, un framework UI moderno que permite desarrollar aplicaciones nativas de alto rendimiento para múltiples plataformas con un solo código base.

La aplicación integra tecnologías avanzadas para procesamiento de imágenes y renderización 3D, incluyendo **OpenCV** para el procesamiento de imágenes y **Unity** para la creación y manipulación de modelos 3D.

## Tecnologías Utilizadas

- **Flutter**: Framework UI multiplataforma que permite desarrollar aplicaciones móviles nativas con un solo código base. Flutter es conocido por su alto rendimiento y flexibilidad en la creación de interfaces de usuario atractivas.
- **Dart**: Lenguaje de programación utilizado con Flutter. Dart ofrece una sintaxis limpia y características modernas, ideales para el desarrollo de aplicaciones móviles.
- **OpenCV**: Biblioteca de procesamiento de imágenes utilizada para convertir imágenes 2D en datos procesables. Se utiliza en conjunto con Flutter para manipular imágenes directamente desde la aplicación móvil.
- **Unity**: Motor de renderización 3D utilizado para generar y manipular modelos 3D a partir de archivos SVG generados desde imágenes procesadas. La integración de Unity se maneja a través de un plugin de Flutter.
- **flutter_unity_widget**: Plugin utilizado para integrar Unity dentro de la aplicación Flutter, permitiendo la visualización e interacción de modelos 3D.
- **Provider**: Paquete de Flutter utilizado para la gestión del estado de la aplicación, facilitando el manejo de la lógica de negocio y la interacción con la UI de manera eficiente.

## Arquitectura del Frontend

La arquitectura del frontend sigue un enfoque basado en componentes y una gestión de estado reactiva, utilizando el patrón **MVVM (Model-View-ViewModel)** para separar la lógica de negocio de la UI. Esto facilita el mantenimiento, la escalabilidad y las pruebas de la aplicación. Los componentes principales son:

1. **Modelos (Models)**: Representan la estructura de datos que maneja la aplicación, como la información del usuario, las rutas, y los modelos 3D.
2. **Vista (Views)**: Componentes de la UI construidos con Flutter que renderizan la información en la pantalla del usuario. Estas vistas son reactivas y se actualizan automáticamente cuando el estado cambia.
3. **ViewModels**: Contienen la lógica de negocio de la aplicación. Interactúan con los modelos y actualizan las vistas en respuesta a las acciones del usuario y los eventos de la aplicación.

## Funcionalidades Principales

- **Carga y Procesamiento de Imágenes**: Permite a los usuarios cargar imágenes desde su dispositivo, que luego son procesadas para convertirlas en formato SVG utilizando OpenCV.
- **Generación de Modelos 3D**: Convierte imágenes procesadas en modelos 3D utilizando Unity, y permite a los usuarios interactuar con estos modelos dentro de la aplicación.
- **Modo Offline**: Soporte para operaciones offline, donde los datos y las operaciones críticas se almacenan localmente y se sincronizan cuando se restablece la conexión a internet.
- **Gestión de Usuarios**: Funcionalidades para registro, inicio de sesión y gestión de perfiles de usuario.
- **Notificaciones Push**: Envío de notificaciones para alertar a los usuarios sobre nuevas funcionalidades, actualizaciones y recordatorios importantes.
- **Interactividad y Personalización**: Permite a los usuarios interactuar con modelos 3D y personalizar la interfaz de usuario (UI) según sus preferencias.

## Configuración del Entorno de Desarrollo

Sigue los pasos a continuación para configurar el entorno de desarrollo del frontend:

1. **Instalación de Flutter**: Asegúrate de tener Flutter instalado en tu máquina. Puedes seguir las instrucciones oficiales de instalación en [Flutter.dev](https://flutter.dev/docs/get-started/install).

2. **Clonar el Repositorio**:
   ```bash
   git clone https://github.com/tu-usuario/sistema-navegacion-frontend.git
   cd sistema-navegacion-frontend
