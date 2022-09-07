
#**Indices de Ajuste por Inflación**


En esta sección tendremos disponibles la tabla de indices de Ajuste por Inflación mensuales. Esta tabla depende de una consulta a un servicio web perteneciente al INDEC,
con base en el año 2016 y actualizaciones mensuales.
Al instalar el módulo de Ajuste, tendrá precargados los indices desde el primero con base 1/12/2016 hasta el último que se haya publicado.

##La tabla consta de tres columnas:

* **Num. de Linea**
* **Fecha**
* **Indice**


| Num. de Linea | Fecha | Indice | 
| ----------- | ----------- | ----------- |
| 1 | 1/12/2016 | 100.00 |
| ... | ... | ... |

##Consulta de Indices


El proceso de Ajuste por Inflación consultará esta tabla para realizar los calculos de ajuste en los saldos de las cuentas que han sido marcadas para el
proceso. Los montos ajustados que se visualizarán en el módulo de presupuesto, serán el resultado de:


* ***Indice de cierre / Indice de origen  =  Coeficiente***


Donde: 

* *Indice de Cierre:* **fecha hasta** la que se desea correr el proceso de ajuste por inflación.
* *Indice de Origen:* **fecha de registración o de origen** de las transacciones que componen el saldo de la cuenta contable.
* *Coeficiente:* resultado obetenido luego de dividir el valor del índice correspondiente a la fecha de cierre por el valor del índice correspondiente a la fecha o período de origen de la partida.
Este coeficiente será el que luego, se aplicará al monto origen de la partida para obtener el monto ajustado y luego la diferencia de estos por el Ajuste, que será parte de las lineas cuando se generen los asientos en el diario.


###Ejemplo:

* **Cuenta: 000113254 "Inversiones"**

Se corre el proceso con el siguiente periodo de fechas:

![Screenshot](img/Indices/fechasAjuste.jpg)

<br>
**Movimientos:**
<hr>
1. $400  →  Fecha de Registración: 22/7/2022  → **(Indice: 1/7/2022 = 851.761)**

2. $500  →  Fecha de Registración: 2/4/2022  → **(Indice: 1/4/2022 = 716.9399)**

3. $1000  →  Fecha de Registración: 13/3/2022  → **(Indice: 1/3/2022 = 676.0566)**

<br>
**Coeficientes:**
<hr>
1. *Coeficiente de Julio* 851.761/851.761 = 1.0000.-
2. *Coeficiente de Abril* 851.761/716.9399 = 1.1880.-
3. *Coeficiente de Marzo* 851.761/676.0566 = 1,2598.-
<hr>

*Estos son los coeficientes a aplicar para cada partida o transacción que componen el saldo de $1.900.- de la cuenta contable. Fecha hasta 31-07-2022.

##**Tabla de Indices de Ajuste por Inflación - Business Central**

*En la parte superior tendremos disponible la opción de Actualizar Indices de Inflación, esto nos permitirá obtener los últimos indices publicados a la fecha.*

![Screenshot](img/Proceso/indices.jpg)







