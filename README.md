# LasActividadesVanAqui
Las actividades de Inteligencia artificial van aqui
#Ejercicios Basicos en Python, Ramon Samuel Blanco Ramirez, 1905501, N1
nosaludar = ["Ana", "Juan", "Pedro"]#lista de nombres que no debe saludar
nombre = input("Cual es tu nombre: ") #preguntar cual es tu nombre
z=0 
for x in nosaludar:
    if nombre == x:
        z=z+1  
        break   
#se declara la variable z para contar si el nombre es alguno de la lista
if z==0: #si la condicion anterior no se cumplio siginifica que x aun es 0
    print("Hola ",nombre)
#sino no dira nada
print("//////////////")#separacion
def x_function(lista):#crear funcion para invertir lista
    newlista=lista[::-1]#se usa -1 para hacerlo y se imprime
    for x in newlista:
        print(x)

ola = ["va", "le","como","profe", "ola"]#listas aleatorias
thistuple = ("apple", "banana", "cherry", "apple", "cherry")#lista aleatoria
x_function(ola) #invertir lista
print("//////////////")
def marco_funtion(lista): #funcion para hacer un marco donde este centrada 
    print("********************")#imprimo el encabezado del marco
    for x in lista: 
        z=len(x) #veo cuantos caracteres tiene cada uno de los elementos de la lista
        f=round((18-z)/2) #hago un calculo para centrarla
        print("*", end="") #imprimo el primero *
        for v in range(f): #imprimo el espacio suficiente para que quede centrado usando un for
            print(end=" ")
        print(x, end="") #imprimo la palabra
        q=18-f-z#hago un calculo para saber cuanto espacio falta 
        for g in range(q):#lo imprimo
            print(end=" ")
        print("*")#imprimo el * final
    print("********************")#imprimo la base

marco_funtion(thistuple)
