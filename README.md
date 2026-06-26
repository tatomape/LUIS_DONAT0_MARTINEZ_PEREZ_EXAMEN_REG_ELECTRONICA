# LUIS_DONAT0_MARTINEZ_PEREZ_EXAMEN_REG_ELECTRONICA

Profesor:Erick Moreno Negrete
Institución: Tecnológico Salesiano Carlos Gómez
Asignatura: Simulación Electrónica y Tecnología y Taller de Electronica
Fecha: 26 de Junio de 2026
Objetivo del Proyecto
Diseñar, analizar analíticamente, simular y desarrollar el diseño de circuito impreso (PCB) de un convertidor reductor (Buck Converter) síncrono de una fase, empleando herramientas de software profesional (Multisim y KiCad) y justificando técnicamente la selección de componentes mediante hojas de datos.
Problema Asignado:
Se analiza un convertidor reductor de una fase operando bajo los siguientes parámetros nominales:
Voltaje de entrada (VG): 48 V
Voltaje de salida (Vo): 12 V
Inductancia : 220 uH
Capacitancia : 470 uF
Resistencia de carga : 12 Ohms
Frecuencia de conmutación : 50 kHz
Metodología Utilizada
1. Cálculo Teórico: Deducción de ecuaciones fundamentales del convertidor Buck en Modo de Conducción Continua (MCC).
2. Simulación en Multisim: Implementación del circuito esquemático con parámetros reales para evaluar transitorios de arranque y estado estable.
3. Análisis Comparativo: Evaluación del error porcentual entre la teoría matemática y las mediciones simuladas.
4. Diseño en KiCad: Creación de esquemático y ruteo de la PCB considerando planos de tierra y anchos de pista óptimos para potencia.
Resultados Obtenidos (Resumen)
Variable | Valor Teórico | Valor Simulado | Error (%)
Ciclo de trabajo (D): 0.25 (25%)
Voltaje de Salida (Vo): 12.0 V
Corriente de Salida (Io): 1.0 A
Rizado de Corriente (Delta iL): 0.8182 A
Corriente Máxima (iL,max): 1.4091 A
Corriente Mínima (iL,min): 0.5909 A
Rizado de Voltaje (Delta Vo): 4.352 mV
Rizado (%): 0.0363 %
Conclusiones
El convertidor opera exitosamente en Modo de Conducción Continua (MCC) debido a que la corriente mínima en el inductor (0.5909 A) es estrictamente mayor que cero. El rizado de tensión teórico obtenido (4.352 mV) demuestra un excelente filtrado por parte del capacitor de 470 uF. La implementación del driver NCP81253 asegura que la señal PWM de 5V sea capaz de conmutar adecuadamente al MOSFET de potencia RFD3055LE superando las capacidades parásitas de compuerta.
