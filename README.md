# Manejo-De-Archivos-Gutierrez-Gayosso-Jose-Alejandro-1185-3W

2=Para abrir el archivo, utilice la función incorporada open().
La open()función devuelve un objeto de archivo, que tiene un read()método para leer el contenido del archivo:
EjemploObtenga su propio servidor Python
f = open("demofile.txt", "r")
print(f.read())
![image](https://github.com/user-attachments/assets/c3bfe21e-d409-4d70-9f61-066cabb4dbeb)

![image](https://github.com/user-attachments/assets/45ecb928-79fc-4e3a-968d-923102b1fdb7)

3=Si el archivo se encuentra en una ubicación diferente, deberá especificar la ruta del archivo, de esta manera:
Ejemplo
Abrir un archivo en una ubicación diferente:
f = open("D:\\myfiles\welcome.txt", "r")
print(f.read())

![image](https://github.com/user-attachments/assets/300df4c5-e81e-4e35-a1a4-2e9ba3e19d9b)

![image](https://github.com/user-attachments/assets/ef047384-4fbe-4975-8e42-a9d6a96a6407)

4= Leer solo partes del archivo
De forma predeterminada, el read()método devuelve el texto completo, pero también puedes especificar cuántos caracteres quieres devolver:
Ejemplo
Devuelve los 5 primeros caracteres del archivo:
f = open("demofile.txt", "r")
print(f.read())

![image](https://github.com/user-attachments/assets/b5f3852b-b545-497b-9b59-95d3d55393c1)

![image](https://github.com/user-attachments/assets/953d2e73-2fd8-4be9-963b-5dcffa190bd7)


5=Escritura de archivos en Python
❮ AnteriorPróximo ❯Escribir en un archivo existente
Para escribir en un archivo existente, debe agregar un parámetro a la open()función:
"a"- Anexar - se agregará al final del archivo
"w"- Escribir: sobrescribirá cualquier contenido existente

![image](https://github.com/user-attachments/assets/98763251-d5f4-488a-8b56-8dfef20aa728)

![image](https://github.com/user-attachments/assets/da0d0fc6-dc71-4689-97ae-a544e6dea2c9)

6=Ejemplo
Abra el archivo "demofile3.txt" y sobrescriba el contenido:
f = open("demofile3.txt", "w")
f.write("Woops! I have deleted the content!")
f.close()
#open and read the file after the overwriting:
f = open("demofile3.txt", "r")
print(f.read())

![image](https://github.com/user-attachments/assets/bd387bb3-5023-49a1-9f49-98e47e617870)

![image](https://github.com/user-attachments/assets/5b93ae75-2337-424e-87f6-61a4079cbaab)

7= liminar archivo de Python
❮ AnteriorPróximo ❯Eliminar un archivo
Para eliminar un archivo, debes importar el módulo del sistema operativo y ejecutar su os.remove()función:
Ejemplo
Eliminar el archivo "demofile.txt":
import os
os.remove("demofile.txt")

![image](https://github.com/user-attachments/assets/6bab8945-931d-46d6-8af0-3e2c570babc4)

![image](https://github.com/user-attachments/assets/86ad6026-ca8a-4da3-903a-379272722580)

8=Comprobar si el archivo existe:
Para evitar obtener un error, es posible que desees verificar si el archivo existe antes de intentar eliminarlo:
Ejemplo
Comprueba si el archivo existe  elimínalo:
import os
if os.path.exists("demofile.txt"):
  os.remove("demofile.txt")
else:
  print("The file does not exist")
![image](https://github.com/user-attachments/assets/c2a199a3-aaf5-47c9-9afe-3926058df3f6)

![image](https://github.com/user-attachments/assets/3f01eaaa-4968-4882-9857-8026e1666a56)

9=Eliminar carpeta
Para eliminar una carpeta entera, utilice el os.rmdir()método:
Ejemplo
Eliminar la carpeta "myfolder":
import os
os.rmdir("myfolder")
