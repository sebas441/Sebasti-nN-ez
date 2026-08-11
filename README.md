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

# Ejercicio 2 Taller   
 
2. **Control de temperatura del motor**  
    
Durante una inspección de rutina, se mide la temperatura de un motor de turbina. Si la temperatura es mayor a un valor crítico,  
se debe indicar "Peligro: sobrecalentamiento". Si está dentro del rango seguro, indicar "Operación normal". Si es demasiado baja,  
indicar "Motor frío – Calentar antes de operar".  

 
<img width="702" height="832" alt="Taller Ejercicio2 drawio (1)" src="https://github.com/user-attachments/assets/0d5a477a-b17d-4764-86b3-843adf9bda64" />  

Bucles   
1. **Registro de altitudes de vuelo**  
    
Un sistema debe registrar la altitud de vuelo cada 10 minutos durante una hora y mostrar todas las mediciones al final.  

Inicio 
cont = 0
leer alt_max
while alt_max sea >= max 0.1
      cont = cont + 1     
fin while
Mostrar " Tiempo transcurrido " cont
Fin

Bucles y Condicionales

2. **Control de temperatura en cabina**

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

Ejercicios mayor complejidad 

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





   
