# Ejercicio 2  
Analicemos el siguiente problema y representemos su solución mediante un algoritmo secuencial.  

Construye un algoritmo que, al recibir como datos el ID del empleado y los seis primeros sueldos del año, calcule el ingreso total semestral y el promedio mensual, e imprima el ID del empleado, el ingreso total y el promedio mensual.  
| Nombre | Tipo | Unidad |  
| ID | Entero| --- |  
| S1 | float | $ |  
| S2 | float | $ |  
| S3 | float | $ |  
| S4 | float | $ |  
| S5 | float | $ |  
| S6 | float | $ |  
| Nombre | Definición | Tipo | Unidad |  
| IT | Ingreso T | float| $ |  
| PM |Prom-mensual| float| $ |  
| ID | Identif | float| $ |  

<img width="172" height="982" alt="Diagrama2 drawio" src="https://github.com/user-attachments/assets/36e4aa16-5156-43ed-ba09-7927ab8972a2" />

# Ejercicio Cumpleaños  

<img width="438" height="822" alt="cumple drawio" src="https://github.com/user-attachments/assets/5206eb42-789f-45a2-9248-8f917ee396fe" />

# Taller Algoritmos  

# 1. **Verificación de peso de despegue**  
    
En una pista de pruebas de aeronaves, el sistema debe verificar si el peso total de la aeronave, incluyendo combustible y carga,    
supera el límite máximo permitido para el despegue. Dependiendo del resultado, el sistema deberá indicar si la aeronave está lista    
para despegar o si debe reducir carga o combustible.  

Inicio  
Escribir "Ingrese el peso total de la aeronave: "  
Leer peso  
Si peso <= máximo entonces  
Escribir "La aeronave esta lista para despegar"  
Si no  
Escribir "Debe reducir carga o combustible"  
Fin si  
Fin   
 
#2. **Control de temperatura del motor**    
    
Durante una inspección de rutina, se mide la temperatura de un motor de turbina. Si la temperatura es mayor a un valor crítico,    
se debe indicar "Peligro: sobrecalentamiento". Si está dentro del rango seguro, indicar "Operación normal". Si es demasiado baja,    
indicar "Motor frío – Calentar antes de operar".    

 
<img width="702" height="832" alt="Taller Ejercicio2 drawio (1)" src="https://github.com/user-attachments/assets/0d5a477a-b17d-4764-86b3-843adf9bda64" />    

# Bucles     
# 3. **Registro de altitudes de vuelo**    
    
Un sistema debe registrar la altitud de vuelo cada 10 minutos durante una hora y mostrar todas las mediciones al final.    

Inicio   
cont = 0  
leer alt_max  
while alt_max sea >= max 0.1  
      cont = cont + 1      
fin while  
Mostrar " Tiempo transcurrido " cont  
Fin  

# 4. **Control de combustible en pruebas**    
    
Durante un ensayo en banco de un motor a reacción, se mide el nivel de combustible cada minuto y se detiene el registro cuando    
el combustible baja del 10%. Mostrar el tiempo total de operación antes de llegar a ese punto.    

Inicio     
tiempo = 0    
Escribir "Ingrese el nivel inicial de combustible: "    
Leer combustible    
Mientras combustible >= 10     
         tiempo = tiempo + 1     
         Escribir "Ingrese el nivel de combustible: "    
         Leer combustible    
Fin mientras    
Escribir "Tiempo total de operación: ", tiempo, "minutos"  
Fin  

# Bucles y Condicionales    

# 5. **Detección de turbulencia en trayecto**  
    
  Un sensor mide la aceleración vertical de la aeronave en intervalos de un segundo durante un trayecto de 2 minutos.    
  Si el valor medido supera un umbral, indicar que se ha detectado turbulencia en ese instante. Al final, mostrar    
  cuántas turbulencias se detectaron.       

  Inicio    
  segundo = 1    
  turbulencias = 0    
  Mientras segundo <= 120   
  Escribir "Ingrese su aceleración vertical: "     
  Leer aceleración   
  Si aceleración > umbral     
     Escribir "Turbulencia detectada"     
     turbulencias = turbulencias + 1     
 Fin mientras    
 Escribir "Total de turbulencias" , turbulencias  
 Fin   
  
    

# 6. **Control de temperatura en cabina**  

Un sistema mide cada 5 minutos la temperatura en cabina durante una hora. Si en algún momento se detecta una temperatura    
mayor a 27°C o menor a 18°C, debe indicar que se active el sistema de climatización.     

Inicio  
cont = 0  
Leer temp  
mientras cont < 12  
         si la temp >= 27 o temp <= 18  
         Mostrar " Activar climatización "  
         Fin si  
         cont = cont + 1   
Fin mientras  
Fin  

# 7. **Simulación de conteo de pasajeros**
    
Durante el abordaje, un sistema cuenta a los pasajeros que ingresan. Si el número total supera la capacidad máxima, el
sistema debe detener el conteo y mostrar un mensaje de alerta.

<img width="612" height="752" alt="Punto 7 drawio" src="https://github.com/user-attachments/assets/b8468f00-f33a-49e1-9402-9d1187be6012" />  


# Ejercicios mayor complejidad   

# 8. **Planificación de misión satelital**  
    
Desarrollar un algoritmo que reciba datos de consumo de energía por hora de un satélite durante un día completo. Si en  
cualquier hora el consumo excede un límite crítico, debe registrarse como una alerta. Al final, mostrar el consumo total  
y el número de alertas generadas.  

Inicio    
hora = 1    
total = 0    
alertas = 0    
Mientras hora <= 24   
         Escribir "Ingrese consumo de la hora", hora   
         Leer consumo  
         total = total + consumo  
         si consumo > límite  
         alertas = alertas + 1  
         Escribir "Alertas de consumo"  
         Fin si  
    hora = hora + 1      
Fin mientras   
Escribir "Consumo total: ",total    
Escribir "Número de alertas: ",alertas    
Fin  

# 9. **Simulación de carga y balanceo de aeronave**
    
Una aeronave tiene varias bodegas de carga. El sistema debe permitir ingresar el peso cargado en cada bodega y verificar que:  
    
- El peso total no exceda el máximo permitido  
- Ninguna bodega individual supere su límite.  
Mostrar mensajes de advertencia si alguna condición no se cumple.

Inicio  
total = 0  
Para bodega = 1 hasta 3  
Escribir "Ingrese peso de la bodega: ",bodega  
Leer peso  
     Si peso > límiteBodega   
     Escribir "Advertencia la bodega supera su límite.."    
Fin si    
total = total + peso    
Fin para    
Si total > límiteTotal    
   Escribir "Advertencia se supera a el peso máximo.."    
   si no  
   Escribir "Peso total permitido ✅"     
   Fin si  
Fin  
# 10. Monitoreo de aproximación a pista  

Durante la aproximación, un sistema recibe datos de altitud y velocidad cada 5 segundos hasta el aterrizaje. Si la velocidad  
excede el valor máximo seguro o la altitud no desciende adecuadamente, debe indicarse un mensaje de corrección de maniobra.  
Mostrar un resumen final de todos los avisos emitidos.

Inicio   
cont = 0    
leer vel, alt     
while altitud > 0    
      si velocidad > 250    
      Mostrar " Corregir altitud "    
      cont = cont + 1     
      fin si    
leer new_alt, new_vel    
fin mientras     
mostrar " Aterrizaje realizado "    
mostrar " resumen de avisos ", cont    
Fin    
 




   
