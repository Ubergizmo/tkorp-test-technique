# Tkorp Test Technique

## Installation

Vous devrez cloner les dépôts du backend et du frontend.

### Backend

1. Clonez le dépôt du backend :

   ```bash
   git clone https://github.com/Ubergizmo/tkorp-app.git
   cd tkorp-app
2. Installez les packages :

   ```bash
   npm install
3. Connectez votre BDD mySQL:

   Dans le dossier "src" modifier le fichier app.module.ts

    ```bash
    TypeOrmModule.forRoot({
        type: 'mysql',
        host: 'localhost', //Ici
        port: 3306, //Ici
        database: 'tkorpdb', //Ici
        synchronize: true,
        username: 'root', //Ici
        password: '1234', //Ici
        entities: [PersonEntity, AnimalEntity],
        logging: true,
      }),
4. Lancez le serveur:

     ```bash
     npm run start
5. La réponse aux questions se trouvent à la racine du projet "graphql-requete.txt"

### Frontend

1. Clonez le dépôt du frontend :

   ```bash
   git clone https://github.com/Ubergizmo/tkorp-front.git
   cd tkorp-front
2. Installez les packages :

   ```bash
   npm install
3. Lancez le front:

     ```bash
     npm run start
