# ProbabilityStatistics
Space for activities carried out in the subject of Probability and Statistics taught by M.C. Christian Ríos Chavarría, professor of the Software Engineering Academy at the "Universidad Politécnica de Durango".

![COLAB icon](https://registry.npmmirror.com/@lobehub/icons-static-png/latest/files/dark/colab-color.png)
## ESTADÍSTICA DESCRIPTIVA & VISUALIZACIÓN DE DATOS
<table>
<tr>
<td>
 Para obtener información sobre la inversión en investigación y desarrollo tecnológico en Durango, utilizamos las siguientes fuentes del <strong>INEGI</strong>:

<strong>Investigación, desarrollo tecnológico e innovación:</strong> Proporciona datos sobre recursos humanos y financieros destinados a actividades de investigación y desarrollo tecnológico en el sector productivo. 

<strong>Encuesta Sobre Investigación y Desarrollo Tecnológico 2017:</strong> Ofrece información detallada sobre la inversión en investigación y desarrollo tecnológico en México, incluyendo datos por entidad federativa. 

</td>
</tr>
</table>


## 2.- ANÁLISIS DESCRIPTIVO
Una vez recopilados los datos, procedemos a calcular las principales medidas estadísticas utilizando Python y las bibliotecas Pandas, Matplotlib y Seaborn.

#### Python code:
```
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Crear un DataFrame manualmente con datos simulados
data = {
    'Sector': ['Educación', 'Salud', 'Industria', 'Transporte', 'Otros'],
    'Año': [2020, 2021, 2022, 2023, 2024],
    'Inversion': [1200000, 1500000, 1800000, 2000000, 2200000]  
# Monto en miles de pesos
}

df = pd.DataFrame(data)

# Mostrar el DataFrame creado
print("Datos cargados:\n", df)

# Calcular medidas de tendencia central y dispersión
media = df['Inversion'].mean()
mediana = df['Inversion'].median()
moda = df['Inversion'].mode()[0]
varianza = df['Inversion'].var()
desviacion_estandar = df['Inversion'].std()

print(f"\nAnálisis descriptivo:")
print(f"Media: {media}")
print(f"Mediana: {mediana}")
print(f"Moda: {moda}")
print(f"Varianza: {varianza}")
print(f"Desviación Estándar: {desviacion_estandar}")
```

![image](https://github.com/user-attachments/assets/4826f50d-5a2d-48e3-801c-950e6dfacfb3)

<hr>

## 3.- VISUALIZACIÓN

Procedemos a crear las visualizaciones para representar las distribuciones y características del conjunto de datos.
<table>
  <tr>
    <td>
      Estos gráficos nos permiten visualizar la distribución de las inversiones, identificar posibles valores atípicos y comparar la inversión entre diferentes sectores.
    </td>
  </tr>
</table>

```
# Configurar el estilo de los gráficos
sns.set(style="whitegrid")

# Histograma
plt.figure(figsize=(10, 6))
sns.histplot(df['Inversion'], bins=20, kde=True)
plt.title('Distribución de la Inversión en Tecnología en Durango')
plt.xlabel('Monto de Inversión')
plt.ylabel('Frecuencia')
plt.show()

# Diagrama de caja (boxplot)
plt.figure(figsize=(8, 4))
sns.boxplot(x=df['Inversion'])
plt.title('Diagrama de Caja de la Inversión en Tecnología en Durango')
plt.xlabel('Monto de Inversión')
plt.show()

# Gráfico de barras por sector (si se dispone de esta información)
plt.figure(figsize=(12, 6))
sns.barplot(x='Sector', y='Inversion', data=df, estimator=sum, ci=None)
plt.title('Inversión Total en Tecnología por Sector en Durango')
plt.xlabel('Sector')
plt.ylabel('Inversión Total')
plt.xticks(rotation=45)
plt.show()
```

### Histograma
![Imagen de WhatsApp 2025-01-23 a las 13 47 45_38a4f0db](https://github.com/user-attachments/assets/e4f9aabf-e640-445d-9684-bcaf0d7aba35)

### Caja
![Imagen de WhatsApp 2025-01-23 a las 13 48 06_caa5f019](https://github.com/user-attachments/assets/f90212d4-874a-4ace-9a9d-960b3bfdfb5c)

### Barras
![Imagen de WhatsApp 2025-01-23 a las 13 48 23_e5271cb2](https://github.com/user-attachments/assets/be2c6606-f78d-4ac9-a5c3-064fb6486117)

<hr>

## 4.- INTERPRETACIÓN
Con base en los resultados obtenidos podemos concluir lo siguiente:


### Medidas de tendencia central y dispersión:
* La media y la mediana nos indican el promedio y el punto medio de las inversiones, respectivamente.
* La moda muestra el monto de inversión más frecuente. 
* La varianza y la desviación estándar nos indican la dispersión de los datos, es decir, cuánto varían las inversiones respecto a la media.


### Gráficos:
* El histograma muestra cómo se distribuyen los montos de inversión, permitiendo identificar si hay sesgos o concentraciones en ciertos rangos.
* El diagrama de caja ayuda a detectar valores atípicos y visualizar la dispersión de los datos.
* El gráfico de barras por sector permite comparar la inversión total entre diferentes sectores, identificando cuáles reciben más o menos inversión.


Finalmente, estas interpretaciones nos permiten sacar conclusiones sobre el comportamiento de la inversión en avances tecnológicos en Durango, identificando tendencias, posibles áreas de mejora y sectores prioritarios para futuras inversiones.

Este análisis proporciona una visión clara y concisa de la inversión en tecnología en Durango.

<hr>

# Team

<table>
 <tr>
  <td>
    <img src="https://github.com/user-attachments/assets/49f24da2-18b5-4eff-9a5d-dc266d362052" alt="FotoDeIvan" width="300" height="300">   
  </td>
  <td>
   <img src="https://github.com/user-attachments/assets/db390ce9-c030-4fe0-8177-c80e5464f148" alt="FotoMia" width="300" height="300">
  </td>
  <td>
   <img src="https://github.com/user-attachments/assets/709f2fb3-fc24-45b9-9b2d-1625b73a19c7" alt="FotoMia" width="300" height="300">
  </td>
 </tr>
 <tr>
  <td>IVAN A RAMOS GONZALEZ</td>
  <td>EHECATL E REYES NAJERA</td>
  <td>LUIS A SIMENTAL OCHOA</td>
 </tr>
</table>
