# promedio

## Calcular promedio
 - Importar las librerías necesarias.
 - Crear un DataFrame (o cargar uno existente).
 - Calcular el promedio de la columna deseada.
 - Visualizarlo usando Seaborn.

### codigo 

~~~
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Crear un DataFrame
data = {
    'Valores': [10, 20, 30, 40, 50]
}
df = pd.DataFrame(data)

# Calcular el promedio
promedio = df['Valores'].mean()
print("El promedio es:", promedio)

# Visualizar usando Seaborn
sns.set(style="whitegrid")
plt.figure(figsize=(6, 4))
sns.barplot(x=df['Valores'].index, y=df['Valores'], palette='viridis')  # Use index for x-axis
plt.title('Promedio de la columna "Valores"')
plt.ylabel('Valores')
plt.ylim(0, 60)
plt.show()
~~~
- ### El promedio es: 30.0


![image](https://github.com/user-attachments/assets/65e67d9d-e690-4df6-89bb-85fa89b14e90)

