1

## Objetivo

El presente manual tiene por objetivo explicar las configuraciones necesarias
para la emisión del aplicativo Si.Fe.Re. Convenio Multilateral.

Dicho aplicativo busca informar los importes inherentes a retenciones y
percepciones sufridas Impuesto sobre los Ingresos Brutos que tributan por
Convenio Multilateral en un período determinado.

Se podrán emitir los siguientes archivos:

-   Retenciones de Ingresos Brutos Sufridas

-   Percepciones de Ingresos Brutos Sufridas

-   Retenciones Bancarias Sufridas

-   Percepciones Aduaneras Sufridas

## Retenciones de Ingresos Brutos Sufridas

Los campos que integran el archivo son los siguientes:

-   *Código de Jurisdicción:* es la jurisdicción dada de alta en el aplicativo
    para la clase de comprobante aplicable a la retención.

    Para las retenciones el dato se toma del formulario Aplicativos de la Clase
    de comprobante. El formulario está ubicado en **LATAM → CLASE DE
    COMPROBANTE.**

    **![Interfaz de usuario gráfica, Aplicación Descripción generada
    automáticamente](img/SIFERE/d245eba96dab3670610776256f0fbeda.png)**

    ![Interfaz de usuario gráfica, Aplicación, Word Descripción generada
    automáticamente](img/SIFERE/7fb9c72a18d7541d1b80e7aeee2cd904.png)

    *Nota 1: se aclara que se podrá configurar un aplicativo para diferenciar y
    poder tomar los códigos de comprobantes, jurisdicciones, tipo de documentos,
    etc. Asegúrese de crear un Id de Aplicativo por cada Archivo Magnético que
    necesite.*

    *Nota 2: se aclara que a nivel de configuración requiere la creación de un
    comprobante valor de tipo retención para cada jurisdicción de Ingresos
    Brutos sufrida por la compañía.*

    *Nota 3: no se recomienda utilizar comprobantes de retención creados y
    utilizados en los Pagos a Proveedores.*

-   *CUIT del Agente de Retención:* es el número de identificación de País
    (CUIT) del cliente que ha realizado la Retención.

    Este campo se toma del maestro Clientes, ubicado en la Solapa Latam

    *![Interfaz de usuario gráfica, Tabla Descripción generada
    automáticamente](img/SIFERE/39ceb5b3894188209be4a09e5bcc3090.png)*

-   *Fecha de la Retención:* se trata de la fecha del Certificado de Retención.
    Este campo se obtiene del tab LATAM de la línea que representa la Retención
    Sufrida, Fecha de Documento.

    Las transacciones se ingresarán mediante el diario ubicado en **TESORERIA →
    DIARIO DE RECIBO DE EFECTIVO.**

    **![Interfaz de usuario gráfica, Aplicación Descripción generada
    automáticamente](img/SIFERE/4fc9390e8869b7c44669f6c46505f6a6.png)**

    *Nota: debe asegurarse que al cargar la transacción se coloque allí la fecha
    que figura en el Certificado de Retención.*

-   *Número de Sucursal:* es el campo Punto de Venta que figura para la clase de
    comprobante de la línea de Retención.

    ![Interfaz de usuario gráfica, Aplicación Descripción generada
    automáticamente](img/SIFERE/adc2cf6f69f21ebc458f7c374fb3e41a.png)

    *Nota 1:* *debe asegurarse que al cargar la transacción se coloque allí la
    sucursal que figura en el Certificado de Retención.*

    *Nota 2: se recomienda que el comprobante que representa la retención se
    encuentre configurado con numeración manual y habilitado para el ingreso del
    punto de venta o sucursal. De no tener sucursal, se recomienda completar con
    ceros, el campo.*

-   *Número de constancia:* se trata del campo Número de Comprobante que figura
    para la clase de comprobante de la línea de Retención.

    **![Interfaz de usuario gráfica, Aplicación Descripción generada
    automáticamente](img/SIFERE/f7d76f92bec5697154b37123fc6b03ce.png)**

    *Nota 1:* *debe asegurarse que al cargar la transacción se coloque allí el
    número de certificado que figura en el comprobante entregado por el
    cliente.*

    *Nota 2: se recomienda que el comprobante que representa la retención se
    encuentre configurado con numeración manual.*

-   *Tipo de Comprobante (F, R, D, C, O):* es un campo que diferencie los Tipos
    de Clase de comprobantes. Para este archivo, será necesario configurar en la
    clase de comprobante que represente el Recibo o Cobro (Comprobante No
    Valor), en el Botón Aplicativo, el Tipo de comprobante que se requiere. Para
    el Caso del Recibo será ‘R’.

    **![Interfaz de usuario gráfica, Aplicación, Word Descripción generada
    automáticamente](img/SIFERE/42bc369a39d79cf300ec60667ae68591.png)**

    *Nota 1: se aclara que se podrá configurar un aplicativo para diferenciar y
    poder tomar los códigos de comprobantes, jurisdicciones, tipo de documentos,
    etc. Asegúrese de crear un Id de Aplicativo por cada Archivo Magnético que
    necesite.*

    *Nota 2:*

    -   F= Factura

    -   R= Recibo

    -   D= Nota de Debito

    -   C= Nota de Crédito

    -   O= Otros

