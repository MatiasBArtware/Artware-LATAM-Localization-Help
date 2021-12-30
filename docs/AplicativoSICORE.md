## Objetivo

El presente manual tiene por objetivo explicar las configuraciones necesarias
para la emisión del aplicativo SICORE (Sistema de Control de Retenciones).

Dicho aplicativo busca informar los regímenes e importes inherentes a
retenciones y percepciones realizadas en un período determinado.

Se podrá emitir el siguiente archivo:

-   Transacciones sobre Retenciones Realizadas de Impuestos a las Ganancias e
    IVA y Percepciones Realizadas de IVA.

## Archivo de Sujetos Retenidos y Percibidos

Los campos que integran el archivo son los siguientes:

-   *Número de documento del Retenido/Percibido:* es el número de documento país
    del cliente o proveedor que realizó o sufrió la percepción o retención
    respectivamente.

    Este campo se toma del maestro Clientes o Proveedores, ubicado en dentro del
    Cliente o Proveedor seleccionado en la Solapa Latam

**Clientes**

![](img/SICORE/ab2ef2abbddef9596fef92bcd3cb4611.png)

**Proveedores**

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/SICORE/3a178f0fb5e947344836d92dc977599f.png)

-   *Razón Social:* es el nombre legal del cliente o proveedor que realizó o
    sufrió la percepción o retención respectivamente.

    **![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico
    Descripción generada
    automáticamente](img/SICORE/c03e35f5ef914ea05be985243a8c2f60.png)**

-   *Domicilio Fiscal:* es la calle de la dirección principal del cliente o
    proveedor que realizó o sufrió la percepción o retención respectivamente.

-   *Localidad:* es la ciudad de la dirección principal del cliente o proveedor
    que realizó o sufrió la percepción o retención respectivamente.

-   *Provincia:* es el Código de Aplicativo para el Estado de la dirección
    principal del cliente o proveedor que realizó o sufrió la percepción o
    retención respectivamente.

-   Estos campos se toman del maestro de Estados, ubicado en **INFORMACIÓN DE LA
    EMPRESA → CONFIGURACIÓN DE LA APLICACIÓN → CONFIGURACIÓN DE CONTABILIDAD →
    ACCIONES → LATAM → APLICATIVOS DE IMPUESTOS**

-   *Código Postal:* es el código postal de la dirección principal del cliente o
    proveedor que realizó o sufrió la percepción o retención respectivamente.

-   *Tipo de documento del Retenido/Percibido:* es el Código Aplicativo para el
    Tipo de Documento del cliente o proveedor que realizó o sufrió la percepción
    o retención respectivamente.

    Estos campos se toman del maestro Tipos de documento, donde se selecciona
    una de las tipos de documento ya cargados **ACCIONES → APLICATIVO DE
    IMPUESTOS**

![Interfaz de usuario gráfica, Tabla Descripción generada
automáticamente](img/SICORE/07d32ebafa1f78e5720bc98ab9f307d3.png)

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/SICORE/3315da598ed4fc8c7b25b26a2fc1a9ec.png)

## Archivo de Percepciones y Retenciones

Los campos que integran el archivo son los siguientes:

-   *Código de Clase de Comprobante:* es el Código Aplicativo relativo a la
    clase de comprobante para la que se calcula la Retención o Percepción.

    Para las Retenciones, se tomará la clase de comprobante que represente el
    pago desde el Diario de Pagos, como por ejemplo Orden de Pago:

Se debe ingresar al formulario ubicado en **LATAM → COMPROBANTE → CLASE DE
COMPROBANTE → ACCIONES → APLICATIVO DE IMPUESTOS**

![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico Descripción
generada automáticamente](img/SICORE/763e9e818dd67b2492d8135a20766596.png)

![Interfaz de usuario gráfica, Aplicación, Tabla Descripción generada
automáticamente](img/SICORE/ee9674f34ce423e789977d3b94a18002.png)

Para las Percepciones, se tomará la clase de comprobante que represente la
venta, como por ejemplo Factura, Nota de Crédito, Nota de Débito, etc.:

![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico Descripción
generada automáticamente](img/SICORE/2e2c691266941aeb569358a9e50fc3a7.png)

![Interfaz de usuario gráfica, Aplicación, Tabla Descripción generada
automáticamente](img/SICORE/829639b897df786b173d94e63b1186da.png)

