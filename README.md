# 🏦 Bank Statement Manager (Google Colab)

Sistema automatizado para parsear, almacenar y analizar estados de cuenta bancarios de bancos ecuatorianos. Desarrollado por **Isaac Esteban Haro Torres**.

---

## 📝 Descripción

Sistema profesional para el procesamiento automático de estados de cuenta bancarios en formato PDF. Ideal para personas y pequeñas empresas que necesitan gestionar múltiples cuentas bancarias de forma eficiente.

### ¿Qué hace este proyecto?

- **Extracción de datos**: Parsea automáticamente transacciones de PDFs de Banco del Austro y Banco del Pacífico
- **OCR avanzado**: Utiliza Tesseract para procesar PDFs escaneados o con imágenes
- **Almacenamiento estructurado**: Guarda todos los datos en SQLite para consulta posterior
- **Análisis financiero**: Genera reportes, calcula intereses y estadísticas de gasto
- **Simulador de pagos**: Calcula meses necesarios para pagar deudas según pagos realizados

---

## ✨ Características Principales

| Característica | Descripción |
|----------------|-------------|
| 📄 **Multi-formato PDF** | Soporta PDFs digitales y escaneados |
| 🏦 **Bancos soportados** | Banco del Austro, Banco del Pacífico |
| 🔍 **OCR Inteligente** | Tesseract con reconocimiento en español |
| 💾 **Base de datos SQLite** | Almacenamiento persistente y consultas SQL |
| 📊 **Análisis financiero** | Gráficos, estadísticas y tendencias |
| 🧮 **Simulador de pagos** | Calcula deuda restante y meses para pagar |

---

## 🛠️ Stack Tecnológico

- **Entorno**: Google Colab
- **Lenguaje**: Python 3.12
- **Procesamiento PDF**: pdfplumber, pdf2image, pdfminer
- **OCR**: Tesseract + pytesseract
- **Base de datos**: SQLite + SQLAlchemy
- **Análisis de datos**: Pandas, NumPy
- **Visualización**: Matplotlib, Seaborn

---

## 🚀 Instalación y Uso

### En Google Colab

```python
# 1. Ejecutar celda de instalación de dependencias
# 2. Montar Google Drive para acceder a tus PDFs
from google.colab import drive
drive.mount('/content/drive')

# 3. Subir tus estados de cuenta a la carpeta /content/estados_cuenta/
# 4. Ejecutar las celdas de procesamiento
```

### Localmente

```bash
# Instalar dependencias del sistema
!apt-get update
!apt-get install -y poppler-utils tesseract-ocr tesseract-ocr-spa

# Instalar librerías Python
pip install pdfplumber pandas sqlalchemy pytesseract pdf2image pillow

# Ejecutar
python estados_cuenta.py
```

---

## 📁 Estructura del Proyecto

```
bank-statement-manager-colab/
├── Estados de cuenta.ipynb    # Notebook principal
├── README.md                  # Este archivo
└── estados_cuenta.db         # Base de datos SQLite (generado)
```

---

## 💡 Casos de Uso

1. **Contabilidad personal**: Registra todos tus gastos y ingresos automáticos
2. **Gestión empresarial**: Consolida estados de cuenta de múltiples cuentas
3. **Análisis de gastos**: Categoriza y visualiza tus patrones de gasto
4. **Control de deuda**: Sigue el progreso de pagos de préstamos
5. **Auditoría financiera**: Historial completo de transacciones

---

## 📊 Ejemplo de Análisis Generado

- Total de transacciones por mes
- Gastos por categoría
- Ingresos vs Gastos
- Promedio de transacciones diarias
- Saldo promedio
- Intereses generados

---

## ⚠️ Requisitos

- Cuenta de Google (para Colab) o Python 3.8+ local
- Estados de cuenta en formato PDF
- Al menos 500MB de espacio en disco

---

## 🤝 Contribuciones

¿Encontraste un bug? ¿Tienes sugerencias? 
¡Abre un issue en GitHub!

---

## 👨‍💻 Desarrollado por Isaac Esteban Haro Torres

**Ingeniero en Sistemas · Full Stack · Automatización · Data**

- 📧 Email: zackharo1@gmail.com
- 📱 WhatsApp: 098805517
- 💻 GitHub: https://github.com/ieharo1
- 🌐 Portafolio: https://ieharo1.github.io/portafolio-isaac.haro/

---

© 2026 Isaac Esteban Haro Torres - Todos los derechos reservados.