-   *Letra del Comprobante:* es la Letra del Comprobante configurada en el
    comprobante que represente el Recibo o Cobro (Comprobante No Valor), en el
    Botón Aplicativo. Para el caso del Recibo será ‘C’.

![Interfaz de usuario gráfica, Aplicación, Word Descripción generada
automáticamente](img/SIFERE/66bcc1ea3bae6794dc7ccfb43d015389.png)

*Nota: se aclara que se podrá configurar un aplicativo para diferenciar y poder
tomar los códigos de comprobantes, jurisdicciones, tipo de documentos, etc.
Asegúrese de crear un Id de Aplicativo por cada Archivo Magnético que necesite.*

-   *Número de Comprobante Original***:** es el campo Número de Comprobante del
    comprobante que representa el Recibo o Cobro (Comprobante No Valor). Debe
    asegurarse que al cargar la transacción se coloque allí el número de Recibo
    o Cobro.

    ![Interfaz de usuario gráfica, Aplicación Descripción generada
    automáticamente](img/SIFERE/0656b841ee664d41b8934a153e75783e.png)

    *Nota: en general este comprobante se encuentra configurado con numeración
    automática por lo que al registrar se asigna la numeración.*

-   *Importe Retenido:* es el importe que figura sobre la línea de Retención.
    Este importe debe ingresarse en la transacción a partir del comprobante
    entregado por el Cliente.

    **![Interfaz de usuario gráfica, Aplicación Descripción generada
    automáticamente](img/SIFERE/f9514ac85d3886d6ce344fc20a67c304.png)**

## Configuración del Reporteador de Impuestos

A efectos de la generación del Archivo de Retenciones de Ingresos Brutos
Sufridas será necesaria la confección de un formato de reporte para esta salida
en el formulario ubicado en **CONFIGURACION → LATAM CONFIGURACION DE REPORTES →
REPORTES DE IMPUESTOS.**

**![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/SIFERE/c89a135880800be32580abb3b78d099d.png)**

**Solapa General**

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/SIFERE/992f8b6e1f4e53dae18b2dc1089b7128.png)

Los campos a completar son los siguientes:

-   *N°:* en este campo se deberá completar el código de identificación del
    reporte que se está parametrizando. Por ejemplo, SIF-RETSUF.

-   *Descripción:* en este campo se deberá completar el NOMBRE LEGAL del
    reporte. Es muy importante este campo, ya que será la denominación legal que
    se imprimirá en el reporte. Por ejemplo, SIFERE- RETENCIONES SUFRIDAS.

Dentro de Acciones se podrán configurar las siguientes solapas

![Interfaz de usuario gráfica, Texto, Aplicación Descripción generada
automáticamente](img/SIFERE/cdb5ca391cc79dd46ff6404a745a3bc0.png)

**Solapa Secciones**

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/SIFERE/df0e3c10d639588ccab1d55dd2cd8cba.png)

Los campos a completar son los siguientes:

-   *Orden 1, 2, 3:* establecerá el orden en el que se mostrarán los
    comprobantes en el aplicativo.

-   *Grupo de clase de comprobante:* en este campo se deberá seleccionar los
    conjuntos de comprobantes previamente configurados en el formulario Latam
    Lista de grupos de clase de comprobante. Dichos conjuntos deberán contener
    aquellos comprobantes que representen Retenciones sufridas de Ingresos
    brutos en los cobros.

![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico Descripción
generada automáticamente](img/SIFERE/7ac8873d3cbcc9eefe8b9c7c4bf731a1.png)

![Interfaz de usuario gráfica, Aplicación, Word Descripción generada
automáticamente](img/SIFERE/f6b38c7c087242505a10ec95f3f51c14.png)

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

Solapa Columnas

Para el aplicativo SIFERE Retenciones Sufridas, se deberá configurar una columna
en el reporte impositivo, de la siguiente manera:

-   *Columna 1:* Monto de la Retención

    Esta columna deberá configurarse para mostrar el importe de las retenciones
    a informar. Por ese motivo, en la grilla de Conjunto de impuestos por
    columna, se deberá configurar como ‘Retención: Monto’*, con su ID de grupo
    de retenciones que contenga todos los códigos de retención de IIBB de las
    jurisdicciones que nos realizan retención*

*![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/SIFERE/760b531d356dc6e063af1f0f11eac2c5.png)*

*![Interfaz de usuario gráfica, Aplicación, Word Descripción generada
automáticamente](img/SIFERE/5ba348cca20c575ddb9d369848e33a5a.png)*

**Solapa General**

![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico Descripción
generada automáticamente](img/SIFERE/e19c62e473d7ce2c24c4646104458d87.png)

Los campos a completar son los siguientes:

-   *Ordenar por:* este campo permite indicar el orden a tomar en los
    documentos. Se recomienda la opción ‘Fecha + Comprobante + Número de
    documento’

-   *Cantidad de decimales:* este campo permite indicar la cantidad de decimales
    a mostrar en los campos de Tipo monto. Se recomienda colocar 2 decimales.

-   *Separados de miles:* este campo permite indicar el separador de miles a
    utilizar en el reporte a emitir, no del archivo. El archivo tomará como
    separador de miles el Punto (.)

-   *Separador de decimales:* este camp permite indicar el separador de
    decimales a utilizar en el reporte a emitir, no del archivo. El archivo
    tomará como separador de decimales la Coma (,).

