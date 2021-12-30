## Objetivo

Este formulario permite dar de alta grupos de comprobantes habilitados y
predeterminados, para asociar a clientes o proveedores, de manera que el usuario
final al momento de cargar transacciones solo tenga disponible los comprobantes
pertinentes.

Para dar de alta a grupo de comprobantes se debe ingresar al formulario ubicado
en **LATAM → COMPROBANTE → GRUPO DE TIPO DE CUENTA**

## Solapa Grupo de Tipo de Cuenta

![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico Descripción
generada automáticamente](img/GrupoTipoCuenta/6ebfad1a9c2f2b5b695290eb2316ed10.png)

Los campos a completar son los siguientes:

-   *Tipo de cuenta:* este campo permite seleccionar el tipo de cuenta (Cliente
    o Proveedor) a la que corresponde el conjunto que está dando de alta.

-   *N°:* este campo se completará manualmente, identificando con un código al
    conjunto que se esté dando de alta.

-   *Descripción:* este campo se completará manualmente, ampliando la
    identificación del campo anterior.

## Solapa Clase de Comprobante cliente/proveedor

![Tabla Descripción generada automáticamente con confianza
media](img/GrupoTipoCuenta/c1431df08d25b1cf0afc8e00f965c941.png)

Esta sección permite parametrizar los comprobantes habituales con los que
trabaja un grupo de clientes o proveedores. Por ejemplo, con el Conjunto de
clientes Responsables Inscriptos se utilizan los siguientes comprobantes:

-   FACTURA A

-   NOTA DE CREDITO A

-   NOTA DE DEBITO A

-   RECIBO

-   REMITO

    Los campos a completar son los siguientes:

-   *Clase Comprobante:* este campo desplegable permite seleccionar uno de los
    comprobantes previamente dados de alta en el Maestro de Clase de
    comprobante.

-   *Descripción:* es un campo no editable que muestra el nombre del ID de clase
    seleccionado.

## Solapa Clase de comprobante por defecto cliente/proveedor

![Tabla Descripción generada
automáticamente](img/GrupoTipoCuenta/492f8183590e0d160906fc96170fd0c0.png)

Esta sección permite parametrizar los comprobantes predeterminados para las
diferentes transacciones de BC que se pueden realizar con el cliente. Se podrán
seleccionar entre los comprobantes habilitados en la sección Comprobantes
habilitados, y siempre que el tipo de comprobante se encuentre permitido para la
transacción a la que se le quiere asociar el comprobante predeterminado.

El campos a completar es el siguiente:

-   *Clase de comprobante por defecto:* en estos campos se podrá configurar, a
    partir de los comprobantes habilitados, el comprobante predeterminado para
    cada transacción de BC que se realice con el cliente o proveedor.