-   *Fecha de emisión del comprobante (DD/MM/YYYY):* es la fecha en que se
    registró el comprobante de retención o de percepción.

    Para las Retenciones, el dato se tomará del campo Fecha de documento, de la
    línea de retenciones. Las transacciones se ingresarán mediante el formulario
    ubicado en

    **TESORERIA → DIARIOS DE PAGOS → SECCION DE DIARIO**

    ![Aplicación, Tabla Descripción generada
    automáticamente](img/SICORE/f9fb7eca6bedb81c5fd85607076dacc3.png)

Para las Percepciones, el dato se tomará del campo Fecha del comprobante
original en el cual se ha calculado la percepción.

![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico Descripción
generada automáticamente](img/SICORE/5ba90e73f25419c77f163a021031da3d.png)

-   *Número del comprobante:* es el número de comprobante de la línea de tipo
    Proveedor o Cliente donde se calcularon las retenciones (Pagos) o
    percepciones (Ventas).

    Para las Retenciones, el dato se tomará de los campos ‘Punto de venta +
    Número de Comprobante’ de la línea de la Orden de Pago.

    **![](img/SICORE/6af06161f2e59f713435fc353e0d2620.png)**

    Para las Percepciones, el dato se tomará de los campos ‘Punto de venta +
    Número de Comprobante’ del Comprobante de Ventas en el cual se ha calculado
    la percepción.

    **![Interfaz de usuario gráfica, Aplicación Descripción generada
    automáticamente](img/SICORE/c59acf19c69b15142067e82d22302246.png)**

-   *Importe del comprobante:* es el monto de la línea de tipo Proveedor o tipo
    Cliente donde se calcularon las retenciones (Pagos) o percepciones (Ventas).

    Para las Retenciones, el dato se tomará de la línea de Proveedor, el monto
    de la Orden de Pago.

    Para las Percepciones, el dato se tomará del monto total del Comprobante de
    Ventas (Factura, Nota de débito y Nota de crédito).

    **![Interfaz de usuario gráfica, Texto, Aplicación Descripción generada
    automáticamente](img/SICORE/9941b59d859c049850a80e1db07cc767.png)**

-   *Código de impuesto:* es el Código Aplicativo para el Código de Retención o
    Código de Impuesto aplicable para la percepción o retención respectivamente.

    Para las retenciones el dato se toma del formulario Aplicativos del Código
    de Retención que tiene asociada la clase de comprobante de la retención
    LATAM\>\>CLASE DE COMPROBANTES\>\> ACCIONES\>\> LATAM RELACIÓN DE APLICATIVO
    DE IMPUESTO

    ![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico
    Descripción generada
    automáticamente](img/SICORE/a4add59b65d8a6b0aca76f057ace4d58.png)

    ![Tabla Descripción generada
    automáticamente](img/SICORE/1dbf5a4d0ea51d77267db7b2aa7d8f2d.png)

    Para las percepciones el dato se toma del formulario Aplicativos del Código
    de Impuesto que tiene asociado el cliente. El campo se toma del
    JURISDICCIONES FISCALES

    **![Interfaz de usuario gráfica, Aplicación, Word Descripción generada
    automáticamente](img/SICORE/ad8149f744e83be421dbd975edea1037.png)**

-   *Código de régimen:* es el código de Régimen para el Código de Retención o
    Código de Impuesto aplicable para la percepción o retención respectivamente.

    Para las retenciones el dato se toma del formulario Aplicativos del Código
    de Retención que tiene asociado el proveedor. **LATAM → CLASE DE
    COMPROBANTES → ACCIONES → LATAM DE APLICATIVO DE IMPUESTO**

    ![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico
    Descripción generada
    automáticamente](img/SICORE/a4add59b65d8a6b0aca76f057ace4d58.png)

    ![Tabla Descripción generada
    automáticamente](img/SICORE/1dbf5a4d0ea51d77267db7b2aa7d8f2d.png)

    Para las percepciones el dato se toma del formulario Aplicativos del Código
    de Impuesto que tiene asociado el cliente. El campo se toma de
    **JURISDICCIONES FISCALES → SELECCIONO EL CODIGO → LATAM → APLICATIVO DE
    IMPUESTOS**

    **![Interfaz de usuario gráfica, Tabla Descripción generada
    automáticamente](img/SICORE/b5cfb34b60aa09f5d2fe29da304c826c.png)**

    **![](img/SICORE/131b5076f740d0246d7db7631a7269c2.png)**

    **![Tabla Descripción generada
    automáticamente](img/SICORE/dc07be0a0776e424d265524fa205ed2f.png)**

