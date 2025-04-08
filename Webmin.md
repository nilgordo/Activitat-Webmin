- Entregueu link a un repositori **públic** (un link per alumne) de Github on feu les següents tasques.
- Expliqueu el que feu amb text i captures.
- **Fer tot des de webmin**
- Rúbrica:
  - 2 punts - Estructura del document (portada, índex, captures correctes, text ben formatat...).
  - 1 punt - Exercici 1.
  - 1 punt - Exercici 2.
  - 1 punt - Exercici 3.
  - 1 punt - Exercici 4.
  - 1.5 punt - Exercici 5.
  - 1.5 punt - Exercici 6.
  - 1 punt - Exercici 7.


# Utilitzant webmin per administrar el servidor
![image](https://github.com/user-attachments/assets/382a9ff1-7b10-42d5-b3ef-ec1571905910)

# Índex
  
* [1.- Crear i modificar usuaris](#1)
* [2.- Programar tasques](#2)
* [3.- Instal·lació de software](#3)
* [4.- Serveis](#4)
* [5.- Quotes de disc](#5)
* [6.- Còpies de seguretat](#6)
* [7.- Compartició](#7)




<a id="1"> </a>

## 1.- Crear i modificar usuaris

**Fer tot des de webmin**

- Has de crear dos usuaris bakalao_X i techno_X on (X és el vostre cognom).
  ![image](https://github.com/user-attachments/assets/bec525cc-790f-47fa-b56a-3f6f322eff41)
  ![image](https://github.com/user-attachments/assets/9d10e6e8-da20-43d8-8f33-6ff5dfb3a540)
  Baixem i donem a Crear
  ![image](https://github.com/user-attachments/assets/fafb4c54-f2f3-4d69-b975-d6fbf02caf5e)
  Baixem i donem a Crear
  
- Els usuaris et passaran el hash de la seva contrasenya, no la contrasenya real. (podeu fer servir openssl).
  ![image](https://github.com/user-attachments/assets/9a463782-ac0c-4dc4-a954-d50863f04f47)
  ![image](https://github.com/user-attachments/assets/996b9748-4169-4a7c-a68c-de32d7698555)

- Cada usuari tindrà un directori a home igual al seu nom d'usuari.
  ![image](https://github.com/user-attachments/assets/f8c69151-50d1-48ed-bba6-9961234c6efb)
  Fet automaticament en el procees de creació de l'usuari
  
- Utilitzaran bash com a shell.
  ![image](https://github.com/user-attachments/assets/2124cb79-9f56-4c26-861c-5c1a834004e9)
  Baixem i donem a Guardar
  ![image](https://github.com/user-attachments/assets/cf6d7b0e-773c-492a-8e77-3d4b783926f1)
  Baixem i donem a Guardar


- Els usuaris estaran dins del grup que tingui el seu mateix nom i dins del grup usuaris_empresa.
  Creem el grup de bakalao_Gordo i techno_Gordo i usuaris_empresa
  ![image](https://github.com/user-attachments/assets/dba47e45-9479-4eda-b82e-772c59845e87)

  ![image](https://github.com/user-attachments/assets/68e97669-1928-4ec0-ac5f-37e8781c547b)

  ![image](https://github.com/user-attachments/assets/d404dc05-830b-4751-965a-22b6bbca0659)

  Entrem a l'usuaris i canviem els seus grups
  ![image](https://github.com/user-attachments/assets/2ddc1536-78bd-47ea-8213-aeb8d1dfb557)
  ![image](https://github.com/user-attachments/assets/25a705bf-34f8-4ef4-8221-36178a6ccda9)

  Li donem a Guardar
  
- L'usuari techno no podrà fer login després del dia 31-03-2025.
  
  ![image](https://github.com/user-attachments/assets/3803868b-02fb-4c3c-8ac1-c1bd9ce8d8bf)
  
  Li donem a Guardar
  
- Comproveu que els usuaris poden iniciar sessió.
  
  ![image](https://github.com/user-attachments/assets/5f4ecb4a-02dd-42ad-b955-259bce1f1246)

- Canvia la data del sistema (utilitzant webmin) i comprova que techno no pot iniciar sessió si estem a dia 01-04-2025.
  ![image](https://github.com/user-attachments/assets/3e00626c-dbe1-4c7e-91e6-9690933fd056)

  ![image](https://github.com/user-attachments/assets/eae9ca41-93f4-40c7-b9a4-4ba6440d5c18)

  ![image](https://github.com/user-attachments/assets/819c4fe8-f749-43bc-9326-34e7802e8fd8)

  ![image](https://github.com/user-attachments/assets/cfe20f85-7e4d-4bad-ab30-65d95b07acf2)


<a id="2"> </a>
## 2.- Programar tasques

- Programa una tasca que neteja els paquets de Linux que ja no s'utilitzen una vegada al mes.
  ![image](https://github.com/user-attachments/assets/8d022e6b-0f7d-45a1-abef-9e8c0fbc6382)

  ![image](https://github.com/user-attachments/assets/b0c692fb-e804-4de9-af68-f5c06ea297c4)

  Baixem i li donem a Crear


- Programa una tasca diaria que apaga l'ordinador a les 14:00.
  ![image](https://github.com/user-attachments/assets/ab41ec04-efc1-431f-92e6-6fda981bc9c4)

  Baixem i li donem a Crear

- Comprova que funcionen (canvia dia i hora del sistema mitjançant webmin).
  ![image](https://github.com/user-attachments/assets/ef9f69b1-8031-42eb-8d66-caaecc010f1b)


  <a id="3"> </a>

## 3.- Instal·lació de software

- Utilitza webmin per mostrar quins paquets de software es podrien actualitzar.
  ![image](https://github.com/user-attachments/assets/608fa2a9-1ce4-4b68-abfe-531f8b8cd6ab)
  ![image](https://github.com/user-attachments/assets/06248580-1d38-4ef6-b257-e06e1d5b6a5f)

- Des de webmin actualitza un paquet.
  ![image](https://github.com/user-attachments/assets/410cc604-8cdb-45e8-a281-8b7688d15d87)
  Seleccionem un paquet en aquest cas el acl i li donem a Update Select packages
  ![image](https://github.com/user-attachments/assets/79580d08-688e-4f45-8c52-93e705122251)
  Li donem a install now
  ![image](https://github.com/user-attachments/assets/9ea29b6e-a8e3-456a-b84d-5284e1507a6b)
  Ja tindriem el paquet actualitzat

- Utilitza webmin per instal·lar un joc de apt.
  ![image](https://github.com/user-attachments/assets/7e57f64d-4d24-46fd-ad53-137e7ba8ec33)
  Anem a Software packages i anem a install a new package
  ![image](https://github.com/user-attachments/assets/ab5bee77-88f5-4688-9585-8d995178fdc5)
  Li donem a Package from APT
  ![image](https://github.com/user-attachments/assets/a0e71763-fe7c-4d4d-9090-9c6066b98e9e)
  Introduim nsnake a Package from APT i li donem a Install
  ![image](https://github.com/user-attachments/assets/397ffacc-9b96-4dc6-bd2f-2524e69a3063)
  Li donem a Install now
  ![image](https://github.com/user-attachments/assets/91b78d9a-22e8-463a-8723-fc591c3ea75a)
  Ja estaria instal·lat
  ![image](https://github.com/user-attachments/assets/87aa3973-c6c4-46dc-b0a1-efbdc5687fe4)


- Utilitza webmin per instal·lar gimp de apt.
  ![image](https://github.com/user-attachments/assets/7d89862f-c5ff-443b-9edb-f2027d11187f)
  Introduïm gimp a Package from APT i li donem a Install
  ![image](https://github.com/user-attachments/assets/37566ef6-8f2d-4c5b-968a-2a63bb8b4776)
  Li donem a install now
  ![image](https://github.com/user-attachments/assets/1b4d10da-ace9-4409-9f91-fb9ade781f53)
  Ja tenim el gimp instalat
  ![image](https://github.com/user-attachments/assets/04412cd1-c759-48d5-8c18-10975a57b099)

- Utilitza webmin per desinatl·lar el joc que heu instal·lat abans.
  ![image](https://github.com/user-attachments/assets/04b26cfe-7279-4904-9449-3ad5be236998)
  Introduïm nsnake al search for package
  ![image](https://github.com/user-attachments/assets/183425ef-e361-4ff6-9798-b0d421b2dc17)
  Fem click a Search for package
  ![image](https://github.com/user-attachments/assets/e3fb9b18-f6ad-488f-9182-ed23a8010b13)
  Li donem a Uninstall
  ![image](https://github.com/user-attachments/assets/d8164a50-75c0-44a6-9f7f-ddadabafd299)
  Li donem a Delete
  I ja no el tenim instalat
  ![image](https://github.com/user-attachments/assets/4847571a-5f69-41a4-8f85-6073c3ce710e)

<a id="4"> </a>
  
## 4.- Serveis

- Utilitza webmin per mostrar els serveis que s'inicien amb el sistema.
  Anem a Bootup and Shutdown
  ![image](https://github.com/user-attachments/assets/5b6e2179-ea6e-47e3-a4f4-f16378071c3c)
  I en aquest apartat tots els serveis que fica Start at boot? Yes, vol dir que s'inicien amb el sistema, si baixem podem veure més serveis
  
- Utilitza webmin per mostrar els serveis que estan actius.
  
  Desde el mateix apartat podem veure els serveis actius, si mirem la columna de Service Status
  ![image](https://github.com/user-attachments/assets/9937f3ee-9d7c-4d1e-9768-6a4c80e56933)

- Utilitza webmin per mostrar els serveis que s'inicien amb el sistema.

  ![image](https://github.com/user-attachments/assets/52e42d21-9ce4-423d-b48f-557f5ddf0420)

- Utilitza webmin per mostrar els serveis que estan actius.

  ![image](https://github.com/user-attachments/assets/e35ac7dd-ba00-4ead-97a9-4211e64e6dd8)

- Utilitza webmin per mostrar l'estat del servidor Apache.

  ![image](https://github.com/user-attachments/assets/d6673e96-13f6-4561-97cd-d0936d390d79)

- Utilitza webmin per aturar Apache.

  ![image](https://github.com/user-attachments/assets/44a28203-ef34-436c-9acc-7b12a9cfa50c)

- Utilitza webmin per mostrar l'estat del servidor Apache apagat.

  ![image](https://github.com/user-attachments/assets/b427431c-11ac-444d-8313-14098a1ba157)

- Utilitza webmin per reiniciar Apache.

  ![image](https://github.com/user-attachments/assets/c0e31830-60fc-469f-a29b-fd6fda4106c7)

- Utilitza webmin per mostrar l'estat del servidor Apache reiniciat.

  ![image](https://github.com/user-attachments/assets/04be2112-456f-42cb-8f95-694cd8a82e61)

  ![image](https://github.com/user-attachments/assets/f35f2a46-15ea-49dd-90a4-ed826cbc20a1)

  <a id="5"> </a>

## 5.- Quotes de disc

Activa les quotes de disc pels usuaris amb la comanda: 

```
sudo apt install quota quotatool
```
  ![image](https://github.com/user-attachments/assets/0a9b6018-5f02-4678-8234-944ba232cb98)

- Utilitza webmin perquè l'usuari bakalao_X no pugui tenir més de 2 MB d'informació al disc.

  ![image](https://github.com/user-attachments/assets/9eab0203-1faa-4d6a-baa3-2c91243fddae)

- Comprova que el límit de la quota funciona.

  ![image](https://github.com/user-attachments/assets/b87fb140-74fd-4907-84cb-7bda96afce76)

- Utilitza webmin perquè l'usuari techno no pugui tenir més de 10 fitxers al disc.

  ![image](https://github.com/user-attachments/assets/a6d342b0-5057-41d6-abd3-c97e3f35dcec)

- Comprova que el límit de la quota funciona.

  ![image](https://github.com/user-attachments/assets/0dbdf0c4-3201-45af-b7be-f14965d4c634)

  <a id="6"> </a>

## 6.- Còpies de seguretat

- Utilitzant el mòdul de Webmin Filesystem Backup fes una còpia de seguretat del directori /home al directori /backups (l'haureu de crear si no existeix).

  ![image](https://github.com/user-attachments/assets/8baef292-3235-423d-911e-476093c616f5)

- Modifica alguns fitxers de /home.

  ![image](https://github.com/user-attachments/assets/2ec7c4f1-6339-47be-b9d7-b4d285e04db1)

- Recupera la còpia de seguretat.

  ![image](https://github.com/user-attachments/assets/adfa693f-1575-4061-9f73-dd19991e9703)

- Comprova que els fitxers de /home són els correctes.

  ![image](https://github.com/user-attachments/assets/c32919cc-9a36-45d1-86a2-51a3f32f7068)

- Programa una còpia de seguretat de /home/bakalao_X per els divendres a les 21:00.

  ![image](https://github.com/user-attachments/assets/877fbc2b-30d7-431f-8cec-da0e8a68b0f1)

- Esborra la còpia de seguretat programada anteriorment.

  ![image](https://github.com/user-attachments/assets/7f78889e-e159-495f-b511-debde9d4e2e2)

  ![image](https://github.com/user-attachments/assets/7d1425d8-185d-4e6e-8ce6-8c6144ba3418)

    <a id="7"> </a>

## 7.- Compartició

- Crea un recurs a webmin que, utilitzant samba, comparteixi una carpeta anomenada "area_public_X" per a usuaris sense autenticar en forma de lectura i escriptura.
  ![image](https://github.com/user-attachments/assets/04f4eef4-7ed2-464e-8893-59ba1ae4f14f)
  ![image](https://github.com/user-attachments/assets/60325078-eabb-4b62-b290-bbd9b960f384)
  ![image](https://github.com/user-attachments/assets/f2c4dc6a-5176-4f26-8def-d51ebf0e25d5)
  ![image](https://github.com/user-attachments/assets/cc26bab7-df3a-41a0-9517-edea7823afb2)

  ![image](https://github.com/user-attachments/assets/c87071b4-9630-4eb6-9daf-752503c05352)

  ![image](https://github.com/user-attachments/assets/3680530b-2f3d-42fa-acd1-dd00a6ce2d2d)
  I li donem a Save

  ![image](https://github.com/user-attachments/assets/ab8966f2-0447-4ca5-b98d-b751ec55a328)

  ![image](https://github.com/user-attachments/assets/7723f25f-b19d-441f-8232-b6f1c42260fe)

  ![image](https://github.com/user-attachments/assets/1f6b51ed-6182-44a3-b0ef-220f3bc1c023)






- Crea un recurs a webmin que, utilitzant samba, comparteixi una carpeta anomenada "pontaeri_privat_X" per a usuaris _X i techno només de lectura.

  ![image](https://github.com/user-attachments/assets/9d994a91-ef52-4102-a3af-db6fa0077253)

  ![image](https://github.com/user-attachments/assets/d263d769-8fac-43db-8c3a-36e6343508e4)

  ![image](https://github.com/user-attachments/assets/08633cf0-ba03-4f93-95be-eca89731df52)

  ![image](https://github.com/user-attachments/assets/c3ad7d3f-92f8-4782-ae27-936d0e32dc7f)

  ![image](https://github.com/user-attachments/assets/f061eabe-2f81-4ad1-897e-5826c119e2b8)

  ![image](https://github.com/user-attachments/assets/d8da4103-39ae-44ff-8240-ac849ed8f9c3)



- Comprovar des de Windows que aquests recursos funcionen.

  ![image](https://github.com/user-attachments/assets/ab5a0c7f-a144-4d09-9611-77822ab3a0e4)

  ![image](https://github.com/user-attachments/assets/a8beeba1-5c70-4cf7-a12f-2d799dd067c3)

  ![image](https://github.com/user-attachments/assets/95d8d90d-9997-42c0-89f8-fc74de5427bf)

  ![image](https://github.com/user-attachments/assets/f2e28a07-82aa-4b8d-9a4a-afbac14bd27d)

  ![image](https://github.com/user-attachments/assets/3bfc573d-2a46-4f0f-9b47-4618cea7242a)

  ![image](https://github.com/user-attachments/assets/b2e87223-9f7b-4219-814b-a89fc6e0a03f)


