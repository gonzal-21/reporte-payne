# Dashboard Torres del Paine

Sistema de análisis y visualización de datos turísticos para guías del Parque Nacional Torres del Paine.

## 📊 Características

### Dashboard Principal
- **Métricas clave**: Total de turistas (446), Ingresos ($38.5M CLP), Pasos promedio (35,863), Nacionalidades (9)
- **Visualizaciones interactivas**:
  - Gráfico de barras: turistas por país
  - Línea de tiempo: actividad diaria de pasos
  - Distribución de alojamientos
  - Ingresos por fecha

### Secciones Especializadas

#### 1. Análisis de Tours
- Comparación de tres tipos de tours:
  - **Base Torres**: 225 turistas - $95,000 CLP
  - **Miradores Payne**: 156 turistas - $75,000 CLP
  - **City Tour**: 65 turistas - $65,000 CLP

#### 2. Reporte Médico
- Contactos de emergencia
- Protocolo de emergencias paso a paso
- Métricas de salud (pasos y distancia diaria)
- Inventario de botiquín

#### 3. Inventario de Equipamiento
- Lista completa de equipamiento de montaña
- Estados: Disponible, En uso, En mantención
- Fechas de última revisión

#### 4. Sistema de Reservas
- Tabla completa de reservas
- Filtros por estado (Disponible, Confirmado, Pendiente)
- Información de guía, país, tour y fecha

#### 5. Plantilla Cornell
- Sistema de notas estructuradas:
  - Título de la nota
  - Conceptos clave (lateral izquierdo)
  - Apuntes principales (área grande)
  - Resumen y comentarios (inferior)
- Funciones: Guardar localmente, Exportar JSON, Limpiar

## 🚀 Instalación y Uso

### Uso Local
1. Clonar el repositorio:
```bash
git clone https://github.com/gonzal-21/reporte-payne.git
cd reporte-payne
```

2. Abrir con servidor HTTP local:
```bash
python3 -m http.server 8000
# O con Python 2:
python -m SimpleHTTPServer 8000
```

3. Abrir navegador en: `http://localhost:8000`

### Estructura de Archivos
```
reporte-payne/
├── index.html          # Dashboard principal
├── form.html          # Formulario de reportes
├── data/              # Datos CSV
│   ├── turismo - salud.csv
│   ├── turismo - servicioxpais.csv
│   ├── turismo - hostalxpais.csv
│   ├── turismo - fechaxpais.csv
│   └── turismo - base-baset.csv
└── README.md
```

## 📱 Características Técnicas

### Diseño Responsive
- Adaptable a móviles, tablets y escritorio
- Grid flexible que se ajusta al tamaño de pantalla
- Navegación optimizada para pantallas pequeñas

### Funcionalidad Offline
- Todos los estilos embebidos (sin dependencias externas)
- Almacenamiento local para notas Cornell
- Detección de estado online/offline

### Visualizaciones
- Gráficos de barras personalizados con CSS
- Gráficos de línea interactivos
- Hover tooltips para información adicional
- Animaciones suaves

## 🎨 Tecnologías Utilizadas

- **HTML5**: Estructura semántica
- **CSS3**: Estilos modernos con gradientes y animaciones
- **JavaScript ES6+**: Lógica de aplicación
- **LocalStorage API**: Persistencia de notas
- **Fetch API**: Carga de datos CSV
- **No dependencias externas**: 100% autónomo

## 📊 Datos de Ejemplo

El dashboard incluye datos de ejemplo de la temporada 2024:
- 10 días de actividad registrada
- 9 países representados
- 3 tipos de tours diferentes
- 9 alojamientos registrados
- 10 reservas de ejemplo

## 🔧 Personalización

### Agregar Nuevos Datos
1. Editar archivos CSV en la carpeta `data/`
2. Mantener el formato de columnas existente
3. Recargar el dashboard

### Modificar Visualizaciones
Los gráficos se generan dinámicamente desde los datos CSV. Para personalizarlos:
- Editar funciones `createBarChart()` y `createLineChart()` en `index.html`
- Modificar colores en las secciones de estilos CSS

## 📞 Contactos de Emergencia

- **Emergencias**: 131
- **Ambulancia**: (61) 241 1888
- **Carabineros**: (61) 241 1262
- **SAR (Búsqueda y Rescate)**: +56 9 9999 9999

## 🎯 Uso Recomendado

1. **Antes del tour**: Revisar inventario de equipamiento
2. **Durante el tour**: Usar plantilla Cornell para tomar notas
3. **Después del tour**: Completar formulario de reporte
4. **Análisis**: Revisar dashboard para tendencias

## 📄 Licencia

Proyecto para uso interno de guías turísticos en Torres del Paine.

## 🤝 Contribuir

Para reportar problemas o sugerir mejoras, crear un issue en el repositorio.

---

Desarrollado para facilitar la gestión y análisis de servicios turísticos en Torres del Paine 🏔️
