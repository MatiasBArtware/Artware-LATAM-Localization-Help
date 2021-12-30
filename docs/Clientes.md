#Clientes  
 
##Objetivo 
 
Esta sección permitirá agregar datos adicionales de Clientes, requeridos a nivel informativo, que serán de utilidad para cumplir con las formalidades de las regulaciones impositivas. 
 
Para realizar la correspondiente configuración se deberá ingresar al Maestro de Clientes, y al cliente seleccionado ingresar a la Sección Latam


## LATAM 
  
![Screenshot](img/Clientes/Cliente_Latam.png)
 
Los campos para completar son los siguientes:
* **Tipo de contribuyente:** en este campo desplegable se podrá seleccionar del maestro Tipo de contribuyente, el que corresponda a la condición del cliente. Por ejemplo, sí se trata en una compañía radicada en Argentina como tipo de contribuyente se podrán seleccionar responsable Inscripto, Monotributista, Exento, etc.   

* **País de radicación:** en este campo desplegable se deberá seleccionar el País donde se encuentra radicado el cliente, se validará que los países ofrecidos como opciones correspondan para el tipo de contribuyente seleccionado. 

* **Tipo documento de país:** este campo desplegable solo permitirá seleccionar tipos de documento país que surjan de la intersección entre los tipos admitidos para el País donde se encuentra radicado el cliente, y los configurados para el tipo de contribuyente seleccionado. Este campo será obligatorio o no a partir de lo configurado en el maestro Tipo de Contribuyente. 
* **N° documento país:** en este campo se deberá ingresar manualmente el número que identifica al cliente frente al Fisco Nacional, o de su país en caso de ser del exterior, siempre respetando la máscara configurada en el maestro Tipo Documento. Este campo será obligatorio o no dependiendo de lo configurado en el maestro Tipo de Contribuyente.  
Se recomienda la siguiente configuración:  
    * Si el contribuyente no es interno y no es del exterior, el Número de identificación país debería ser obligatorio. 
    * Si el contribuyente es interno, el Número de identificación país debería ser No obligatorio. 
    * Si el contribuyente es del exterior, el Número de identificación país podría ser obligatorio o no.  
  
* **Inscripto en jurisdicción:** en este campo se deberá seleccionar el código de estado o provincia en el que se encuentra inscripto el cliente, en caso de tributar impuestos jurisdiccionales o provinciales. Este campo será obligatorio dependiendo de lo configurado en el maestro Tipo de Contribuyente.  
Se recomienda la siguiente configuración:  
    * Si el contribuyente no es interno ni del exterior, el Inscripto en jurisdicción debería ser obligatorio.
	* Si el contribuyente es interno, el Inscripto en jurisdicción debería ser No obligatorio
	* Si el contribuyente es del exterior, el Inscripto en jurisdicción podría ser obligatorio o no.  

 
* **Tipo documento de estado:** este campo desplegable solo permitirá seleccionar tipos de documento estado que surjan de la intersección entre los tipos admitidos para el Estado donde se encuentra inscripto el cliente, y los configurados para el tipo de contribuyente seleccionado. 

* **Número de identificación de estado:** en este campo se deberá ingresar manualmente el número que identifica al cliente frente al Fisco de la Jurisdicción, siempre respetando la máscara configurada en Tipo de Documento. Este campo será obligatorio dependiendo de lo configurado en el maestro Tipo de Contribuyente.  
Se recomienda la siguiente configuración: 
    * Si el contribuyente no es interno ni del exterior, el Número identificación de estado debería ser obligatorio. 
    * Si el contribuyente es interno, el Número de identificación de estado debería ser No obligatorio. 
    * Si el contribuyente es del exterior, el Número de identificación de estado podría ser obligatorio o no.  
* **Grupo de clientes:** en este campo desplegable se podrá seleccionar un conjunto de los configurados en el maestro Grupo de Tipo de Cuenta. Esto permitirá asociar al cliente los comprobantes habilitados y/o predeterminados para ciertas transacciones. 
 
 
* **Conceptos y Notas:** en esta sección se podrá añadir datos adicionales acerca del cliente, a modo informativo. Las etiquetas de estos campos se configuran en Configuración General LATAM. 
