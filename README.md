# 📊 Análisis Estratégico de Tiendas Retail - Recomendación Comercial

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-1.3%2B-orange)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.4%2B-green)

## 📌 Objetivo del Proyecto
Análisis comparativo de cuatro tiendas retail (Bogotá, Cali, Medellín y Cartagena) para determinar la ubicación óptima que maximice las ventas del Sr. Juan, evaluando:

- Desempeño comercial
- Satisfacción del cliente
- Eficiencia logística
- Mix de productos

## 🔍 Hallazgos Clave

### 📈 Rendimiento Comercial
| Tienda    | Ventas Totales | % Participación | Costo Envío Promedio |
|-----------|----------------|-----------------|----------------------|
| Medellín  | $52M           | 35%             | $18,300              |
| Bogotá    | $45M           | 30%             | $12,500              |
| Cali      | $38M           | 25%             | $15,200              |
| Cartagena | $15M           | 10%             | $22,100              |

### ⭐ Satisfacción del Cliente
![Calificaciones](https://i.imgur.com/calificaciones.png)

### 🏷️ Mix de Productos
```python
# Distribución por categoría
categorias = {
    'Electrónicos': 45%,  # Bogotá y Cali
    'Muebles': 30%,      # Medellín
    'Juguetes': 15%      # Cartagena
}
