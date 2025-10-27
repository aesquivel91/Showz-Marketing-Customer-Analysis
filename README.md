# 🎟️ Showz Marketing & Customer Analysis

## 📋 Descripción del Proyecto
Showz es una empresa de **venta de entradas para eventos** que busca **optimizar sus gastos de marketing** y comprender mejor el comportamiento de sus clientes.  

Este análisis abarca datos de **visitas, pedidos y costos de marketing** desde **enero de 2017 hasta diciembre de 2018**, con el propósito de medir la **eficiencia de adquisición de clientes**, el **valor que generan** y el **momento en que la inversión se recupera (payback period)**.

---

## 🎯 Objetivos
1. Analizar cómo los usuarios interactúan con el servicio (DAU, WAU, MAU).  
2. Identificar **cuándo los clientes comienzan a comprar** y su tiempo promedio de conversión.  
3. Calcular el **LTV (Lifetime Value)** y entender cuánto aporta cada cliente.  
4. Determinar **cuándo los ingresos cubren los costos de adquisición** mediante cohortes y métricas de marketing.  

---

## 📚 Fuentes de Datos
El proyecto utiliza tres archivos principales:

| Archivo | Descripción |
|:--|:--|
| `visits_log.csv` | Registros de visitas al sitio web (usuario, fuente, timestamp). |
| `orders_log.csv` | Datos de pedidos con monto, fecha y usuario. |
| `costs.csv` | Estadísticas de gasto en marketing por fuente y mes. |

---

## 🧩 Estructura del Proyecto
```
showz-marketing-analysis/
│
├── data/
│   ├── visits_log.csv       # Datos de visitas
│   ├── orders_log.csv       # Datos de pedidos
│   └── costs.csv            # Gastos de marketing
│
├── notebooks/
│   └── showz.ipynb          # Notebook principal de análisis
│
├── README.md                # Descripción del proyecto
└── images/                  # Visualizaciones y gráficos
```

---

## 🔍 Metodología del Análisis

### 1️⃣ Exploración de usuarios y comportamiento
- **DAU / WAU / MAU** → usuarios activos por día, semana y mes.  
- **Sesiones por día** → actividad general del sitio.  
- **Duración promedio de sesiones** → indicador de engagement.  
- **Frecuencia de retorno** → número promedio de visitas por usuario.

---

### 2️⃣ Análisis de ventas y conversión
- **Tiempo hasta la primera compra** → días desde la primera visita hasta el primer pedido.  
- **Frecuencia de compra** → promedio de pedidos por cliente.  
- **Tamaño promedio por compra (AOV)** → ticket promedio mensual.  
- **LTV (Lifetime Value)** → ingresos acumulados generados por usuario o cohorte.

---

### 3️⃣ Análisis de rentabilidad
- **CAC (Customer Acquisition Cost)** → gasto medio por fuente dividido entre nuevos clientes.  
- **ROI (Return on Investment)** → comparación entre LTV y CAC.  
- **Payback Period** → tiempo en el que los ingresos igualan el costo de adquisición.  

El análisis se realiza por **cohortes mensuales**, lo que permite identificar qué grupos de clientes son más rentables y en qué momento alcanzan el equilibrio.

---

## 📈 Principales Resultados

- Los **usuarios comienzan a comprar en promedio pocos días después de la primera visita**, lo que indica un funnel de conversión ágil.  
- La **mayoría de las conversiones** proviene de unas pocas **fuentes de tráfico altamente efectivas**, mientras que otras generan tráfico sin conversión.  
- El **LTV aumenta gradualmente** con el tiempo, reflejando una base de clientes fiel y recurrente.  
- En la mayoría de los cohortes, el **punto de recuperación de CAC** se alcanza dentro de los primeros **4 a 6 meses**.  
- Las fuentes con mejor relación **LTV/CAC > 1** son las más sostenibles a largo plazo.

---

## 🧠 Conclusiones
- Los usuarios activos muestran una tendencia estable, con **incremento de sesiones en eventos estacionales**.  
- Las campañas con menor CAC y mayor conversión deben recibir **prioridad presupuestal**.  
- Las cohortes recientes muestran **mejor retención** y menor tiempo de recuperación de inversión.  
- Se recomienda implementar un **sistema de monitoreo continuo** de LTV, CAC y ROI por canal de adquisición.

---

## ⚙️ Tecnologías Utilizadas
- **Python:** pandas, numpy, matplotlib, seaborn, datetime  
- **Entorno:** Jupyter Notebook  
- **Análisis de Cohortes:** cálculos de LTV, CAC y ROI  
- **Visualización:** gráficos de tendencia, heatmaps y embudos de conversión  

---

## 🚀 Cómo Ejecutar el Proyecto

### 1️⃣ Crear y activar un entorno virtual
```bash
python -m venv showz_env
source showz_env/bin/activate      # macOS/Linux
showz_env\Scripts\activate       # Windows
```

### 2️⃣ Instalar dependencias
```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 3️⃣ Ejecutar el notebook
```bash
jupyter notebook notebooks/showz.ipynb
```

---

## 👤 Autor
**Andrés Esquivel Díaz**  
📍 *Data Analyst | Python · SQL · Tableau · Power BI*  
🔗 [LinkedIn](https://www.linkedin.com/in/andres-esquivel-diaz-08691337) · [GitHub](https://github.com/aesquivel91)
