
## Objetivo

El presente manual tiene por objetivo explicar las configuraciones necesarias
para la emisión del aplicativo Ganancias.

Dicho aplicativo busca informar los importes inherentes a retenciones y
percepciones sufridas del Impuesto a las Ganancias en un período determinado.

## Archivo de Retenciones y Percepciones de Ingresos Brutos Sufridas

Los campos que integran el archivo son los siguientes:

* **Tipo de operación:** es el campo Código de Impuesto del Aplicativo para la
    Clase de comprobante o Código de Impuesto aplicable para la retención o
    percepción respectivamente.

    Para las retenciones el dato se toma del formulario Aplicativos de Clase de
    comprobante. El campo se toma del maestro Clase de comprobante ubicado en
    **LATAM \>\> CLASE DE COMPROBANTE \>\> APLICATIVO DE IMPUESTOS.**

    ![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico
    Descripción generada
    automáticamente](img/GananciasSociedades/GananciasSociedades-RetencionesPercepcionesIIBBSufridas.png)

    ![Interfaz de usuario gráfica, Aplicación Descripción generada
    automáticamente](img/GananciasSociedades/GananciasSociedades-RetencionesPercepcionesIIBBSufridas2.png)

    Para las percepciones el dato se toma del formulario Aplicativos del Código
    de Impuesto que tiene asociado el proveedor. El campo se toma del maestro
    Códigos de impuestos ubicado en El formulario está ubicado en
    **JURISDICCIONES FISCALES \>\> LATAM \>\> APLICATIVO DE IMPUESTOS.**

    ![Interfaz de usuario gráfica Descripción generada automáticamente con
    confianza baja](img/GananciasSociedades/d5b9bc545b9c31cf6a6642f4b96e26f0.png)

    ![Interfaz de usuario gráfica, Aplicación Descripción generada
    automáticamente](img/GananciasSociedades/1db1a3c5074991af737d84f24cc358cc.png)

    *Nota: Si se trata de una Retención, se informará el número ‘1’ en este
    campo. En cambio, si se trata de una Percepción, se informará el número ‘2’
    en este campo.*

* **CUIT del agente de retención:** es el número de identificación de País
    (CUIT) del proveedor o cliente. Este dato se tomará del maestro de Cliente o
    Proveedor, Solapa LATAM.

    **![Interfaz de usuario gráfica, Aplicación, Tabla Descripción generada
    automáticamente](img/GananciasSociedades/119be313e97d940acddedf38a2ea9811.png)**

    ![Interfaz de usuario gráfica, Tabla Descripción generada
    automáticamente](img/GananciasSociedades/f33e1f355d8379f946cd14479e6828dd.png)

* **Número de certificado:** es el número de comprobante de la línea valor del
    tipo retenciones sufridas (Cobros).

    El dato se tomará del campo ‘Número de Comprobante’ de la línea de la
    Retención.

    ![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico
    Descripción generada
    automáticamente](img/GananciasSociedades/0c3612c309e994f71bacf39511450b44.png)

    En Percepciones este dato no se informa.

* **Fecha de retención (DD/MM/YYYY):** es la fecha en que se registró el
    comprobante de retención/percepción.

    Para las Retenciones, el dato se tomará del campo Fecha de documento, de la
    línea de retenciones. Las transacciones se ingresarán mediante el formulario
    ubicado en **TESORERIA \>\> DIARIO DE PAGOS \>\> SECCION DE DIARIO.**

    *![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico
    Descripción generada
    automáticamente](img/GananciasSociedades/1c0a773152b7557f1c35eb3aae5ba4f7.png)*

    Para las Percepciones, el dato se tomará del campo Fecha de documento de
    compras, donde se registró el código de impuestos que representa a la
    percepción. Las transacciones se ingresarán mediante el formulario ubicado
    en **COMPRAS \>\> FACTURAS DE COMPRAS**

    **![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico,
    Sitio web Descripción generada
    automáticamente](img/GananciasSociedades/057d0c76806ad0bd145b72d5a0df63f1.png)**

