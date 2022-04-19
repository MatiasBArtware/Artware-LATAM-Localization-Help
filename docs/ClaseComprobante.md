
## Objetivo

Este formulario permitirá dar de alta los diferentes comprobantes con los que
puede trabajar la compañía en relación con terceros. Ejemplo: Factura, Nota de
Débito, Nota de Crédito, etc.

Además, se utilizará para cargar comprobantes representativos de valores como
ser: Cheques al día, propios o diferidos y comprobantes utilizados en
transacciones de Tesorería como Recibo u Orden de Pago.

Para realizar la correspondiente configuración se deberá ingresar al formulario
ubicado en **LATAM → COMPROBANTE → CLASE DE COMPROBANTE.**

## Solapa General

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/ClaseComprobante/4b865bda7bbe66e3b3c24f04c75ffd6f.png)


Los campos para completar son:

-   *N°:* este campo deberá ser completado manualmente, identificando con un
    código al comprobante que se esté dando de alta.

*NOTA: Como se ha expresado anteriormente, aquí se podrán cargar los
comprobantes representantes de Medios de Cobro/Pago.*

-   *Descripción:* este campo deberá ser completado manualmente, ampliando con
    un detalle el código de comprobante que se esté dando de alta.

-   *Descripción legal:* este campo deberá ser completado manualmente, cuando se
    desee que en los reportes impositivos se muestre una descripción diferente a
    la utilizada en el sistema.

-   *Tipo clase comprobante:* en este campo se podrá seleccionar una única
    opción del menú desplegable. Las opciones disponibles para seleccionar serán
    las configuradas en el maestro de Tipo de clase de comprobante.

*NOTA: el Tipo de clase de comprobante determinará el comportamiento en la
configuración del Comprobante. Los Solapas que estarán disponibles para todos
los comprobantes serán: General, Nombres de diario, Datos Adicionales, Máscara
de documento y Dimensiones.*

*Si el Tipo de clase de comprobante seleccionado es un Medio de Cobro/Pago
(maestro de Tipo de clase de comprobante → Checkbox Medio de cobro/pago
habilitado); se visualizará una solapa adicional, Solapa Medio de Cobro/Pago, de
lo contrario no se visualiza.*

-   *Letra:* en este campo se podrá seleccionar una única opción del menú
    desplegable. Las opciones disponibles para seleccionar serán las
    configuradas en el maestro de Letra de clase de comprobante.

-   *Prefijo:* este campo será completado automáticamente por el sistema,
    concatenando el Prefijo configurado para el tipo de clase de comprobante y
    Prefijo configurado para la letra seleccionada. Este campo no podrá ser
    modificado. Si los prefijos de Letra de comprobante y/o Tipo de comprobante
    se encontraran vacíos, este campo se completará con los espacios en Blanco.

-   *Inactivo:* esta casilla de verificación permitirá inactivar un comprobante
    que no se utilice. Si el comprobante se encuentra utilizado en alguna
    transacción no se podrá eliminar, por lo que esta tilde impide que sea
    visualizado por el usuario final.

-   *Cálculo de Retención:* este campo permite en el caso de comprobante de
    pago, como ser ‘Orden de Pago’ calcular retenciones. Es importante tenerlo
    habilitado para tales comprobantes, de lo contrario no se calcularán
    retenciones en el mismo.

-   *Tasa de Cambio origen*: para el caso de los comprobantes utilizados para el
    pago como ‘Orden de Pago’, que apliquen documentos en Moneda extranjera, se
    puede indicar que para dichos comprobantes no se calcule diferencia de
    cambio.

    Si esta tilde se encuentra habilitado para la Orden de Pago, se
    sobrescribirá el Tipo de cambio cruzado con el Tipo de Cambio Original del
    documento aplicado de manera de no calcular Diferencia de cambio nativa.

    Este campo no estará disponible para los tipos de comprobantes ‘Medios de
    Cobro/Pago’.

-   *Separador:* en este campo se podrá configurar el separador del número de
    comprobante. Si se deja en blanco, el número de comprobante deberá
    concatenar Prefijo del Tipo de Comprobante, Prefijo de la Letra del
    Comprobante, Prefijo del Punto de Venta y Número de manera seguida. Por
    ejemplo: FCA000100000001

    Si se configura un separador, por ejemplo, el guion (-), éste se utilizará
    al formatear el número de comprobante. Por ejemplo: FCA-0001-00000001.

-   *Copiar documento:* este campo se utilizará para indicar en qué campo nativo
    deberá replicarse el número de comprobante. Las opciones para seleccionar
    son las siguientes:

-   *Ninguno:* el número de comprobante no se replicará en ningún campo nativo.

    -   *N° Doc. Interno:* si se encuentra marcada esta opción, el número de
        Documento completo se guardará en el campo nativo *Número de Documento
        Interno*.

    -   *N° Doc. Externo:* si se encuentra marcada esta opción, el número de
        documento completo se guardará en el campo nativo *Numero de Documento
        Externo*.

    -   *N° Doc. Interno & Externo:* se replicará en los campos *Número Interno
        & Externo* al mismo tiempo.

Es importante destacar que existen ciertos comprobantes que deberán contar con
una parametrización determinada, SIN EXCEPCIÓN, para el correcto funcionamiento
de los Diarios:

-   Comprobantes de Compras y Ventas (Facturas, Notas de Débito, Notas de
    Crédito): dichos comprobantes deberán estar configurados para replicar en
    Número de documento y Factura.

-   Comprobantes de Tesorería (Orden de Pago, Recibo) y Medios de Cobro/Pago
    (Cheques, Transferencias, etc.): dichos comprobantes deberán estar
    configurados para replicar únicamente en Número de documento.

*NOTA: Las opciones en donde se encuentran ubicados estos campos varían según la
transacción.*

-   *Requiere CA:* este campo de verificación indicará si la carga de número de
    CA será obligatoria al momento de cargar una transacción. En caso de no
    estar habilitada esta opción, en la solapa LATAM de las ventanas de
    registro, los campos CA y Fecha de Vencimiento no se deberán visualizar como
    datos adicionales de Transacciones.

-   *Código de control requerido:* este campo de verificación indicará si la
    carga del código de control será obligatoria al momento de cargar una
    transacción. En caso de no estar habilitada esta opción, en la solapa LATAM
    de las ventanas de registro, el campo Código de control no se deberá
    visualizar como datos adicionales de Transacciones.

-   *Tipo de código de control:* en este campo desplegable podrá seleccionar una
    de las siguientes opciones que indican como se generará el código:

    -   Manual: el código de control deberá ingresarse de forma manual en cada
        transacción y será un campo obligatorio.

    -   Automático: el código de control deberá generarlo el sistema para cada
        transacción de acuerdo con el algoritmo especificado en la
        configuración, y será un campo no editable. El campo Código de
        autorización auxiliar del maestro CA de ventas será un campo
        obligatorio, donde ingresar la Llave digital requerida para el cálculo.

