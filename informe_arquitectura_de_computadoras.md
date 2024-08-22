# Informe de Investigación Sobre Arquitectura de Computadoras

Electronica IV - TP - Arquitectura de Computadora

> Barrionuevo, Fátima María

## Introducción

    Un definición simplificada y general para computadora puede expresarse como una máquina que es capaz de realizar una secuencia de operaciones mediante un programa,  de tal manera, que procesa un conjunto de datos de entradas y luego se obtienen otro conjunto de datos a su salida.

    Si bien en la actualidad la imagen de computadora esta bastante generalizada a un dispositivo electrónico digital, a lo largo del tiempo esta máquina paso por muchas transformaciones para llegar al dispositvo que conocemos hoy en día.

    A grandes rasgos, según el principio de operación podían dividirse en computadoras analógicas y computadoras digitales.

    Las computadoras analógicas se remotan a las primeras máquinas que facilitaban cálculos y aprovechaban el hecho de que algunos de los fenómenos físicos pueden ser descriptos bajo relaciones matemáticas parecidas, lo que implicaba obtener una solución rápida a la configuración establecida para ese problema. Por otro lado, si el problema que se deseaba resolver respondia a relaciones matemáticas distintas a las establecidas en el dispositivo, para su resolución es necesario reconfigurar todos los circuitos (Hardware).Ejemplos de estas computadoras analógicas son ábaco, máquina de Pascal.

    Las computadoras digitales, por su lado,están basadas en dispositivos biestables (solo tienen dos valores posibles a tomar, '0' ó '1') que poseen la ventaja de poder ejecutar distintos programas para diferentes problemas sin la necesidad de modificar físicamente la máquina.

    

    Una computadora se encuentra compuesta por los siguientes elementos que se conectan entre ellos a través de buses internos:
- **CPU**: (Central Proccessing Unit) controla todas las acciones que hace la computadora. Es el encargado de ejecutar las instrucciones dadas a través de un programa guardado en una memoria.

- **Memoria** Existen varios tipos, pero los mas básicos son:
	- **RAM**: (ramdon access memory) es una memoria que se puede escribir y leer, volátil es decir que si se desconecta la computadora de su alimentación se pierde el contenido de esta. Se utiliza para guardar datos
	- **ROM**: (read only memory) es una memoria que solo puede ser leída, es no volátil es decir que si se desconecta la alimentación de la computadora no se pierde su contenido. 
	- **Caché**: es una memoria ram que posee datos a los que se accede de forma frecuente, lo que permite tener un acceso mas rápido a estos.
- **Puertos de entrada/salida**: es una conexión física que posee la computadora para enviar y recibir información de dispositivos externos a esta llamados permitiendo  interactuar con el exterior.

Un Bus de dirección  es una conexión que tiene especificaciones eléctricas particulares, lo que permite que ambos puntos de conexión puedan tener una comunicación eficiente. Se encuentra compuesto por varias líneas lo que permite enviar un bit por cada una de ellas. Los tipos básicos son:
- **Bus de Direcciones**: es utilizado por el microporcesador para seleccionar la posición de direcciones de memoria o puertos que desea leer o escribir.

- **Bus de Datos**: permite enviar instrucciones del programa y datos entre el CPU, las memorias y los puertos. El ancho de este bus nos indica la potencia que posee la computadora. El flujo de datos es bidireccional.

- **Bus de Control**: es usado para enviar y recibir señales de control a los distintos dispositivos conectados  desde y hacia el procesador. Posee un flujo de datos bidireccional.



    


