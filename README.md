# Examen parcial 2023c

Una aseguradora nacional te ha contratado para que desarrolles una solución en su proceso de
cálculo de seguros de gastos médicos mayores. Por cada cotización se debe calcular el costo anual de la póliza utilizando el siguiente procedimiento:

Empieza calculando _factor_

1. Si el cliente es hombre entonces _factor_ es igual a 15%, si es mujer entonces _factor_ es igual 13%
2. Si edad (sólo considerar el mes y año de nacimiento)
   * menor o igual a 25 años, factor + 2.5%
   * mayor a 25 y menor o igual a 45 años, factor + 3.5%
   * mayor a 45 y menor o igual a 65 años, factor + 4.5%
   * mayor a 65 años, factor + 6% 
3. Estado de residencia:
   * Sumar 5% si vive en CDMX, Nuevo León o Jalisco.
   * Sumar 3% si vive en otro Estado.

Ahora calcula el costo anual con la siguiente fórmula:

`costo anual = factor X costo paquete`

## Paquetes

1. Amplio (costo $55,000.00)
   1. Deducible: $11,000.00
   2. Gama hospitalaria: Diamante
   3. Emergencia en el extranjero: Ampara
   4. Medicamentos fuera del hospital: Ampara
   5. Complicaciones de gastos médicos mayores no cubiertos: Ampara
2. Esencial (costo 35,000.00)
   1. Deducible: $21,000.00
   2. Gama hospitalaria: Esmeralda
   3. Emergencia en el extranjero: Ampara
   4. Medicamentos fuera del hospital: Ampara
   5. Complicaciones de gastos médicos mayores no cubiertos: No ampara
3. Básico (costo $20,000.00)
   1. Deducible: $31,000.00
   2. Gama hospitalaria: Zafiro
   3. Emergencia en el extranjero: No ampara
   4. Medicamentos fuera del hospital: No ampara
   5. Complicaciones de gastos médicos mayores no cubiertos: No ampara 

## Criterios

1. El dato de costo anual se calcula correctamente siguiendo el procedimiento indicado (5 punto)
2. Al seleccionar un Paquete se muestran los términos correctos en la sección "Paquete a contratar" (1 punto)  
3. El resumen o confirmación de la información de la cotización cuenta con la siguiente información (1 punto):
    1. Costo anual (importe)
    2. Nombre del paquete (texto)
    3. Forma de pago (texto)
    4. Nombre del cliente (texto)
    5. Edad (años)
    6. Sexo (hombre o mujer)
    7. Estado de residencia (texto)    
4. Los datos de nombre del asegurado, sexo, fecha de nacimiento, Estado de residencia, paquete a contratar y la aceptación de los términos son datos obligatorios, los cuales se valida su captura o selección antes de mostrar el resumen y calcular el costo anual. Por cada dato obligatorio faltante, el programa lo reporta con un mensaje de **error explícito** (usa window.alert). (1.5 puntos)
5. El dato de la "Edad del cliente" se calcula considerando el mes y año de la fecha de nacimiento. Asume que todos los años tienen la misma cantidad de días (1.5 puntos)
