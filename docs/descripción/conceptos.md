# Conceptos básicos
En esta sección se explican los conceptos básicos que se abordan en el proyecto:

## Virtualización

Se puede definir la virtualización como “La creación de una versión virtual (lógica) de algún recurso tecnológico, como puede ser una plataforma de hardware, un sistema operativo, un dispositivo de almacenamiento u otros recursos de red” ( Wikipedia) . Otra posible definición sería  “Combinación de hardware y software que permite a un recurso físico funcionar como múltiples recursos lógicos” (El Arte de virtualización, FLOSSystems S.L.).

Dentro del concepto de virtualización existen a su vez diferentes terminologías  y tipos siendo el más extendido a nivel de usuario la denominada virtualización de plataforma, que permite disponer de múltiples “máquinas virtuales” sobre la misma “máquina física” (soluciones muy conocidas como VirtualBox y VMWare Workstation, entre otras,  nos ofrecen esta funcionalidad). Este tipo de virtualización es ampliamente utilizada por administradores y desarrolladores para recrear y simular diferentes entornos.

Los Centros de Proceso de Datos (CPDs) actuales están mayoritariamente “virtualizados” y la tendencia es emplear:

- Virtualización de plataforma para virtualizar máquinas (con tecnologías como KVM, Xen y VMWare ESXI).
- Virtualización a nivel de sistema operativo para crear los denominados contenedores (LXC , Docker y OpenVZ).
- Virtualizar el almacenamiento y la redes (Software Defined Networking, SDN).

El uso  de tecnologías de virtualización es por lo tanto vital para cualquier profesional informático.

 

##Cloud computing

Cloud Computing  es un paradigma o modelo que permite ofrecer servicios de computación bajo demanda a través de una red. El objetivo es utilizar la tecnología para implantar infraestructuras “invisibles” que permitan convertir recursos como computación, almacenamiento, redes, aplicaciones, etc. en un servicio donde se pague por su uso  sin que sean necesarias inversiones iniciales. Permite a las organizaciones externalizar parte de su cómputo y de su almacenamiento a un proveedor que típicamente ofrece un modelo de pago por uso, o crear nubes privadas (on-premise) para tener las ventajas de las tecnologías cloud dentro de una organización, sin necesidad de depender de un proveedor público.

La nube (cloud) es por lo tanto una metáfora que engloba recursos virtuales y físicos alojados y ofrecidos por un determinado proveedor (Cloud de Google, Cloud de Amazon, Cloud de Microsoft, ….) o de forma privada. Cada proveedor ofrece su servicios con un modelo de pago por uso (tiempo de uso de CPU, uso de almacenamiento, tráfico de red, etc..) siendo el objetivo principal ajustar el consumo de recursos a las necesidades de las aplicaciones y usuarios de forma dinámica, elástica y rápida adaptando el consumo a la demanda.  

En el modelo tradicional las inversiones en hardware se quedan obsoletas en poco tiempo y la demanda de recursos de cómputo puede ser muy variable. Si hay un sobre-dimensionamiento parte de los recursos no son utilizados y es necesaria una inversión de hardware para determinados intervalos de tiempo, y con un sub-dimensionamiento si hay picos de carga que no se pueden atender, no se ofrece el servicio de forma adecuada.

Existen tres modelos a la hora de desplegar un cloud:

- **Cloud público**
    * Servicio abierto al público ofrecido por un proveedor
    * Recursos hardware propiedad del proveedor.
    * Gestión del cloud por parte del proveedor.
    * Suscripción del usuarios en el  proveedor (el tiempo que quieras).
    * Pago por uso (usuarios, empresas, organizaciones, etc.).

- **Cloud privado**
    - Uso exclusivo de una organización y/o múltiples usuarios.
    - Gestión del cloud por la propia organización.
    - Puede delegarse la gestión y operación a una compañía especializada.
    - Recursos hardware propios.

- **Cloud híbrido**
      - Dos o más infraestructuras de cloud distintas que aparecen como entidad única.
      - Combinan ambos modelos de cloud (privado o público). Por ejemplo, se delega temporalmente en un cloud público cuando se excede la capacidad de cómputo de un cloud privado.

El campo de cloud computing es muy amplio y es posible realizar varias clasificaciones y diferenciar entre múltiples tipos de cloud con diversidad de matices, pero la clasificación más genérica y extendida es la que se propone a continuación:

- **Software as a service (SaaS).**
    - Orientado a usuarios.
    - Aplicaciones ejecutando sobre una infraestructura cloud son ofrecidas como servicio.
    - Los usuarios pagan por el uso, no por poseer el software (ni siquiera licencias)
    - Ejemplos: Dropbox, Google Drive, Evernote, Office 365, …
- **Platform as a service (PaaS)**
    - Orientado a desarrolladores.
    - Plataforma de software y entornos de desarrollo y pruebas ofrecidos como servicio.
    - Abstrae hardware y servicios.
    - Permite el despliegue y ejecución de aplicaciones.
    - Servicio para todas las fases de desarrollo y pruebas de software.
    - Ejemplos
        - Proveedores de PaaS públicos: OpenShitft, Heroku, Google App Engine, Microsoft Azure, Amazon Web Services, Force.com, Jelastic …
        - Software para desplegar PaaS: OpenShitft Origin, Deis, Cloudfoundry Dokku, Tsuru, Apache Stratos, …
- **Infrastructure as a service (IaaS)**
    - Orientado a administradores.
    - Capacidades de cómputo,  almacenamiento y red (máquinas/hardware) ofrecidas como servicio. Se ofrecen máquinas virtuales.
    - Ejemplos
        - Proveedores de Iaas:  Amazon Web Services, RackSpace Google Compute Engine, Microsoft Azure Service Plataform, HP Cloud, GoGrid, …
      - Software para desplegar IaaS:  OpenStack,  OpenNebula, Cloudstack Eucalyptus, Vmware vCloud, …

De hecho, la tendencia es ofrecer cada vez más cualquier tipo de recurso como un servicio y se suele hablar del término:  XaaS (Anything as a Service).

 

## Big Data

Big Data es un término común bajo el que se agrupan toda clase de técnicas de tratamiento de grandes volúmenes de datos, fuera de los análisis y herramientas clásicas. Este concepto engloba muchas ideas y aproximaciones, pero todas con un objetivo común: extraer información de valor de los datos, de forma que pueda ser de ayuda para las decisiones y procesos de negocio (fuente: UAM).

Todos somos conscientes de que las grandes compañías (en todos los ámbitos) recopilan una gran cantidad de información, cada vez mayor, que gracias a las nuevas capacidades de procesamiento se puede utilizar para analizar, averiguar y extraer patrones  que permiten responder a  muchas respuestas e incluso “averiguar el futuro”. El valor está en comprender los datos.

Destacar que los IaaS ofrecen un entorno muy adecuado para desplegar rápidamente clusters con la capacidad de cómputo y almacenamiento necesarios que permitan gestionar estas cantidades de datos y el software que los analiza.