-   *Etiqueta de Concepto 1, 2 y 3*: los conceptos serán campos alfanuméricos
    que permitirán guardar información adicional al momento de la carga de los
    comprobantes. En este maestro se configurarán las etiquetas para definir los
    conceptos. En la transacción, estos campos deberán visualizarse con la
    etiqueta configurada y a su vez, deberán permitir el ingreso de un cierto
    valor. Se podrán configurar hasta tres conceptos.

-   *Notas 1, 2 y 3:* Permitirá agregar información relacionada con el
    comprobante. No replicará en las ventanas transaccionales, pero si en la
    impresión del comprobante. Son campos de tipo memo*.*

-   *Reporte:* Mediante este campo se vincula el comprobante con un formato de
    reporte diseñado para su impresión. Las opciones disponibles a seleccionar
    serán las configuradas en el maestro de Configuración de reportes.

    Si existe un reporte está configurado en este campo, la ventana de Impresión
    de Documentos de Venta lo toma por default y no deja elegir otro.

    Si no está configurado, al momento de la impresión el sistema sugiere el Id
    de Reporte que en la ventana Referencia de reportes SSRS tiene configurado
    con el check correspondiente a Factura de venta, por ejemplo.

    Para emitir múltiples documentos que tengan diferente Id de Reporte, el
    sistema agrupa y muestra tantas ventanas de emisión como Id de Reporte
    existan en el conjunto seleccionado, aplicando la misma lógica que se
    describe antes.

*NOTA: aplica solo para los comprobantes comerciales de venta como Facturas,
Notas de Débito, Nota de Crédito y Remitos.*

-   *Detalla contribuyente:* este campo será utilizado, sí se requiere que, al
    momento de utilizar la clase de comprobante en una transacción, se requiera
    como obligatorios los datos impositivos del contribuyente. Al habilitar este
    campo automáticamente para el comprobante se configurará como Requerido los
    siguientes campos de la sección Datos adicionales:

-   Tipo de Contribuyente

-   Razón Social

-   País

-   Número de documento País

En caso de que la opción en este campo se encuentre activa, al momento de
ingresar la transacción, en la Sección LATAM, solicitará estos campos como
requeridos y el usuario deberá ingresarlos manualmente ya que no los hereda del
maestro del cliente o del proveedor. Sin embargo, para los comprobantes de tipo
Valor (cartera propio y cartera de terceros ) sí hereda los datos del maestro de
clientes/proveedores, tengan configurada la opción SI o NO en el campo Detalla
Contribuyente.

-   *Incluir impuestos:* este campo de verificación permitirá identificar sí el
    comprobante que se está configurando se ingresa con impuestos o sin
    impuestos.

    En Argentina se entiende por Comprobante con impuestos, los comprobantes que
    deben informarse a cualquier ente Fiscal a través del Libro IVA Compras e
    IVA Ventas, como son las Facturas, Notas de Débito y Notas de crédito, y
    demás comprobantes.

    Si el campo se encuentra habilitado validará que en un mismo asiento de:

-   Diario de Factura (Cuentas por pagar \>\> Diarios \>\> Factura \>\> Diarios
    de Factura)

-   Diario General (Contabilidad General \>\> Diarios \>\> Diarios General)

-   Diario de Pago (Cuentas por pagar \>\> Diarios \>\> Pagos \>\> Diarios de
    Pago)

-   Diario de Pago (Cuentas por cobrar \>\> Diarios \>\> Pagos \>\> Diarios de
    Pago)

    no se ingresé más de una línea de tipo Cliente o Proveedor con comprobante
    con impuestos, ni más de una línea con la misma moneda extranjera pero
    distinto tipo de cambio.

    Si el campo se encuentra deshabilitado no realizara tal validación.

## Solapa Medios de Cobro/Pago

En esta sección se ingresará toda la información relacionada con aquellos
comprobantes, cuyo Tipo de Comprobante posea tildada la opción Medio de
Cobro/Pago en el maestro Tipo de Clase de comprobante. Los campos incluidos allí
se habilitarán sólo si se cumple esta condición.

Esta sección estará compuesto por los siguientes campos:

-   *Tipo de Medio Cobro/Pago:* este campo será obligatorio si la sección se
    encuentra habilitada. Se trata de un menú desplegable, con las siguientes
    opciones:

-   **Cartera de Terceros**: esta opción será utilizada en medios como Cheques
    de Terceros, Tarjetas de Crédito/Débito, Prendas, Letras, Pagarés, etc.

![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico Descripción
generada automáticamente](img/ClaseComprobante/35cae7280431ab5fc0da32aafd802166.png)

Al seleccionarse esta opción, se habilitarán los siguientes campos para
configurar:

-   *Acciones:* las acciones Ingreso, Egreso y Reingreso se encontrarán
    habilitadas para este tipo de medio.

    La acción ‘Ingreso’ determinará la entrada del valor en la cuenta corriente
    del Cliente. Dicha entrada genera un documento con saldo en la cuenta
    corriente del Cliente. Por ejemplo: cobro mediante un Cheque de Terceros (Al
    día/diferido).

    La acción ‘Egreso’ determinará la salida del valor de la cuenta corriente
    del Cliente, por ejemplo: depósito de un Cheque de Terceros en un banco
    determinado. Esta acción genera que el valor quede con saldo 0,00 en la
    cuenta corriente.

    La acción ‘Reingreso’ se utilizará cuando sea necesario que un valor,
    previamente egresado, vuelva a ingresar a la cuenta corriente del Cliente.
    Por ejemplo: para el circuito de Cheques rechazados.

-   *Perfil de registración de cliente:* en este campo obligatorio se podrá
    seleccionar entre los perfiles de contabilización de Clientes. Este perfil
    se utilizará cada vez que se realicen transacciones con el medio asociado.

-   *Moneda:* en esta parte se podrán configurar los siguientes campos:

-   *Habilitar modificación de moneda de MCP:* si este campo de verificación se
    encuentra seleccionado, la moneda del medio podrá ser editada al momento de
    transaccionar en la ventana de Medios de cobro/pago. De no estar marcado
    este campo, no podrá modificarse la moneda del medio en la transacción.

-   *Moneda:* en este campo se podrá seleccionar la moneda predeterminada del
    medio.

-   *Fecha diferida:* al tildar este campo, el sistema controlará que la fecha
    del documento sea inferior a la fecha de vencimiento.

*NOTA:* En los Diarios, este Tipo de Valor generará una línea con el Tipo de
Cuenta: Cliente.

-   *Banco:* esta opción será utilizada en medios como Débitos Bancarios,
    Acreditaciones Bancarias, Transferencias Bancarias, y todo medio que afecte
    directamente a un Banco.

![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico Descripción
generada automáticamente](img/ClaseComprobante/864e31828fa5a7d15a2c8f5e9ea1f3d8.png)

