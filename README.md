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

