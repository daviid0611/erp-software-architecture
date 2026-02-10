---
date: Enero 2023
title: Plantilla ![arc42](images/arc42-logo.png)
---

# 

**Acerca de arc42**

arc42, La plantilla de documentación para arquitectura de sistemas y de
software.

Por Dr. Gernot Starke, Dr. Peter Hruschka y otros contribuyentes.

Revisión de la plantilla: 7.0 ES (basada en asciidoc), Enero 2017

© Reconocemos que este documento utiliza material de la plantilla de
arquitectura arc42, <https://www.arc42.org>. Creada por Dr. Peter
Hruschka y Dr. Gernot Starke.

# Introducción y Metas

## Objetivo del sistema
El sistema ERP para Restaurante tiene como objetivo apoyar la gestión integral de los procesos operativos del negocio, permitiendo el control de inventario, compras, ventas y proveedores de manera centralizada, eficiente y segura.

El Módulo de Compras se enfoca en garantizar el abastecimiento oportuno de insumos y productos necesarios para la operación del restaurante.

## Requisitos de negocio del Módulo de Compras
- Registrar y administrar productos del inventario.
- Gestionar proveedores y sus precios.
- Crear y gestionar órdenes de compra.
- Consultar el historial de compras.
- Mantener actualizado el stock de productos.

## Vista de Requerimientos
Las siguientes decisiones tecnológicas y restricciones fueron definidas para el desarrollo del sistema ERP:

- El backend se desarrollará en Java utilizando el framework Spring Boot.
- El frontend será una aplicación web tipo SPA desarrollada con React.
- La comunicación entre frontend y backend se realizará mediante servicios REST usando JSON.
- La base de datos será PostgreSQL.
- El sistema se ejecutará sobre una arquitectura monolítica para simplificar el desarrollo y mantenimiento.
- El acceso al sistema se realizará a través de un navegador web.
## Metas de Calidad

## Partes interesadas (Stakeholders)

| Rol/Nombre   | Contacto        | Expectativas        |
|--------------|-----------------|---------------------|
| *\<Role-1\>* | *\<Contact-1\>* | *\<Expectation-1\>* |
| *\<Role-2\>* | *\<Contact-2\>* | *\<Expectation-2\>* |

# Restricciones de la Arquitectura

# Alcance y Contexto del Sistema
El sistema ERP interactúa con distintos actores del restaurante y con sistemas externos para cumplir sus funciones.

El Administrador y el personal operativo utilizan el sistema para gestionar productos, compras y pedidos.  
Adicionalmente, el ERP se comunica con un sistema contable externo para el manejo de información financiera.

## Diagrama de Contexto (C1)

## Contexto de Negocio

**\<Diagrama o Tabla\>**

**\<optionally: Explanation of external domain interfaces\>**

## Contexto Técnico

**\<Diagrama o Tabla\>**

**\<Opcional: Explicación de las interfases técnicas\>**

**\<Mapeo de Entrada/Salida a canales\>**

# Estrategia de solución

# Vista de Bloques
El sistema ERP está compuesto por los siguientes contenedores principales:

## Aplicación Web (Frontend)
Proporciona la interfaz de usuario para administradores y personal del restaurante. Permite registrar productos, gestionar compras y consultar información.

## API Backend
Contiene la lógica de negocio del sistema, procesa las solicitudes del frontend y aplica las reglas del dominio del restaurante.

## Base de Datos
Almacena de forma persistente la información de productos, proveedores, órdenes de compra y usuarios.
## Sistema General de Caja Blanca

***\<Diagrama general\>***

Motivación  
*\<Explicación en texto\>*

Bloques de construcción contenidos  
*\<Desripción de los bloques de construcción contenidos (Cajas
negras)\>*

Interfases importantes  
*\<Descripción de las interfases importantes\>*

### \<Caja Negra 1\>

*\<Propósito/Responsabilidad\>*

*\<Interfase(s)\>*

*\<(Opcional) Características de Calidad/Performance\>*

*\<(Opcional) Ubicación Archivo/Directorio\>*

*\<(Opcional) Requerimientos Satisfechos\>*

*\<(Opcional) Riesgos/Problemas/Incidentes Abiertos\>*

### \<Caja Negra 2\>

*\<plantilla de caja negra\>*

### \<Caja Negra N\>

*\<Plantilla de caja negra\>*

### \<Interfase 1\>

…​

### \<Interfase m\>

## Nivel 2

### Caja Blanca *\<bloque de construcción 1\>*

*\<plantilla de caja blanca\>*

### Caja Blanca *\<bloque de construcción 2\>*

*\<plantilla de caja blanca\>*

…​

### Caja Blanca *\<bloque de construcción m\>*

*\<plantilla de caja blanca\>*

## Nivel 3

### Caja Blanca \<\_bloque de construcción x.1\_\>

*\<plantilla de caja blanca\>*

### Caja Blanca \<\_bloque de construcción x.2\_\>

*\<plantilla de caja blanca\>*

### Caja Blanca \<\_bloque de construcción y.1\_\>

*\<plantilla de caja blanca\>*

# Vista de Ejecución
Este escenario describe el flujo de ejecución cuando un gestor de inventario registra un nuevo producto en el sistema.

1. El gestor de inventario ingresa los datos del producto en la aplicación web.
2. El frontend envía la información al backend mediante una solicitud REST.
3. El backend valida los datos ingresados.
4. El producto es almacenado en la base de datos.
5. El sistema retorna una confirmación al usuario.
## \<Escenario de ejecución 1\>

- *\<Inserte un diagrama de ejecución o la descripción del escenario\>*

- *\<Inserte la descripción de aspectos notables de las interacciones
  entre los bloques de construcción mostrados en este diagrama.\>*

## \<Escenario de ejecución 2\>

## …​

## \<Escenario de ejecución n\>

# Vista de Despliegue
El sistema ERP se desplegará en un servidor centralizado que aloja:

- Un servidor web para la aplicación frontend.
- Un servidor de aplicaciones para el backend.
- Un servidor de base de datos PostgreSQL.

Los usuarios acceden al sistema mediante un navegador web a través de Internet o red local.

## Nivel de infraestructura 1

***\<Diagrama General\>***

Motivación  
*\<Explicación en forma textual\>*

Características de Calidad/Rendimiento  
*\<Explicación en forma textual\>*

Mapeo de los Bloques de Construcción a Infraestructura  
*\<Descripción del mapeo\>*

## Nivel de Infraestructura 2

### *\<Elemento de Infraestructura 1\>*

*\<diagrama + explicación\>*

### *\<Elemento de Infraestructura 2\>*

*\<diagrama + explicación\>*

…​

### *\<Elemento de Infraestructura n\>*

*\<diagrama + explicación\>*

# Conceptos Transversales (Cross-cutting)

## *\<Concepto 1\>*

*\<explicación\>*

## *\<Concepto 2\>*

*\<explicación\>*

…​

## *\<Concepto n\>*

*\<explicación\>*

# Decisiones de Diseño

# Requerimientos de Calidad

## Árbol de Calidad

## Escenarios de calidad

# Riesgos y deuda técnica

# Glosario
**Producto**  
Artículo o insumo utilizado por el restaurante, registrado en el inventario.

**Proveedor**  
Empresa o persona que suministra productos al restaurante.

**Orden de Compra**  
Documento que registra la solicitud de compra de productos a un proveedor.

**Gestor de Inventario**  
Usuario responsable de administrar productos y stock.

**ERP**  
Sistema de Planificación de Recursos Empresariales que integra los procesos del negocio.
