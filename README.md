# Simulación de Arquitecturas Lambda y Kappa para Procesamiento de Datos

## Introducción

Este proyecto presenta una simulación práctica de las arquitecturas de procesamiento de datos **Lambda** y **Kappa** utilizando Python, Pandas y Jupyter Lab.

Ambas arquitecturas se emplean en sistemas que requieren procesar grandes volúmenes de información, especialmente cuando los datos son generados de forma continua. Aunque fueron desarrolladas para entornos distribuidos y sistemas de Big Data, es posible representar sus principios fundamentales mediante conjuntos de datos estáticos tratados como flujos de eventos.

### Arquitectura Lambda

La arquitectura Lambda divide el procesamiento en dos capas principales:

- **Batch Layer**: procesa el conjunto histórico completo para obtener conocimiento acumulado, estadísticas y patrones de comportamiento.
- **Speed Layer**: procesa nuevos eventos conforme llegan al sistema, permitiendo detectar anomalías o generar alertas en tiempo real.

La combinación de ambas capas proporciona una visión tanto histórica como inmediata del sistema analizado.

### Arquitectura Kappa

La arquitectura Kappa simplifica el modelo eliminando la capa Batch.

Todos los datos son tratados como un flujo continuo de eventos, y las métricas se construyen dinámicamente a medida que nuevos registros ingresan al sistema.

Su principal característica es que todo el procesamiento ocurre sobre el flujo de datos, sin depender de análisis históricos previamente calculados.

### Objetivo del Proyecto

Implementar simulaciones de ambas arquitecturas mediante:

- Procesamiento histórico de datos.
- Generación de métricas descriptivas.
- Actualización dinámica de indicadores.
- Simulación de eventos en flujo.
- Detección de alertas y condiciones relevantes.

Los datasets utilizados representan distintos escenarios de análisis y permiten observar las diferencias conceptuales entre ambas arquitecturas.

---

## Requisitos

- Python 3.10 o superior
- Jupyter Lab
- Dependencias incluidas en `requirements.txt`

---

## Instalación

### 1. Clonar el repositorio

```bash
git clone <URL_DEL_REPOSITORIO>
```

Entrar al directorio:

```bash
cd <NOMBRE_DEL_REPOSITORIO>
```

---

### 2. Crear y activar el entorno virtual

#### Windows

```bash
python -m venv .venv
```

Activar:

```bash
.venv\Scripts\activate
```

#### Linux

```bash
python3 -m venv .venv
```

Activar:

```bash
source .venv/bin/activate
```

---

### 3. Instalar dependencias

```bash
pip install -r requirements.txt
```

---

### 4. Abrir Jupyter Lab

```bash
jupyter lab
```

Esto abrirá la interfaz web de Jupyter Lab en el navegador.

---

## Ejecución del Proyecto

Los notebooks fueron diseñados para ejecutarse desde Jupyter Lab.

### Importante

No se recomienda ejecutar los archivos directamente desde terminal mediante:

```bash
python archivo.py
```

ni abrir los notebooks fuera de Jupyter Lab.

Para una ejecución correcta:

1. Abrir Jupyter Lab.
2. Navegar hasta el notebook deseado.
3. Abrir el archivo `.ipynb`.
4. Ejecutar las celdas en orden desde el inicio.

---

## Estructura General

```text
Proyecto/
│
├── data/
│   ├── Hospital/
│   ├── Universidad/
│   └── Ciudades/
│
├── lambda/
│   ├── Hospital_Lambda.ipynb
│   ├── Universidad_Lambda.ipynb
│   └── Ciudades_Lambda.ipynb
│
├── kappa/
│   ├── Hospital_Kappa.ipynb
│   ├── Universidad_Kappa.ipynb
│   └── Ciudades_Kappa.ipynb
│
├── requirements.txt
│
└── README.md
```

---

## Tecnologías Utilizadas

- Python
- Pandas
- Jupyter Lab
- Git
- GitHub

---

## Autoría:

Zea García Danae (investigación de arquitectura Kappa)

Hernández Huerta Ari Leonardo (Implementación de código)

Carmona Capula Andrés Tadeo (Investigación de arquitectura Lambda)

Ayala Carrasco Said Giuliano (Investigación de arquitectura Lambda)