![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico Descripción
generada automáticamente](img/ClaseComprobante/cdb65b6b33b6055dedcfed269d9f39c8.png)

![Interfaz de usuario gráfica, Texto, Aplicación Descripción generada
automáticamente](img/ClaseComprobante/1f00ea6a44f2e1e239dc9593ef244b84.png)

Al seleccionarse esta opción, se habilitarán los siguientes campos para
configurar:

-   *Grupo de campos “Acción”:* no admite acciones.

-   *Moneda:* en esta parte se podrán configurar los siguientes campos:

-   *Habilitar modificación de moneda de MCP:* si este campo de verificación se
    encuentra seleccionado, la moneda del medio podrá ser editada al momento de
    transaccionar en la ventana de Medios de cobro/pago. De no estar marcado
    este campo, no podrá modificarse la moneda del medio en la transacción.

-   *Moneda:* en este campo se podrá seleccionar la moneda predeterminada del
    medio.

-   *Fecha diferida:* al tildar este campo, el sistema controlará que la fecha
    del documento sea inferior a la fecha de vencimiento.

-   *Grilla “Cuenta Bancaria por clase de comprobante”:* se ingresará desde
    Acciones → Cuenta Bancaria; en esta grilla se deberán cargar los siguientes
    campos:

-   *Cuenta Bancaria:* en este campo desplegable se ofrecerán los registros de
    cuentas bancarias cargados en el formulario de Ficha Banco.

-   *Nombre:* este campo será la descripción de la cuenta bancaria.

Al momento de cargar una transacción, dicha configuración ofrecerá, de manera
predeterminada, la cuenta bancaria seleccionada en la grilla. En caso de haber
más de una cuenta bancaria cargada en la grilla, se deberá seleccionar cuál se
desea utilizar en la transacción.

*NOTA: En los Diarios, este Tipo de Valor generará una línea con el Tipo de
Cuenta: Banco.*

-   *Retenciones realizadas:* esta opción se utilizará para el ingreso de
    Retenciones que efectúa la compañía a sus proveedores en el pago.

![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico Descripción
generada automáticamente](img/ClaseComprobante/98b921b90d7fb2d370955ecffc91ff01.png)

Al seleccionarse esta opción, se habilitarán los siguientes campos para
configurar:

-   *Grupo de campos “Acción”:* no admite acciones.

-   *Moneda:* en esta parte se podrán configurar los siguientes campos:

-   *Habilitar modificación de moneda de MCP:* si este campo de verificación se
    encuentra seleccionado, la moneda del medio podrá ser editada al momento de
    transaccionar en la ventana de Medios de cobro/pago. De no estar marcado
    este campo, no podrá modificarse la moneda del medio en la transacción.

-   *Moneda:* en este campo se podrá seleccionar la moneda predeterminada del
    medio.

-   *Fecha diferida:* al tildar este campo, el sistema controlará que la fecha
    del documento sea inferior a la fecha de vencimiento.

-   *Grilla “Cuenta Bancaria por clase de comprobante”:* se ingresará desde
    Acciones → Cuenta Bancaria; en esta grilla se deberán cargar los siguientes
    campos:

-   *Cuenta Bancaria:* en este campo desplegable se ofrecerán los registros de
    retenciones cargados en el formulario de Detalles de Cuentas Bancarias.

-   *Nombre:* este campo será la descripción de la retención realizada.

Al momento de cargar una transacción, dicha configuración ofrecerá, de manera
predeterminada, la retención seleccionada en la grilla. En caso de haber más de
una retención cargada en la grilla, se deberá seleccionar cuál se desea utilizar
en la transacción.

*NOTA: En los Diarios, este Tipo de Valor generará una línea con el Tipo de
Cuenta: Banco.*

-   *Valores propios:* este tipo de medio se utilizará para representar los
    Cheques Propios al Día y cualquier otro documento emitido por la empresa,
    que no posea una fecha de Vencimiento.

![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico Descripción
generada automáticamente](img/ClaseComprobante/01a3849098b4aa6413e1fbe636ac6f3b.png)

Al seleccionarse esta opción, se habilitarán los siguientes campos para
configurar:

-   *Acciones:* las acciones Emisión y Cancelación se encontrarán habilitadas
    para este tipo de medio.

    La acción “Emisión” determinará la generación del valor para el pago de una
    deuda con un proveedor determinado, impactando directamente en el saldo de
    la cuenta bancaria asociada.

    La acción “Cancelación” se podrá utilizar, por ejemplo, cuando el proveedor
    haya rechazado el cheque emitido y sea necesario generar nuevamente la
    deuda.

-   *Moneda:* en esta parte se podrán configurar los siguientes campos:

-   *Habilitar modificación de moneda de MCP:* si este campo de verificación se
    encuentra seleccionado, la moneda del medio podrá ser editada al momento de
    transaccionar en la ventana de Medios de cobro/pago. La Cuenta Bancaria
    asociada al medio (si tuviera) deberá poseer la misma Moneda que la asociada
    al Valor, el sistema deberá impedir el cambio. De no estar marcado este
    campo, no podrá modificarse la moneda del medio en la transacción.

-   *Moneda:* en este campo se podrá seleccionar la moneda predeterminada del
    medio.

-   *Fecha diferida:* al tildar este campo, el sistema controlará que la fecha
    del documento sea inferior a la fecha de vencimiento.

-   *Grilla “Cuenta Bancaria por clase de comprobante”:* se ingresará desde
    Acciones → Cuenta Bancaria; en esta grilla se deberán cargar los siguientes
    campos:

-   *Cuenta Bancaria:* en este campo desplegable se ofrecerán los registros de
    cuentas bancarias cargados en el formulario de Ficha Banco.

-   *Nombre:* este campo será la descripción de la cuenta bancaria.

    Al momento de cargar una transacción, dicha configuración ofrecerá, de
    manera predeterminada, la cuenta bancaria seleccionada en la grilla. En caso
    de haber más de una cuenta bancaria cargada en la grilla, se deberá
    seleccionar cuál se desea utilizar en la transacción.

*NOTA: En los Diarios, este Tipo de Valor generará una línea con el Tipo de
Cuenta: Banco.*

-   *Cartera propia:* este tipo de medio se utilizará para representar los
    cheques Propios Diferidos o cualquier otro documento que posea fecha de
    Vencimiento*.*

![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico Descripción
generada automáticamente](img/ClaseComprobante/770f1cabe5d2107155471164ac119204.png)

Al seleccionarse esta opción, se habilitarán los siguientes campos para
configurar:

