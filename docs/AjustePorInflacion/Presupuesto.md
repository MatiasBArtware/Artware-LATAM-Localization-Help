#Detalle del Proceso de Ajuste

En un principio se debió haber establecido si se deseaba que el proceso de ajuste por inflación generara solamente un presupuesto contable con las cuentas ajustadas o
un presupuesto y además la creación de asientos en el diario configurado también anteriormente en la ventana principal.

A continuación detallaremos cada proceso:

##Presupuesto Contable

El módulo de presupuesto será el primer impacto que tendrá este proceso de ajuste. 
Luego de la selección de fechas dentro de la ventana de configuración para el proceso, se generará un presupuesto contable que tendrá como finalidad ser una
pre visualización de las cuentas que fueron afectadas y sus nuevos saldos ajustados. Además, dentro del presupuesto, ingresando en cada cuenta en particular
podremos ver el detalle de su anticuación¹.

Al ingresar dentro del detalle de la cuenta en este modulo, podremos observar que las partidas se encuentran agrupadas por fechas. Es decir, observemos el siguiente ejemplo:

*La cuenta **000070922 "Inversiones"**, posee los siguientes movimientos:*

![Screenshot](img/PresupuestoYAsientos/contabilidad.jpg)

Podemos observar que la cuenta contiene movimientos durante los meses de febrero, marzo y abril, y que hay más de un movimiento dentro de cada mes.


Para entender mejor lo que visualizaremos dentro del detalle y las agrupaciones por fecha que mencionamos para el módulo de presupuesto, tendremos en cuenta lo siguiente:

![Screenshot](img/PresupuestoYAsientos/contabilidad2.jpg)


Cuando se corra el proceso de Ajuste por Inflación, dentro de este periodo de fechas:

![Screenshot](img/PresupuestoYAsientos/fechas.jpg)

Se generará de manera automatica un presupuesto que contendrá el detalle de las cuentas que fueron afectadas por el proceso.

![Screenshot](img/PresupuestoYAsientos/presupuesto.jpg)

![Screenshot](img/PresupuestoYAsientos/detallepresupuesto.jpg)

Si ingresamos al detalle de la cuenta **"Inversiones"**, haciendo click sobre el saldo, podremos ver la agrupación de las partidas que se encuentran comprendidas dentro
del periodo de fechas seleccionado para el proceso de ajuste.

![Screenshot](img/PresupuestoYAsientos/partidas.jpg)

Como podemos ver, se crearon unicamente tres registros en donde se utilizo como fecha de cierre de cada una de las partidas, el último dia del mes en el que se encuentran comprendidas, y
el saldo a ser ajustado es la sumatoria de saldos de estos movimientos.