## 4.7. Software Object-Oriented Design {#cap-4-7}

&emsp;&emsp;&emsp;&emsp;En esta sección se presentan y explican los Diagramas de Clases UML para el Backend (Web Service) del sistema **atelier**, dividiéndolo por *Bounded Contexts* de acuerdo con el enfoque *Domain-Driven Design* (DDD). Cada diagrama detalla las clases, interfaces, enumeraciones y sus relaciones, incluyendo los miembros para cada clase (atributos, métodos) y el *scope* en cada caso (private, public, protected), así como la calificación, dirección y multiplicidad de las relaciones.

### 4.7.1.&emsp;&emsp;Class Diagrams {#cap-4-7-1}

&emsp;&emsp;&emsp;&emsp;A continuación se presenta el diagrama de clases general del *Web Service* (Backend), abarcando la totalidad de la aplicación. Posteriormente, el diseño se desglosa y detalla según cada *Bounded Context*.

**Figura XX**

*Class Diagram*

![](assets/class-diagram.svg "Class Diagram - General")
[Enlace al diagrama completo](https://drive.google.com/file/d/10egYtCO9XkUSs_AtSltKLX53fD8nvHCr/view?usp=sharing)



**Bounded Context: Core (Identity and Multi-Tenancy)**

&emsp;&emsp;&emsp;&emsp;El siguiente diagrama detalla la estructura orientada a objetos para la gestión de usuarios, roles, talleres y suscripciones, garantizando el esquema *multi-tenant* de la plataforma.

**Figura XX**

*Class Diagram - Core (Identity and Multi-Tenancy)*

![](assets/class-diagram-core.svg "Class Diagram - Core")

**Bounded Context: IoT (Hardware y Telemetría)**

&emsp;&emsp;&emsp;&emsp;En este diagrama se exponen los componentes encargados de la ingesta, procesamiento y gestión de la telemetría generada por los dispositivos OBD2 instalados en los vehículos.

**Figura XX**

*Class Diagram - IoT (Hardware and Telemetry)*

![](assets/class-diagram-iot.svg "Class Diagram - IoT")

**Bounded Context: Operations (Work Orders)**

&emsp;&emsp;&emsp;&emsp;El diagrama ilustra el modelo de dominio central para la operación de los talleres, focalizándose en el ciclo de vida de las órdenes de trabajo y las tareas mecánicas asignadas.

**Figura XX**

*Class Diagram - Operations (Work Orders)*

![](assets/class-diagram-operations.svg "Class Diagram - Operations")

**Bounded Context: Fleet (Fleet Management)**

&emsp;&emsp;&emsp;&emsp;Este modelo describe la estructura requerida para administrar la cartera de clientes de cada taller y la gestión del registro de los vehículos de sus flotas respectivas.

**Figura XX**

*Class Diagram - Fleet (Fleet Management)*

![](assets/class-diagram-fleet.svg "Class Diagram - Fleet")

**Bounded Context: Inventory (Warehouse)**

&emsp;&emsp;&emsp;&emsp;El diagrama de clases presenta la gestión del catálogo de productos, repuestos e insumos, así como el control transaccional del stock en los almacenes del taller.

**Figura XX**

*Class Diagram - Inventory (Warehouse)*

![](assets/class-diagram-inventory.svg "Class Diagram - Inventory")

**Bounded Context: Billing (Invoicing and Payments)**

&emsp;&emsp;&emsp;&emsp;Finalmente, este diagrama detalla los componentes relacionados con la facturación, el desglose de los montos de servicio y la gestión de estados financieros y tributarios.

**Figura XX**

*Class Diagram - Billing (Invoicing and Payments)*

![](assets/class-diagram-billing.svg "Class Diagram - Billing")
