# ACME AIR — Maquetación Web

Proyecto Campusland (HTML5 + CSS). Maquetación completa app móvil ACME AIR, fiel a mockups UI/UX. Sin lógica JS, solo estructura semántica + navegación simulada vía enlaces.

## Contexto

ACME AIR, aerolínea, renueva experiencia digital con app web adaptable a móvil. Interfaz antigua tenía: diseño no adaptativo, navegación confusa, inconsistencia visual, accesibilidad limitada. Nuevo diseño resuelve esto: interfaz limpia, intuitiva, responsiva.

## Objetivo

Maquetación completa app móvil ACME AIR basada en mockups, usando solo HTML5 y CSS. Responsividad, coherencia visual, navegabilidad fluida.

## Vistas

| Vista | Archivo | Descripción |
|---|---|---|
| Login | `index.html` | Email, contraseña, "Recordar mis datos", enlaces a registro/recuperar |
| Registro | `registro.html` | Nombre, identificación, email, teléfono, ciudad |
| Crear contraseña | `crear-contrasena.html` | Contraseña + repetir |
| Recuperar contraseña | `recuperar-contrasena.html` | Email, envía a crear contraseña |
| Menú principal | `menu.html` | Tarjetas: Buscar vuelos, Check-in, Mis vuelos |
| Búsqueda de vuelos | `buscar-vuelos.html` | Origen, destino, fechas, checkbox solo ida |
| Vuelos disponibles | `vuelos.html` | Grid vuelos (ruta, fecha, hora, precio) |
| Check-in | `checkin.html` | Número de vuelo/reserva, contacto emergencia |
| Mis vuelos | `mis-vuelos.html` | Listado vuelos reservados/previos |

## Navegación simulada

- Login → Ingresar → Menú
- Login → Crear cuenta → Registro
- Login → ¿Olvidaste tu contraseña? → Recuperar contraseña
- Registro → Guardar → Crear contraseña
- Recuperar contraseña → Enviar → Crear contraseña
- Crear contraseña → Guardar → Menú
- Menú → Buscar vuelos → Búsqueda de vuelos → Buscar → Vuelos disponibles → Volver → Menú
- Menú → Check-in → Guardar → Menú
- Menú → Mis vuelos → Volver → Menú
- Cualquier vista con "Cerrar sesión" → Login

## Estructura del proyecto

```
acme-air-app/
├── index.html               (Login)
├── menu.html                (Menú principal)
├── registro.html            (Registro)
├── crear-contrasena.html    (Nueva contraseña)
├── buscar-vuelos.html       (Búsqueda de vuelos)
├── vuelos.html              (Vuelos disponibles)
├── checkin.html             (Check-in)
├── mis-vuelos.html          (Mis vuelos)
├── recuperar-contrasena.html (Recuperar contraseña)
├── css/
│   ├── style.css
│   ├── forms.css
│   ├── layout.css
│   └── responsive.css
└── img/
    └── icons/
```

## Responsividad

Breakpoints:
- 320px — móvil pequeño
- 768px — tablet
- 1024px — desktop (vista centrada, padding lateral)

Formularios fluidos (`max-width` + tipografía proporcional).

## Estilo corporativo

- Paleta: degradado rosa–violeta (`#d13cff` → `#00b0ff`)
- Tipografía: Poppins / Open Sans
- Botones primarios: `box-shadow` + hover `transform: scale(1.02)`

## Equipo

| Dev | Vistas |
|---|---|
| Nicolas | Login, Registro, Crear contraseña, Recuperar contraseña |
| Oliver | Menú principal, Búsqueda de vuelos |
| Sergio | Vuelos disponibles, Check-in, Mis vuelos |
