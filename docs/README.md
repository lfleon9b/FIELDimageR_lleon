# Documentación FIELDimageR

## Índice General

Esta documentación proporciona una guía completa y práctica del paquete **FIELDimageR**, organizada desde los conceptos básicos hasta las técnicas más avanzadas.

---

## 📚 Contenido

### Parte 1: Fundamentos

- **[00. Introducción](00_introduccion.md)**2
  - ¿Qué es FIELDimageR?
  - Arquitectura del paquete
  - Conceptos clave
  - Flujo de trabajo general

- **[01. Instalación](01_instalacion.md)**
  - Requisitos del sistema
  - Instalación de dependencias
  - Instalación del paquete
  - Configuración inicial
  - Solución de problemas comunes

- **[02. Carga y Visualización](02_carga_visualizacion.md)**
  - Cargar mosaicos (RGB, multiespectral)
  - Funciones de visualización
  - Inspección de propiedades
  - Reducir resolución para análisis rápido

- **[03. Preprocesamiento](03_preprocesamiento.md)**
  - `fieldCrop`: Recortar imágenes
  - `fieldRotate`: Rotar y alinear
  - `fieldMask`: Remover suelo y fondo
  - Mejores prácticas de preprocesamiento

---

### Parte 2: Análisis de Parcelas

- **[04. Definición de Parcelas](04_parcelas.md)**
  - `fieldShape`: Crear shapefiles de parcelas
  - `fieldMap`: Mapear identificadores
  - Integrar datos experimentales
  - Parcelas de diferentes dimensiones

- **[05. Índices de Vegetación](05_indices_vegetacion.md)**
  - `fieldIndex`: Calcular índices
  - Índices RGB (NGRDI, BGI, VARI, etc.)
  - Índices multiespectrales (NDVI, NDRE, EVI)
  - Crear índices personalizados
  - Catálogo completo de índices

- **[06. Extracción de Datos](06_extraccion_datos.md)**
  - `fieldInfo`: Extraer valores por parcela
  - Estadísticos (media, mediana, cuantiles)
  - Múltiples bandas/índices
  - Exportar resultados

---

### Parte 3: Análisis Específicos

- **[07. Conteo de Objetos](07_conteo_objetos.md)**
  - `fieldCount`: Contar plantas
  - Conteo de semillas y polen
  - `fieldObject`: Análisis de objetos individuales
  - Filtrado por tamaño y forma
  - Validación de conteos

- **[08. Área y Cobertura](08_area_cobertura.md)**
  - `fieldArea`: Calcular porcentaje de dosel
  - Áreas de daño o enfermedad
  - Cobertura temporal
  - Interpretación de resultados

- **[09. Altura de Plantas](09_altura_plantas.md)**
  - `fieldHeight`: Modelo de altura (CHM)
  - Modelo de volumen (CVM - biomasa digital)
  - Trabajar con DSM (Digital Surface Model)
  - Interpolación de superficie base
  - Estimación de biomasa

- **[10. Mediciones y Distancias](10_mediciones_distancias.md)**
  - `fieldDraw`: Dibujar líneas y polígonos manualmente
  - Medir distancias entre plantas
  - `fieldPolygon`: Polígonos personalizados
  - Análisis de distribución espacial

---

### Parte 4: Análisis Avanzados

- **[11. Imágenes Multiespectrales e Hiperespectrales](11_multiespectral.md)**
  - Trabajar con múltiples bandas espectrales
  - Análisis hiperespectral (474+ bandas)
  - Firmas espectrales
  - Aplicaciones en fenotipado

- **[12. Análisis Temporal](12_analisis_temporal.md)**
  - Ciclo de crecimiento del cultivo
  - Reutilizar shapefoles entre fechas
  - Análisis de series temporales
  - `fieldAUC`: Área bajo la curva

- **[13. Casos Avanzados](13_casos_avanzados.md)**
  - Procesamiento paralelo
  - Análisis de múltiples imágenes (loop y parallel)
  - Automatización de pipelines
  - Optimización de memoria y rendimiento
  - Integración con OpenDroneMap

---

### Parte 5: Referencia

- **[14. Funciones de Referencia](14_funciones_referencia.md)**
  - Catálogo completo de funciones
  - Parámetros detallados
  - Valores de retorno
  - Ejemplos mínimos
  - Troubleshooting

---

## 🎯 Flujo de Trabajo Típico

```
1. Cargar imagen → 2. Recortar → 3. Rotar → 4. Remover suelo 
   ↓
5. Definir parcelas → 6. Calcular índices → 7. Extraer datos
   ↓
8. Análisis específicos (conteo, área, altura) → 9. Exportar resultados
```

---

## 🚀 Inicio Rápido

Si es tu primera vez con FIELDimageR, te recomendamos seguir este orden:

1. Lee la [Introducción](00_introduccion.md) para entender los conceptos
2. Sigue la guía de [Instalación](01_instalacion.md)
3. Practica con [Carga y Visualización](02_carga_visualizacion.md)
4. Domina el [Preprocesamiento](03_preprocesamiento.md)
5. Aprende a crear [Parcelas](04_parcelas.md)
6. Explora [Índices de Vegetación](05_indices_vegetacion.md)
7. Extrae tus primeros datos con [Extracción de Datos](06_extraccion_datos.md)

---

## 📖 Convenciones de esta Documentación

- **Código de ejemplo**: Todos los ejemplos son ejecutables
- **⚠️ Advertencias**: Aspectos importantes a tener en cuenta
- **💡 Consejos**: Mejores prácticas y trucos útiles
- **🔗 Referencias**: Enlaces a otras secciones relacionadas

---

## 🤝 Contribución

Esta documentación está en constante desarrollo. Si encuentras errores o quieres contribuir, por favor:

1. Reporta issues en el repositorio
2. Sugiere mejoras
3. Comparte casos de uso

---

## 📄 Licencia

Este paquete y documentación se distribuyen bajo licencia GPL-2.

---

## 📚 Recursos Adicionales

- **Repositorio oficial**: [OpenDroneMap/FIELDimageR](https://github.com/OpenDroneMap/FIELDimageR)
- **Artículo científico**: [The Plant Phenome Journal](https://doi.org/10.1002/ppj2.20005)
- **Foro de usuarios**: [Google Groups](https://groups.google.com/forum/#!forum/fieldimager)
- **Videos tutoriales**: Ver README principal del repositorio

---

**Última actualización**: Diciembre 2025

