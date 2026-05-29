# Raccoon Airlines - Interfaz de Usuario

Este proyecto contiene el prototipo y la interfaz gráfica de usuario para **Raccoon Airlines**, un portal web de una aerolínea. Está construido utilizando exclusivamente **HTML5 y CSS3** nativos, diseñado para ser totalmente responsivo y visualmente coherente. El objetivo principal de este proyecto es presentar la maquetación y el flujo de navegación de la aplicación sin depender de JavaScript.

## Características Principales
- **Diseño Responsivo:** Adaptado a pantallas de móviles, tabletas y computadoras de escritorio.
- **Sin JavaScript:** Transiciones y flujos simulados mediante atributos HTML nativos (como validaciones de formulario con `pattern`) y CSS (como redirecciones mediante `<meta http-equiv="refresh">`).
- **CSS Modular:** Los estilos están organizados en carpetas (`css/layout.css`, `css/forms.css`, `css/responsive.css`, etc.) para mantener la escalabilidad.

---

## Guía de Navegación

A continuación se detalla la estructura de pantallas y el flujo que sigue un usuario al navegar por el sistema. Puedes probar el flujo completo simplemente abriendo el archivo **`index.html`** en tu navegador.

### 1. Autenticación y Acceso
Son las pantallas públicas antes de entrar a la plataforma.
- **[index.html](./index.html)**: Página de inicio. Es el punto de entrada principal al sistema.
  <br><img src="./img/screenshots/index-desktop.png" height="350" alt="Vista index desktop"> <img src="./img/screenshots/index-mobile.png" height="350" alt="Vista index mobile"><br><hr><br>
- **[login.html](./login.html)**: Pantalla de inicio de sesión para usuarios registrados.
  <br><img src="./img/screenshots/login-desktop.png" height="350" alt="Vista login desktop"> <img src="./img/screenshots/login-mobile.png" height="350" alt="Vista login mobile"><br><hr><br>
- **[register.html](./register.html)**: Formulario para registrar una cuenta nueva.
  <br><img src="./img/screenshots/register-desktop.png" height="350" alt="Vista register desktop"> <img src="./img/screenshots/register-mobile.png" height="350" alt="Vista register mobile"><br><hr><br>
- **[recover.html](./recover.html)**: Formulario para la recuperación de contraseña olvidada.
  <br><img src="./img/screenshots/recover-desktop.png" height="350" alt="Vista recover desktop"> <img src="./img/screenshots/recover-mobile.png" height="350" alt="Vista recover mobile"><br><hr><br>
- **[create-password.html](./create-password.html)**: Pantalla para establecer una contraseña nueva (flujo posterior a recuperar contraseña).
  <br><img src="./img/screenshots/create-password-desktop.png" height="350" alt="Vista create-password desktop"> <img src="./img/screenshots/create-password-mobile.png" height="350" alt="Vista create-password mobile"><br><hr><br>

### 2. Panel Principal (Dashboard)
- **[menu.html](./menu.html)**: El tablero principal del usuario autenticado. Funciona como el centro de distribución hacia el resto de las funcionalidades de la aerolínea.
  <br><img src="./img/screenshots/menu-desktop.png" height="350" alt="Vista menu desktop"> <img src="./img/screenshots/menu-mobile.png" height="350" alt="Vista menu mobile"><br><hr><br>

### 3. Vuelos y Reservas
Flujo de búsqueda y gestión de vuelos.
- **[search-flights.html](./search-flights.html)**: Pantalla principal de búsqueda, con campos para origen, destino, fechas y número de pasajeros.
  <br><img src="./img/screenshots/search-flights-desktop.png" height="350" alt="Vista search-flights desktop"> <img src="./img/screenshots/search-flights-mobile.png" height="350" alt="Vista search-flights mobile"><br><hr><br>
- **[flights.html](./flights.html)**: Resultados de la búsqueda de vuelos, donde el usuario puede comparar y seleccionar su billete.
  <br><img src="./img/screenshots/flights-desktop.png" height="350" alt="Vista flights desktop"> <img src="./img/screenshots/flights-mobile.png" height="350" alt="Vista flights mobile"><br><hr><br>
- **[my-flights.html](./my-flights.html)**: Panel donde el usuario puede consultar el historial y el estado de sus reservas actuales.
  <br><img src="./img/screenshots/my-flights-desktop.png" height="350" alt="Vista my-flights desktop"> <img src="./img/screenshots/my-flights-mobile.png" height="350" alt="Vista my-flights mobile"><br><hr><br>

### 4. Check-In en Línea
- **[checkin.html](./checkin.html)**: Pantalla donde el usuario puede realizar la facturación de su vuelo ingresando su código de reserva (PNR) y apellido.
  <br><img src="./img/screenshots/checkin-desktop.png" height="350" alt="Vista checkin desktop"> <img src="./img/screenshots/checkin-mobile.png" height="350" alt="Vista checkin mobile"><br><hr><br>

### 5. Pasarela de Pago
Un flujo completamente simulado sin back-end para completar transacciones.
- **[payment.html](./payment.html)**: Formulario de captura de datos de tarjeta de crédito/débito. Utiliza validación nativa de HTML5 para los campos.
  <br><img src="./img/screenshots/payment-desktop.png" height="350" alt="Vista payment desktop"> <img src="./img/screenshots/payment-mobile.png" height="350" alt="Vista payment mobile"><br><hr><br>
- **[processing.html](./processing.html)**: Pantalla de transición visual. Muestra una animación CSS indicando que el pago está siendo "procesado", y automáticamente (tras 3 segundos) redirige de vuelta a `menu.html`.
  <br><img src="./img/screenshots/processing-desktop.png" height="350" alt="Vista processing desktop"> <img src="./img/screenshots/processing-mobile.png" height="350" alt="Vista processing mobile"><br><br>

### 6. Atención al Cliente y Comentarios
- **[feedback-form.html](./feedback-form.html)**: Formulario para envío de comentarios y solicitudes de soporte por parte de los clientes. Incluye validaciones visuales de los campos y animaciones de interacción en los botones.
  <br><img src="./img/screenshots/feedback-form-desktop.png" height="350" alt="Vista feedback-form desktop"> <img src="./img/screenshots/feedback-form-mobile.png" height="350" alt="Vista feedback-form mobile"><br><br>