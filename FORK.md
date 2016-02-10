# Fork RoLLodeQc de SydJS

Configurer dans le fichier .env:

```
MONGO_URI=mongodb://localhost/DB-NAME
CLOUDINARY_URL=cloudinary://CODE1:CODE2@NAME
```

Pour les login 3rd party, remplacer http://127.0.0.1:3000 par votre URL.

Pour GitHub, https://github.com/settings/applications/new
et remplacez ID1 et SECRET1.

```
GITHUB_CLIENT_ID=ID1
GITHUB_CLIENT_SECRET=SECRET1
GITHUB_CALLBACK_URL=http://127.0.0.1:3000/auth/github?cb
```

Pour Twitter, https://apps.twitter.com/app/new
et remplacez ID2 et SECRET2.

```
TWITTER_CONSUMER_KEY=KEY2
TWITTER_CONSUMER_SECRET=SECRET2
TWITTER_CALLBACK_URL=http://127.0.0.1:3000/auth/twitter?cb
```

Pour Google, https://console.developers.google.com/project
cliquez «Create project»
Une fois sur le dashboard du projet, par exemple
https://console.developers.google.com/home/dashboard?project=[CODE-DU-PROJET]
cliquez sur «Enable APIs and get credentials like keys»
pour obtenir les client ID et secret et remplacez ID3 et SECRET3.
Enfin, activez l'API Google+ et désactivez les autres API au besoin.

```
GOOGLE_CLIENT_ID=ID3
GOOGLE_CLIENT_SECRET=SECRET3
GOOGLE_CALLBACK_URL=http://127.0.0.1:3000/auth/google?cb
```
