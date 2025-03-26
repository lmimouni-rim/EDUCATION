```mermaid

classDiagram
    
    class Étudiant {
        +Int id
        +Int num_etu
    }

    class Enseignant {
        +Int id
        +String formation 
        +Int id_cours
    }

    class Cours {
        +Int id
        +String nom_cours
    }

    class Collaboration {
        +Int id
        +Int id_etudiant1
        +Int id_etudiant2
        +String type_collaboration
    }

    Cours --> Enseignant : introduit par 
    Enseignant --> Étudiant : échange
    Étudiant <---> Collaboration : participe à

```