-   *Código de operación:* si se trata de una Retención, se informará el número
    ‘1’ en este campo. En cambio, si se trata de una Percepción, se informará el
    número ‘2’ en este campo.

    **![Interfaz de usuario gráfica, Aplicación Descripción generada
    automáticamente](img/SICORE/decb2ff042fc82a7f09df404a26d39b6.png)**

-   *Base de cálculo:* en este campo, se informará la base sujeta a retención o
    percepción, según corresponda.

    Para las Retenciones, en el Diario de Pagos, para la línea de Retención, el
    campo de donde se tomará la información será ‘Base Imponible’. En el reporte
    se configurará que esta información se muestre en la columna ‘Base de
    retención’.

    ![Interfaz de usuario gráfica, Aplicación Descripción generada
    automáticamente](img/SICORE/ace9650f8bb2540c63fdf6534e6cb10b.png)

    Para las Percepciones, el campo de donde se tomará la información será
    Origen del monto desde la ventana Impuestos sobre las ventas, del
    comprobante de Ventas. En el reporte se configurará que esta información se
    muestre en la columna ‘Base de percepción’.

    ![Tabla Descripción generada
    automáticamente](img/SICORE/0b9399a06b54924f295e667a2af1733a.png)

-   *Fecha de Emisión de la retención (DD/MM/YYYY):* es la fecha en que se
    registró el comprobante de retención o de percepción.

    Para las Retenciones, el dato se tomará del campo Fecha de documento, de la
    línea de retenciones. Las transacciones se ingresarán mediante la siguiente
    ruta:

    **TESORERIA → DIARIOS DE PAGOS → SECCION DE DIARIO**

    **![](img/SICORE/0d3e25946bdb6dd2804197818c689b27.png)**

    Para las Percepciones, el dato se tomará del campo Fecha del comprobante
    original en el cual se ha calculado la percepción.

    **![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico
    Descripción generada
    automáticamente](img/SICORE/0564e531994f10f16a1bc0cb5560181f.png)**

-   *Código de Condición:* es el Código Aplicativo para el Tipo de contribuyente
    del cliente o proveedor que realizó o sufrió la percepción o retención
    respectivamente.

    ![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico
    Descripción generada
    automáticamente](img/SICORE/02f8ccd530faab4d0a08babe647ed08a.png)

-   *Retención practicada a sujetos suspendidos***:** este campo siempre se
    informará en 0.

-   *Importe de la Retención/Percepción:* es el monto de las retenciones (Pagos)
    o percepciones (Ventas).

    Para las Retenciones, en el Diario de Pagos, el campo de donde se tomará la
    información será de la línea de retenciones.

    ![Interfaz de usuario gráfica, Aplicación, Tabla Descripción generada
    automáticamente](img/SICORE/7b42d8bb991d82a3253cd66f57749ea8.png)

    Para las Percepciones, el campo de donde se tomará la información será Monto
    de impuesto sobre las ventas calculado desde la ventana Impuestos sobre las
    ventas, del comprobante de Ventas.

    ![Tabla Descripción generada
    automáticamente](img/SICORE/ca0915dd5e22f856dc21987142303e7e.png)

    *Nota: es muy importante seleccionar el Grupo de Impuestos de Cliente que
    posea la Percepción a realizar ya que, de lo contrario, no se calculará en
    la transacción y será necesario invertirla y cargarla nuevamente, utilizando
    el Grupo de Impuestos que corresponda.*

-   *Porcentaje de exclusión:* Se emite vacío.

-   *Fecha de emisión del boletín:* se emite 01/01/1900

-   *Tipo de documento del retenido:* es el Código Aplicativo para el Tipo de
    documento país del cliente o proveedor que realizó o sufrió la percepción o
    retención.

    Para las retenciones el dato se toma del formulario Aplicativos del Tipo de
    Contribuyente que tiene asociado el proveedor. El campo se toma de LATAM →
    TIPO DE DOCUMENTO

    **![Interfaz de usuario gráfica, Aplicación Descripción generada
    automáticamente](img/SICORE/b680b1a4d54ef7eccb60c22a4f141cd7.png)**