**Solapa de Formato**

Se recomienda asignar un formato de reporte a efectos de poder visualizar la
información ingresada y controlar el contenido de lo informado en el Archivo.

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/SIFERE/0365b5c6e9150f366115365a4d7987be.png)

## Percepciones de Ingresos Brutos Sufridas

Los campos que integran el archivo son los siguientes:

-   *Código de Jurisdicción:* es la jurisdicción dada de alta en el aplicativo
    para el código de impuestos que represente la percepción.

    Para las percepciones el dato se toma del formulario Aplicativos del Código
    de impuesto. El formulario está ubicado en **JURISDICCIONES FISCALES → LATAM
    → APLICATIVO DE IMPUESTO.**

*![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/SIFERE/3ff99bf6e02969df5cad8ffd1df5fb66.png)*

*![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/SIFERE/f60e4d3b40022eee93306c79846d210e.png)*

*Nota 1: se aclara que se podrá configurar un aplicativo para diferenciar y
poder tomar los códigos de comprobantes, jurisdicciones, tipo de documentos,
etc. Asegúrese de crear un Id de Aplicativo por cada Archivo Magnético que
necesite.*

*Nota 2: se aclara que a nivel de configuración requiere la creación de un
código de impuestos (Percepción sufrida) para cada jurisdicción de Ingresos
Brutos.*

-   *CUIT del Agente de Percepción:* es el número de identificación de País
    (CUIT) del proveedor que ha realizado la Percepción.

    Este campo se toma del maestro Proveedores, ubicado en la Solapa Latam

**![Interfaz de usuario gráfica, Aplicación, Tabla Descripción generada
automáticamente](img/SIFERE/119be313e97d940acddedf38a2ea9811.png)**

-   *Fecha de la Percepción:* se trata de la fecha de la transacción en la cual
    se ha registrado la Percepción, es decir la fecha de contabilización.

**![Interfaz de usuario gráfica, Tabla Descripción generada
automáticamente](img/SIFERE/7f1842a386bd9033b39ef882e18169dd.png)**

-   *Número de Sucursal:* es el campo Punto de Venta que figura sobre la línea
    del comprobante en donde se encuentra la Percepción. Debe asegurarse que al
    cargar la transacción se coloque allí la sucursal o Punto de Venta que
    figura en el comprobante entregado por el proveedor.

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/SIFERE/b3648f65d6ce8cb0075c3c63503beae2.png)

*Nota: el comprobante que representa la Factura del Proveedor debería
configurarse con numeración manual y poseer habilitado el ingreso del punto de
venta o sucursal.*

-   *Número de constancia:* se trata del campo Número de Comprobante que
    contiene la Percepción, como por ejemplo Factura. Debe asegurarse que al
    cargar la transacción se coloque allí el número de comprobante que ha
    entregado el proveedor.

**![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/SIFERE/09d5e6fe4bfb300e7791493c66e44fae.png)**

*Nota: el comprobante que representa la Factura del Proveedor debería
configurarse con numeración manual y poseer habilitado el ingreso del punto de
venta o sucursal.*

-   *Tipo de Comprobante (F, R, D, C, O):* es un campo que diferencie los Tipos
    de Comprobantes. Para este archivo, será necesario configurar en el
    comprobante que contenga la Percepción, posea en el Botón aplicativo, el
    tipo de comprobante que se requiere. Para el caso de Factura, por ejemplo,
    será ‘F’.

![Interfaz de usuario gráfica, Aplicación, Correo electrónico Descripción
generada automáticamente](img/SIFERE/8021d479aa988b80f3c532404c37d91a.png)

![Interfaz de usuario gráfica, Aplicación, Word Descripción generada
automáticamente](img/SIFERE/358b4e83b59a4527c1fd856fad630c07.png)

*Nota: se aclara que se podrá configurar un aplicativo para diferenciar y poder
tomar los códigos de comprobantes, jurisdicciones, tipo de documentos, etc.
Asegúrese de crear un Id de Aplicativo por cada Archivo Magnético que necesite.*

-   *Letra del Comprobante:* es la Letra del Comprobante que contiene la
    Percepción. Se deberá configurar a través del botón Aplicativo. Por ejemplo,
    ‘A’.

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/SIFERE/d43fd05274f07add7abdb5cf8c7cf980.png)

*Nota: se aclara que se podrá configurar un aplicativo para diferenciar y poder
tomar los códigos de comprobantes, jurisdicciones, tipo de documentos, etc.
Asegúrese de crear un Id de Aplicativo por cada Archivo Magnético que necesite.*

-   *Importe Percibido:* es el importe de la Percepción. Para poder tomar el
    importe correcto de la Percepción se requiere tener configurado un Código de
    Impuesto por cada Percepción de Ingresos Brutos de cada jurisdicción.
    Adicionalmente debe asegurarse que, a nivel de la transacción, dicho código
    de impuesto, se encuentre asignado para que la Percepción se calcule y
    queden los datos relacionados a la transacción.

## Configuración del Reporteador de Impuestos

A efectos de la generación del archivo de Percepciones de Ingresos Brutos
Sufridas será necesaria la confección de un formato de reporte para esta salida
en el formulario ubicado en **CONFIGURACION → LATAM CONFIGURACION DE REPORTES →
REPORTES DE IMPUESTOS.**

