# 🚧 AUDITORÍA EXCLUSIVA PMT

### Acta Digital de Control – Plan de Manejo de Tránsito (PMT)

![Image](https://www.electromanferonline.com/75-large_default/chaleco-reflectivo-en-malla.jpg)

![Image](https://www.provesi.com.co/828-large_default/senalizador-vial-tubular-base-cono-naranja-baliza-3-reflectivos-pg-.jpg)

![Image](https://www.electromanferonline.com/1329-large_default/barrera-tipo-malet%C3%ADn-para-tr%C3%A1fico-15m-x-055m-x-045m-.jpg)

![Image](https://rotoplast.com.co/uploads/product_pictures/BARRERA%20SIN%20FONDO.png)

Aplicación web desarrollada en **HTML, CSS y JavaScript puro** para la inspección técnica del:

> **Plan de Manejo de Tránsito (PMT)**
> Control de Interventoría – Seguridad Vial en obra

Diseñada para el proyecto:

**Mejoramiento Vía Granada – Guatapé (Sector La Sonadora – La Peña)**

Optimizada para:

* 📱 Trabajo en campo (celular / tablet)
* 💻 Escritorio técnico
* 🖨 Generación inmediata de PDF institucional

---

# 🎯 Objetivo del Sistema

Garantizar el cumplimiento normativo del PMT en frentes de obra vial mediante:

* Evaluación técnica estructurada
* Registro fotográfico en sitio
* Evidencia documental inmediata
* Control de seguridad vial
* Generación de acta formal en PDF

---

# ⚙️ Características Principales

* 🚦 Sistema semáforo (Cumple / No Cumple / N/A)
* 📸 Evidencia fotográfica múltiple por ítem
* 🏷 Carga dinámica de logos institucionales
* 📅 Fecha automática
* 📱 Diseño totalmente responsive
* 🖨 Formato profesional listo para impresión
* 🔒 Funciona offline (sin servidor)
* 🧹 Reinicio rápido del acta

---

# 📂 Estructura del Proyecto

```
📁 auditoria-pmt/
 └── 📄 index.html
```

Incluye en un solo archivo:

* Maquetación estructurada
* Estilos pantalla + impresión
* Adaptación móvil avanzada
* Lógica JavaScript integrada
* Optimización para iOS y Android
* Funcionalidad Offline (Service Worker)

No requiere:

* Base de datos
* Backend
* Frameworks
* Librerías externas (solo web APIs nativas)

---

# 📋 Módulos de Auditoría Incluidos

---

## 1️⃣ Dispositivos Manuales y Personal (Bandereros)

* Chaleco reflectivo NTC-4739
* Impermeable amarillo reflectivo
* Paletas PARE/SIGA (mín. 45 cm – Tipo IV)
* Soporte mínimo 1.60 m
* Radios bidireccionales

---

## 2️⃣ Señalización Vertical

* Fondo naranja reflectivo
* Postes metálicos reglamentarios
* Prohibición de hormigueo
* Anclaje en concreto 14 MPa
* Empotramiento mínimo 50 cm

---

## 3️⃣ Canalización y Logística de Cierres

* Cantidades mínimas:

  * 44 Barreras tipo maletín
  * 42 Balizas
  * 2 Barricadas de listón
* Ancho libre mínimo 2.50 m
* Gestión de cierres parciales
* Desvíos y pasacalles informativos
* Control de vía alterna

---

# 🚨 Alerta Crítica Integrada

El sistema incluye advertencia destacada:

> ⚠ Si se ejecutan rieles o placas huellas en vía de 5m, el acero de refuerzo bloquea completamente el tránsito.
> **Debe exigirse cierre total y uso de vía alterna por La Peña (8.5 km).**

Esto permite respaldo documental ante incumplimientos graves.

---

# 💾 Exportación e Importación de Datos (JSON)

Para asegurar la integridad de los registros sin usar bases de datos en la nube, el sistema incluye:

* **Guardar .json:** Descarga toda la información diligenciada (textos, selecciones, evidencias y firmas comprimidas) en un archivo local `.json`.
* **Cargar Datos:** Permite restaurar auditorías previamente guardadas mediante la subida de archivos `.json` o `.gsc` antiguos. Ideal para iniciar una nueva auditoría basada en la de la semana pasada sin volver a escribir datos estáticos.

---

# ✍️ Firma Digital Integrada

En la zona de firmas se incluye una función que permite capturar la firma digital directamente en el dispositivo (móvil o computador).

* Se abre un modal de dibujo `canvas`
* Se permite firmar con el dedo, stylus o ratón
* También permite cargar una foto de la firma (`📁`) o borrarla (`❌`).

---

# 📱 Adaptación Móvil Inteligente y Aplicación PWA

La herramienta es una **Progressive Web App (PWA)**, lo que significa que se puede instalar como una aplicación nativa:

1. Visitar la URL o abrir `index.html` en el dispositivo.
2. Seleccionar la opción de "Añadir a la pantalla de inicio".
3. Gracias al archivo `sw.js` y `manifest.json`, funciona **totalmente offline** sin depender de internet.

En pantallas pequeñas:

* Las tablas se convierten en tarjetas verticales
* Se agregan etiquetas automáticas con `data-label`
* Galería en 2 columnas
* Firmas apiladas
* Botones flotantes accesibles

Optimizado para:

* iPhone
* Android
* Tablets en obra

---

# 📸 Sistema de Evidencia Fotográfica

Cada ítem incluye:

* Carga múltiple desde cámara o galería
* Visualización inmediata
* Eliminación con confirmación
* Adaptación automática a impresión

Las imágenes:

* Se comprimen antes de mostrarse y guardarse internamente (optimización de peso y rendimiento en móviles).
* No se suben a ningún servidor.
* Permanecen en memoria durante la sesión.
* Se integran en el PDF generado.

---

# 🚦 Sistema Semáforo

Estados disponibles:

* 🟢 CUMPLE
* 🔴 NO CUMPLE
* ⚪ N/A

El color cambia automáticamente al seleccionar.

Se incluyen además notificaciones estilo "Toast" modernas que reemplazan los `alert()` nativos para informarle al usuario sobre el estado de la carga de información temporal.

Funciona correctamente en:

* iOS Safari
* Chrome Android
* Navegadores de escritorio
* App local instalada (PWA)

---

# 🖨 Generación de PDF Profesional

Al presionar:

```
🖨 Guardar PDF
```

El sistema:

* Activa modo impresión
* Oculta botones y zonas de carga
* Mantiene colores institucionales
* Ajusta tablas a formato formal
* Repite membrete en cada página
* Conserva evidencia fotográfica

Recomendado:

> Imprimir → Guardar como PDF

---

# 🧹 Reinicio del Acta

Botón:

```
🗑 Limpiar
```

* Confirma antes de borrar
* Recarga la página
* Elimina datos, firmas y fotos

---

# 👷 Perfil de Usuario

* Interventor PMT
* Ingeniero Civil
* Supervisor Vial
* Coordinador de Seguridad Vial
* Entidad contratante
* Alcaldía Municipal

---

# 🔒 Seguridad y Limitaciones

* No guarda información al cerrar navegador
* No almacena datos en nube
* No reemplaza sistema oficial documental
* Recomendado generar PDF inmediatamente después de diligenciar

---

# 📄 Licencia

Uso técnico institucional.
Libre adaptación según requerimientos contractuales y normativos.

---

Si quieres, puedo prepararte también:

* 📘 Manual Técnico PMT en PDF formal
* ☁ Versión con almacenamiento en nube
* 📊 Dashboard consolidado de hallazgos
* 🖊 Versión con firma digital avanzada
* 🏛 Versión con identidad gráfica oficial municipal

Solo dime cuál desarrollamos.