-   *Número de documento del retenido:* es el número de identificación de País
    (CUIT) del proveedor o cliente. Este dato se tomará del maestro de Cliente o
    Proveedor, Solapa LATAM o de la transacción, si la clase de comprobante está
    configurada como detalla contribuyente:

    ![](img/SICORE/ca066ca2e91c21bdd2af6f47af768e2a.png)

    ![](img/SICORE/27bc6d7b7bc8c6e3c694b659443f689f.png)

-   *Número certificado original:* este campo se utilizará para informar datos
    de Beneficiarios del Exterior. Dicha funcionalidad no se encuentra abarcada
    por el alcance actual del desarrollo de emisión del archivo.

-   *Denominación del ordenante:* este campo se utilizará para informar datos de
    Beneficiarios del Exterior. Dicha funcionalidad no se encuentra abarcada por
    el alcance actual del desarrollo de emisión del archivo.

-   *Acrecentamiento:* este campo se utilizará para informar datos de
    Beneficiarios del Exterior. Dicha funcionalidad no se encuentra abarcada por
    el alcance actual del desarrollo de emisión del archivo.

-   *CUIT del país del retenido:* este campo se utilizará para informar datos de
    Beneficiarios del Exterior. Dicha funcionalidad no se encuentra abarcada por
    el alcance actual del desarrollo de emisión del archivo.

-   *CUIT del ordenante:* este campo se utilizará para informar datos de
    Beneficiarios del Exterior. Dicha funcionalidad no se encuentra abarcada por
    el alcance actual del desarrollo de emisión del archivo.

## Configuración del Reporteador de Impuestos

A efectos de la generación del Archivo de Retenciones y Percepciones Realizadas
de IVA y Ganancias, será necesaria la confección de un formato de reporte para
esta salida en el formulario ubicado en **CONFIGURACION → LATAM CONFIGURACION DE
REPORTES → REPORTE DE IMPUESTOS**

**![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/SICORE/c89a135880800be32580abb3b78d099d.png)**

![](img/SICORE/6288ff6a4b40017baeba55ffe2bf9149.png)

Los campos a completar son los siguientes:

-   *N°:* en este campo se deberá completar el código de identificación del
    reporte que se está parametrizando. Por ejemplo, SICORE.

-   *Descripcion:* en este campo se deberá completar el NOMBRE LEGAL del
    reporte. Es muy importante este campo, ya que será la denominación legal que
    se imprimirá en el reporte. Por ejemplo, SICORE.

Dentro de Acciones se podrán configurar las siguientes solapas

![Interfaz de usuario gráfica, Aplicación, Tabla Descripción generada
automáticamente](img/SICORE/9dcc793559b5a480c18259eda184a831.png)

**Solapa Secciones**

![](img/SICORE/0bd5c9fc8c9a397d6529ee5dc36249df.png)

Los campos a completar son los siguientes:

-   *Orden 1, 2, 3:* establecerá el orden en el que se mostrarán los
    comprobantes en el aplicativo. Para este caso, las Retenciones se mostrarán
    primero y, a continuación, las Percepciones.

-   *Grupo de clase de comprobante* en este campo se deberá seleccionar los
    conjuntos de comprobantes previamente configurados en el formulario
    ‘Conjunto de clase de comprobantes’. Dichos conjuntos deberán contener
    aquellos comprobantes que donde se calcularon las Retenciones realizadas de
    Impuesto a las Ganancias e IVA (OP) y Percepciones realizadas de IVA
    (FC/ND/NC).

    *PERCEPCIONES*

    ![Tabla Descripción generada
    automáticamente](img/SICORE/82783bf2e26e77a1ffa38364f794fa41.png)

    *RETENCIONES*

    ![](img/SICORE/78d65deeb2223a055379e0a1219d880a.png)

-   *Nombre:* este campo ampliará con una descripción el código indicado en el
    campo ‘Id. de conjunto de comprobantes’. No es un campo editable.

-   *Nombre para mostrar:* este campo se utilizará para asignar el nombre del
    conjunto que deberá visualizarse en el reporte. En caso de estar en blanco,
    en el reporte saldrá vacío.

-   *Invertir el signo:* por cada conjunto de comprobantes se podrá determinar
    si en la visualización del reporte se debe invertir el signo. No será
    necesario marcar para este Archivo.