**![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/SIFERE/c89a135880800be32580abb3b78d099d.png)**

![Interfaz de usuario gráfica, Texto, Aplicación Descripción generada
automáticamente](img/SIFERE/6f450b9293868be4607245befd5c5f56.png)

Los campos a completar son los siguientes:

-   *N°:* en este campo se deberá completar el código de identificación del
    reporte que se está parametrizando. Por ejemplo, SIF-PERCSUF.

-   *Descripcion:* en este campo se deberá completar el NOMBRE LEGAL del
    reporte. Es muy importante este campo, ya que será la denominación legal que
    se imprimirá en el reporte. Por ejemplo, SIFERE- PERCEPCIONES SUFRIDAS.

Dentro de Acciones se podrán configurar las siguientes solapas

*![Interfaz de usuario gráfica, Texto, Aplicación Descripción generada
automáticamente](img/SIFERE/6340c7d4f212d7ecc32b66b551b9df02.png)*

**Solapa Secciones**

![Interfaz de usuario gráfica Descripción generada automáticamente con confianza
media](img/SIFERE/ff95e3e2cfe63ad473a96f2704e1dd32.png)

Los campos a completar son los siguientes:

-   *Orden 1, 2, 3:* establecerá el orden en el que se mostrarán los
    comprobantes en el aplicativo.

-   *Grupo de comprobante:* en este campo se deberá seleccionar los conjuntos de
    comprobantes previamente configurados en el formulario Latam Lista de grupos
    de clase de comprobante.. Dichos conjuntos deberán aquellos contener
    comprobantes que representen Percepciones sufridas de Ingresos Brutos en las
    compras.

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/SIFERE/f007a77d8702f8f668b718732bdf6f3e.png)

*Nota: se recomienda colocar en un mismo conjunto todos los comprobantes,
incluyendo las Notas de Crédito, ya que éstas se deberán informar con su signo
original (negativo).*

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

Para el aplicativo SIFERE Percepciones Sufridas, se deberá configurar dos
columnas en el reporte impositivo, de la siguiente manera:

![Interfaz de usuario gráfica, Aplicación, Word Descripción generada
automáticamente](img/SIFERE/b09ceacfe3ad498de10ede66cab58d1b.png)

-   *Columna 1:* Monto de la Percepción.

    Esta columna deberá configurarse para mostrar el importe de las percepciones
    a informar. Por ese motivo, en la grilla de Conjunto de impuestos por
    columna, se deberá configurar como ‘Impuesto: Monto’.

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/SIFERE/37ae58bb1d7a4328b6b594887cf17bb4.png)

-   *Columna 2:* Total

    Esta columna deberá configurarse para mostrar sólo las transacciones que
    posean los códigos de impuestos configurados en la columna 1, y configurarla
    como ‘Excluir Comprobante en Cero’ (ver imagen arriba). En la grilla
    inferior deberá seleccionar ‘Impuesto: Monto Sujeto’ con el conjunto de
    comprobantes seleccionado en la Columna 1.

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/SIFERE/71fec79cb3398e994b80c939f430a93b.png)

**  
**

**Solapa General**

![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico Descripción
generada automáticamente](img/SIFERE/f9859469c60909129fadc83cafeb5330.png)

Los campos a completar son los siguientes:

-   *Ordenar por:* este campo permite indicar el orden a tomar en los
    documentos. Se recomienda la opción ‘Fecha + Comprobante + Número de
    documento’

-   *Cantidad de decimales:* este campo permite indicar la cantidad de decimales
    a mostrar en los campos de Tipo monto. Se recomienda colocar 2 decimales.

-   *Separados de miles:* este campo permite indicar el separador de miles a
    utilizar en el reporte a emitir, no del archivo. El archivo tomará como
    separador de miles el Punto (.)

-   *Separador de decimales:* este camp permite indicar el separador de
    decimales a utilizar en el reporte a emitir, no del archivo. El archivo
    tomará como separador de decimales la Coma (,).

**Solapa de Formato**

Se recomienda asignar un formato de reporte a efectos de poder visualizar la
información ingresada y controlar el contenido de lo informado en el Archivo.

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/SIFERE/9a29d80caf36531d7706b08ca0f215f5.png)

## Retenciones de Ingresos Brutos de Banco Sufridas

Los campos que integran el archivo son los siguientes:

-   *Código de Jurisdicción:* es la jurisdicción dada de alta en el aplicativo
    para el código de impuesto aplicable a la retención. Las retenciones
    bancarias, se configuran como códigos de impuestos, ya que las mismas se ven
    reflejadas en el ingreso del resumen bancario.

    Para este caso en particular el dato se toma del formulario Aplicativos de
    Códigos de Impuestos. El formulario está ubicado en **IMPUESTOS \>\>
    IMPUESTOS INDIRECTOS\>\> IMPUESTOS \>\> CÓDIGOS DE IMPUESTOS SOBRE LAS
    VENTAS \>\> BOTON LATAM \>\> APLICATIVOS.**

![Interfaz de usuario gráfica, Tabla Descripción generada
automáticamente](img/SIFERE/504b66eef9939269f194d3ef0901f0ba.png)

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/SIFERE/dbb18286e618f5fec7581153411f01e5.png)

