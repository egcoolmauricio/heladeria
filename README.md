# 🍦 Punto Gelato — Sistema de Gestión

Aplicación web de página única (SPA) para la gestión interna de una heladería. Desarrollada en HTML, CSS y JavaScript vanilla, sin dependencias ni frameworks, usando Firebase como backend en la nube.

## Características

- **Compra / Venta** — registrá ventas y compras del día en segundos
- **Stock e Inventario** — controlá el stock de productos y sabores (sección exclusiva para administradores)
- **Ventas** — historial de ventas con filtros por fecha
- **Configuración** — conectá la app a tu proyecto Firebase y gestioná los accesos
- **Control de roles** — acceso diferenciado entre empleados y administradores mediante Firebase Auth
- **Sin instalación** — corre directo en el navegador, sin servidor ni build step

## Archivos

| Archivo         | Descripción                                       |
| --------------- | ------------------------------------------------- |
| `index.html`    | Aplicación principal                              |
| `migrador.html` | Utilidad para importar un backup JSON a Firestore |

## Tecnologías

- HTML / CSS / JavaScript (vanilla)
- [Firebase v10](https://firebase.google.com/) — Firestore + Authentication
- Google Fonts (Playfair Display, DM Sans)

## Primeros pasos

1. Creá un proyecto en [Firebase Console](https://console.firebase.google.com/).
2. Habilitá **Firestore** y **Authentication** (proveedor: Email/Contraseña).
3. Abrí `index.html` en el navegador.
4. En la pestaña **Configuración**, ingresá las credenciales de tu proyecto Firebase y hacé clic en **Conectar**.
5. La configuración se guarda en `localStorage`, por lo que solo tenés que hacerlo una vez por dispositivo.

## Migración de datos

Si ya contás con un backup en formato JSON, abrí `migrador.html`, ingresá las credenciales Firebase, cargá el archivo y hacé clic en **Migrar todo a Firebase**. El migrador sube ventas, productos, precios, sabores y stock a Firestore.

## Licencia

Uso personal / familiar. Sin licencia de distribución.
