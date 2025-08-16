# paradigmas-de-programacion

# 🧮 Calculadora en Python (Paradigma Estructurado)

## 📌 Descripción
Se resaliza una **calculadora simple en Python** desarrollada bajo el paradigma impérativa estructurado, usando instrucciones secuenciales.

La calculadora permite realizar las siguientes operaciones:  
- Suma  
- Resta  
- Multiplicación  
- División  

El programa se ejecuta en un *bucle repetitivo*, mostrando un menú de opciones hasta que el usuario decida salir.  

---

## ⚙️ Funcionamiento
1. Se muestra un menú de opciones en pantalla.  
2. El usuario elige la operación que desea realizar.  
3. Si la opción es válida, se piden dos números.  
4. El programa realiza la operación y muestra el resultado.  
5. El proceso se repite hasta que el usuario elija salir (opción 5).  

---

## 💻 Código principal

```python
while True:
    print("\n1. Sumar")
    print("2. Restar")
    print("3. Multiplicar")
    print("4. Dividir")
    print("5. Salir")

    opcion = input("Elige una opción: ")

    if opcion == "5":
        print("Fin de la calculadora")
        break

    num1 = float(input("Número 1: "))
    num2 = float(input("Número 2: "))

    if opcion == "1":
        print("Resultado:", num1 + num2)
    elif opcion == "2":
        print("Resultado:", num1 - num2)
    elif opcion == "3":
        print("Resultado:", num1 * num2)
    elif opcion == "4":
        if num2 != 0:
            print("Resultado:", num1 / num2)
        else:
            print("Error: no se puede dividir entre cero")
    else:
        print("Opción inválida")
```

---

## 📊 Ejemplo de ejecución

```
1. Sumar
2. Restar
3. Multiplicar
4. Dividir
5. Salir

Elige una opción: 1
Número 1: 10
Número 2: 5
Resultado: 15.0
```

---

## 📚 Conclusión
realizo un ejemplo sencillo del uso del **paradigma estructurado en Python**, aplicando:  
- **Secuencia** → instrucciones paso a paso.  
- **Condicionales** → decisiones con `if - elif - else`.  
- **Repetición** → bucle `while` para mantener activo el menú.  
