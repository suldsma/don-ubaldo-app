# 🛒 DON UBALDO – Caja y Stock

Sistema web liviano, rápido y funcional diseñado para la gestión integral de comercios de barrio (Despensa, Verdulería y Fiambrería). Está desarrollado en **un único archivo HTML** con CSS y JavaScript nativos, lo que permite ejecutarlo de forma instantánea sin necesidad de servidores complejos ni bases de datos externas.

---

## ✨ Características Principales

* **Modo Venta (POS):** 
  * Interfaz rápida con filtrado por categorías mediante botones táctiles o atajos de teclado.
  * Control dinámico del ticket de compra, desglose de subtotales y cálculo automático del vuelto.
  * Soporte para múltiples medios de pago (*Efectivo, Transferencia, Débito, Crédito, QR / Mercado Pago*).
* **Gestión de Stock:**
  * Panel protegido por PIN de seguridad exclusivo para el administrador/dueño.
  * Altas, bajas y modificaciones en tiempo real de productos, códigos de barras, precios y unidades (por kilo o por unidad).
  * Alertas visuales automáticas para productos con bajo stock.
* **Control de Precios y Competencia:**
  * Herramienta para comparar los precios de tu local frente a grandes cadenas de supermercados (*Coto, Jumbo, Carrefour, Mas Online*).
  * Historial de cambios de precios registrados automáticamente.
* **Reportes y Estadísticas:**
  * Panel de resumen diario con el total recaudado, cantidad de ventas y desglose por rubro y método de pago.
  * Opción para exportar el historial completo de ventas a formato **CSV**.
* **Lector de Códigos de Barra:**
  * Compatible con lectores de código USB y escaneo mediante la cámara del dispositivo móvil o PC (vía *BarcodeDetector* y *ZXing*).
* **Modo Oscuro / Claro automático:**
  * Diseño adaptado mediante variables CSS (`color-scheme`) que respeta las preferencias del sistema.

---

## ⌨️ Atajos de Teclado

Para agilizar la atención en el mostrador, el sistema cuenta con atajos globales:

| Tecla | Acción |
| :--- | :--- |
| **F1** | Ir a Venta y enfocar buscador |
| **F2** | Ir a Stock (Área de dueño) |
| **F3** | Ir a Reporte de Ventas |
| **F4** | Ir a Comparativa de Precios |
| **F5 – F8** | Filtrar categorías (Todos / Despensa / Verdulería / Fiambrería) |
| **F9** | Cambiar medio de pago |
| **Shift + F9** | Vaciar ticket actual |
| **F10** | Cobrar / Finalizar venta |
| **Alt + E** | Abrir escáner de cámara |
| **Enter** | Agregar el primer resultado / Confirmar acción |
| **Escape** | Limpiar búsqueda / Cerrar modales |

---

## 🚀 Tecnologías Utilizadas

* **HTML5 Semantic**
* **CSS3** (Grid Layout, Flexbox, Custom Properties / Variables)
* **JavaScript (ES6+)** nativo
* **LocalStorage API** para la persistencia local de los datos (sin dependencias externas pesadas)

---

## 📲 Uso y Despliegue (GitHub Pages)

Al tratarse de una aplicación web estática contenida en un único archivo, puedes ponerla en marcha en segundos:

1. Clona o descarga este repositorio.
2. Asegúrate de que el archivo principal se llame `index.html`.
3. ¡Listo! Puedes abrirlo directamente en cualquier navegador web moderno o activarlo de forma gratuita en **GitHub Pages** desde la configuración de tu repositorio (`Settings > Pages > Branch: main`).
