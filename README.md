# **Worshop - Introduction to React**

Durant ce Workshop, vous allez apprendre les principales fonctionnalités de React sans utiliser de CSS.

## **Qu'est ce que React ?**

React est une bibliothèque JavaScript développée par Facebook pour créer des interfaces utilisateur interactives sur le web. Elle utilise des composants réutilisables et un modèle de programmation basé sur des composants pour simplifier le développement d'applications web réactives.


## **STEP 0: Installation**

Pour pouvoir participer à ce Bootstrap il est important de venir avec Node.js / npm et npx installé sur vos ordinateurs.
Npm est le gestionnaire de paquets officiel de Node.js. Il permet d'installer, de partager et de gérer les dépendances (bibliothèques, outils, etc.) nécessaires à un projet JavaScript. Npx est un outil inclus avec npm (depuis la version 5.2.0) qui permet d'exécuter des paquets Node.js directement, sans avoir besoin de les installer au préalable.

## **Comment allons-nous procéder ?**

Vous trouverez les exercices avec du code pour chaque exercices .Il vous suffira de copier le code et le coller dans app.js, et le compléter.

## **STEP 1: Composant de base**

Nous allons commencer doucement, afin de vous mettre en main avec la programmation web, créez donc un composant React simple appelé HelloWorld qui affiche "Hello, World!".

    import React from 'react';

    const HelloWorld = () => {
    // Complétez le code ici
    };
    
    export default HelloWorld;

## **STEP 2: Propriétés**

Modifiez le composant HelloWorld pour qu'il accepte une propriété name et affiche "Hello, [name]!".

    import React from 'react';

    const HelloWorld = (props) => {
    // Complétez le code ici
    };

    export default HelloWorld;

## **STEP 3: État local**

Créez un compteur simple. Le composant doit afficher un bouton et le nombre de clics sur ce bouton.

    import React, { useState } from 'react';

    const Counter = () => {
        const [count, setCount] = useState(0);
        // Complétez le code ici
    };

    export default Counter;

## **STEP 4: Effets secondaires (Utilisation de useEffect)**

Créez un composant qui utilise useEffect pour mettre à jour le titre de la page avec le nombre actuel de clics du compteur.

    import React, { useState, useEffect } from 'react';

    const CounterWithEffect = () => {
    const [count, setCount] = useState(0);

    // Complétez le code ici
    };

    export default CounterWithEffect;

## **STEP 5: Gestion des formulaires**

Créez un formulaire simple avec un champ de texte pour le nom et un bouton de soumission. Affichez le nom soumis en dessous du formulaire.

    import React, { useState } from 'react';

    const SimpleForm = () => {
        const [name, setName] = useState('');
        const [submittedName, setSubmittedName] = useState('');

        const handleSubmit = (e) => {
            e.preventDefault();
            setSubmittedName(name);
        };
        // Complétez le code ici
    };

    export default SimpleForm;

## **STEP 6: Requêtes API**

Utilisez l'API JSONPlaceholder (https://jsonplaceholder.typicode.com/) pour récupérer et afficher une liste de tâches.

    import React, { useState, useEffect } from 'react';

    const TaskList = () => {
        const [tasks, setTasks] = useState([]);
        // Complétez le code ici
    };

    export default TaskList;

## **STEP 7: Routage avec React Router**

Pour ce dernier exercides vous allez utiliser React Router pour créer deux pages : une page d'accueil et une page "À propos". Ajoutez une navigation pour passer de l'une à l'autre.

    import React from 'react';
    import { BrowserRouter as Router, Link, Route, Routes } from 'react-router-dom';

    const Home = () => <div>Home Page</div>;
    const About = () => <div>About Page</div>;

    const AppWithRouter = () => {
        // Complétez le code ici
    }

    export default AppWithRouter;

### **MERCI**
Merci d'avoir suivi ce Workshop vous avez maintenant de très bonnes bases pour faire un site web avec REACT. À vous de jouer pour créer votre propre site Web !