## Condicionales   
print(10 > 5)  
print("Hola" != "Mundo")  
que imprimira?? imprime True  

 x = "hola"   
type(x)  
<class'str'>  
a = 3.14 <= 4.5   
print(3.14 <= 4.5)  
dira que es buleano como en todos   

nombre = "Juan"  
print(nombre == "Juan")  
true  

## Ejercicio 2  
 
Resuelve el siguiente problema usando el condicional simple.  

Un almacén cobra `$9 000` por costos de envío, pero ofrece el envío a domicilio gratis para compras superiores a `$100 000`. En caso contrario,  
no hay ningún descuento. Solicite al usuario el valor de la compra y calcule el valor total a pagar.  

## Análisis del problema  

Para resolver este problema, te propongo analizarlo usando un diagrama de flujo. Este tipo de diagramas son muy útiles para entender la manera  
como se va ejecutando el programa, es decir, su flujo de ejecución.  

<img width="433" height="399" alt="image" src="https://github.com/user-attachments/assets/5d294be6-32b4-4941-b672-a1c6a4bc1ace" />  


Ahora intenta escribir el código de la solución en lenguaje Python.   

envio = 0  
compra = int(input("Ingrese el valor de la compra>> "))  
if compra < 100000:  
	envio = 9000  
total = compra + envio  
print(f"El total de la compra es {total}")  

⚠️ Advertencia  
Recuerda que = es para asignar valores, mientras que == es para comparar.  
 
## Ejercicio 4  

El Ministerio de Salud clasifica las personas según las etapas del ciclo de vida, con el fin de tener una idea sobre su vulnerabilidad.  
Diseñe un algoritmo que pida al usuario su edad y la clasifique según la etapa del ciclo de vida que le corresponda. Verifique que el  
usuario no ingrese valores menores a cero. Clasificación etaria de la población colombiana:  

- Infancia [0-6) años)     
- Niñez [6 - 12) años)     
- Adolescencia (12 - 20 años)     
- Juventud (20 - 25 años)     
- Adultez (25- 60 años)      
- Ancianidad / Vejez (60 años o más)   

Edad = int(input("Introduzca su edad actual: "))    
if Edad > 0:   
    if Edad <= 6:  
        etapa = "Infancia"    
    elif Edad < 12:  
        etapa = "Niñez"   
    elif Edad < 20:   
        etapa = "Adolecencia"   
    elif Edad < 25:  
        etapa = "Juventud"  
    elif Edad < 60:  
        etapa = "Vejez"   
    else:  
        etapa = "Vejez"   
else:  
     print("Edad invalida")  
 
print(f"Usted está en la etapa: {etapa} ")  

## Ejercicio Calculadora  

a = float(input("Ingrese número 1: "))  
oper = input("Ingresa la operación deseada +,-,*,/, ^: ")  
b = float(input("Ingrese número 2: "))  
if oper == '+':  
    resultado = a + b  
elif oper == '-':  
    resultado = a - b  
elif oper == '*':  
    resultado = a * b  
elif oper == '/':  
    resultado = a / b   
elif oper == '^':  
    resultado = a ** b  
else:  
    print("Sintax error")  
    resultado = "No ejecutado"  
print(f"{a} {oper} {b} = {resultado} ")  

## Otro pero con case
a = float(input("Ingrese número 1: "))
# oper = input("Ingresa la operación deseada +,-,*,/, ^: ")
# b = float(input("Ingrese número 2: "))

# match oper:

    case '+':
        resultado = a + b
    case '-':
        resultado = a - b
    case '*':
        resultado = a * b
    case '/':
        if b == 0:
            print("Sintax error")    ## Averiguar el error
    case '/': 
            resultado = a / b 
    case '^':
        resultado = a ** b
    case _:
        print("Sintax error")
        resultado = "No ejecutado"
print(f"{a} {oper} {b} = {resultado} ")









