# 📈 MowZone Strategy

## Descripción
Esta es una estrategia de trading automatizada desarrollada en Pine Script v6 para la plataforma TradingView. La estrategia combina el indicador **SuperTrend**, el **ATR (Average True Range)** y la **fuerza absoluta del mercado** para generar señales de compra y venta. Además, incorpora reglas de gestión de riesgo mediante **Stop Loss (SL)** y **Take Profit (TP)** dinámicos.

## 📌 Características
- **Detección automática de tendencias** con SuperTrend y ATR.
- **Órdenes de entrada Long y Short** basadas en cruces de precios con niveles dinámicos.
- **Gestión de riesgo avanzada** con cálculos automáticos de Stop Loss y Take Profit.
- **Backtesting optimizado**, permitiendo evaluar el rendimiento en diferentes períodos de tiempo.
- **Tablas de estadísticas** para analizar resultados de operaciones ganadoras, perdedoras, porcentaje de aciertos y PnL neto.

## ⚙️ Parámetros
- `profitTargetMultiplier`: Multiplicador del ATR para calcular el Take Profit.
- `stopLossMultiplier`: Multiplicador del ATR para calcular el Stop Loss.
- `superTrendFactor`: Factor de SuperTrend para determinar la tendencia del mercado.
- `backtestPeriodStart` / `backtestPeriodEnd`: Fechas para ejecutar pruebas retrospectivas.

## 📊 Reglas de Trading
### ✅ Entrada en Long
1. Se detecta un cruce alcista sobre el nivel de soporte.
2. El color de la tendencia debe indicar un mercado alcista.
3. Se confirma la vela actual.
4. Se establece el SL y TP en función del ATR.

### ❌ Entrada en Short
1. Se detecta un cruce bajista bajo el nivel de resistencia.
2. El color de la tendencia debe indicar un mercado bajista.
3. Se confirma la vela actual.
4. Se establece el SL y TP en función del ATR.

### 📉 Salida de operaciones
- **Take Profit alcanzado**: Se cierra la operación al llegar al nivel de TP.
- **Stop Loss alcanzado**: Se cierra la operación para minimizar pérdidas.

## 📊 Estadísticas en TradingView
La estrategia incluye una tabla que muestra:
- Número total de operaciones ganadoras y perdedoras.
- Porcentaje de éxito (% de operaciones ganadoras sobre el total).
- Beneficio neto acumulado.
- Promedio de ganancias y pérdidas por operación.

## 🚀 Instalación y Uso
1. Copiar el código Pine Script en TradingView.
2. Crear un nuevo indicador y pegar el código.
3. Ajustar parámetros según preferencias.
4. Aplicar al gráfico y analizar resultados.

## 📜 Licencia
Este código es de uso libre bajo la licencia MIT. Si lo usas o modificas, se agradece el reconocimiento al autor.

---
_⚠️ **Nota:** Esta estrategia es solo para fines educativos y de investigación. No garantiza rentabilidad y no debe considerarse asesoramiento financiero._

