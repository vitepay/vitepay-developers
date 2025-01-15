---
label: Intégration Wordpress - WooCommerce
---

## Compte développeur

Lorsqu'un compte marchand est créé, vous recevez une paire de clés d'API (`api_key` et `api_secret`):

```
api_key: KMyjxAdJdtVk4GmcX90992sL25abPc
api_secret: MCVVzJXVK1f65WkGT1210OObHzO0
```

<hr />

Les clés d'API sont des identifiants numériques utilisés pour interagir avec les services de Vitepay. Elles sont essentielles pour intégrer les APIs de paiement Vitepay.

!!!
Assurez-vous d'abord de disposer d'un compte marchand Vitepay. Si ce n'est pas encore le cas, vous pouvez en [créer](https://checkout.vitepay.com/demo).
!!!

Connectez-vous à votre compte et accédez à l'option "Paramètres" puis "Kit d'intégration" pour recuperer les clés d'API.

Si vous jugez que votre clé secrète est corrompue vous pouvez accéder à votre espace marchand et générer de  nouvelles clés.


## Intégration WordPress - WooCommerce

La présente documentation est destinée aux développeurs souhaitant installer le plugin Woocommerce dans WordPress et configurer Vitepay sur un site marchand.

[!button  icon="download" size="xs" text="Télécharger v-2.0"] Cliquer sur le bouton `Télécharger` pour télécharger le plugin Vitepay.

### I. Telecharger, Installer et Activer le plugin Woocommerce

#### 1. Téléchargement et installation Automatique du plugin Woocommerce

Le plugin `Woocommerce` est disponible sur le site [Wordpress plugins](https://wordpress.org/plugins/woocommerce).

Pour télécharger et installer automatiquement le plugin Woocommerce, cliquer sur **Ajouter** du menu **Extensions** et lancer une recherche du plugin Woocommerce en utilisant **Woocommerce excelling ecommerce** au niveau de la barre de recherche de la page Ajouter des extensions. A la fin de la recherche le plugin Woocommerce s'affichera vous pourrez alors cliquer sur le bouton **Installer maintenant** pour lancer l'installation de Woocommerce.

![](./static/img/demo-popup.png)

Après le téléchargement et l'installation de Vitepay vous serez redirigé vers une page qui vous indiquera que l'extension Vitepay a été bien installée.

Pour activer le plugin Vitepay, cliquer sur le bouton **Activer l'extension**.

#### 2. Téléchargement et installation Manuel du plugin Woocommerce
![](./static/img/demo-popup.png)

##### A. Télécharger le plugin Woocommerce
![](./static/img/demo-popup.png)

##### B. Décompresser le fichier ZIP ou RAR
![](./static/img/demo-popup.png)

##### C. Transfère des données

Transférer par FTP le dossier woocommerce dans le dossier **wp-content/plugins** de votre installation WordPress
![](./static/img/demo-popup.png)

##### D. Activation du plugin Woocommerce

Activer le plugin Woocommerce dans l'interface d'administration ou Back-office de WordPress en cliquant sur le menu **Extensions** puis **Extensions installées** et enfin cliquer sur **Activer** le plugin Woocommerce.
![](./static/img/demo-popup.png)

##### E. Interface du menu

Une fois le plugin Woocommerce Activé, il s’affichera dans le menu de WordPress
![](./static/img/demo-popup.png)

### II. Télécharger, Installer et Activer le plugin Vitepay

Il n’est possible d’installer Vitepay que lorsque le plugin Woocommerce a été bien téléchargé et installé.

#### 1. Télécharger et installer Vitepay

Le plugin Vitepay est disponible sur le site [Wordpress plugins](https://wordpress.org/plugins/vitepay).

Pour télécharger et installer Vitepay, cliquer sur **Ajouter** du menu **Extensions** et lancer une recherche du plugin Vitepay au niveau de la barre de recherche de la page Ajouter des extensions. A la fin de la recherche le plugin Vitepay s’affichera vous pourrez alors cliquer sur le bouton **Installer maintenant** pour lancer l’installation de Vitepay.
![](./static/img/demo-popup.png)

#### 2. Activer Vitepay

Après le téléchargement et l’installation de Vitepay vous serez redirigé vers une page qui vous indiquera que l’extension Vitepay a été bien installée.

Pour activer le plugin Vitepay, cliquer sur le bouton **Activer** l'extension.
![](./static/img/demo-popup.png)

Une fois Vitepay Télécharger, Installer et Activer vous serez redirigé vers la page des Extensions de WordPress.
![](./static/img/demo-popup.png)

### III. Configuration de Vitepay

Après avoir installé et activé le plugin Woocommerce et Vitepay nous allons procéder à la configuration de Vitepay dans le plugin Woocommerce.

Pour configurer Vitepay dans Woocommerce, cliquer sur Woocommerce dans le menu WordPress, sur l’onglet Commande dans paramètres puis sur Vitepay.
![](./static/img/demo-popup.png)

Le menu Vitepay est composé de plusieurs éléments qui sont : `Enable/Disable`, `Title`, `Description`, `Vitepay API key`, `Vitepay API secret`, `Vitepay API signature`, `Woo cart page ID`, `Vitepay Test Mode`, `Default Locale`, `Default Currency`, et `Country`.
![](./static/img/demo-popup.png)

Les différents composants du formulaire Vitepa

- **Enable/Disable :** permet d’activer ou de désactiver le mode de paiement Vitepay.
- **Title :** Vitepay, s’affiche sur l’interface de votre site, où il peut être choisi par un client comme mode de paiement d’un produit.
- **Description :** une brève explication de comment le paiement est effectué, il correspond au texte dans le placeholder qui s’affiche une fois le moyen de paiement Vitepay choisi.
- **Vitepay API key, Vitepay API secret et Vitepay API signature** vous seront donnés et seront utilisés une fois par configuration c’est-à-dire à chaque nouvelle configuration de Vitepay, vous aurez un nouveau API key, API secret et API signature de Vitepay.
- **Woo cart page ID :** est l’id de la page sur laquelle un client sera redirige lors de l’annulation d’une commande.
- **Vitepay Test Mode :** en mode actif, il permet de faire des simulations de paiement en ligne sans passé par Orange money c’est-à-dire tester tout le processus sans que le prix du produit choisi ne soit soustrait de la somme de votre compte Orange money. Vous pouvez choisir de confirmer le paiement en saisissant le 77000001 comme numéro de téléphone lors du paiement ou le 77000009 pour annuler le paiement.<br/>
Il permet comme son nom l’indique de tester le mode de paiement une fois désactivé le paiement en ligne est possible.
- **Default Locale, Default Currency, et Country** sont des champs à remplir avec un nom normalisé par ISO (Organisation Internationale de Normalisation).
- **Default Locale :** pour la langue (fr pour le français).
- **Default Currency :** pour la monnaie (XOF pour le FCFA).
- **Country :** pour le pays (ml pour le Mali).
- Sauvegarder les informations saisies en cliquant sur le bouton **Enregistrer les changements**.


### IV. Tester Vitepay

Pour vérifier si le mode de paiement Vitepay a été bien configuré dans le plugin Woocommerce de WordPress, commander un produit sur l’interface du site (front-end) avec le moyen de paiement Vitepay pour cela choisir **Vitepay**, accepter les **conditions générales de vente** et passer la commande en cliquant sur le bouton **COMMANDER**.
![](./static/img/demo-popup.png)