* **Código de régimen:** es el campo Código de Régimen del Aplicativo para la
    Clase de comprobante o Código de Impuesto aplicable para la retención o
    percepción respectivamente.

    Para las retenciones el dato se toma del formulario Aplicativos de Clase de
    comprobante. El campo se toma del maestro Clase de comprobante ubicado en
    **PAGINA PRINCIPAL \>\> LATAM \>\> COMPROBANTES \>\> CLASE DE COMPROBANTE
    \>\> ACCIONES \>\> BOTÓN APLICATIVOS.**

    ![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico
    Descripción generada
    automáticamente](img/GananciasSociedades/7a332d77f9882e59ff368203c4ee8671.png)

    ![Interfaz de usuario gráfica Descripción generada automáticamente con
    confianza media](img/GananciasSociedades/7ee415c5117f6b9b13e0d64b8c4dced4.png)

    Para las percepciones el dato se toma del formulario Aplicativos del Código
    de Impuesto que tiene asociado el proveedor. El campo se toma del maestro
    Códigos de impuestos ubicado en **PAGINA PRINCIPAL \>\> BUSCAR\>\>
    JURISDICCIONES FISCALES \>\> LATAM \>\> APLICATIVOS DE IMPUESTOS.**

    ![Interfaz de usuario gráfica Descripción generada automáticamente con
    confianza baja](img/GananciasSociedades/d5b9bc545b9c31cf6a6642f4b96e26f0.png)

    ![Interfaz de usuario gráfica, Tabla Descripción generada automáticamente
    con confianza media](img/GananciasSociedades/17f10583ce410249c141574b9dd3f063.png)

## Configuración del Reporteador de Impuestos

A efectos de la generación del Archivo de Retenciones y Percepciones de
Ganancias Sufridas será necesaria la confección de un formato de reporte para
esta salida en el formulario ubicado **PAGINA PRINCIPAL \>\> CONFIGURACION \>\>
LATAM CONFIGURACION DE REPORTES \>\> REPORTES DE IMPUESTOS.**

**![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/GananciasSociedades/c89a135880800be32580abb3b78d099d.png)**

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/GananciasSociedades/8533124550f2d21f1388042c4576c648.png)

Los campos a completar son los siguientes:

* N°:* en este campo se deberá completar el código de identificación del
    reporte que se está parametrizando. Por ejemplo, RETPER GAN.

* Descripcion:* en este campo se deberá completar el NOMBRE LEGAL del
    reporte. Es muy importante este campo, ya que será la denominación legal que
    se imprimirá en el reporte. Por ejemplo, RET-PER GANANCIAS.

Se completarán las siguientes solapas

![Interfaz de usuario gráfica, Texto, Aplicación Descripción generada
automáticamente](img/GananciasSociedades/b3e41a6520c1f344774feafba09385c1.png)

**Solapa Secciones**

![Tabla Descripción generada
automáticamente](img/GananciasSociedades/fdade9003f0b5bf9c00aeeaed069ecba.png)

Los campos a completar son los siguientes:

* **Orden 1, 2, 3:** establecerá el orden en el que se mostrarán los
    comprobantes en el aplicativo.

* **Grupo de clase de comprobante:** en este campo se deberá seleccionar los
    conjuntos de comprobantes previamente configurados en el formulario Latam
    Lista de grupos de clase de comprobante.

    Un conjunto deberá contener aquellos comprobantes que representen
    Percepciones Sufridas:

    ![Interfaz de usuario gráfica, Aplicación, Word Descripción generada
    automáticamente](img/GananciasSociedades/21a1df720b7de68919fc6ae052db92a5.png)

    Otro conjunto para representar comprobantes que representan Retenciones
    Sufridas de Ganancias.

    ![Interfaz de usuario gráfica, Aplicación, Tabla Descripción generada
    automáticamente](img/GananciasSociedades/f5befd770a088711e8d2243e6421303d.png)

