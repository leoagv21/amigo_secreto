🎄 Amigo Secreto - Dashboard de Regalos
Una aplicación web interactiva y festiva para gestionar la lista de deseos del juego "Amigo Secreto". Esta aplicación funciona como un panel público en tiempo real, conectándose directamente a una hoja de cálculo de Google (Google Sheets) para mostrar los participantes y sus preferencias de regalos.

Demo en vivo: https://amigo-secreto-xi-ruddy.vercel.app/

✨ Características
🔄 Actualización en Tiempo Real: La lista se actualiza automáticamente (polling) cada 5 segundos sin necesidad de recargar la página.

📱 Diseño Mobile-First: Interfaz "Ultra Compacta" optimizada específicamente para teléfonos móviles, aprovechando el 100% de la pantalla.

⏳ Cuenta Regresiva: Contador automático hasta la fecha del intercambio (12 de Diciembre), con alertas visuales de urgencia.

❄️ Modo Navidad: Botón interactivo para activar/desactivar efectos de nieve y cambiar la paleta de colores.

🚨 Alertas Inteligentes: Modal emergente al iniciar que advierte sobre el tiempo restante para comprar el regalo.

🎨 Detalles Personalizados: Muestra talla, color favorito (con visualización gráfica) y preferencias de "lo que no desea".

📊 Estadísticas: Contadores de participantes registrados y total de regalos solicitados.

🛠️ Tecnologías Usadas
Frontend: HTML5, CSS3 (Grid/Flexbox), JavaScript (ES6+).

Backend / Base de Datos: Google Sheets (como base de datos).

API: Google Apps Script (para servir los datos del Sheet como JSON).

Despliegue: Vercel.

⚙️ Configuración del Proyecto
Si descargas este código, necesitarás configurar dos variables principales en el archivo index.html para conectarlo a tus propios datos:

1. Conectar a Google Sheets
Busca la constante API_URL en el script:

JavaScript

const API_URL = 'TU_URL_DEL_SCRIPT_DE_GOOGLE_APPS_SCRIPT';
Debes crear un script en Google Sheets que devuelva los datos en formato JSON (doGet).

2. Conectar al Formulario
Busca la función irAlFormulario():

JavaScript

const URL_FORMULARIO = 'ENLACE_A_TU_GOOGLE_FORM';
3. Imagen de Fondo
Asegúrate de tener una imagen llamada navidad.jpg en la raíz del proyecto para que el fondo funcione correctamente, o actualiza la ruta en el CSS (body).

📱 Optimización Móvil
El proyecto incluye un sistema de estilos avanzado (@media queries) que transforma la experiencia en celulares:

Eliminación de márgenes y bordes.

Botones grandes y táctiles.

Estadísticas en una sola línea horizontal.

Textos compactos para evitar scroll excesivo.

🚀 Despliegue
Este proyecto es estático (solo HTML/JS), por lo que se puede desplegar fácilmente en:

Vercel (Recomendado)

GitHub Pages

Netlify

¡Feliz Navidad y próspero Amigo Secreto! 🎅🎁