-   *Acciones:* las acciones Emisión, Devengamiento y Cancelación se encontrarán
    habilitadas para este tipo de medio.

    La acción “Emisión” se utilizará para realizar el pago a un proveedor
    determinado. No impactará directamente en la cuenta bancaria asociada al
    medio, ya que esta alternativa se utiliza para valores con diferimiento en
    la acreditación en la cuenta. En este momento, la deuda con el proveedor
    continúa existiendo y el valor se muestra en la cuenta corriente.

    La acción “Devengamiento” se utilizará para afectar la cuenta bancaria
    asociada al medio, quedando saldada la deuda con el proveedor.

    La acción “Cancelación” se utilizará para generar nuevamente la deuda con el
    proveedor en la cuenta corriente, por ejemplo, por un rechazo del valor.
    Esta acción podrá realizarse para valores antes o después de su
    Devengamiento, correspondiendo distintos movimientos a nivel de cuenta
    contable y cuenta corriente.

-   *Perfil de registración de proveedor:* en este campo obligatorio se podrá
    seleccionar entre los perfiles de contabilización de Proveedor. Este perfil
    se utilizará cada vez que se realicen transacciones con el medio asociado.

-   *Moneda:* en esta parte se podrán configurar los siguientes campos:

-   *Habilitar modificación de moneda de MCP:* si este campo de verificación se
    encuentra seleccionado, la moneda del medio podrá ser editada al momento de
    transaccionar en la ventana de Medios de cobro/pago. La Cuenta Bancaria
    asociada al medio (si tuviera) deberá poseer la misma Moneda que la asociada
    al Valor, el sistema deberá impedir el cambio. De no estar marcado este
    campo, no podrá modificarse la moneda del medio en la transacción.

-   *Moneda:* en este campo se podrá seleccionar la moneda predeterminada del
    medio.

-   *Fecha diferida:* al tildar este campo, el sistema controlará que la fecha
    del documento sea inferior a la fecha de vencimiento.

-   *Grilla “Cuenta Bancaria por clase de comprobante”:* se ingresará desde
    Acciones → Cuenta Bancaria; en esta grilla se deberán cargar los siguientes
    campos:

-   *Cuenta Bancaria:* en este campo desplegable se ofrecerán los registros de
    cuentas bancarias cargados en el formulario de Ficha Banco.

-   *Nombre:* este campo será la descripción de la cuenta bancaria.

Al momento de cargar una transacción, dicha configuración ofrecerá, de manera
predeterminada, la cuenta bancaria seleccionada en la grilla. En caso de haber
más de una cuenta bancaria cargada en la grilla, se deberá seleccionar cuál se
desea utilizar en la transacción.

*NOTA: En los Diarios, este Tipo de Valor generará una línea con el Tipo de
Cuenta: Proveedor, cuya contrapartida será Proveedor si la acción es Emisión.*

*Si la acción es Devengamiento, se generará una línea con el Tipo de Cuenta:
Proveedor, cuya contrapartida será Banco.*

-   *Retenciones sufridas:* esta opción se utilizará para el ingreso de
    Retenciones que realicen los clientes a la compañía.

![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico Descripción
generada automáticamente](img/ClaseComprobante/39ef1d5f86d62225e4b095fe35ef0fb5.png)

Al seleccionarse esta opción, se habilitarán los siguientes campos para
configurar:

-   *Acciones:* no admite acciones.

-   *Moneda:* en esta parte se podrán configurar los siguientes campos:

-   *Habilitar modificación de moneda de MCP:* si este campo de verificación se
    encuentra seleccionado, la moneda del medio podrá ser editada al momento de
    transaccionar en la ventana de Medios de cobro/pago. La Cuenta Bancaria
    asociada al medio (si tuviera) deberá posea la misma Moneda que la asociada
    al Valor, el sistema deberá impedir el cambio. De no estar marcado este
    campo, no podrá modificarse la moneda del medio en la transacción.

-   *Moneda:* en este campo se podrá seleccionar la moneda predeterminada del
    medio.

-   *Fecha diferida:* al tildar este campo, el sistema controlará que la fecha
    del documento sea inferior a la fecha de vencimiento.

-   *Grilla “Cuenta Bancaria por clase de comprobante”:* se ingresará desde
    Acciones → Cuenta Bancaria; en esta grilla se deberán cargar los siguientes
    campos:

-   *Cuenta Bancaria:* en este campo desplegable se ofrecerán los registros de
    retenciones cargados en el formulario de Detalles de Cuentas Bancarias.

-   *Nombre:* este campo será la descripción de la retención realizada.

Al momento de cargar una transacción, dicha configuración ofrecerá, de manera
predeterminada, la retención seleccionada en la grilla. En caso de haber más de
una retención cargada en la grilla, se deberá seleccionar cuál se desea utilizar
en la transacción.

*NOTA: En los Diarios, este Tipo de Valor generará una línea con el Tipo de
Cuenta: Banco.*

-   **Efectivo: esta opción será utilizada en medios de efectivo.**

![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico Descripción
generada automáticamente](img/ClaseComprobante/d5cd14da5d911be3393f6378b4cf0830.png)

Al seleccionarse esta opción, se habilitarán los siguientes campos para
configurar:

-   *Acciónes:* no admite acciones.

-   *Moneda:* en esta parte se podrán configurar los siguientes campos:

-   *Habilitar modificación de moneda de MCP:* si este campo de verificación se
    encuentra seleccionado, la moneda del medio podrá ser editada al momento de
    transaccionar en la ventana de Medios de cobro/pago. La Cuenta Bancaria
    asociada al medio (si tuviera) deberá posea la misma Moneda que la asociada
    al Valor, el sistema deberá impedir el cambio. De no estar marcado este
    campo, no podrá modificarse la moneda del medio en la transacción.

-   *Moneda:* en este campo se podrá seleccionar la moneda predeterminada del
    medio.

-   *Fecha diferida:* al tildar este campo, el sistema controlará que la fecha
    del documento sea inferior a la fecha de vencimiento.

-   *Grilla “Cuenta Bancaria por clase de comprobante”:* se ingresará desde
    Acciones → Cuenta Bancaria; en esta grilla se deberán cargar los siguientes
    campos:

-   *Cuenta Bancaria:* en este campo desplegable se ofrecerán los registros de
    cuentas bancarias cargados en el formulario de Ficha Banco.

-   *Nombre:* este campo será la descripción de la cuenta bancaria.

Al momento de cargar una transacción, dicha configuración ofrecerá, de manera
predeterminada, la cuenta bancaria seleccionada en la grilla. En caso de haber
más de una cuenta bancaria cargada en la grilla, se deberá seleccionar cuál se
desea utilizar en la transacción.

*NOTA: En los Diarios, este Tipo de Valor generará una línea con el Tipo de
Cuenta: Banco.*

## Solapa Nombres de Diario

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/ClaseComprobante/7e52db5301049cb93714db9e864f127b.png)

En esta seccion se podrán definir los Nombres de Diarios, en los cuales se
habilitará la selección del comprobante.

Los diarios que se podrán incluir son los que se hayan creado en el Maestro de
Nombres de Diario.

Botones disponibles:

-   *Nueva linea:* Al pulsar este botón el sistema creara una nueva línea para
    la sección.