* **Nombre:** este campo ampliará con una descripción el código indicado en el
    campo ‘Id. de conjunto de comprobantes’. No es un campo editable.

* **Nombre para mostrar:** este campo se utilizará para asignar el nombre del
    conjunto que deberá visualizarse en el reporte. En caso de estar en blanco,
    en el reporte saldrá vacío.

* **Invertir el signo:** por cada conjunto de comprobantes se podrá determinar
    si en la visualización del reporte se debe invertir el signo. No será
    necesario marcar para este Archivo.

* **Filtrar por:** este campo permite seleccionar una de las opciones de
    filtrado que se aplicaran sobre el conjunto de comprobantes seleccionado. La
    opción recomendada es:

-   Sin filtro: no tiene en cuenta ninguna de las columnas siguientes.

**Solapa Columnas**

Para el aplicativo RET PER GANANCIAS se deberán configurar tres columnas en el
reporte impositivo, de la siguiente manera:

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/GananciasSociedades/e1644fc1dcb72c58c89e0a3653022088.png)

* **Columna 1:** Monto Retención

    Esta columna deberá configurarse para mostrar el importe de las retenciones
    a informar. Por ese motivo, en la grilla de Conjunto de impuestos por
    columna, se deberá configurar como ‘Retención: Monto’.

    ![Tabla Descripción generada
    automáticamente](img/GananciasSociedades/206dd25cf393464e3ebaada49fed92a3.png)

* **Columna 2:** Monto Percepción

    Esta columna deberá configurarse para mostrar el importe de las percepciones
    a informar. Por ese motivo, en la grilla de Conjunto de impuestos por
    columna, se deberá configurar como ‘Impuesto: Monto’.

    *![Tabla Descripción generada automáticamente con confianza
    media](img/GananciasSociedades/53f78773746e1602feda2e830fcac322.png)*

* **Columna 3:** Monto total

    Esta columna deberá configurarse para mostrar sólo las transacciones que
    posean los códigos de retención configurados en la columna 1 y los códigos
    de impuestos configurados en la columna 2, y configurarla como ‘Excluir
    Comprobante en Cero’.

    *![Tabla Descripción generada
    automáticamente](img/GananciasSociedades/9e085ae64d42966a4bd9e2d001b8e15c.png)*

**  
**

**Solapa General**

**![Interfaz de usuario gráfica Descripción generada
automáticamente](img/GananciasSociedades/e70ab4849922817de03ad9898ca892e4.png)**

Los campos a completar son los siguientes:

* **Ordenar por:** este campo permite indicar el orden a tomar en los
    documentos. Se recomienda la opción ‘Fecha + Comprobante + Número de
    documento’

* **Cantidad de decimales:** este campo permite indicar la cantidad de decimales
    a mostrar en los campos de Tipo monto. Se recomienda colocar 2 decimales.

* **Separados de miles:** este campo permite indicar el separador de miles a
    utilizar en el reporte a emitir, no del archivo. El archivo tomará como
    separador de miles el Punto (.)

* **Separador de decimales:** este camp permite indicar el separador de
    decimales a utilizar en el reporte a emitir, no del archivo. El archivo
    tomará como separador de decimales la Coma (,).

**Solapa de Formato**

Se recomienda asignar un formato de reporte a efectos de poder visualizar la
información ingresada y controlar el contenido de lo informado en el Archivo.

![Tabla Descripción generada
automáticamente](img/GananciasSociedades/8607ed8fc8aa51804b672d65600eaa67.png)

## Definición de exportación de medios magnéticos

Una vez realizada la configuración general para cada archivo será necesario
configurar específicamente la exportación de los archivos, en el formulario
ubicado **CONFIGURACION \>\> LATAM CONFIGURACION DE REPORTES \>\> DEFINICIÓN DE
MEDIOS MAGNÉTICOS.**

