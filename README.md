# Draw++ : Langage de Programmation Graphique & Compilateur

*(English version below)*

## 🇫🇷 Français

**Draw++** est un langage de programmation graphique conçu de zéro pour dessiner et manipuler des formes via des instructions spécifiques. Ce projet comprend un environnement de développement intégré (IDE) web, un compilateur complet en Python (Lexer, Parser, Interpréteur) et un générateur de code intermédiaire en C.

Projet académique réalisé dans le cadre de la formation ING1 Génie Mathématique et Informatique à CY Tech.

### Fonctionnalités principales

* **Langage sur-mesure (DSL)** : Instructions élémentaires (création de curseurs, déplacements, dessin de cercles/carrés/lignes) et avancées (boucles `for`/`while`, conditions `if`, gestion de variables).
* **Pipeline de compilation complet** : 
  * *Lexer* (analyse lexicale par expressions régulières).
  * *Parser* (analyse syntaxique et création de l'arbre d'instructions).
  * *Interpréteur* (exécution logique).
* **Génération de code C** : Traduction du code Draw++ en code C intermédiaire exécuté via la bibliothèque `drawlib.so` (utilisant `ctypes`).
* **Web IDE (Flask)** : Interface utilisateur interactive avec un éditeur de code et un Canvas de rendu en temps réel.
* **Système de gestion d'erreurs** : Détection personnalisée (LexicalError, SyntaxError) pour assister le débogage.

### Technologies
* **Backend & Compilateur** : Python 3, Flask, ctypes, SQLite (sauvegarde des dessins).
* **Frontend** : HTML, CSS, JavaScript, Canvas API.
* **Moteur de rendu graphique** : C.


## English


# Draw++: Graphical Programming Language & Compiler

**Draw++** is a custom graphical programming language built from scratch to draw and manipulate shapes through specific instructions. This project includes a Web-based Integrated Development Environment (IDE), a full Python compiler (Lexer, Parser, Interpreter), and an intermediate C code generator.

Academic project developed during the ING1 Applied Mathematics and Computer Science program at CY Tech.

## Key Features

* **Custom Domain-Specific Language (DSL)**: Basic instructions (cursor creation, movement, drawing circles/squares/lines) and advanced instructions (`for`/`while` loops, `if` conditions, variable handling).
* **Complete Compilation Pipeline**: 
  * *Lexer* (regex-based lexical analysis).
  * *Parser* (syntax analysis and instruction grouping).
  * *Interpreter* (logical execution).
* **C Code Generation**: Translates Draw++ code into intermediate C code executed through the `drawlib.so` compiled library (using `ctypes`).
* **Web IDE (Flask)**: Interactive user interface featuring a code editor and a real-time rendering Canvas.
* **Error Handling System**: Custom detection (`LexicalError`, `SyntaxError`) to assist with live debugging.

## Technologies

* **Backend & Compiler**: Python 3, Flask, ctypes, SQLite (for saving drawings).
* **Frontend**: HTML, CSS, JavaScript, Canvas API.
* **Graphics Engine**: C.

## Installation and Usage

1. Clone the repository and navigate to the project folder:
   ```bash
   git clone [https://github.com/matteo-dev/automate-cy-tech.git](https://github.com/matteo-dev/automate-cy-tech.git)
   cd automate-cy-tech
2. Install the requirements and run the app
   ```bash
   pip install -r requirements.txt
   python app.py