-   *Borrar linea:* Al pulsar este botón se eliminará el nombre de Diario que
    contiene la grilla.

El campo Nombre de modelo de diario traerá un listado desplegable con todos los
Nombres de Diario que se encuentren configurados para el Tipo de medio de
Cobro/Pago y para el Tipo de Acción determinados. Si el comprobante no es un
medio de cobro/pago traerá todos los Nombres de Diario del maestro.

Si el comprobante es un medio de cobro/pago de tipo Cartera de Terceros, se
habilitarán dos columnas adicionales en la grilla: estado inicial y estado
final.

Se desplegarán en estos campos, los motivos que hayan sido creados en el maestro
de Códigos de Razón o motivos y que tengan el check de Cartera de Terceros.

![Tabla Descripción generada
automáticamente](img/ClaseComprobante/0db46f79d68f3512735d1e45966c2775.png)

Los estados aquí configurados son los que tomarán los comprobantes de tipo
Cartera de Terceros una vez hayan sido registrados y serán visibles en el campo
Código de razón o motivo en los diarios.

Los campos a ingresar son:

-   *Estado Inicial:* será el estado con el que ingresa el comprobante al
    Diario.

-   *Estado Final*: será el estado que tomará el comprobante una vez haya sido
    registrada la transacción en el diario especificado.

Ambos o uno de los campos podrán quedar vacíos de acuerdo con las necesidades de
configuración del comprobante.

## Solapa Datos Adicionales

![Tabla Descripción generada
automáticamente](img/ClaseComprobante/5f2f26f2bda2cdd22483d599cb795dcf.png)

En esta sección se detallará para cada opción, los campos que deberán
habilitarse cuando se registre una transacción parametrizada con cada tipo de
medio.

Los campos que podrán configurarse son los siguientes:

-   *Comportamiento de campos de datos adicionales*

-   *Conjunto de Banco:* esta opción se encontrará disponible para todas las
    clases de comprobantes. Permitirá, en la transacción en la cual se utilice
    el medio, seleccionar el banco al cual pertenece.

-   *Origen del Cheque:* esta opción se encontrará disponible para todas las
    clases de comprobantes. Permitirá, en la transacción en la cual se utilice
    el medio, seleccionar si el medio es Propio o de Terceros.

-   *Documento País:* esta opción se encontrará disponible para todos los
    comprobantes. Permitirá en la transacción en la cual se utilice informar el
    tipo de documento del cliente y el número de documento País, del cliente,
    proveedor, etc. Por ejemplo: CUIT y su número correspondiente.

-   *Beneficiario:* esta opción se encontrará disponible para todos los
    comprobantes. Este campo podrá utilizarse cuando el beneficiario sea
    distinto del Proveedor o Cliente.

-   *Número de cuenta del titular:* esta opción se encontrará disponible para
    todos los comprobantes. Se podrá utilizar, por ejemplo, para rellenar el
    número de cuenta corriente del cliente. Al transaccionar, deberá respetar el
    tipo de máscara configurada.

-   *Máscara del número de cuenta del titular:* este campo se encontrará
    disponible para todos los comprobantes. Se utilizará para completar con la
    máscara que deberá respetar el campo Número de cuenta del titular.

-   *Monto Base:* esta opción se encontrará disponible para todos los
    comprobantes. Se utilizará para los comprobantes de tipo ‘Retención’ y
    mostrará el monto sujeto de la Retención.

-   *Base acumulada:* esta opción se encontrará disponible para todos los
    comprobantes. En este campo se mostrará el monto sujeto de la Retención
    acumulado para un periodo de tiempo determinado.

-   *Monto acumulado:* esta opción se encontrará disponible para todos los
    comprobantes. En este campo se mostrará el monto de la Retención acumulado
    para un periodo de tiempo determinado.

-   *Alícuotas:* esta opción se encontrará disponible para todos los
    comprobantes. Se utilizará para los comprobantes de tipo ‘Retención’ y
    mostrará el porcentaje de la Retención.

-   *Tasa de cambio:* esta opción se encontrará disponible para todos los
    comprobantes. Se utilizará para los comprobantes de tipo ‘Retención’.

-   *Comportamiento de grupo contribuyente*

-   *Tipo de contribuyente:* esta opción se encontrará disponible para todos los
    comprobantes. Permitirá en la transacción en la cual se utilice, informar el
    tipo de contribuyente del cliente, proveedor, etc.

-   *Razón Social:* esta opción se encontrará disponible para todos los
    comprobantes. Permitirá en la transacción en la cual se utilice informar la
    razón social del cliente, proveedor, etc.

-   *País:* esta opción se encontrará disponible para todos los comprobantes.
    Permitirá en la transacción en la cual se utilice informar el país de
    radicación del cliente, proveedor, etc.

-   *N° de Documento:* esta opción se encontrará disponible para todos los
    comprobantes. Permitirá en la transacción en la cual se utilice informar el
    tipo de documento del cliente y el número de documento Pais, del cliente,
    proveedor, etc.

-   *Estado:* esta opción se encontrará disponible para todos los comprobantes.
    Permitirá en la transacción en la cual se utilice informar la jurisdicción
    dentro del país de radicación donde el cliente, proveedor, etc se encuentre
    inscripto para tributar por impuestos jurisdiccionales o provinciales.

-   *Documento Estado:* esta opción se encontrará disponible para todos los
    comprobantes. Permitirá en la transacción en la cual se utilice informar el
    tipo de documento del cliente y el número de documento Estado, del cliente,
    proveedor, etc. Por ejemplo: IIBB BS AS y su número correspondiente.

###Comportamiento de campos concepto

-   *Concepto 1:* esta opción se encontrará disponible para todos los
    comprobantes. Se podrá utilizar para completar con información adicional.

-   *Concepto 2:* esta opción se encontrará disponible para todos los
    comprobantes. Se podrá utilizar para completar con información adicional.

-   *Concepto 3:* esta opción se encontrará disponible para todos los
    comprobantes. Se podrá utilizar para completar con información adicional.

-   *Comportamiento de campos lista*: En estos campos se determina cual será el
    comportamiento de las listas creadas en el maestro de campos lista, en el
    comprobante

-   *Lista 1…Lista 10:* Se usará para vincular listas al comprobante. Para cada
    concepto, podrá seleccionarse una de las siguientes opciones:

-   *Deshabilitado:* para este tipo de comprobante, el campo se encontrará
    deshabilitado y no se mostrará en la ventana de la transacción en la cual se
    esté utilizando el comprobante así configurado.

-   *Habilitado:* para este tipo de comprobante, el campo se encontrará
    habilitado para ser editado pero no será requerida su carga obligatoria en
    la transacción.

-   *Requerido:* para este tipo de comprobante, el campo se encontrará
    habilitado para ser editado y su carga será obligatoria en la transacción.

