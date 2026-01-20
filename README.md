# **ALURA CHALLENGE:TELECOM X**

<img width="511" height="407" alt="Distribución de la evasión, 27% de los clientes cancelaron" src="https://github.com/user-attachments/assets/09393b16-77c1-4e15-8468-0fc37aaf687b" />

---
<p align="left">
<img src="https://img.shields.io/badge/ESTADO-COMPLETO-green" alt="Badge Estado Completo">
<img src="https://img.shields.io/badge/LENGUAJE-PYTHON-magenta" alt="Badge Lenguaje Python">
<img src="https://img.shields.io/badge/ORGANIZACIÓN-ALURA-blue" alt="Badge Organización Alura">
<img src="https://img.shields.io/badge/PROYECTO-3-orange" alt="Badge Proyecto 3">
</p>


## **ÍNDICE**

- [Introducción](#introducción)  
- [Materiales y requisitos](#materiales)  
- [Estructura del reporte](#estructura-del-reporte)  
  - [Preparación](#1-preparación)  
  - [Limpieza de la base](#2-limpieza-de-la-base)  
  - [Análisis de la base](#3-análisis-de-la-base)  
  - [Informe Final](#4-informe-final)
- [Diccionario](#diccionario)  


---

## **INTRODUCCIÓN**

La evasión de clientes, también conocida como churn, cancelación o fuga de clientes, se refiere a la situación en la que un cliente decide dejar de utilizar un producto o servicio. Este fenómeno representa un problema importante para las empresas, ya que la pérdida de clientes afecta directamente su rentabilidad y crecimiento.
En este trabajo se cuenta con 7,266 registros de clientes de Telecom X y su condición (cancelarón o no). El objetivo es analizar cuales son los principales factores que afectan la cancelación de los clientes y que estrategias puede adoptar la companía para evitarla.


---

## **MATERIALES**

El análisis fue desarrollado utilizando:

- **Python 3.12.12**
- Librerías:
  - `pandas`
  - `matplotlib`
  - `numpy`

El notebook con todo el desarrollo se encuentra en este mismo repositorio.

Las bases de datos fueron provistas por [Alura Latam](https://www.aluracursos.com/) 


---

## **ESTRUCTURA DEL REPORTE**

El reporte se divide en cinco secciones principales:
### **1. Preparación**

Se proveen los diccionarios de datos (mismos encotnrados en este Readme). 
La carga de librerías.
Creación de las funciones.
Se importan los archivos CSV alojados en el repositorio para asegurar la reproducibilidad del análisis.  


---

### **2. Limpieza de la base**

Se extraen y normalizan las variables (originalmente en formato JSON).
Se analizan las variables en busca de clientes duplicados, valores nulos o inconsistencias.
Se crean nuevas variables (ver diccionario al final del readme).

---
### **3. Análisis de la base**
Nuevamente se análisa la base, pero esta vez se presenta la distribución del churn (evasión) en busca de patrones. Adicionalemente de provee una matriz de correlación.


---
### **4. Informe Final**
El mismo cuenta con:
- Introducción
- Resumen de la limpieza y tratamiento de datos
- Análisis exploratorio de datos (resumen del análisis de la base).
- Conclusiones e Insights
- Recomendaciones
- Limitaciones



## **DICCIONARIO**

- customer_id: número de identificación único de cada cliente
- churn: cliente dejó la empresa (1:Sí, 0:No)
- gender_male: género (1:masculino, 0:femenino)
- senior_citizen_65: cliente mayor a 64 años (1:Sí, 0:No)
- partner: cliente tiene una pareja (1:Sí, 0:No)
- dependents: cliente tiene dependientes (1:Sí, 0:No)
- tenure: meses de contrato del cliente
- phone_service: cliente suscrito al servicio telefónico (1:Sí, 0:No)
- multiple_lines: cliente suscrito a más de una línea telefónica (1:Sí, 0:No)
- internet_service: cliente suscrito a un proveedor de internet (1:Sí, 0:No)
- online_security: cliente suscrito al seguridad en línea (1:Sí, 0:No)
- online_backup: cliente suscrito a respaldo en línea (1:Sí, 0:No)
- device_protection: cliente suscrito a protección del dispositivo (1:Sí, 0:No)
- tech_support: cliente suscrito a soporte técnico (1:Sí, 0:No)
- streaming_tv: cliente suscrito a televisión por cable (1:Sí, 0:No)
- streaming_movies: cliente suscrito a streaming de películas (1:Sí, 0:No)
- contract: tipo de contrato (month_to_month, one_year, two_year)
- paperless_billing: cliente prefiere recibir la factura en línea (1:Sí, 0:No)
- payment_method: forma de pago
- charges_monthly: total de todos los servicios del cliente por mes
- charges_total: total gastado por el cliente
- family: El cliente tiene pareja o dependientes. (1:sí, 0:no)
- tenure_log: logaritmo de la antigüedad del cliente.
- dsl: toma el valor 1 si el servicio de internet es por DSL, 0 en otro caso.
- fiber_optic: toma el valor 1 si el servicio de internet es por fibra optica, 0 en otro caso.
- no_internet: toma el valor 1 si no hay servicio de internet.
- subcription_total: Cuenta la cantidad de servicios a lo que el usuario esta subscrito.
- subcription_no_streaming: Cuenta la cantidad de servicios a lo que el usuario esta subscrito, ignorando los de streaming
- streaming: cliente suscrito a streaming_tv o streaming_movies (1:sí, 0:no)
- month_to_month: toma el valor 1 si el contrato es de ese tipo, 0 en otro caso.
- one_year: toma el valor 1 si el contrato es de ese tipo, 0 en otro caso.
- two_year: toma el valor 1 si el contrato es de ese tipo, 0 en otro caso.
- charges_average : Se suman los gaston mensuales y totales (los gastos acumulados más los gastos de este mes) y se dividen por tenure + 1 (contando el mes).
- charges_average_log : logaritmo de los gastos promedios.
- charges_total_log : logaritmo de los gastos totales.
- electronic_check: toma el valor 1 si el método de pago es de ese tipo, 0 en otro caso.
- mailed_check: toma el valor 1 si el método de pago es de ese tipo, 0 en otro caso.
- bank_transfer_automatic: toma el valor 1 si el método de pago es de ese tipo, 0 en otro caso.
- credit_card_automatic: toma el valor 1 si el método de pago es de ese tipo, 0 en otro caso.
- automatic_payment: : toma el valor 1 si el método de pago es credit_card_automatic o bank_transfer_automatic, 0 en otro caso.


