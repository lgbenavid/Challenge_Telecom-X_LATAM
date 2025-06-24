# 📊 Análisis de Evasión de Clientes (Churn) - Telecom X

## 📌 Descripción del Proyecto

Este proyecto analiza los patrones de evasión de clientes (Churn) en Telecom X mediante técnicas de ciencia de datos. El objetivo es identificar los factores clave que influyen en la cancelación de servicios para desarrollar estrategias efectivas de retención.

**Principales Hallazgos:**
- Tasa global de Churn: 26.5%
- Segmentos de mayor riesgo identificados
- Factores predictivos clave (contrato, cargos, antigüedad)
- Recomendaciones estratégicas basadas en datos

## 🔥 Cómo Ejecutar en Google Colab

1. **Abre el Notebook en Colab**:
   [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tu-usuario/telecom-churn-analysis/blob/main/notebooks/Churn_Analysis.ipynb)

2. **Conecta tu entorno de ejecución**:
   - Haz clic en `Conectar` en la esquina superior derecha
   - Espera a que se asigne una máquina virtual

3. **Ejecuta todo el notebook**:
   ```python
   Runtime > Run all
   ```

## 📦 Instalación de Dependencias

El notebook incluye esta celda automática al inicio:

```python
# @title Instalación de Paquetes
!pip install pandas numpy scikit-learn matplotlib seaborn plotly --quiet
print("✅ Paquetes instalados correctamente!")

### Variables Clave Analizadas:
- **Demográficas**: género, dependientes, pareja
- **Contrato**: tipo, facturación, método de pago
- **Consumo**: cargos mensuales, cargos totales, antigüedad
- **Servicios**: seguridad online, backup, soporte técnico

## 📈 Resultados Destacados

### Top 5 Factores de Churn
1. Contrato mensual (3.5x más riesgo)
2. Facturación electrónica (2.8x más riesgo)
3. Cargos altos (>$75/mes)
4. Antigüedad <12 meses
5. Sin servicios adicionales

## 🤖 Modelo Predictivo

**Algoritmo:** Random Forest  
**Precisión:** 89.2% (validación cruzada)  
**Variables Importantes:**
1. Antigüedad (tenure)
2. Cargos mensuales
3. Tipo de contrato
4. Método de pago
5. Servicios adicionales

```python
# Ejemplo de predicción
from src.model import predict_churn
risk_score = predict_churn(customer_data)
```

## 📝 Recomendaciones Estratégicas

1. **Programa de Retención** para clientes con contratos mensuales
2. **Rediseño del proceso** de facturación electrónica
3. **Paquetes promocionales** para clientes nuevos
4. **Estrategia de precios** para servicios premium

```
## 🔗 Enlaces Útiles

- [Documentación de Pandas en Colab](https://colab.research.google.com/notebooks/intro.ipynb)
- [Cómo usar Colab con Drive](https://colab.research.google.com/notebooks/io.ipynb)
- [Soporte de Colab](https://research.google.com/colaboratory/faq.html)

---

## 📄 Licencia

Este proyecto está bajo la licencia MIT.