*Nota 1: se aclara que se podrá configurar un aplicativo para diferenciar y
poder tomar los códigos de comprobantes, jurisdicciones, tipo de documentos,
etc. Asegúrese de crear un Id de Aplicativo por cada Archivo Magnético que
necesite.*

*Nota 2: se aclara que a nivel de configuración requiere la creación de un
código de Impuestos que represente la Retención que realiza el Banco para cada
jurisdicción de Ingresos Brutos.*

-   *CUIT del Agente de Recaudación:* es el número de identificación de País
    (CUIT) del Banco que ha realizado la Retención.

    Los bancos deberán crearse como Proveedores. Si se posee más de una cuenta
    bancaria en un mismo Banco, se recomienda crear dos proveedores. Este campo
    se toma del maestro Proveedores, ubicado en la Solapa Latam.

**![Interfaz de usuario gráfica Descripción generada
automáticamente](img/SIFERE/5a40beb3c31156f93e9e201a3403aaa6.png)**

-   *Período de Retención:* se trata de la fecha del Comprobante de Banco. Este
    campo se obtiene del tab LATAM de la línea que representa la Retención
    Sufrida, Fecha de Documento. A partir de ese dato se informará el Mes y el
    Año.

**![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/SIFERE/a6d523500b2449913da87e1c4b8d6dcc.png)**

-   *CBU:* este campo se deberá configurar en el maestro del Proveedor que
    represente al banco. En la información adicional de Cuentas Bancarias,
    dentro del campo IBAN.

**![Tabla Descripción generada automáticamente con confianza
media](img/SIFERE/dbb30537d9b59b548d2e74412b8654ea.png)**

**![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/SIFERE/ec550911bd60ba58e21b91f8c117ea59.png)**

-   *Tipo de Cuenta (CA, CC, OO):* deberá asociarse en el maestro de Proveedor
    que represente al Banco. El campo a utilizarse será Código de Propósito del
    Banco Central, en el correspondiente maestro se deberán crear los siguientes
    códigos:

-   CA = Caja de Ahorro

-   CC= Cuenta Corriente

-   OO= Otros

    El Id del Propósito del Banco Central, deberá ser igual al Id que se deba
    indicar en el Archivo.

    ![Interfaz de usuario gráfica, Aplicación Descripción generada
    automáticamente](img/SIFERE/2352a7ad471a1d0bb852939fd3375860.png)

-   *Tipo de Moneda (P, E, O):* es la moneda predeterminada en el maestro de
    Proveedor que represente al Banco. Para informar el código solicitado por el
    Aplicativo, será necesario configurar en el Botón Aplicativo del maestro de
    Monedas el código correspondiente:

    -   P= Pesos

    -   E= Moneda Extranjera

    -   O= Otros

        El formulario está ubicado en **INFORMACION DE EMPRESA → CONFIGURACION
        DE LA APLICACIÓN → CONFIGURACION DE CONTABILIDAD → ACCIONES → LATAM →
        APLICATIVO DE IMPUESTOS**

        **![Interfaz de usuario gráfica, Aplicación Descripción generada
        automáticamente](img/SIFERE/3ca67cfb855492fdd04392b1097e6179.png)**

        **![Interfaz de usuario gráfica, Aplicación Descripción generada
        automáticamente](img/SIFERE/c5abd957a0312e90b0a0319d45284bfc.png)**

![Interfaz de usuario gráfica, Texto, Aplicación Descripción generada
automáticamente](img/SIFERE/11f122e3bc0aecb8f57ee8fdf24da150.png)

-   *Importe Retenido:* es el importe de la Retención (Código de Impuesto). Para
    poder tomar el importe correcto de la Retención se requiere tener
    configurado un Código de Impuesto por cada Retención de Ingresos Brutos de
    Banco por cada jurisdicción. Adicionalmente debe asegurarse que, a nivel de
    la transacción, dicho código de impuesto, se encuentre asignado para que se
    calcule y queden los datos relacionados a la transacción.

## Configuración del Reporteador de Impuestos

A efectos de la generación del Archivo de Retenciones de Banco Sufridas será
necesaria la confección de un formato de reporte para esta salida en el
formulario ubicado en **CONFIGURACION → LATAM CONFIGURACION DE REPORTES →
REPORTE DE IMPUESTOS**

**![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/SIFERE/c89a135880800be32580abb3b78d099d.png)**

**![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico
Descripción generada
automáticamente](img/SIFERE/5ed0f994ac4ce74116363ce93a2a11e2.png)**

Los campos a completar son los siguientes:

-   *N°:* en este campo se deberá completar el código de identificación del
    reporte que se está parametrizando. Por ejemplo, SIF-RETBCO.

-   *Descripcion:* en este campo se deberá completar el NOMBRE LEGAL del
    reporte. Es muy importante este campo, ya que será la denominación legal que
    se imprimirá en el reporte. Por ejemplo, SIFERE- RETENCIONES BANCARIAS.

    **![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico
    Descripción generada
    automáticamente](img/SIFERE/9975c0b64bed95cb9d4cc1850a86570b.png)**

Dentro de Acciones se podrán configurar las siguientes solapas:

**Solapa Secciones**

![Interfaz de usuario gráfica Descripción generada automáticamente con confianza
media](img/SIFERE/ff95e3e2cfe63ad473a96f2704e1dd32.png)

