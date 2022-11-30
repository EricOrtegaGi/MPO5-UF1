# Activitats: 

Per dibuixar els diagrames de flux podeu fer servir [draw.io](https://draw.io) o qualsevol altra eina online.

1. Calcula el CC de les següents figures:
  - ![image](https://user-images.githubusercontent.com/110727546/204613022-4ab64342-2e06-438d-a7e8-570685b3c406.png)
  - ![image](https://user-images.githubusercontent.com/110727546/204613180-6d55bf09-28b8-417e-96f4-f71a762ac44c.png)
  - ![image](https://user-images.githubusercontent.com/110727546/204655229-8c3f28d7-3d8b-4746-a55d-331f89da39d2.png)

### FORMULA: **x camins - y nodes + 2 = z**

  - **Resultat 1:**

16 - 14 + 2 = 4

  - **Resultat 2:**

16 - 14 + 2 = 4

  - **Resultat 3:**

8 - 6 + 2 = 4


2. Dibuixa el diagrama de flux representat per aquest codi i després calcula la seva CC:


![image](https://user-images.githubusercontent.com/114953110/204743467-d995c8ac-3ec2-4940-a564-5fe32b6bbc7e.png)
  - **Diagrama:**

![Diagrama sense títol (3)](https://user-images.githubusercontent.com/114953110/204749441-def8271e-b527-467f-b871-564907fb9998.jpg)

  - **Resultat CC:**
  - 2 sentencies condicionals + 1 = 3

3. Dibuixa el diagrama de flux representat per aquest codi i després calcula la seva CC:

```
public class proves {
    public static  String queEmPoso(int temperatura) {
        String roba = "res";
        if(temperatura<0){
           roba = "roba d'esquiar";
        }
        else if(temperatura<10){
           roba = "roba de muntanya";
        }
        else if(temperatura<20){
           roba = "roba d'hivern";
        }
        else if(temperatura<30){
           roba = "roba d'estiu";
        }
        return roba;
    }    
}
```

  - **Diagrama:**
![Diagrama sense títol (2)](https://user-images.githubusercontent.com/114953110/204748111-95cc177e-4664-4bbd-9c47-11e70396a569.jpg)


  - **Resultat CC:**
  - 4 sentencies condicionals + 1 = 5

4. Dibuixa el diagrama de flux representat per aquest codi, calcula la seva CC i crea una prova per a cada camí posible:

```
    public static Boolean llumsEncesos(int hora) {
        Boolean llums = false;
        if(hora <= 8 || hora >= 20){
            llums = true;
        }
        return llums;
    }
```
  - **Diagrama:**
![Diagrama sense títol (5)](https://user-images.githubusercontent.com/114953110/204754919-f6175452-e762-41b5-8937-44f8077c323f.jpg)


  - **Resultat CC:**
  - 2 sentencies condicionals + 1 = 3
  - **Resultat proves camins:**
  - 1: hora >= 20 llums = true, return llums
  - 2: hora <= 8, llums = true, return llums
  - 3: hora > 8 --> hora < 20 --> llums false, return llums

5. Investiga sobre les proves de caixa negra:

  - Què són?
  - Es el metode de probes que es realitza a un element estudiat desde el punt de vista de les entrade que reb i les sortides o respostes que produeix

  - Quina diferència principal tenen sobre les de caixa blanca?

  - la diferencia principal entre aquests dos metodes de probes es que en el de caixa negra desconeixem la estructura disseny o implementacio interna dels elements que estem probant 
