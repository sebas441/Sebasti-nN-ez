## Bucles y/o Ciclos  
# Ejemplo 1  
numero = 1  
while numero <= 5:  
    print(numero)  
    numero += 1      #numero = numero + 1  


# Ahora cambia que el número inicial sea 10 y llegue hasta 50 contando solo los números primos    
 
numero = 10  
while numero <= 50:   
    print(numero)  
    numero += 2      #numero = numero + 1  

# Ahora imprimir los números entre 1000 y 0 en orden descendente múltiplos de 13  

numero = 1000  
while numero > 0:  
    if numero % 13 == 0:  
        print(numero)  
    numero -= 1  
