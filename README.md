

# Java

```java
class Main{
  public static void main(String[] args){
    System.out.println("Hello world");
  }
}
```

Description de la fonction main
La fonction "main" est la fonction principale d'un programme en java. C'est ici que on crée les objets et que l'on compose l'interface utilisateur en ligne de commande. Elle s'écrit de la manière suivante :
```java
public static void main(String[] args)  {        
        garage g = new garage();
        int choix;
        int choix2;
        int panne;
        String NomDeVoiture;
        String NomDeMoto;
        do {            
            
            System.out.println("_____MENU_____");
            System.out.println("0.Quitter");
            System.out.println("1.Montrer Garage");
            System.out.println("2.Ajouter");
            Scanner reader = new Scanner(System.in);
            choix = reader.nextInt();
            switch(choix){
                case 1:
                    System.out.println(g);
                    break;
                case 2:
                    System.out.println("---CHOIX DU VEHICULE---");
                    System.out.println("1.Voiture");
                    System.out.println("2.Moto");
                    Scanner reader2 = new Scanner(System.in);
                    choix2 = reader2.nextInt();
                    switch(choix2){
                        case 1:
                            System.out.println("Taper le nom:");
                            Scanner reader3 = new Scanner(System.in);
                            NomDeVoiture = reader3.nextLine();
                            System.out.println("En Panne?");
                            System.out.println("1.Oui");
                            System.out.println("2.Non");
                            Scanner reader5 = new Scanner(System.in);
                            panne = reader5.nextInt();
                            if (panne==1) {
                                g.add(new voiture(NomDeVoiture));
                                
                            }
                            break;
                        case 2:
                            System.out.println("Taper le nom");
                            Scanner reader4 = new Scanner(System.in);
                            NomDeMoto = reader4.nextLine();
                            System.out.println("En Panne?");
                            System.out.println("1.Oui");
                            System.out.println("2.Non");
                            Scanner reader6 = new Scanner(System.in);
                            panne = reader6.nextInt();
                            if (panne==1) {
                                g.add(new moto(NomDeMoto));
                                
                            }
                    }
                   
                 
            }
        }while (choix != 0);
    }
    
}
```
Voici un exemple ci-dessus pour une classe main.

##Prototype d'une méthode

Une méthode est rendue unique et distincte grâce à son prototype : nom de la méthode, type de valeur de retour, liste et types des arguments)

##Types

##Classe

##Instance

##Constructeur

##Static

Usage du mot clé `static`

##Abstract

Usage du mot clé `abstract`

##Boucles

##Classes utilitaires

1.    ArrayList



##Interfaces

##Exceptions
1.  try... catch... finally

2. throw

3. throws

# Design Patterns

##Decorator

Permet d'agrémenter un objet de nouvelles methodes en l'encapsulant dans une classe Decorator.

##Singleton

Description du singleton

##Observer

![Pattern Observer](https://raw.githubusercontent.com/clm-a/java-notes/master/observer.png "Pattern Observer")

Description d'observer

##MVC

Description du pattern MVC

##Factory

Description du pattern Factory
