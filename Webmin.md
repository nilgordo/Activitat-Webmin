# Utilitzant webmin per administrar el servidor

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


  sudo apt install nsnake
- Utilitza webmin per instal·lar gimp de apt.
- Utilitza webmin per desinatl·lar el joc que heu instal·lat abans.

## 4.- Serveis

- Utilitza webmin per mostrar els serveis que s'inicien amb el sistema.
- Utilitza webmin per mostrar els serveis que estan actius.
- ----------------------------------------------------------------------
- Utilitza webmin per mostrar l'estat del servidor Apache.
- Utilitza webmin per aturar Apache.
- Utilitza webmin per mostrar l'estat del servidor Apache apagat.
- Utilitza webmin per reiniciar Apache.
- Utilitza webmin per mostrar l'estat del servidor Apache reiniciat.

## 5.- Quotes de disc

Activa les quotes de disc pels usuaris amb la comanda: 

```
sudo apt install quota quotatool
```

- Utilitza webmin perquè l'usuari bakalao_X no pugui tenir més de 2 MB d'informació al disc.
- Comprova que el límit de la quota funciona.
- Utilitza webmin perquè l'usuari techno no pugui tenir més de 10 fitxers al disc.
- Comprova que el límit de la quota funciona.

## 6.- Còpies de seguretat

- Utilitzant el mòdul de Webmin Filesystem Backup fes una còpia de seguretat del directori /home al directori /backups (l'haureu de crear si no existeix).
- Modifica alguns fitxers de /home.
- Recupera la còpia de seguretat.
- Comprova que els fitxers de /home són els correctes.
- Programa una còpia de seguretat de /home/bakalao_X per els divendres a les 21:00.
- Esborra la còpia de seguretat programada anteriorment.

## 7.- Compartició

- Crea un recurs a webmin que, utilitzant samba, comparteixi una carpeta anomenada "area_public_X" per a usuaris sense autenticar en forma de lectura i escriptura.
- Crea un recurs a webmin que, utilitzant samba, comparteixi una carpeta anomenada "pontaeri_privat_X" per a usuaris _X i techno només de lectura.
- Comprovar des de Windows que aquests recursos funcionen.
