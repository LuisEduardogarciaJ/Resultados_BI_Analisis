#  Análisis de Business Intelligence - Cartera de Crédito

Este repositorio contiene los resultados del análisis de BI sobre la evolución de la cartera de crédito, riesgo, cobranza y desempeño por sucursal.

##  Estructura del archivo Excel

El archivo `Resultados_BI_Analisis.xlsx` contiene las siguientes pestañas:

### 1. `Crecimiento`
- **Descripción:** Evolución mensual del capital otorgado y número de créditos.
- **Variables:**
  - `Month_Year_Orig`: Fecha de originación
  - `Capital`: Monto total otorgado
  - `Num_Creditos`: Cantidad de créditos

### 2. `Vintage_Riesgo`
- **Descripción:** Análisis vintage con saldos y morosidad a 90 días.
- **Variables:**
  - `Month_Year_Orig`: Fecha de originación
  - `Capital`, `Saldo`, `Saldo_Vencido_90`, `Bad_Rate_90`

### 3. `Cobranza`
- **Descripción:** Montos pagados por mes.
- **Variables:**
  - `Month_Year_Pago`: Fecha de pago
  - `monto_pagado`: Total pagado en el mes

### 4. `Sucursales`
- **Descripción:** Indicadores por sucursal: atraso, saldo, solicitudes y pobreza.
- **Variables:**
  - `Clave_Sucursal`, `Dias_De_Atraso`, `Saldo`, `Solicitud`, `Extrema Pobreza (E)`

### 5. `Estadisticas`
- **Descripción:** Pruebas estadísticas clave.
- **Variables:**
  - `T-Stat Cycle`, `P-Value Cycle`, `Mean Delay New`, `Mean Delay Recurring`, `Correlation Capacity`, `P-Value Capacity`

### 6. `Riesgo_Global`
- **Descripción:** Tasas de cartera vencida.
- **Variables:**
  - `PAR30 Rate`, `PAR90 Rate`

##  Principales hallazgos
- Crecimiento sostenido en capital y número de créditos hasta 2022, con caídas en 2023 y recuperación parcial en 2024-2025.
- Alta correlación entre originación y morosidad en ciertos periodos.
- Diferencias significativas en atraso promedio entre sucursales.
- Indicadores de riesgo global (PAR30 y PAR90) superiores al 79%.

##  Uso
Este análisis puede ser utilizado para:
- Evaluar tendencias de crecimiento
- Identificar sucursales con mayor riesgo
- Analizar estacionalidad en cobranza
- Modelar pérdidas esperadas
