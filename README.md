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
- **[login.html](./login.html)**: Pantalla de inicio de sesión para usuarios registrados.
- **[register.html](./register.html)**: Formulario para registrar una cuenta nueva.
- **[recover.html](./recover.html)**: Formulario para la recuperación de contraseña olvidada.
- **[create-password.html](./create-password.html)**: Pantalla para establecer una contraseña nueva (flujo posterior a recuperar contraseña).

### 2. Panel Principal (Dashboard)
- **[menu.html](./menu.html)**: El tablero principal del usuario autenticado. Funciona como el centro de distribución hacia el resto de las funcionalidades de la aerolínea.

### 3. Vuelos y Reservas
Flujo de búsqueda y gestión de vuelos.
- **[search-flights.html](./search-flights.html)**: Pantalla principal de búsqueda, con campos para origen, destino, fechas y número de pasajeros.
- **[flights.html](./flights.html)**: Resultados de la búsqueda de vuelos, donde el usuario puede comparar y seleccionar su billete.
- **[my-flights.html](./my-flights.html)**: Panel donde el usuario puede consultar el historial y el estado de sus reservas actuales.

### 4. Check-In en Línea
- **[checkin.html](./checkin.html)**: Pantalla donde el usuario puede realizar la facturación de su vuelo ingresando su código de reserva (PNR) y apellido.

### 5. Pasarela de Pago
Un flujo completamente simulado sin back-end para completar transacciones.
- **[payment.html](./payment.html)**: Formulario de captura de datos de tarjeta de crédito/débito. Utiliza validación nativa de HTML5 para los campos.
- **[processing.html](./processing.html)**: Pantalla de transición visual. Muestra una animación CSS indicando que el pago está siendo "procesado", y automáticamente (tras 3 segundos) redirige de vuelta a `menu.html`.
