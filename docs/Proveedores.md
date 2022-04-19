Objetivo

Esta sección permitirá agregar datos adicionales de proveedores, requeridos a nivel
informativo, que serán de utilidad para cumplir con las formalidades de las
regulaciones impositivas.

Para realizar la correspondiente configuración se deberá ingresar al Maestro de
Proveedores, y al proveedor seleccionado ingresar a la Sección Latam

**Solapa LATAM**

**![Interfaz de usuario gráfica, Tabla Descripción generada
automáticamente](img/Proveedores/0445d59f772c8e68e16e7642347b62c7.png)**

Los campos a completar son los siguientes:

-   *Tipo de contribuyente:* en este campo desplegable se podrá seleccionar del
    maestro Tipo de contribuyente, el que corresponda a la condición del
    proveedor. Por ejemplo, sí se trata en una compañía radicada en Argentina como
    tipo de contribuyente se podrán seleccionar responsable Inscripto,
    Monotributista, Exento, etc.

-   *País de radicación:* en este campo desplegable se deberá seleccionar el
    País donde se encuentra radicado el proveedor, se validará que los países
    ofrecidos como opciones correspondan para el tipo de contribuyente
    seleccionado.

-   *Tipo documento de país:* este campo desplegable solo permitirá seleccionar
    tipos de documento país que surjan de la intersección entre los tipos
    admitidos para el País donde se encuentra radicado el proveedor, y los
    configurados para el tipo de contribuyente seleccionado. Este campo será
    obligatorio o no a partir de lo configurado en el maestro Tipo de
    Contribuyente.

-   *N° documento país:* en este campo se deberá ingresar manualmente el número
    que identifica al proveedor frente al Fisco Nacional, o de su país en caso de
    ser del exterior, siempre respetando la máscara configurada en el maestro
    Tipo Documento.

Se recomienda la siguiente configuración:

-   Si el contribuyente no es interno y no es del exterior, el Número de
    identificación país debería ser obligatorio.

-   Si el contribuyente es interno, el Número de identificación país debería ser
    No obligatorio.

-   Si el contribuyente es del exterior, el Número de identificación país podría
    ser obligatorio o no.

Este campo será obligatorio o no dependiendo de lo configurado en el maestro
Tipo de Contribuyente.

-   *Inscripto en jurisdicción:* en este campo se deberá seleccionar el código
    de estado o provincia en el que se encuentra inscripto el proveedor, en caso
    de tributar impuestos jurisdiccionales o provinciales.

Se recomienda la siguiente configuración:

-   Si el contribuyente no es interno ni del exterior, el Inscripto en
    jurisdicción debería ser obligatorio.

-   Si el contribuyente es interno, el Inscripto en jurisdicción debería ser No
    obligatorio.

-   Si el contribuyente es del exterior, el Inscripto en jurisdicción podría ser
    obligatorio o no.

Este campo será obligatorio dependiendo de lo configurado en el maestro Tipo de
Contribuyente.

-   *Tipo documento de estado:* este campo desplegable solo permitirá
    seleccionar tipos de documento estado que surjan de la intersección entre
    los tipos admitidos para el Estado donde se encuentra inscripto el proveedor,
    y los configurados para el tipo de contribuyente seleccionado.

-   *Número de identificación de estado:* en este campo se deberá ingresar
    manualmente el número que identifica al proveedor frente al Fisco de la
    Jurisdicción, siempre respetando la máscara configurada en Tipo de
    Documento.

Se recomienda la siguiente configuración:

-   Si el contribuyente no es interno ni del exterior, el Número identificación
    de estado debería ser obligatorio.

-   Si el contribuyente es interno, el Número de identificación de estado
    debería ser No obligatorio.

-   Si el contribuyente es del exterior, el Número de identificación de estado
    podría ser obligatorio o no.

-   *Grupo de proveedores:* en este campo desplegable se podrá seleccionar un
    conjunto de los configurados en el maestro Grupo de Tipo de Cuenta. Esto
    permitirá asociar al proveedor los comprobantes habilitados y/o
    predeterminados para ciertas transacciones.

Este campo será obligatorio dependiendo de lo configurado en el maestro Tipo de
Contribuyente.

-   *Conceptos y Notas: e*n esta sección se podrá añadir datos adicionales
    acerca del proveedor, a modo informativo. Las etiquetas de estos campos se
    configuran en Configuración General LATAM.