## Solapa Máscara de documento

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/ClaseComprobante/f5fa9d45476b12d1805f9f15e5096046.png)

Los campos a completar para cada tipo de cuenta son:

-   *Grupo de campos “Punto de Venta”:* este grupo de campos sólo podrán ser
    editados si la casilla de verificación *Habilitado* se encuentra tildada. Si
    está casilla se encuentra tildada, se deberán completar los siguientes
    campos:

-   *Longitud:* en este campo se indicará la longitud admitida para el campo
    Punto de venta en las transacciones.

-   *Máscara:* en este campo se indicará el formato de máscara admitido en la
    carga de comprobantes. La cantidad de caracteres se completa
    automáticamente, pues debe ser exactamente la misma que la definida en
    Longitud.

Es posible configurar máscaras de longitud fija:

-   Admite caracteres alfanuméricos (X)

-   Admite únicamente caracteres numéricos (9).

-   Admite únicamente caracteres alfabéticos (A).

Es posible configurar máscaras de longitud variable:

-   Autocomplete con ceros a la izquierda (0).

-   Rellene con espacios en blanco (Y).

*NOTA: en Colombia los comprobantes utilizan mascara de longitud variable.*

-   *Tipo de Entrada:* en este campo se podrá seleccionar una de las siguientes
    opciones:

-   *Automático:* si se encuentra seleccionada esta opción, el campo Punto de
    venta deberá seleccionarse del maestro Puntos de venta.

-   *Manual:* si se encuentra seleccionada esta opción, el campo de Punto de
    venta deberá completarse manualmente y será editable en la transacción.

-   *Campo “Obligatorio”:* si este campo de verificación se encuentra tildado,
    la carga del punto de venta será obligatoria al momento de ingresar la
    transacción. De lo contrario podrá dejarse en blanco.

-   *Grupo de campos “Número de comprobante”:* en este grupo de campos se
    deberán completar las siguientes opciones:

-   *Campo “Obligatorio”:* si este campo de verificación se encuentra tildado,
    la carga del número de comprobante será obligatoria al momento de ingresar
    la transacción. De lo contrario podrá dejarse en blanco.

-   *Validar Máscara:* Esta opción estará únicamente disponible, sí la
    parametrización en el campo ‘Entrada’ es Manual. Se utilizará para aquellos
    comprobantes, donde el número de comprobante es de longitud variable y no
    requiere de máscara alguna. Al seleccionarse este campo, los campos Longitud
    y Mascara, tanto para el punto de venta como para el Número de comprobante
    son no editables.

-   *Longitud:* en este campo se indicará la longitud admitida para el campo
    Número de comprobante en las transacciones. Este campo admite un máximo de
    20 caracteres si no se utiliza el punto de venta y no se configura separador
    de número de comprobante.

-   *Máscara:* en este campo se indicará el formato de máscara admitido en la
    carga de comprobantes. La cantidad de caracteres se completa
    automáticamente, pues debe ser exactamente la misma que la definida en
    Longitud.

    Es posible configurar máscaras de longitud fija:

-   Admite caracteres alfanuméricos (X)

-   Admite únicamente caracteres numéricos (9).

-   Admite únicamente caracteres alfabéticos (A).

    Es posible configurar máscaras de longitud variable:

-   Autocomplete con ceros a la izquierda (0).

-   Rellene con espacios en blanco (Y).

*NOTA: en Colombia los comprobantes utilizan mascara de longitud variable.*

-   *Tipo de Entrada:* este campo vendrá dado por lo configurado en el campo
    Entrada del Punto de venta.

-   *Automático*: si en el campo Entrada del Punto de venta se encuentra
    seleccionada esta opción, en este campo se replicará la misma y no podrá ser
    editada.

-   *Manual*: si en el campo Entrada del Punto de venta se encuentra
    seleccionada esta opción, en este campo se replicará la misma y no podrá ser
    editada.

-   *Tipo Asignación:* este campo sólo estará disponible para ser editado cuando
    el campo Entrada del Número de comprobante se encuentre configurado como
    Automático. Se podrá seleccionar una de las siguientes opciones:

-   *Antes de registrar*: esta configuración permitirá asignar el número de
    comprobante en un momento previo a la registración de la transacción. Para
    ello, el sistema buscará en la secuencia numérica configurada en el maestro
    de Clase de comprobante en Punto de Venta, a partir de la información de
    Clase de comprobante, Punto de Venta y Tipo de Cuenta seleccionado en la
    transacción, asignando el siguiente número correlativo.

-   *Después de registrar:* esta configuración permitirá asignar el número de
    comprobante en un momento posterior a la registración de la transacción. En
    este caso el campo Numero de documento permanecerá grisado y sin numeración,
    con la leyenda Pendiente, hasta que la transacción se registre. Luego, el
    sistema buscará en la secuencia numérica configurada en el maestro de *Clase
    de comprobante en Punto de Venta*, a partir de la información de Clase de
    comprobante, Punto de Venta y Tipo de Cuenta seleccionado en la transacción,
    asignando el siguiente número correlativo.

-   *Al Facturar:* esta configuración permitirá asignar el número de comprobante
    mediante conexión con un servicio externo.

Es el caso de Argentina, donde es el organismo fiscal, AFIP, quien asigna el
número de documento a los documentos de venta a través de una conexión por Web
Services. El campo Numero de documento permanecerá grisado y sin numeración, con
la leyenda Pendiente inclusive después de registrada la transacción, hasta que
se realice el llamado al servicio externo y este apruebe y asigne la numeración.

## Solapa Dimensiones

![Interfaz de usuario gráfica, Aplicación, Correo electrónico Descripción
generada automáticamente](img/ClaseComprobante/a4ede507bb293db687c84e396d41e8c4.png)

Para acceder a esta sección, se debe ingresar a Acciones → Dimensiones dentro
del comprobante seleccionado.

![Interfaz de usuario gráfica, Texto, Aplicación Descripción generada
automáticamente](img/ClaseComprobante/ced657de3193869d1c4425f540c458ec.png)

En esta sección, se podrán configurar dimensiones predeterminadas, para que se
asignen de forma automática en el momento de seleccionar el comprobante para
transaccionar.

Para la asignación de Dimensiones, la secuencia a seguir será la siguiente:

-   Si el Comprobante en Punto de Ventas posee dimensiones configuradas, éstas
    serán las que se asignarán en la transacción. Esta configuración no aplica
    para los comprobantes de entrada Manual.

-   Si el Comprobante en Punto de Ventas no posee dimensiones configuradas, pero
    sí el Comprobante, éstas serán las que se asignarán al momento de
    transaccionar.

-   Por último, buscará la configuración nativa de Dimensiones, en el maestro de
    Clientes o Proveedores.

Cabe destacar que, si al momento de transaccionar, las dimensiones asignadas son
modificadas manualmente por el usuario, éstas prevalecen.

