# DEPASIA DOCS — TEMPLATE MAESTRO DE PRESUPUESTO V1

**Estado:** Diseño base listo para implementación  
**Documento:** Presupuesto  
**Versión:** V1  
**Moneda comercial por defecto:** USD

---

## 1. Objetivo

Definir la primera plantilla oficial de Presupuesto de DEPASIA para utilizarla en DEPASIA DOCS.

Debe funcionar para presupuestos de distintos importes y distintos tipos de servicios.

El importe nunca es fijo en la plantilla.

---

# 2. Formato

- Tamaño: A4
- Orientación: vertical
- Documento pensado para PDF.
- Diseño limpio, profesional y moderno.
- Buena lectura tanto en pantalla como impreso.
- Puede ocupar más de una página cuando el contenido lo requiera.
- Evitar que una sección quede cortada de forma poco profesional entre páginas.

---

# 3. Estructura visual

## ENCABEZADO

Debe contener:

**DEPASIA**

**Sistemas que hacen crecer tu negocio**

Y la identificación del documento:

**PRESUPUESTO**

**Presupuesto #001**

**Fecha: DD/MM/AAAA**

El número y la fecha son variables.

---

# 4. Datos del cliente

Título:

**CLIENTE**

Campos:

- Empresa / Nombre
- Persona de contacto
- Email
- Teléfono
- Localidad / País (opcional)

No mostrar campos vacíos innecesarios.

---

# 5. Introducción

Título:

**PROPUESTA**

Breve texto introductorio opcional.

Ejemplo:

> Propuesta económica para el desarrollo e implementación de una landing web comercial para FOI Tools.

Este texto es variable.

No debe existir una introducción obligatoria si el presupuesto no la necesita.

---

# 6. Servicio

Título:

**SERVICIO PROPUESTO**

Campos:

- Nombre del servicio
- Descripción breve

Ejemplo:

**Landing web comercial**

> Diseño y desarrollo de una landing orientada a presentar los servicios de FOI Tools y facilitar el contacto con potenciales clientes.

---

# 7. Alcance

Título:

**ALCANCE DEL PROYECTO**

Lista de elementos incluidos.

Ejemplo:

- Diseño visual de la landing.
- Desarrollo responsive.
- Estructura orientada a conversión.
- Integración de formularios de contacto.
- Publicación de la web.
- Configuración básica necesaria para su funcionamiento.

El número de elementos es variable.

---

# 8. Inversión

Esta es una de las secciones principales.

Título:

**INVERSIÓN**

Debe permitir uno o varios conceptos.

Estructura conceptual:

| Concepto | Importe |
|---|---:|
| Servicio / concepto | USD 700 |
| Otro concepto | USD XXX |
| **TOTAL** | **USD XXX** |

No fijar cantidad máxima de conceptos en la lógica.

El total debe calcularse automáticamente.

---

# 9. Moneda

## Regla comercial estándar

Los presupuestos de DEPASIA se expresan en **USD por defecto**.

Ejemplo:

**TOTAL: USD 700**

El importe puede ser cualquier valor.

No debe existir un valor fijo de USD 700 dentro del template.

---

# 10. Conversión a pesos argentinos

La conversión a ARS es opcional.

No debe ejecutarse automáticamente mediante una cotización externa.

DEPASIA puede decidir en cada presupuesto si desea mostrar:

### Modalidad A — Solo USD

```text
TOTAL
USD 700
```

Condición opcional:

> *En caso de abonar en pesos argentinos, el importe será convertido según el tipo de cambio acordado entre DEPASIA y el cliente al momento del pago.

### Modalidad B — USD + equivalente de referencia

```text
TOTAL
USD 700

* Equivalente de referencia:
ARS $980.000

* Tipo de cambio utilizado:
ARS $1.400 por USD 1.
```

Los siguientes datos son variables:

- Moneda principal.
- Monto principal.
- Moneda secundaria.
- Monto convertido.
- Tipo de cambio.
- Fecha del tipo de cambio.
- Referencia o descripción del tipo de cambio.

La conversión puede ser:

- Calculada automáticamente a partir del tipo de cambio ingresado.
- O cargada manualmente si existe un importe acordado.

No asumir una fuente de cotización.

---

# 11. Pago

Título:

**CONDICIONES DE PAGO**

Campos posibles:

- Forma de pago.
- Cantidad de pagos.
- Porcentaje inicial.
- Saldo.
- Fechas o hitos de pago.
- Condiciones especiales.

Ejemplo:

> 50% al iniciar el proyecto y 50% contra entrega.

Todos los datos son variables.

No inventar condiciones.

---

# 12. Plazo

Título:

**PLAZO ESTIMADO**

Ejemplo:

> 10 días corridos desde la recepción de la información necesaria y la confirmación de inicio.

El plazo es variable.

---

# 13. Validez

Título:

**VALIDEZ DEL PRESUPUESTO**

Ejemplo:

> Este presupuesto tiene una validez de 15 días.

El número de días es variable.

---

# 14. Observaciones

Título:

**OBSERVACIONES**

Sección opcional.

Puede utilizarse para:

- aclaraciones;
- exclusiones;
- condiciones particulares;
- información adicional;
- dependencias del cliente.

Si no hay observaciones, la sección puede ocultarse.

---

# 15. Mantenimiento

La sección de mantenimiento es opcional.

Ejemplo:

**MANTENIMIENTO**

> Mantenimiento mensual: USD 30 / mes.