-   *Filtrar por:* este campo permite seleccionar una de las opciones de
    filtrado que se aplicarán sobre el conjunto de comprobantes seleccionado. La
    opción recomendada es:

-   Sin filtro: no tiene en cuenta ninguna de las columnas siguientes.

**Solapa Columnas**

Para el aplicativo SICORE Transacciones, se deberán configurar seis columnas en
el reporte impositivo, de la siguiente manera:

-   *Columna 1:* Base Percepción

    La primera columna deberá configurarse para mostrar el monto base de las
    percepciones a informar. Por ese motivo, en la grilla de Conjunto de
    impuestos por columna, se deberá configurar como ‘Impuesto: Monto base’,
    seleccionando el Id. De conjunto de impuestos que contenga a las
    percepciones a informar.

    ![](img/SICORE/dde045e2ef59b891cfcbbb7ca5b13d6f.png)

    ![Tabla Descripción generada
    automáticamente](img/SICORE/47aeae622babd0a74ac100f5741201f3.png)

    ![Interfaz de usuario gráfica, Aplicación Descripción generada
    automáticamente](img/SICORE/ff09073ebf1d4a86f9460c024855fb60.png)

    ![](img/SICORE/e3dbe411e76e5f3f6b4587b6e7a6d237.png)

-   *Columna 2:* Importe Percepción

    La segunda columna deberá configurarse para mostrar los montos de
    percepciones. Por ese motivo, en la grilla ‘Tipo de monto por columna’, se
    deberá configurar como ‘Impuesto: Monto’, seleccionando el Id. De conjunto
    de impuestos que contenga a las percepciones a informar, seleccionado en la
    Columna 1.

    ![](img/SICORE/4ff7d2d7765e2427e3f407e970c6b1e3.png)

    ![Interfaz de usuario gráfica, Aplicación Descripción generada
    automáticamente](img/SICORE/239bd1e2121c12b4abe420bb1a33171e.png)

-   *Columna 3:* Base Retención

    La tercera columna deberá configurarse para mostrar el monto base de las
    retenciones a informar. Por ese motivo, en la grilla de Conjunto de
    impuestos por columna, se deberá configurar como ‘Retención: Monto base’,
    sin Conjunto de Impuestos por tratarse de retenciones, pero sí con el
    conjunto de retenciones.

    ![Interfaz de usuario gráfica, Aplicación Descripción generada
    automáticamente](img/SICORE/759e0436f0259d924c3da8e92fe8f350.png)

    ![Interfaz de usuario gráfica, Aplicación Descripción generada
    automáticamente](img/SICORE/e43cc983efe274554453e2fc81d5f7f4.png)

    ![](img/SICORE/1d3373e38235bcbccfdd3b7156e0b615.png)

    ![](img/SICORE/e58999cc330bd7e88b786a6b75949585.png)

    ![](img/SICORE/7afec41b8643b48b02e84e7efaa26daf.png)

-   *Columna 4:* Importe Retención

    La cuarta columna deberá configurarse para mostrar el importe de las
    retenciones a informar. Por ese motivo, en la grilla de Conjunto de
    impuestos por columna, se deberá configurar como ‘Retención: Monto’.

    ![](img/SICORE/ac38b7f65870a940aa1bad76bc91909f.png)

    ![](img/SICORE/ae24a4b495e6f0df78c8350e9c13879e.png)

-   *Columna 5:* Total

    Esta columna se adicionará a efectos de mostrar sólo las transacciones que
    posean los códigos de impuestos y retenciones configurados en las columnas
    precedentes. Para ello deberá crear una columna y configurarla como ‘Excluir
    Comprobante en Cero’. Adicionalmente en la grilla inferior deberá
    seleccionar ‘Impuesto: Monto Sujeto’ con el conjunto de comprobantes
    seleccionado en la Columna 1 y una línea como ‘Retención: Monto Sujeto’.

    ![Interfaz de usuario gráfica, Aplicación Descripción generada
    automáticamente](img/SICORE/c85a1b7b1271d4595e9d6adeb68b797b.png)

    ![Tabla Descripción generada
    automáticamente](img/SICORE/e677a6d2723e75d1e5c58fc732256c02.png)

**Solapa General**

![](img/SICORE/c528698fd564cd907b766092738a6bea.png)

Los campos a completar son los siguientes:

