# 🏥 MediCare Pro

**Sistema de Historias Clínicas, Recetas y Facturación para Consultorio Médico**

> Aplicación web completa para gestión de consultorios médicos en Panamá. Desarrollada como una sola página HTML autocontenida — sin servidor, sin instalación, sin base de datos externa.

---

## ✨ Características principales

### 📋 Gestión de Pacientes
- Registro completo: datos personales, contacto, alergias, antecedentes
- Historia clínica con pestañas: Resumen, Consultas, Recetas, Laboratorio, Citas, Datos
- Búsqueda rápida por nombre o cédula

### 🗓️ Agenda
- Vista del día y próximas citas
- Calendario mensual integrado
- Gestión de citas por estado (confirmada, pendiente, cancelada)

### 🩺 Consultas
- Registro de motivo, anamnesis, examen físico, diagnóstico (CIE-10), plan y seguimiento
- Signos vitales (presión, temperatura, pulso, peso, talla, saturación)
- Vinculación automática al expediente del paciente

### 💊 RxDigital — Recetas Médicas Digitales
- Base de **338 medicamentos** con presentaciones, dosis y vías de administración
- Autocompletado inteligente de medicamentos
- Calculadora de posología por tratamiento (tabletas, jarabes, ampollas)
- Alerta automática de alergias del paciente
- Generación de **PDF profesional** con firma y sello del médico
- Diagnóstico, indicaciones y fecha integrados

### 🧪 Laboratorio
- Solicitud y registro de resultados de exámenes
- Vinculación al expediente del paciente

### 🧾 Facturación
- Emisión de facturas con múltiples ítems
- Manejo de **ITBMS 7%** con ítems exentos (consultas médicas en Panamá)
- Desglose: Subtotal / Exento / Base imponible / ITBMS / Total
- **Impresión de facturas** en formato formal con membrete del médico
- Nota legal de exención (Art. 1057-V Código Fiscal)

### 📊 Estadísticas
- Resumen de actividad: pacientes, consultas, recetas, facturas
- Totales e ingresos del período

### ⚙️ Configuración
- Datos del médico y la clínica
- Información de ITBMS e impuestos

---

## 🚀 Cómo usar

### Opción 1 — Directamente en el navegador
1. Descarga `index.html`
2. Ábrelo con cualquier navegador moderno (Chrome, Firefox, Edge, Safari)
3. ¡Listo! No requiere internet, servidor ni instalación

### Opción 2 — GitHub Pages (acceso desde cualquier dispositivo)
1. Haz un fork de este repositorio
2. Ve a **Settings → Pages**
3. En "Source" selecciona `main` / `/ (root)`
4. GitHub te dará una URL pública (ej: `https://tuusuario.github.io/medicare-pro/`)

> ⚠️ **Nota importante:** Los datos se guardan solo en memoria. Al recargar la página los datos se pierden. Para uso clínico real se recomienda guardar/exportar los datos regularmente o integrar una base de datos.

---

## 📁 Estructura del proyecto

```
medicare-pro/
│
├── index.html          # Aplicación completa (HTML + CSS + JS)
├── README.md           # Este archivo
├── LICENSE             # Licencia MIT
└── .gitignore          # Archivos ignorados por Git
```

La aplicación es **autocontenida en un solo archivo HTML**. Todo el CSS y JavaScript está integrado directamente, sin dependencias locales.

**Dependencias externas (CDN — requieren internet al abrir):**
- [Google Fonts](https://fonts.google.com/) — Playfair Display, DM Sans, DM Mono
- [jsPDF 2.5.1](https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js) — generación de PDF para recetas

---

## 🛠️ Tecnologías

| Tecnología | Uso |
|---|---|
| HTML5 | Estructura |
| CSS3 (Variables, Flexbox, Grid) | Estilos y diseño responsivo |
| JavaScript (ES6+, Vanilla) | Lógica de la aplicación |
| jsPDF | Generación de recetas en PDF |
| Google Fonts | Tipografías |

---

## 📋 Módulos

| Módulo | Ruta | Descripción |
|---|---|---|
| Dashboard | `#dash` | Resumen general y accesos rápidos |
| Agenda | `#agenda` | Citas del día y calendario |
| Pacientes | `#pacs` | Expedientes clínicos |
| Consultas | `#cons` | Registro de consultas |
| RxDigital | `#rxdigital` | Recetas médicas en PDF |
| Laboratorio | `#lab` | Exámenes y resultados |
| Facturación | `#fac` | Facturas con ITBMS |
| Estadísticas | `#est` | Reportes de actividad |
| Configuración | `#cfg` | Datos del médico y clínica |

---

## ⚖️ Consideraciones legales (Panamá)

- Las **consultas médicas** están exentas de ITBMS según la legislación panameña
- La nota de exención en las facturas cita el Art. 1057-V del Código Fiscal — **verificar con su contador**
- Las recetas generadas cumplen con el formato estándar panameño
- Los datos de pacientes son confidenciales — usar en dispositivos seguros

---

## 🗺️ Próximas mejoras (roadmap)

- [ ] Persistencia de datos con localStorage o IndexedDB
- [ ] Exportación/importación de datos en JSON
- [ ] Base de datos completa de 338 medicamentos con calculadora extendida
- [ ] Guardado automático de recetas en el historial del paciente
- [ ] Modo oscuro
- [ ] Backend opcional (Node.js / Supabase) para multiusuario
- [ ] App móvil (PWA)

---

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Por favor:
1. Haz un fork del proyecto
2. Crea una rama (`git checkout -b feature/nueva-funcionalidad`)
3. Haz commit de tus cambios (`git commit -m 'Agrega nueva funcionalidad'`)
4. Push a la rama (`git push origin feature/nueva-funcionalidad`)
5. Abre un Pull Request

---

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo [LICENSE](LICENSE) para más detalles.

---

*Desarrollado para consultorios médicos en Panamá 🇵🇦*