Al momento de transaccionar, siempre que se seleccionen comprobantes de tipo
Valor mediante, estos comprobantes deberán heredar las dimensiones asignadas en
el momento de Ingreso. Este comportamiento es válido en todos los casos en los
cuales se seleccionen Valores mediante todas las alternativas de selección
existentes (Anulación – Devengamiento – Reingreso – Egreso).

## Botón Aplicativos

![Interfaz de usuario gráfica, Aplicación, Correo electrónico Descripción
generada automáticamente](img/ClaseComprobante/e0478ef1b0a899e15dd99e24ddf218fc.png)

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/ClaseComprobante/be39a79f655e9607925d5b296eb37f2e.png)

Este formulario se utilizará para configurar todos los códigos necesarios para
la importación en los diferentes soportes magnéticos y confección de informes
impositivos, relacionados con el comprobante. Se podrá acceder a esta ventana
mediante el Botón Aplicativos, ubicado sobre el margen superior de la ventana.

Los campos para completar son los siguientes:

-   *Aplicativo:* este campo desplegable permite seleccionar uno de los códigos
    de soportes magnéticos dados de alta en el maestro de Aplicativos.

-   *Descripción:* este campo ampliará la información del aplicativo. No podrá
    ser editado manualmente.

-   *Código de aplicativo:* en este campo se deberá ingresar manualmente el
    código con el que se reconoce al comprobante en el soporte magnético
    seleccionado.

-   *Código de letra*: este campo se deberá ingresar manualmente el código de
    letra con el que se reconoce al comprobante en el soporte magnético
    seleccionado. Es un campo optativo y sólo algunos aplicativos lo utilizan.

## Clase de Comprobante en Punto de Ventas

![Interfaz de usuario gráfica, Aplicación, Tabla, Correo electrónico Descripción
generada automáticamente](img/ClaseComprobante/45e55e2716937ab41e62c2bdabdbfe38.png)

Se podrá acceder a esta ventana ingresando a **LATAM → COMPROBANTE → CLASE DE
COMPROBANTE PUNTO DE VENTA**.

Este botón permitirá ingresar o consultar los registros existentes.

*NOTA: Para más información, ver manual AWF11- D365BC-Manual MAE Clase de
comprobante en Punto de Venta.*

## EJEMPLOS

A continuación, se mostrará un ejemplo de configuración para cada tipo de medio
de Cobro/Pago:

## Ejemplo de tipo de medio de Cobro/Pago “Cartera de Terceros”

**Solapa General**

En esta sección, se deberá configurar que el número de comprobante LATAM se
replique en el campo Número de documento nativo, en las transacciones de Diario.

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/ClaseComprobante/db29a38b72c1795992895a9bf70dfcc6.png)

**Solapa Medios de Cobro/Pago**

En esta sección, los campos se deberán configurar de la siguiente forma:

-   *Tipo de medio cobro/pago:* Cartera de terceros

-   *Acción:* Ingreso - Egreso – Reingreso

-   *Perfil de asiento contable:* se deberá seleccionar un perfil llamado
    “Cheque de terceros” o similar, previamente dado de alta en el formulario
    Perfil de asiento contable de Cliente.

-   *Moneda:* se deberá seleccionar la moneda en la cual trabajará el medio.

-   *Fecha diferida:* campo tildado o destilado, dependiendo de si el valor es
    al día o diferido.

![Interfaz de usuario gráfica Descripción generada
automáticamente](img/ClaseComprobante/eb0d66cce47d0523b414b34b1bfa2f5b.png)

**Solapa Nombres de Diario**

En esta seccion, se deberá seleccionar un Nombre de Diario apropiando al medio
(Deberá darse de alta previamente en el maestro de Nombres de Diario), y asignar
el estado que inicial y/o final que tomará el comprobante en cada uno de ellos
luego del registro de la transacción.

![Tabla Descripción generada
automáticamente](img/ClaseComprobante/7b7751c5c299105635af08e8ee439ad7.png)

**Solapa Datos Adicionales**

Los siguientes datos adicionales deberán configurarse como campos Requeridos:

-   *Comportamiento de grupo bancos*

-   *Origen de cheque*

-   *Tipo de contribuyente*

-   *País*

-   *N° Documento País*

-   *Razón social*

![Tabla Descripción generada
automáticamente](img/ClaseComprobante/5a50c003320f0fe65e2f54f095b7b305.png)

**Solapa Máscara de documento**

En esta sección, se deberán configurar la siguiente máscara:

-   *Cliente: en este caso, el tipo de máscara es Manual, porque para los
    cheques recibidos de Clientes, el número deberá ingresarse manualmente.*

![Interfaz de usuario gráfica, Aplicación, Correo electrónico Descripción
generada automáticamente](img/ClaseComprobante/1bdc9bd7355e86f5760e9b4ed7fcafb2.png)

## Ejemplo de tipo de medio de cobro/pago “Banco”

**Solapa General**

En esta sección, se deberá configurar que el número de comprobante LATAM se
replique en el campo Número de documento nativo, en las transacciones de Diario.

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/ClaseComprobante/191d82461540a142da99463ddfff3388.png)

**Solapa Medios de Cobro/Pago**

En esta sección, los campos se deberán configurar de la siguiente forma:

-   *Tipo de medio cobro/pago:* Banco

-   *Moneda:* se deberá seleccionar la moneda en la cual trabajará el medio.

-   *Cuentas bancarias:* se deberán seleccionar las cuentas con las que
    trabajará este medio.

![Interfaz de usuario gráfica, Texto, Correo electrónico Descripción generada
automáticamente](img/ClaseComprobante/96f626a15e302f8971aada038a168788.png)

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/ClaseComprobante/d57f245539713912710905cc9def70eb.png)

**Solapa Nombres de Diario**

En esta sección, se deberá seleccionar un Nombre de Diario apropiando al medio,
este deberá configurarse previamente el maestro de Nombres de Diario.

![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico Descripción
generada automáticamente](img/ClaseComprobante/5e2a3f4e16baa6605caf236bcda3caf2.png)

**Solapa Datos Adicionales**

Para este tipo de medio, no es necesario seleccionar Datos Adicionales.

![Tabla Descripción generada
automáticamente](img/ClaseComprobante/32401113db467e1a2c3a062d10a94874.png)

**Solapa Máscara de documento**

En esta sección, se deberá configurar la siguiente máscara:

-   *Banco*

![Interfaz de usuario gráfica, Aplicación, Correo electrónico Descripción
generada automáticamente](img/ClaseComprobante/38288ee030fcc3ea619e2a779cf62ce2.png)

## Ejemplo de tipo de medio de cobro/pago “Retención”

**Solapa General**

En esta sección, se deberá configurar que el número de comprobante LATAM se
replique en el campo Número de documento nativo, en las transacciones de Diario.

![Interfaz de usuario gráfica, Aplicación, Tabla Descripción generada
automáticamente](img/ClaseComprobante/efe86e505e6ab8d6a336eea596123bed.png)

