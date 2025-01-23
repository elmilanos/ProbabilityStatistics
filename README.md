# ProbabilityStatistics
Space for activities carried out in the subject of Probability and Statistics taught by M.C. Christian Ríos Chavarría, professor of the Software Engineering Academy at the "Universidad Politécnica de Durango".

# ![COLAB WORK](https://registry.npmmirror.com/@lobehub/icons-static-png/latest/files/dark/colab-color.png)
# ESTADÍSTICA DESCRIPTIVA & VISUALIZACIÓN DE DATOS
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
![](https://iharsh234.github.io/WebApp/images/demo/web_app_face.JPG)

### Query Filled Form
![](https://iharsh234.github.io/WebApp/images/demo/demo_query.JPG)

### Charts
![](https://iharsh234.github.io/WebApp/images/demo/demo_chart1.JPG)
![](https://iharsh234.github.io/WebApp/images/demo/demo_chart2.JPG)
![](https://iharsh234.github.io/WebApp/images/demo/demo_chart3.JPG)


## Mobile support
The WebApp is compatible with devices of all sizes and all OS's, and consistent improvements are being made.

![](https://iharsh234.github.io/WebApp/images/demo/mobile.png)




## [Usage](https://iharsh234.github.io/WebApp/) 

### Development
Want to contribute? Great!

To fix a bug or enhance an existing module, follow these steps:

- Fork the repo
- Create a new branch (`git checkout -b improve-feature`)
- Make the appropriate changes in the files
- Add changes to reflect the changes made
- Commit your changes (`git commit -am 'Improve feature'`)
- Push to the branch (`git push origin improve-feature`)
- Create a Pull Request 

### Bug / Feature Request

If you find a bug (the website couldn't handle the query and / or gave undesired results), kindly open an issue [here](https://github.com/iharsh234/WebApp/issues/new) by including your search query and the expected result.

If you'd like to request a new function, feel free to do so by opening an issue [here](https://github.com/iharsh234/WebApp/issues/new). Please include sample queries and their corresponding results.


## Built with 

- [jQuery - Ajax](http://www.w3schools.com/jquery/jquery_ref_ajax.asp) - jQuery simplifies HTML document traversing, event handling, animating, and Ajax interactions for rapid web development.
- [Google Chart API](https://developers.google.com/chart/interactive/docs/quick_start) - Free , Rich Gallery , Customizable and Cross-browser compatible.
- [Bootstrap](http://getbootstrap.com/) - Extensive list of components and  Bundled Javascript plugins.


## To-do
- Add BSE (India) Symbol to the current App.
- Decide comparison models of Stocks. (suggestions are most welcome).
- Another WebApp, capable of comparing at least 10 stocks.

## Team

[![Harsh Vijay](https://avatars1.githubusercontent.com/u/12688534?v=3&s=144)](https://github.com/iharsh234)  | [![Quandl.com](https://github.com/iharsh234/WebApp/blob/master/images/quandl.jpg)](https://www.quandl.com/)
---|---
[Harsh Vijay ](https://github.com/iharsh234) |[Quandl](https://www.quandl.com)

## [License](https://github.com/iharsh234/WebApp/blob/master/LICENSE.md)

MIT © [Harsh Vijay ](https://github.com/iharsh234)
