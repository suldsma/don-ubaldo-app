# 🛒 DON UBALDO – Caja y Stock

Sistema web liviano y rápido para la gestión de comercios de barrio (**Despensa, Verdulería y Fiambrería**). Es **un único archivo HTML** con CSS y JavaScript nativos: se abre en cualquier navegador, sin servidor ni base de datos.

---

## ✨ Características principales

### 🧾 Venta (POS)
* Filtro por rubro con botones o atajos de teclado, y buscador por nombre o código de barras.
* Ticket con subtotal, **descuento/recargo en %**, total y **cálculo automático del vuelto**.
* Venta de productos **por kilo**: se carga por pesos (`$2000`), por kilos (`0,25`) o con botones rápidos (¼, ½, 1 kg).
* Control de cantidades con `+` / `−`, y quitar productos de a uno.
* Medios de pago: Efectivo, Transferencia, Débito, Crédito y QR / Mercado Pago.
* **Impresión de ticket** (formato 72 mm, impresora térmica) automática o manual, y opción de **compartir por WhatsApp**.
* El stock se descuenta al cobrar y no permite vender más de lo disponible.

### 📦 Stock (solo dueño)
* Protegido con **PIN** (por defecto `1234`, cambialo desde la misma pantalla).
* Alta, edición y baja de productos: nombre, código de barras, rubro, precio, stock y si se vende por unidad o por kilo.
* Buscador de productos y alerta visual de **stock bajo** (5 o menos).
* Evita códigos de barras duplicados.

### 📊 Ventas y reportes
* Resumen por día: total recaudado, cantidad de ventas, y desglose por **rubro** y por **medio de pago**.
* Navegación por fecha o todo el historial.
* **Anular una venta completa** o **quitar un solo producto** de una venta (devuelve el stock; pide PIN del dueño).
* Exportación a **Excel (.xlsx)**:
  * *Cierre del día*: resumen + detalle de las ventas de esa fecha.
  * *Todas las ventas*: detalle, ventas, resumen por día, por producto y stock actual.

### 💲 Precios
* Consulta rápida del precio de cualquier producto escaneando el código o buscando por nombre.
* **Historial de cambios de precio** registrado automáticamente.

### 🔒 Datos seguros
* Guardado automático en el navegador con **copia de respaldo interna** de la versión anterior.
* **Copia de seguridad** descargable (`.json`) y restaurable desde Stock.
* Aviso si pasaron más de 7 días sin descargar una copia.
* Sincronización entre varias pestañas/ventanas abiertas.
* Las ventas borradas se guardan en un respaldo antes de eliminarse.

### 📷 Lector de códigos de barras
* Compatible con **lectores USB** (funcionan como teclado).
* Escaneo con la **cámara** del celular o PC (`BarcodeDetector` nativo, con **ZXing** como alternativa).

### 🌗 Modo claro / oscuro
* Se adapta automáticamente a la preferencia del sistema.

---

## ⌨️ Atajos de teclado

| Tecla | Acción |
| :--- | :--- |
| **F1** | Ir a Venta y enfocar el buscador |
| **F2** | Ir a Stock (área de dueño) |
| **F3** | Ir a Ventas |
| **F4** | Ir a Precios |
| **F5 – F8** | Filtrar rubro: Todos / Despensa / Verdulería / Fiambrería |
| **F9** | Cambiar medio de pago |
| **F10** | Cobrar |
| **Shift + F9** | Vaciar ticket |
| **Alt + Q** | Quitar el último producto del ticket |
| **Alt + P** | Imprimir el último ticket |
| **Alt + E** | Abrir escáner de cámara |
| **Enter** | Agregar el primer resultado de la búsqueda |
| **Esc** | Limpiar búsqueda / cerrar ventanas |

---

## 🚀 Tecnologías

* **HTML5**
* **CSS3** (Grid, Flexbox, variables CSS)
* **JavaScript (ES6+)** nativo
* **LocalStorage** para guardar los datos en el navegador
* Librerías cargadas solo cuando se usan (requieren internet):
  * [SheetJS](https://sheetjs.com/) para exportar a Excel
  * [ZXing](https://github.com/zxing-js/library) como lector de cámara alternativo

---

## 📲 Uso y despliegue (GitHub Pages)

1. Cloná o descargá este repositorio.
2. Asegurate de que el archivo principal se llame `index.html`.
3. Abrilo directamente en el navegador, o publicalo gratis con **GitHub Pages**:
   `Settings > Pages > Branch: main > / (root)`.

> ⚠️ **Importante:** los datos se guardan en el navegador de cada dispositivo. Descargá una **copia de seguridad** con regularidad (Stock → *Descargar copia*) y cambiá el **PIN** por defecto.

---

## 📄 Licencia

Proyecto de uso libre para comercios de barrio. Agregá acá tu licencia si querés definir una.