Los campos a completar son los siguientes:

-   *Orden 1, 2, 3:* establecerá el orden en el que se mostrarán los
    comprobantes en el aplicativo.

-   *Grupo de clase de comprobante:* en este campo se deberá seleccionar los
    conjuntos de comprobantes previamente configurados en el formulario LATAM
    Lista de grupos de clase de comprobante. Puede crearse una clase de
    comprobante resumen bancario, con las mismas parametrizaciones de una
    Factura, o puede utilizarse el comprobante Factura para cargar los datos del
    resumen bancario con las retenciones bancarias.

    ![Interfaz de usuario gráfica, Aplicación Descripción generada
    automáticamente](img/SIFERE/5c6422f8eb8d1b1d0359cc2ee199fca4.png)

-   *Descripcion:* este campo ampliará con una descripción el código indicado en
    el campo ‘Id. de conjunto de comprobantes’. No es un campo editable.

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

    Para el aplicativo SIFERE Retenciones Bancarias, se deberá configurar dos
    columnas en el reporte impositivo, de la siguiente manera:

    ![Interfaz de usuario gráfica, Aplicación, Word Descripción generada
    automáticamente](img/SIFERE/3f0605932a1497b169cd85a1abbc3f3d.png)

-   *Columna 1:* Monto de la Retención de Banco.

    Esta columna deberá configurarse para mostrar el importe de las retenciones
    a informar. Por ese motivo, en la grilla de Conjunto de impuestos por
    columna, se deberá configurar como ‘Impuesto: Monto’.

    *![Interfaz de usuario gráfica Descripción generada
    automáticamente](img/SIFERE/b24381b94e9a807a12c447f2ea4c2bd1.png)*

-   *Columna 2:* Total

    Esta columna deberá configurarse para mostrar sólo las transacciones que
    posean los códigos de impuestos configurados en la columna 1, y configurarla
    como ‘Excluir Comprobante en Cero’. En la grilla inferior deberá seleccionar
    ‘Impuesto: Monto Sujeto’ con el conjunto de comprobantes seleccionado en la
    Columna 1.

    ![Interfaz de usuario gráfica Descripción generada
    automáticamente](img/SIFERE/65b4cd32b2d8b5c8ed174492db5dc793.png)

**  
**

**Solapa General**

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/SIFERE/bedbac77f8a27fae64384ce6fee67874.png)

Los campos a completar son los siguientes:

-   *Ordenar por:* este campo permite indicar el orden a tomar en los
    documentos. Se recomienda la opción ‘Fecha + Comprobante + Número de
    documento’

-   *Cantidad de decimales:* este campo permite indicar la cantidad de decimales
    a mostrar en los campos de Tipo monto. Se recomienda colocar 2 decimales.

-   *Separados de miles:* este campo permite indicar el separador de miles a
    utilizar en el reporte a emitir, no del archivo. El archivo tomará como
    separador de miles el Punto (.)

-   *Separador de decimales:* este camp permite indicar el separador de
    decimales a utilizar en el reporte a emitir, no del archivo. El archivo
    tomará como separador de decimales la Coma (,).

    **Solapa de Formato**

    Se recomienda asignar un formato de reporte a efectos de poder visualizar la
    información ingresada y controlar el contenido de lo informado en el
    Archivo.

    ![Interfaz de usuario gráfica, Aplicación Descripción generada
    automáticamente](img/SIFERE/ee8f0775cb5eaa3a60a422906d6fe148.png)

**  
**

## Percepciones de Ingresos Brutos Aduana Sufridas

Los campos que integran el archivo son los siguientes:

-   *Código de Jurisdicción:* es la jurisdicción dada de alta en el aplicativo
    para el código de impuestos que represente la percepción.

    Para las percepciones el dato se toma del formulario Aplicativos del Código
    de impuesto. El formulario está ubicado en **JURISDICCIONES FISCALES → LATAM
    → APLICATIVO DE IMPUESTO.**

    ![Interfaz de usuario gráfica, Tabla Descripción generada
    automáticamente](img/SIFERE/6d901cd92d2c2b8e39f6816825aaf313.png)

    ![Interfaz de usuario gráfica, Aplicación Descripción generada
    automáticamente](img/SIFERE/40b3e2533af741de5c79ed8cb85ddcec.png)

    *Nota 1: se aclara que se podrá configurar un aplicativo para diferenciar y
    poder tomar los códigos de comprobantes, jurisdicciones, tipo de documentos,
    etc. Asegúrese de crear un Id de Aplicativo por cada Archivo Magnético que
    necesite.*

    *Nota 2: se aclara que a nivel de configuración requiere la creación de un
    código de Impuestos de Aduana (Percepción sufrida) para cada jurisdicción de
    Ingresos Brutos.*

    ![Tabla Descripción generada
    automáticamente](img/SIFERE/c375d620d177589e746b8ad151edcfb8.png)

-   *CUIT del Agente de Percepción:* es el número de identificación de País
    (CUIT) del proveedor que ha realizado la Percepción.

    La Aduana deberá crearse como un proveedor. Este campo se toma del maestro
    Proveedores, ubicado en la Solapa Latam

    ![Interfaz de usuario gráfica, Tabla Descripción generada
    automáticamente](img/SIFERE/8bf65a1a681dbaf38808dca3e3b3e633.png)

    *Nota: el cuit a informar es SOLO el de la Aduana*