**![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/GananciasSociedades/5cbab04ad4cacf2e3cfef583e2fddb27.png)**

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/GananciasSociedades/558a52712d5460dd5d57b328008ce221.png)

![Interfaz de usuario gráfica, Aplicación, Correo electrónico Descripción
generada automáticamente](img/GananciasSociedades/eb4e2db0ea07bec6b0787b1aaa9f1ba0.png)

Se deberá configurar un registro por cada salida. Los campos a completar son los
siguientes:

**Solapa General**

* **ID Medio magnetico:** es la identificación del código para exportación del
    archivo magnético. Se recomienda utilizar un código que el usuario que
    exportará el archivo, pueda distinguir.

* **Descripción:** ingrese una descripción sobre el Tipo de Archivo a Exportar.

**Solapa configuración**

* **Aplicativo de impuesto:** este campo permite seleccionar el código de
    aplicativo, previamente creado en el correspondiente maestro. Cabe destacar
    que este código también se recomienda crearlo con el mismo nombre que el del
    reporte impositivo. Este dato, le indicará al archivo de exportación qué ID
    de aplicativo tomar, para informar, en el caso de los campos que necesitan
    ser mapeados, como ser Tipos de comprobantes, Jurisdicciones, Monedas, etc.

* **Reporte de impuesto reporte/servicio:** este campo permite seleccionar el
    código de reporte impositivo creado de acuerdo a lo visto en pasos
    anteriores.

* **Reporte ID:** ´TaxReportBase´ es el utilizado para Latam según la
    localización de Dynamics.

**Parámetros**

* **Parámetros:** en esta grilla se deberán agregar las distintas etiquetas que
    hacen al nombre del archivo a exportar y el tipo de extensión del archivo.
    Como mínimo se requieren:

-   **Nombre:** RETPERGCIA

-   **Extensión:** .txt.

* **Nombre del archivo:** en este campo se deberán concatenar los campos Nombre
    creados en la grilla Parámetros, precedidos por el símbolo \$ y sin espacios
    entre ellos.

* **Nombre de archivo traducido:** este campo no es editable, solo tomara los
    campos Valor creados en la grilla Parámetros.

## Exportación de medios magnéticos

Desde este formulario se emitirá el archivo y se determinará dónde debe
guardarse, se puede acceder mediante el formulario ubicado **INFORMES \>\>
INFORMES FINANACIEROS \>\> LATAM MEDIOS MAGNETICOS \>\> EXPORTACIÓN DE MEDIOS
MAGNÉTICOS.**

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/GananciasSociedades/ab9de4f685bcd7ad4f10ff63a77d2875.png)

![Tabla Descripción generada
automáticamente](img/GananciasSociedades/aed9040b693987510a6d6512b2a2ba8a.png)

Los campos a completar son los siguientes:

* **ID Medio Magnetico:** aquí se deberá seleccionar el ID de Exportación,
    configurado en el formulario Definición de exportación de medios magnéticos.

* **Fecha desde:** es la fecha inicial a partir de la cual se mostrará la
    información. Será la fecha de Registración de las Transacciones.

* **Fecha hasta:** es la fecha final hasta la cual se mostrará la información.
    Será la fecha de Registración de las Transacciones.

    Nota: al clickear Aceptar, se abre un pop up que nos indicará si deseamos
    abrirel archivo generado

    ![Interfaz de usuario gráfica, Texto Descripción generada
    automáticamente](img/GananciasSociedades/1926fb26487252fde5bc09553eaf63a6.png)

**Ejemplos de Archivos exportados**

RET PER GANANCIAS:

![Imagen que contiene Diagrama Descripción generada
automáticamente](img/GananciasSociedades/7b55bb9712cecb7d2a454c51cde556ef.png)