-   *Ordenar por:* este campo permite indicar el orden a tomar en los
    documentos. Se recomienda la opción ‘Fecha + Comprobante + Número de
    documento’

-   *Cantidad de decimales:* este campo permite indicar la cantidad de decimales
    a mostrar en los campos de Tipo monto. Se recomienda colocar 2 decimales.

-   *Separador de miles:* este campo permite indicar el separador de miles a
    utilizar en el reporte a emitir, no del archivo. El archivo tomará como
    separador de miles el Punto (.)

-   *Separador de decimales:* este campo permite indicar el separador de
    decimales a utilizar en el reporte a emitir, no del archivo. El archivo
    tomará como separador de decimales la Coma (,).

    ![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico
    Descripción generada
    automáticamente](img/SICORE/087738d4978ec9253a3430c971cc0a08.png)

**Solapa Formato**

Se recomienda asignar un formato de reporte a efectos de poder visualizar la
información ingresada y controlar el contenido de lo informado en el archivo.

**![Aplicación, Tabla Descripción generada automáticamente con confianza
media](img/SICORE/d714f97e089029e34695a192da81117c.png)**

**![Tabla Descripción generada
automáticamente](img/SICORE/596932403193bfae58195f86074d247d.png)**

## Definición de exportación de medios magnéticos

Una vez realizada la configuración general para cada archivo será necesario
configurar específicamente la exportación de los archivos, en el formulario
ubicado en **FINANZAS → LATAM → MEDIO MAGNETICOS → DEFINICION DE MEDIOS
MAGNETICOS**

![](img/SICORE/e718803cc51e43ea88b1e4a5686840a4.png)

![Interfaz de usuario gráfica Descripción generada
automáticamente](img/SICORE/8aa9ab56690b8a9b18740f63c8422c63.png)

Se deberá configurar un registro por cada salida. Los campos a completar son los
siguientes:

**Solapa General**

-   *ID Medio magnético:* es la identificación del código para exportación del
    archivo magnético. Se recomienda utilizar un código que el usuario que
    exportará el archivo, pueda distinguir.

-   *Descripción:* ingrese una descripción sobre el Tipo de Archivo a Exportar.

**Configuración**

-   *Aplicativo de impuesto:*  Seleccionar el creado en ‘LATAM Aplicativo de
    impuesto’

-   *Reporte de impuestos:* Seleccionar el reporte de la lista desplegable

-   *Reporte ID:* Se debe seleccionar el ID correspondiente al aplicativo. Este
    ID lo proporciona Desarrollo previamente

    **Parámetros**

-   *Parámetros:* en esta grilla se deberán agregar las distintas etiquetas que
    hacen al nombre del archivo a exportar y el tipo de extensión del archivo.

-   Nombre: SICORE

-   Extensión: .txt.

-   *Nombre del archivo:* en este campo se deberán concatenar los campos Nombre
    creados en la grilla Parámetros, precedidos por el símbolo \$ y sin espacios
    entre ellos.

-   *Nombre de archivo traducido:* este campo no es editable, solo tomará los
    campos Valor creados en la grilla Parámetros.

## Exportación de medios magnéticos

Desde este formulario se emitirá el archivo y se determinará dónde debe
guardarse, se puede acceder mediante el formulario ubicado en **INFORMES →
INFORMES FINANACIEROS →LATAM MEDIOS MAGNETICOS → EXPORTACIÓN DE MEDIOS
MAGNÉTICOS.**

![Interfaz de usuario gráfica, Tabla Descripción generada
automáticamente](img/SICORE/eb6045ee5ba79b405dcdf32d365e95a7.png)

Los campos a completar son los siguientes:

-   *ID Medio magnético:* aquí se deberá seleccionar el ID de Exportación,
    configurado en el formulario Definición de exportación de medios magnéticos.

-   *Fecha desde:* es la fecha inicial a partir de la cual se mostrará la
    información. Será la fecha de Registración de las Transacciones.

-   *Fecha hasta:* es la fecha final hasta la cual se mostrará la información.
    Será la fecha de Registración de las Transacciones.

-   *Nombre del archivo:* en este campo no editable se visualiza el nombre
    completo y extensión configurado en la Definición de exportación de archivos
    magnéticos.

## Ejemplos de Archivos exportados

SICORE- Transacciones

![](img/SICORE/1e66e1a6fa56bbddb0df3b21c70e065f.png)
