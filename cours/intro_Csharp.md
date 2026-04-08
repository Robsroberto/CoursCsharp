---
marp: false
size: 4:3
style: |
  h2, h3, p {
    font-size: 20px;
  }
  li {
    font-size:20px
  }
headingDivider: 1
header: 
paginate: 
footer: Licence 2 Informatique &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ISI (Institut Supérieur D'Informatique) &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; RD
---
<img src="../isi.png" alt="ISI" width="100px">


## **Cours d’introduction au C# – Bases du Langage**

## Par Robert DIASSÉ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
<img src="../C_sharp.png" alt="ISI" width="50px">

### **1. Présentation de C#**
**C#** (prononcé "C Sharp") est un langage de programmation **orienté objet** créé par Microsoft. Il est conçu pour être :
- **Simple à apprendre** : La syntaxe est claire et structurée.
- **Puissant** : Permet de développer tout type d’application.
- **Robuste** : Le typage fort évite de nombreuses erreurs.

Dans ce cours, nous nous concentrerons sur les **concepts fondamentaux de C#**, sans aborder d’environnement complexe.

---

### **2. Utilisation de C#**
C# est idéal pour apprendre les bases de la programmation grâce à :
- Une syntaxe simple et lisible.
- Des concepts applicables à d’autres langages comme Java, Python ou C++.
- Une structure cohérente pour apprendre la programmation orientée objet (POO).

**Applications potentielles** (plus tard) : 
- Automatisation de tâches.
- Jeux avec Unity.
- Résolution de problèmes algorithmiques.

---

### **3. Prérequis**
Pour commencer avec C#, il est utile de :
- **Savoir utiliser un ordinateur** et comprendre les bases des logiciels.
- Avoir des notions simples sur :
  - Ce qu’est un programme (suite d’instructions).
  - Les concepts de base comme les variables, conditions et boucles (pas obligatoire, mais utile).
- Disposer de la motivation pour écrire, tester, et corriger du code.

---

### **4. Outils nécessaires**
Pour débuter simplement :
1. **Un éditeur de texte basique :**
   - **Visual Studio Code**, Sublime Text, ou Visual Studio.
2. **Un compilateur C# :**
   - Installer le **SDK .NET** (même si on se concentre uniquement sur C#). Il fournit l'outil en ligne de commande pour compiler le code.
   - Téléchargez le SDK ici : [https://dotnet.microsoft.com/](https://dotnet.microsoft.com/).
3. **Un terminal ou invite de commande :**
   - Pour compiler et exécuter les programmes .

---

### **5. Syntaxe de base en C#**
Voici une introduction aux concepts essentiels.

#### **a. Structure d’un programme C#**
Un programme C# suit toujours cette structure de base :
```csharp
using System;

class Program
{
    static void Main(string[] args)
    {
        // Code à exécuter
        Console.WriteLine("Bonjour, C#!");
    }
}
```

**Explication :**
- **`using System;`** : Importation de bibliothèques nécessaires pour des fonctions de base (comme afficher du texte).
- **`class Program`** : Définit une classe appelée `Program`, contenant notre code.
- **`static void Main(string[] args)`** : Point d’entrée du programme, où l’exécution commence.
- **`Console.WriteLine`** : Affiche un texte dans la console.

---

#### **b. Les variables**
Une **variable** est un espace en mémoire utilisé pour stocker une donnée.

Exemple :
```csharp
int nombre = 10;              // Variable entière
double pi = 3.14;             // Nombre décimal
string message = "Bonjour";   // Texte
bool estVrai = true;          // Booléen (vrai/faux)
```

**Quelques types courants :**
- **int** : Nombre entier (ex. : 1, 42).
- **double** : Nombre à virgule (ex. : 3.14).
- **char** : Un seul caractère (ex. : 'A').
- **string** : Texte (ex. : "Bonjour").
- **bool** : Vrai ou faux (ex. : `true`, `false`).

---

#### **c. Les conditions**
Les **conditions** permettent d’exécuter du code en fonction d’un test.

Exemple :
```csharp
int age = 18;

if (age >= 18)
{
    Console.WriteLine("Vous êtes majeur !");
}
else
{
    Console.WriteLine("Vous êtes mineur.");
}
```

**Explication :**
- `if` : Vérifie une condition (ici, `age >= 18`).
- `else` : Exécute du code si la condition est fausse.

---

#### **d. Les boucles**
Les **boucles** permettent de répéter une action plusieurs fois.

Exemple avec une boucle `for` :
```csharp
for (int i = 0; i < 5; i++)
{
    Console.WriteLine($"Valeur de i : {i}");
}
```

Exemple avec une boucle `while` :
```csharp
int compteur = 0;
while (compteur < 5)
{
    Console.WriteLine($"Compteur : {compteur}");
    compteur++;
}
```

---

<!-- #### **e. Les fonctions**
Les **fonctions** sont des blocs de code réutilisables.

Exemple :
```csharp
using System;

class Program
{
    static void Main(string[] args)
    {
        Bonjour("Alice");
    }

    static void Bonjour(string nom)
    {
        Console.WriteLine($"Bonjour, {nom} !");
    }
}
```

--- -->

### **5. Exemple pratique**
1. **Objectif :** Écrire un programme qui :
   - Demande à l’utilisateur son nom.
   - Affiche un message personnalisé.

2. **Solution :**
```csharp
using System;

class Program
{
    static void Main(string[] args)
    {
        Console.WriteLine("Entrez votre nom :");
        string nom = Console.ReadLine();  // Lire l’entrée utilisateur
        Console.WriteLine($"Bonjour, {nom} !");
    }
}
```

---


### **Conclusion**
Le C# est un excellent langage pour apprendre les bases de la programmation grâce à sa syntaxe claire et à ses concepts puissants. Avec de la pratique, vous pourrez rapidement écrire des programmes utiles tout en posant les bases pour des projets plus complexes.
