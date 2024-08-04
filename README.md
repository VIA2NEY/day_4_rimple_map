
## Flutter Ripple Animation in a Map Application Design - Day 5

[Youtube Video](https://youtu.be/2SlFFqcGjOY)

## Development Setup
Clone the repository and run the following commands:
```
flutter pub get
flutter run
```

## ScreenShot

<img src="screenshot/preview1.png" height="500em" />&nbsp;<img src="screenshot/preview2.png" height="500em" />

## Structure du Projet

**lib/**: Contient le code source de l'application.
  - **main.dart**: Point d'entrée principal de l'application.
  - **home_page.dart**: Page d'accueil de l'application affichant une liste de lieux avec des animations.

## Description des fichiers

<details>
<summary> *1.1 main.dart*</summary>

- **main.dart**: 
    - Ce fichier est le point d'entrée principal de l'application Flutter.
    - Il contient la fonction `main()` qui appelle la méthode `runApp()` pour lancer l'application.
    - La classe `MyApp` étend `StatelessWidget` et retourne un `MaterialApp` avec `HomePage` comme écran principal.
    - La `MaterialApp` est configurée avec un titre et un thème.

</details>

<details>
<summary> *1.2 home_page.dart*</summary>

- **home_page.dart**:
    - Ce fichier contient la classe `HomePage` qui affiche une liste de lieux avec des animations.
    - **Classe `HomePage`**:
        - La classe `HomePage` étend `StatefulWidget` et crée l'état avec `_HomePageState`.
    - **Classe `_HomePageState`**:
        - Définit l'interface utilisateur pour la page d'accueil en utilisant un `Scaffold` avec une image de fond et des points d'intérêt.
        - Utilise un `Stack` pour superposer les widgets.
        - **Méthode `makePoint`**:
            - Crée un widget `Positioned` avec une animation de lueur autour d'un point, utilisant le package `avatar_glow`.
        - **Méthode `makeItem`**:
            - Crée un widget pour afficher une carte de lieu avec une image, une distance et un nom. Utilise `AspectRatio` pour garder les éléments proportionnels.

</details>