**Solapa Medios de Cobro/Pago**

En esta sección, los campos se deberán configurar de la siguiente forma:

-   *Tipo de medio cobro/pago:* Retención

-   *Moneda:* se deberá seleccionar la moneda en la cual trabajará el medio.

-   *Cuentas bancarias:* se deberán seleccionar las cuentas con las que
    trabajará este medio.

![Tabla Descripción generada
automáticamente](img/ClaseComprobante/77e5831b3d6e754b32a750a698d9c6c6.png)

![Interfaz de usuario gráfica, Texto, Aplicación Descripción generada
automáticamente](img/ClaseComprobante/7b4ea0a1e0726c56a38ef5370e33b8a2.png)

**Solapa Nombres de Diario**

En esta sección, se deberá seleccionar un Nombre de Diario apropiando al medio,
éste deberá darse de alta previamente en el maestro de Nombres de Diario.

![Tabla Descripción generada
automáticamente](img/ClaseComprobante/edf7c194a369818b1b52020f86e60073.png)

**Tab Datos Adicionales**

Para este tipo de medio, se podrán seleccionar los siguientes datos adicionales:

-   *Monto Base*

-   *Base acumulada*

-   *Monto acumulado*

-   *Alícuota*

![Tabla Descripción generada
automáticamente](img/ClaseComprobante/15553c997a5c55fd33ac508de7b38bc5.png)

**Solapa Máscara de documento**

**E**n esta sección, se deberán configurar la siguiente máscara:

-   Banco*: normalmente, este tipo de Valor se configura con una máscara Manual.
    Pero, dependiendo del caso, podrá ser Automática.*

![Interfaz de usuario gráfica, Aplicación, Correo electrónico Descripción
generada automáticamente](img/ClaseComprobante/34eaabc6a1d841c730146fab62bd9893.png)

## Ejemplo de tipo de medio de cobro/pago “Valores Propios”

**Solapa General**

En esta sección, se deberá configurar que el número de comprobante LATAM se
replique en el campo número de Documento nativo, en las transacciones de Diario.

![Interfaz de usuario gráfica, Aplicación, Correo electrónico Descripción
generada automáticamente](img/ClaseComprobante/f67cec3ba8b10577b265d59eba660a08.png)

**Solapa Medios de Cobro/Pago**

En esta sección, los campos se deberán configurar de la siguiente forma:

-   *Tipo de medio cobro/pago:* Valores Propios.

-   *Moneda:* se deberá seleccionar la moneda en la cual trabajará el medio.

-   *Cuentas bancarias:* se deberán seleccionar las cuentas con las que
    trabajará este medio.

![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico Descripción
generada automáticamente](img/ClaseComprobante/cf85a7bca02f0648f59b13af9456089a.png)

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/ClaseComprobante/7fb78da5b07f0d533812642b154c6627.png)

**  
**

**Solapa Nombres de Diario**

En esta sección, se deberá seleccionar un Nombre de Diario apropiando al medio,
el cual deberá darse de alta previamente en el maestro de Nombres de Diario.

![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico Descripción
generada automáticamente](img/ClaseComprobante/5d24355135df288867eb3bd5245b28e2.png)

**Solapa Datos Adicionales**

Para este tipo de medio, se podrán seleccionar los siguientes datos adicionales:

-   *Tipo de contribuyente*

-   *Pais*

-   *Número de documento*

-   *Razón social*

-   *Beneficiario.*

![Tabla Descripción generada
automáticamente](img/ClaseComprobante/dbc298d08ae0a86432abde901fd80eda.png)

**Solapa Máscara de documento**

En esta sección, se deberán configurar las siguientes máscaras:

-   *Banco:* normalmente, la configuración de la máscara será Automática, porque
    se trata de Cheques propios, emitidos por la compañía y, de esta forma, el
    número de cheque se asignará de acuerdo a la secuencia numérica de la
    chequera, configurada en el maestro de Clase de comprobante en Punto de
    Venta.

![Interfaz de usuario gráfica, Aplicación, Correo electrónico Descripción
generada automáticamente](img/ClaseComprobante/de7a2ae1b248461c53766670963171a9.png)

## Ejemplo de tipo de medio de cobro/pago “Cartera Propia”

**Solapa General**

En esta sección, se deberá configurar que el número de comprobante del tab LATAM
se replique en el campo número de Documento nativo, en las transacciones de
Diario.

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](img/ClaseComprobante/646c4c1ae668647d74ddeccc239b3ec2.png)

**  
**

**Solapa  Medios de Cobro/Pago**

En esta sección, los campos se deberán configurar de la siguiente forma:

-   *Tipo de medio cobro/pago:* Cartera propia.

-   *Acción:* Emisión – Devengamiento – Anulación

-   *Perfil de asiento contable:* se deberá seleccionar un perfil llamado
    “Cheque propio diferido” o similar, previamente dado de alta en el
    formulario Perfil de asiento contable de Proveedor.

-   *Moneda:* se deberá seleccionar la moneda en la cual trabajará el medio.

-   *Cuentas bancarias:* se deberán seleccionar las cuentas con las que
    trabajará este medio.

![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico Descripción
generada automáticamente](img/ClaseComprobante/e7957115e0c1c2874b8943ee094cf20d.png)

![Interfaz de usuario gráfica, Texto, Aplicación Descripción generada
automáticamente](img/ClaseComprobante/996a47efac6803841395397ed7d78228.png)

**Solapa Nombres de Diario**

En esta sección, se deberá seleccionar un Nombre de Diario apropiando al medio,
el mismo deberá darse de alta previamente en el maestro de Nombres de Diario.

![Interfaz de usuario gráfica, Texto, Aplicación, Correo electrónico Descripción
generada automáticamente](img/ClaseComprobante/8796a3196d8124c2da082762b9e6ba92.png)

**  
**

**Solapa Datos Adicionales**

Para este tipo de medio, se podrán configurar los siguientes datos adicionales:

-   *Comportamiento de grupo banco*

-   *Origen del cheque*

-   *Beneficiario*

-   *Tipo de contribuyente*

-   *Razón social*

-   *Pais*

-   *N° de documento*

![Tabla Descripción generada
automáticamente](img/ClaseComprobante/208e61c45c64efb16cd6ee46d9e2706c.png)

**Solapa Máscara de documento**

En esta sección, se deberán configurar las siguientes máscaras:

-   *Proveedor:* normalmente, la configuración de la máscara será Automática,
    porque se trata de Cheques propios, emitidos por la compañía y, de esta
    forma, el número de cheque se asignará de acuerdo a la secuencia numérica de
    la chequera, configurada en el maestro de clase de Comprobante en Punto de
    Venta.

![Interfaz de usuario gráfica, Aplicación, Correo electrónico Descripción
generada automáticamente](img/ClaseComprobante/dffdebe88146edcced1b2ebe47a45283.png)
