Análisis de Datos Retail - Proyecto GitHub
Descripción del Proyecto
Este proyecto realiza un análisis completo de datos de ventas minoristas, incluyendo:

Cálculo de ingresos por tienda

Análisis de costos de envío

Evaluación de satisfacción del cliente

Distribución de ventas por categoría

🛠 Tecnologías Utilizadas
Python 3.8+

Pandas (manipulación de datos)

Matplotlib (visualización básica)

Seaborn (visualización avanzada)

📁 Estructura del Código
1. Carga de Datos
python
import pandas as pd

# Datos de ejemplo (pueden reemplazarse con carga desde CSV)
data = {
    'Producto': ['Asistente virtual', 'Mesa de comedor', ...],
    'Categoría': ['Electrónicos', 'Muebles', ...],
    'Precio': [164300.0, 192300.0, ...],
    # ... (otros campos)
}

df = pd.DataFrame(data)


2. Análisis Financiero
python
# Ingresos por tienda
ingresos_tienda = df.groupby('Lugar de Compra')['Precio'].sum()
                   .sort_values(ascending=False)
                   .reset_index()

                   
3. Análisis Logístico
python
# Costos de envío promedio
costos_envio = df.groupby('Lugar de Compra')['Costo de envío'].mean()
                .round(2)
                .sort_values(ascending=False)

                
4. Satisfacción del Cliente
python
# Calificaciones promedio
calificaciones = df.groupby('Lugar de Compra')['Calificación'].mean()
                  .sort_values(ascending=False)
                  .round(2)

                  
📊 Visualización de Datos
Gráfico de Barras (Ingresos)
python
plt.bar(ingresos_tienda['Lugar de Compra'], ingresos_tienda['Precio'])
plt.title('Ingresos por Tienda')
plt.xticks(rotation=45)
plt.show()
Diagrama de Tallo (Calificaciones)
python
plt.stem(calificaciones.index, calificaciones.values,
        linefmt='C0-', markerfmt='C0o')
plt.title('Calificaciones por Tienda')
plt.ylim(0, 5)
plt.show()
