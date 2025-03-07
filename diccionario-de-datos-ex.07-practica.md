---
description: Reservas de un Hotel
cover: >-
  https://images.unsplash.com/photo-1517840901100-8179e982acb7?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHw2fHxIb3RlbCUyMFJlc2VydmF0aW9ufGVufDB8fHx8MTczODc3NzUyMXww&ixlib=rb-4.0.3&q=85
coverY: 0
layout:
  cover:
    visible: true
    size: hero
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Diccionario de Datos - Ex.7 - Practica

#### <mark style="color:orange;">Ejercicio 7 - Exercise 7</mark>

Spanish:

Un hotel maneja sus servicios exclusivamente a través de reservas. Cuando un cliente solicita una reserva, además de indicar sus datos personales (nombre completo y no de documento), indica el tipo de servicio deseado (restaurante, salón de exposiciones, sala de conferencias), el período por el cual lo solicita (fecha inicial y fecha final), y si el servicio solicitado es un salón o sala, indica el horario de utilización.

English:

A hotel manages its services exclusively through reservations. When a customer requests a reservation, in addition to providing their personal information (full name and document number\*), they specify the desired type of service (restaurant, exhibition hall, conference room), the period for which it is requested (start date and end date), and if the requested service is a hall or room, they indicate the usage hours.

***

<mark style="color:green;">**Solution:**</mark>&#x20;

**Diccionario de Datos:**&#x20;

e: reservas = datosPersonales(e) + tipoDeServicio(d) + periodoUso(e) \
\
datosPersonales(e) = nombre + apellido + tipoDocumento(d) + nroDocumento + 1{eMail}n\
tipoDocumento(d) = char(3) ; \[DNI | DU | PAS | LE | LC ]\
\
tipodeServicio(d) = \[ restaurant + (horarioUso) | salónExposiciones + horarioUso | salaConferencias + horarioUso ]\
\
periodoUso(e) = fechaInicial + fechaFinal

**Tipo de Evento:** Evento Externo
