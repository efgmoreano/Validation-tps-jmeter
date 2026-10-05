# Proyecto de Pruebas de Carga para fakestoreapi.com - JMeter

Este repositorio contiene el escenario diseñado para alcanzar un objetivo de **20 TPS** bajo los siguientes SLAs:
* **Tiempo de respuesta máximo:** 1.5 segundos.
* **Tasa de error aceptable:** Menor al 3%.

## Componentes incluidos
* `script_pruebas.jmx`: Script de JMeter con hilos y temporizadores configurados.
* `usuarios.csv`: Archivo para el reciclaje de credenciales en paralelo.

## Instrucciones de ejecución (Modo CLI)
Ejecutar el siguiente comando en la terminal:
```bash
jmeter -n -t "script_pruebas.jmx" -l "resultados.jtl" -e -o "ReporteHTML"
```

---