# Projecte compartició d'impressores

# Índex
*[Activitat 1 - Compartir una impressora de Linux a Windows](#1)
*[Activitat 2 - Compartir una impressora de Windows a Linux](#2)


<a id ="1"> </a>
## Activitat 1 - Compartir una impressora de Linux a Windows

Per a compartir una impresora de Linux a Windows, cal fer lo següent:


### **1. Instalar CUPS**

Aquest servei ens permetrà administrar les impresores

Instalar CUPS:

![image](https://github.com/user-attachments/assets/f3230ca4-6054-4a30-ae51-bb761ad16444)

Instalar drivers:

![image](https://github.com/user-attachments/assets/12bc4e35-91d2-4cfc-b698-7736ab566f3f)

Instalar impresora virtual:

![image](https://github.com/user-attachments/assets/a4baaafd-87f1-4b5a-a1a9-b3bb9cea711d)

### **2. Instalar Samba**

Aquest servei ens permetrà compartir les impresores i en el cas de Samba Client, poder utilitzar la impresora compartida desde Windows

Instalar Samba:

![image](https://github.com/user-attachments/assets/c7dd36db-6318-4627-9b3e-214085170a81)

Instalar Samba Client:

![image](https://github.com/user-attachments/assets/e47b56ae-d4a4-4991-b1ab-4bf22d85e73d)

### **3. Configuració de CUPS i creació de una impresora virtual**

Ara podem accedir a CUPS, per a accedir, tindrem que obrir un navegador i posar lo següent

```
localhost:631
```

Al introduirlo, ens portarà a aquesta pagina, i tindrem la interficie grafica de CUPS

![image](https://github.com/user-attachments/assets/edd71f96-37ec-447f-b1e2-7847333c5751)

Per a administar les impresores, anirem a la secció "Administration", aquí tindrem que activar les seguents caselles, les quals surten a la dreta (Despres d'activarles, assegurat de donarli a "Change Settings", sino no servira de res)

![image](https://github.com/user-attachments/assets/4e85ebc0-69a8-4138-9542-dab473af7550)

Després de canviar les opcions, afeixirem la impresora, en aquest cas, creare una virtual ja que no tinc una a mà, per això, li donarem a l'opció "Add Printer"

![image](https://github.com/user-attachments/assets/207f1250-6d47-46fb-89b9-626e4ee80e57)



![image](https://github.com/user-attachments/assets/f5fce0fd-fdd5-462a-a908-4b3f36275a73)

![image](https://github.com/user-attachments/assets/9e27334a-57d2-4749-bcfa-2b3f833933be)

![image](https://github.com/user-attachments/assets/14d22027-4b44-4b36-8669-4c46fe1fc5b6)

![image](https://github.com/user-attachments/assets/9094f854-9a91-4acc-ba93-eb5642973088)

Connectar la impressora a Windows

![image](https://github.com/user-attachments/assets/0873de7a-4c3f-457c-8c4b-7b25fb33c911)

![image](https://github.com/user-attachments/assets/0d561a2c-39d3-4453-82ed-a8783a99e297)

![image](https://github.com/user-attachments/assets/4fda3534-c3fc-4382-9e98-1db338b1a997)

![image](https://github.com/user-attachments/assets/4d4feb78-4960-4250-b6d1-48ab642fa75a)

![image](https://github.com/user-attachments/assets/a68d19e3-36b1-47cc-9811-995f8f10728b)

Prova d'impressio desde Windows a impressora de Linux
![image](https://github.com/user-attachments/assets/d4f2e860-819b-4671-9be6-0050c8738da2)

![image](https://github.com/user-attachments/assets/1403f3d3-db57-4c73-ae1c-d8ffd10b5618)

![image](https://github.com/user-attachments/assets/452e0a5a-3e79-4a4c-b540-e89b5749de21)


<a id ="2"> </a>

## Activitat 2 - Compartir una impressora de Windows a Linux

![image](https://github.com/user-attachments/assets/7a42e8ff-31e5-45ea-aef7-c8185fd57e3b)

Anem a Administracion de impressoras i fem clic dret a la nostre impressora i a propietats

![image](https://github.com/user-attachments/assets/66c31432-29b7-457f-b1c9-09ab7fe4e89b)

Anem a ús compartit

![image](https://github.com/user-attachments/assets/5ea53233-54ce-49d1-bbac-f54da89d9b31)

Fem clic a comparteix aquesta impressora

![image](https://github.com/user-attachments/assets/36d7affd-b981-40e4-a713-0d1060637d13)

Anem a Seguretat

![image](https://github.com/user-attachments/assets/e33c86d3-677f-42b7-b9e0-eba96d338821)

Li donem els permissos que considerem a els usuaris i li donem a Aplicar i Aceptar

![image](https://github.com/user-attachments/assets/f93f9061-694e-4c7d-b5cd-ecacfae48266)

Com veure una impresora compartida desde Windows a Linux

El unic requeriment per fer aixo es tenir Samba Client, teoricament instalat abans si has sigut el tutorial.

Al tindre Samba Client, i tenir una impresora compartida desde Windows a una mateixa xarxa, Linux hauria de poder veure l'impresora, sino... Pots provar a buscarla manualment. com a la imatge:

![image](https://github.com/user-attachments/assets/12d32310-ee7e-4ccf-99a7-13f3fec2a5fb)

Només hauria falta canviar la IP del exemple per la del Windows teu i el nom de l'impresora de exemple "PDFCreator" per el de la teva impresora.

I ahi la tens! Si no et surt pot ser perque no esta compartida correctament o Samba Client no funciona correctament o no esta instalat (a mi no em surtia perque ja la tenia afegida)

![image](https://github.com/user-attachments/assets/42c38f32-2002-4bc5-aeed-bc0ba55d4e12)