-   *Fecha de la Percepción:* se trata de la Fecha de la Transacción en la cual
    se ha registrado la Percepción, es decir la fecha de Registro.

**![Tabla Descripción generada
automáticamente](img/SIFERE/140ca6d1e8cd19375df97fde44a58c11.png)**

-   *Número de Despacho Aduanero:* se trata del campo Número de Comprobante que
    contiene la Percepción, como por ejemplo Despacho. Debe asegurarse que al
    cargar la transacción se coloque allí el número de despacho.

    **![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico
    Descripción generada
    automáticamente](img/SIFERE/506aca7853215e734cc42158421a1509.png)**

    *Nota: el comprobante que representa el despacho debería configurarse con
    numeración manual.*

-   *Importe Percibido:* es el importe de la Percepción de Aduana. Para poder
    tomar el importe correcto de la Percepción de Aduana se requiere tener
    configurado un Código de Impuesto por cada Percepción de Ingresos Brutos
    para Aduana por cada jurisdicción. Adicionalmente debe asegurarse que, a
    nivel de la transacción, dicho código de impuesto, se encuentre asignado
    para que la Percepción se calcule y queden los datos relacionados a la
    transacción.

    **![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico
    Descripción generada
    automáticamente](img/SIFERE/506aca7853215e734cc42158421a1509.png)**

## Configuración del Reporteador de Impuestos

A efectos de la generación del Archivo de Percepciones de Aduana Sufridas será
necesaria la confección de un formato de reporte para esta salida en el
formulario ubicado en **CONFIGURACION → LATAM CONFIGURACION DE REPORTES →
REPORTE DE IMPUESTO.**

**![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/SIFERE/c89a135880800be32580abb3b78d099d.png)**

**Solapa general**

![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico Descripción
generada automáticamente](img/SIFERE/5e2f6604c8574ba9e21959c8a35be39b.png)

Los campos a completar son los siguientes:

-   *N°:* en este campo se deberá completar el código de identificación del
    reporte que se está parametrizando. Por ejemplo, SIF-PERCADA.

-   *Descripcion:* en este campo se deberá completar el NOMBRE LEGAL del
    reporte. Es muy importante este campo, ya que será la denominación legal que
    se imprimirá en el reporte. Por ejemplo, SIFERE- PERCEPCIONES ADUANAS.

Dentro de Acciones se podrán configurar las siguientes solapas:

![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico Descripción
generada automáticamente](img/SIFERE/c7000fce9a6837d7578913598bb3ec55.png)

**Solapa Secciones**

![Interfaz de usuario gráfica Descripción generada automáticamente con confianza
media](img/SIFERE/b055897bc17b5154cc9f928a831466f0.png)

Los campos a completar son los siguientes:

-   *Orden 1, 2, 3:* establecerá el orden en el que se mostrarán los
    comprobantes en el aplicativo.

-   *Grupo de clase de comprobante:* en este campo se deberá seleccionar los
    conjuntos de comprobantes previamente configurados en el formulario LATAM
    Lista de grupos de clase de comprobante. Dichos conjuntos deberán contener
    aquellos comprobantes que representen Percepciones sufridas de aduanas.

![Interfaz de usuario gráfica, Aplicación, Word Descripción generada
automáticamente](img/SIFERE/2e870f1159ab2258e3b752f0009f5d47.png)

-   *Descripcion:* este campo ampliará con una descripción el código indicado en
    el campo ‘Id. de conjunto de comprobantes’. No es un campo editable.

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

Para el aplicativo SIFERE Percepciones Sufridas de Aduana, se deberá configurar
dos columnas en el reporte impositivo, de la siguiente manera:

![Interfaz de usuario gráfica, Aplicación, Word Descripción generada
automáticamente](img/SIFERE/318afe4596f2d42820614cf0e45b24c3.png)

-   *Columna 1:* Monto de la Percepción de Aduana.

    Esta columna deberá configurarse para mostrar el importe de las percepciones
    a informar. Por ese motivo, en la grilla de Conjunto de impuestos por
    columna, se deberá configurar como ‘Impuesto: Monto’.

![Interfaz de usuario gráfica Descripción generada
automáticamente](img/SIFERE/1901d37c2464d4be17e52aa0833aa818.png)

-   *Columna 2:* Total

    Esta columna deberá configurarse para mostrar sólo las transacciones que
    posean los códigos de impuestos configurados en la columna 1, y configurarla
    como ‘Excluir Comprobante en Cero’. En la grilla inferior deberá seleccionar
    ‘Impuesto: Monto Sujeto’ con el conjunto de comprobantes seleccionado en la
    Columna 1.

![Interfaz de usuario gráfica Descripción generada
automáticamente](img/SIFERE/a8d61a2bf441c3f9f2ca85f39ced3404.png)

**Solapa General**

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/SIFERE/9cd20bfcc0064948d06423d955f5e5f4.png)

Los campos a completar son los siguientes:

-   *Ordenar por:* este campo permite indicar el orden a tomar en los
    documentos. Se recomienda la opción ‘Fecha + Comprobante + Número de
    documento’

-   *Cantidad de decimales:* este campo permite indicar la cantidad de decimales
    a mostrar en los campos de Tipo monto. Se recomienda colocar 2 decimales.