## Define arquitectura de computadoras

    Se trata de un conjunto de reglas, principios y estándares que definen la estructura y el diseño de los componentes de hardware y software que conforman un sistema informático. Esta abarca desde el nivel más bajo (como los circuitos electrónicos y la lógica digita) hasta el nivel más alto (como lo son los sistemas operativos y las aplicaciones).

    La arquitectura de computadoras constituye la base conceptual y técnica que admite la creación de ordenadores y sistemas informáticos funcionales. Incluye la forma en que los componentes se comunican entre sí, la manera en que se gestionan los recursos, cómo se ejecutan las instrucciones, así como el procedimiento de almacenar y acceder a los datos.



 ## Distingue entre microarquitectura, arquitectura y software.


    **Microarquitectura** :  Es la implementacion en el silicio de la arquitectura. Lo que está detrás del set de registros y del modelo de programación. Puede ser muy simple o sumamente robusta y poderosa. Cambia de un modelo a otro dentro de una misma familia.

    **Arquitectura**: Es el conjunto de recursos accesibles para el programador, que por lo general se mantienen a lo largo de los diferentes modelos de procesadores de esa arquitectura


    **Software**: soporte lógico de un sistema informático, es decir, es la parte no física que hace referencia a un programa o conjunto de programas de cómputo que incluye datos, reglas e instrucciones para poder comunicarse con el hardware y que hacen posible su funcionamiento.




## Clases de arquitectura de computadora

> - Explica brevemente los tipos de arquitectura de computadora.

    Entre los modelos de arquitectura de computadoras actuales, los más populares que se encuentran son:

    ARQUITECTURA DE VON NEUMANN: Se basa en la idea de tener una unidad central de procesamiento (CPU) que accede a una memoria compartida para almacenar tanto datos como programas. Las instrucciones y datos se guardan en la misma memoria y se recuperan a través de un bus (o canal) común.

    ARQUITECTURA HARVARD: Es un modelo similar a la arquitectura de Von Neumann, pero este se caracteriza por utilizar memorias físicamente separadas para almacenar las instrucciones del programa y los datos de manera independiente. Esto permite que la CPU acceda simultáneamente a ambos, mejorando el rendimiento en ciertas aplicaciones específicas. Se ha usado principalmente en aplicaciones donde se requiere un alto rendimiento en el procesamiento de señales o en tareas específicas donde el acceso simultáneo a instrucciones y datos es ventajoso.

    ARQUITECTURA RISC (Reduced Instruction Set Computer): Es un enfoque de diseño de procesadores y computadoras que se caracteriza por utilizar un conjunto de instrucciones reducido y altamente optimizado. Los procesadores RISC ejecutan instrucciones en un solo ciclo de reloj, lo que los hace más eficientes en operaciones simples y repetitivas. Además, pueden alcanzar altos niveles de rendimiento, siendo particularmente útiles en aplicaciones que requieren un procesamiento intensivo, como servidores y supercomputadoras. Su efectividad la ha convertido en la base para muchos procesadores modernos.


    ARQUITECTURA CISC (Complex Instruction Set Computer): A diferencia de RISC, los procesadores CISC utilizan un conjunto de instrucciones más amplio y diverso. Estas instrucciones pueden realizar tareas más complejas en un solo ciclo de reloj, lo que facilita la programación, pero puede afectar el rendimiento en ciertos escenarios. Por esta razón, a lo largo del tiempo, se han desarrollado técnicas para mejorar la ejecución de instrucciones CISC, como la segmentación (pipeline) y la ejecución fuera de orden (out-of-order execution).
    

    ARQUITECTURA PARALELA: Es un enfoque de diseño de computadoras que se basa en la utilización de múltiples unidades de procesamiento trabajando en paralelo para realizar tareas y operaciones de manera simultánea. Esto puede lograrse mediante el uso de procesadores multinúcleo o la creación de sistemas con varios procesadores trabajando juntos. Su principal objetivo es mejorar el rendimiento y la eficiencia del sistema informático al dividir las tareas en partes más pequeñas y asignarlas a diferentes procesadores para que trabajen en conjunto.

    ARQUITECTURA DE LA COMPUTACIÓN EN LA NUBE: También conocida como arquitectura de nube. Consiste en una estructura tecnológica que permite el acceso a recursos informáticos a través de internet, como almacenamiento, potencia de procesamiento y aplicaciones, sin que los usuarios tengan que poseer o administrar físicamente los equipos y servidores que los proveen. Esta arquitectura es esencial para la provisión de servicios bajo demanda y la escalabilidad de aplicaciones.