Debe poder utilizarse cuando el servicio incluya mantenimiento recurrente.

El monto y las condiciones son variables.

No todos los presupuestos deben incluir mantenimiento.

---

# 16. Pie del documento

Debe incluir información institucional de DEPASIA.

Como mínimo:

**DEPASIA**  
**Sistemas que hacen crecer tu negocio**

Y los datos de contacto oficiales que estén definidos en la configuración de marca.

No inventar email, teléfono, web u otros datos si todavía no fueron definidos.

---

# 17. Jerarquía visual

La prioridad visual debe ser:

1. DEPASIA / identidad.
2. PRESUPUESTO + número.
3. Cliente.
4. Servicio / alcance.
5. Inversión / total.
6. Condiciones.
7. Información secundaria.
8. Pie institucional.

El total debe ser fácilmente identificable.

---

# 18. Identidad visual

Utilizar el sistema visual DEPASIA:

- Azul: `#2563EB`
- Violeta: `#7C3AED`
- Cyan: `#0686D4`
- Oscuro: `#0F172A`
- Superficie: `#1E293B`
- Bordes: `#334155`
- Texto secundario: `#64748B`
- Texto muted: `#94A3B8`
- Fondo claro: `#F8FAFC`

Tipografía:

**Inter**

El gradiente Cyan → Blue → Violet puede utilizarse como recurso visual de acento.

No utilizar el gradiente en exceso.

---

# 19. Logo

El logo oficial de DEPASIA debe utilizarse sin modificar:

- geometría;
- proporciones;
- colores;
- composición.

Los assets maestros definitivos todavía deben incorporarse al proyecto.

Hasta disponer de ellos, no crear una reinterpretación del logo.

---

# 20. Datos variables

La plantilla debe distinguir claramente entre contenido fijo y variables.

Variables mínimas:

```text
documentNumber
date

clientName
clientContact
clientEmail
clientPhone
clientLocation

intro

serviceName
serviceDescription

scope[]

items[]
  concept
  quantity (opcional)
  unitPrice
  subtotal
  currency

mainCurrency
mainTotal

conversion.enabled
conversion.currency
conversion.exchangeRate
conversion.exchangeRateDate
conversion.convertedAmount
conversion.reference

paymentConditions
estimatedDuration
validityDays

observations

maintenance.enabled
maintenanceAmount
maintenanceCurrency
maintenanceConditions

companyContactData
```

Los nombres son conceptuales y pueden cambiar durante la implementación.

---

# 21. Ejemplo FOI Tools

Este ejemplo sirve únicamente para probar el template.

### Cliente

FOI Tools

### Servicio

Landing web comercial

### Inversión

**USD 700**

### Mantenimiento

**USD 30 / mes**

### Plazo

**10 días estimados**

### Conversión

No mostrar por defecto.

Puede agregarse posteriormente si Tonio acuerda un tipo de cambio con el cliente.

---

# 22. Reglas de validación

Antes de permitir aprobar/generar:

Obligatorios mínimos:

- número;
- fecha;
- cliente;
- servicio;
- al menos un concepto;
- importe;
- moneda;
- condiciones de pago;
- validez.

Los campos opcionales pueden ocultarse.

El sistema debe impedir:

- importes negativos;
- conceptos sin importe cuando corresponda;
- monedas inválidas;
- conversiones sin tipo de cambio;
- totales inconsistentes.

---

# 23. Regla de moneda

La moneda principal puede ser distinta de USD si DEPASIA lo necesita.

Sin embargo:

**USD es la moneda comercial predeterminada de DEPASIA.**

Ejemplos válidos:

- USD 700
- USD 1.250
- ARS 850.000
- EUR 900

La aplicación no debe asumir que todos los presupuestos tienen el mismo monto.

---

# 24. Regla de conversión

Nunca convertir automáticamente usando una cotización externa sin una acción explícita del usuario.

Si se muestra conversión:

```text
Monto principal
+
Tipo de cambio definido
=
Monto convertido
```

La información debe indicar que se trata de un equivalente de referencia cuando corresponda.

---

# 25. Regla de contenido

DEPASIA DOCS debe ser un generador de documentos, no un generador de decisiones comerciales.

El usuario o un agente autorizado proporciona:

- precio;
- condiciones;
- plazo;
- alcance;
- descuentos;
- mantenimiento.

DEPASIA DOCS:

- valida;
- calcula;
- organiza;
- presenta;
- genera el documento.

---

# 26. Versionado

El documento debe permitir identificar versiones posteriormente.

Ejemplo:

**Presupuesto #001 — V1**

Si se modifica después de haber sido aprobado, debe generarse una nueva versión.

No sobrescribir silenciosamente un documento aprobado.

---

# 27. Criterio de aprobación

La plantilla V1 se considera lista para pasar a implementación cuando:

- La estructura sea aprobada.
- La identidad visual sea aplicada.
- Los campos estén definidos.
- El comportamiento monetario esté definido.
- El comportamiento de conversión esté definido.
- El ejemplo FOI pueda representarse.
- No existan datos comerciales fijos en la plantilla.

---

# 28. Próximo paso técnico

Una vez aprobada esta estructura:

1. Diseñar visualmente el documento.
2. Obtener/incorporar assets oficiales del logo.
3. Implementar el template en DEPASIA DOCS.
4. Crear formulario.
5. Crear preview.
6. Generar PDF.
7. Probar con FOI.
8. Corregir.
9. Declarar Presupuesto V1 funcional.
10. Continuar con Notion.