-   *Separados de miles:* este campo permite indicar el separador de miles a
    utilizar en el reporte a emitir, no del archivo. El archivo tomará como
    separador de miles el Punto (.)

-   *Separador de decimales:* este camp permite indicar el separador de
    decimales a utilizar en el reporte a emitir, no del archivo. El archivo
    tomará como separador de decimales la Coma (,).

**Solapa de Formato**

Se recomienda asignar un formato de reporte a efectos de poder visualizar la
información ingresada y controlar el contenido de lo informado en el Archivo.

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/SIFERE/578c5b3f670b48ff47bb9ae208ca7fc1.png)

## Definición de exportación de medios magnéticos

Una vez realizada la configuración general para cada archivo será necesario
configurar específicamente la exportación de los archivos, en el formulario
ubicado en **CONFIGURACION → LATAM CONFIGURACION DE REPORTES → DEFINICIÓN DE
MEDIOS MAGNÉTICOS.**

**![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/SIFERE/5cbab04ad4cacf2e3cfef583e2fddb27.png)**

**![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico
Descripción generada
automáticamente](img/SIFERE/b6cb157b96108e5291d884f9542c7e80.png)**

Se deberá configurar un registro por cada salida. Los campos a completar son los
siguientes:

**Solapa General**

**![Interfaz de usuario gráfica, Aplicación, Correo electrónico Descripción
generada automáticamente](img/SIFERE/1ffdc212b280ed1b1461b1d674c2850b.png)**

**Solapa general**

-   *ID Medio Magnetico:* es la identificación del código para exportación del
    archivo magnético. Se recomienda utilizar un código que el usuario que
    exportará el archivo, pueda distinguir.

-   *Descripción:* ingrese una descripción sobre el Tipo de Archivo a Exportar.

**Solapa configuración**

-   *Aplicativo de impuesto:* este campo permite seleccionar el código de
    aplicativo, previamente creado en el correspondiente maestro. Cabe destacar
    que este código también se recomienda crearlo con el mismo nombre que el del
    reporte impositivo. Este dato, le indicará al archivo de exportación qué ID
    de aplicativo tomar, para informar, en el caso de los campos que necesitan
    ser mapeados, como ser Tipos de comprobantes, Jurisdicciones, Monedas, etc.

-   *Aplicativo de impuesto secundario*

-   *Reporte de impuesto*

-   *Reporte ID:* este campo permite seleccionar el código de reporte impositivo
    creado de acuerdo a lo visto en pasos anteriores.

-   *Nombre del reporte:* este campo está vinculado al reporte elegido en el
    campo anteriormente mencionado.

**Parámetros**

-   *Parámetros:* en esta grilla se deberán agregar las distintas etiquetas que
    hacen al nombre del archivo a exportar y el tipo de extensión del archivo.

-   Nombre: SIFERE_PERCADA

-   Extensión: .txt

-   *Nombre del archivo:* en este campo se deberán concatenar los campos Nombre
    creados en la grilla Parámetros, precedidos por el símbolo \$ y sin espacios
    entre ellos.

-   *Nombre de archivo traducido:* este campo no es editable, solo tomará los
    campos Valor creados en la grilla Parámetros.

## Exportación de medios magnéticos

Desde este formulario se emitirá el archivo y se determinará dónde debe
guardarse, se puede acceder mediante el formulario ubicado **INFORMES → INFORMES
FINANACIEROS →LATAM MEDIOS MAGNETICOS → EXPORTACIÓN DE MEDIOS MAGNÉTICOS.**

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/SIFERE/ab9de4f685bcd7ad4f10ff63a77d2875.png)

![Interfaz de usuario gráfica, Tabla Descripción generada
automáticamente](img/SIFERE/53b32c17bfc6723770800ebf311f5bb8.png)

Los campos a completar son los siguientes:

-   *ID Medio Magnetico:* aquí se deberá seleccionar el ID de Exportación,
    configurado en el formulario Definición de exportación de medios magnéticos.

-   *Fecha desde:* es la fecha inicial a partir de la cual se mostrará la
    información. Será la fecha de Registración de las Transacciones.

-   *Fecha hasta:* es la fecha final hasta la cual se mostrará la información.
    Será la fecha de Registración de las Transacciones.

    Nota: al clickear Aceptar, se abre un pop up que nos indicará si deseamos
    abrir o guardar el archivo, y la ubicación que daremos al mismo.

    ![](img/SIFERE/13ac0ee0e108d006a941797e290927f9.png)

    Una vez finalizado el proceso de exportación, se mostrará la siguiente
    ventana:

    ![](img/SIFERE/2b7568f2773045d9f3cf75a127fb199e.png)

    **Ejemplos de Archivos exportados**

    SIFERE Percepciones Aduaneras:

    **![](img/SIFERE/9135628ba0555ddf089be62b9184a2c1.png)**

    SIFERE Percepciones Sufridas:

    **![](img/SIFERE/134b5fc4f5b5a126a64f981cbb785852.png)**

    SIFERE Retenciones Bancarias:

    **![](img/SIFERE/3ca8411094b8cb8749022dbc28603fd9.png)**

    SIFERE Retenciones Sufridas:

    ![](img/SIFERE/03ea56a1e03fe312f7cad4e5ba178edf.png)