> - Considera *al menos* lo siguiente: máquina de pila, máquina de registros y máquina de acumulador; RISC y CISC; Von Newmann y Harvard

> - Sitúa en este contexto la arquitectura ARMv7M

## Partes de una arquitectura de computadora

La arquitectura ARM se diseñó para permitir implementaciones de tamaño muy reducido y de alto rendimiento. Esto hizo que aparezcan dispositivos con muy bajo consumo de energía. Se caracteriza por ser una computadora de set de instrucciones reducido (Reduced Instruction Set Computer, RISC).

Si bien la arquitectura ARM posee características del diseño RISC esta a su vez incorporo otras cualidades que al mismo tiempo son las que permiten separarlas y diferenciarlas.

Entre las característica que ARM conservo del diseño RISC se puede mencionar:

- Arquitectura de carga y almacenamiento (Load-store): Las instrucciones que acceden a memoria están separadas de las instrucciones que acceden al procesamiento de datos.

- Instrucciones de longitud fija de 32 bits: Simplifica la decodificación de instrucciones.

- Formatos de instrucción de 3 direcciones: Se refiere a un conjunto de instrucciones en los que los operandos fuente y destino se pueden indentificar de manera independiente entre ellos.


Luego entre las nuevas características que implemento la arquitectura ARM se puede mencionar: 

- Todas las instrucciones se ejecutan en un ciclo de reloj.

- Modos de direccionamientos simples: Para el procesamiento de datos solo se opera con contenidos de registro.

- Control sobre la unidad aritmética lógica y el "shifter".

- Modos de direcccionamiento con incremento y decremento automático de punteros.

- Carga y almacenamiento de múltiples instrucciones.

- Técnica  "Pipeline": Permite comenzar con una instrucción antes que la anterior haya terminado.

- Arquitectura "Thumb" : Mejora la densidad de código. Se usa un set de instrucciones de 16 bits que es una forma comprimida del set de instrucciones ARM de 32 ARM.

Todas estas mejoras provocaron que los procesadores implementados con arquitectura ARM tengo una combinación óptima de rendimiento, tamaño reducido en el uso de silicio  y menos código.








> - Explica las distintas partes de una arquitectura de computadora
> - Analiza a la luz de lo desarrollado la arquitectura ARMv7M



## Conclusiones



Se puede concluir que el término arquitectura de computadoras hace referencia a un diseño conceptual y a la estructura operativa fundamental de un sistema informático. Abarca desde la forma en que los componentes físicos (hardware) interactúan entre sí hasta cómo se ejecutan las instrucciones (software).

Se trata de un enfoque más teorico destinado a detallar el como la computadora realiza ciertas instrucciones ó cuales le es posible realizar.


Al momento de elegir una arquitectura de computadoras se debería tener en cuenta varios aspectos, entre los cuales se puede nombrar: compatibilidad con el software a usar, los costos que implican el uso de una u otra arquitectura y que características de seguridad ofrecen.


## Bibliografía



- Miles J. Murdocca - Vincent P. Heuring (2002). *Principios de arquitectura de computadoras*. 1ra Edición. Buenos Aires, Argentina.

- Andrew S. Tanenbaum (2000). *Organización de computadoras - un enfoque estructurado*. 4ta Edición. Amsterdam, Países Bajos.

- Ing. Susana Marta Canel (2007). *Microcontroladores ARM de 31 bits*. Universidad Tecnológica Nacional- Facultad Regional Buenos Aires. Buenos Aires, Argentica

- ARM®v7-M Architecture Reference Manual (2006 - 2008)