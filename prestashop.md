---
label: Intégration PrestaShop
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


## Intégration PrestaShop

La présente documentation est destinée aux développeurs souhaitant installer et configurer Vitepay sur un site marchand Prestashop..

[!button  icon="download" size="xs" text="Télécharger v-2.0"] Cliquer sur le bouton `Télécharger` pour télécharger le plugin Vitepay.

### I. Installation

#### 1. Transfère de données

Le dossier Vitepay vous sera transmis.

Transférer par FTP le dossier Vitepay dans le dossier modules de votre installation Prestashop.

![](./static/img/demo-popup.png)

#### 2. Installation de Vitepay

Installer Vitepay dans l'interface Administration de Prestashop en cliquant sur le menu **MODULES** puis **Paiement**
![](./static/img/demo-popup.png)
Et enfin sur le bouton **Installer**.
![](./static/img/demo-popup.png)


### II. Configuration

#### 1. Configuration de Vitepay

Apres l'installation de Vitepay, nous allons configurer Vitepay pour cela cliquer sur le bouton **Configurer**.
![](./static/img/demo-popup.png)

#### 2. Les différents composants du formulaire Vitepay

Vitepay est composé de plusieurs éléments qui sont : `Vitepay API key`, `Vitepay API secret`, `Vitepay API signature`, `Merchant Locale`, `Merchant Currency`, `Merchant Country`, `Transaction Server`
![](./static/img/demo-popup.png)

- **Mode :** il existe deux modes:
- **le Mode Test** qui permet de faire une simulation du mode de paiement Vitepay sans passé par Orange money c'est-à-dire tester tout le processus sans que le prix du produit choisi ne soit soustrait de la somme de votre compte Orange money. Vous pouvez choisir de confirmer le paiement en saisissant le 77000001 comme numéro de téléphone lors du paiement ou le 77000009 pour annuler le paiement.
- **le Mode Live** une fois choisi vous permet de faire des achats en ligne avec Orange money.
- **API key, Vitepay API secret et API signature** vous seront donnés et seront utilisés une fois par configuration c'est-à-dire à chaque nouvelle configuration de Vitepay, vous aurez un nouveau API key, API secret et API signature de Vitepay.
- **Langue, Pays et Devise** sont des champs à remplir avec un nom normalisé par ISO (Organisation Internationale de Normalisation).
- **Langue :** pour la langue (fr pour le français).
- **Pays :** pour le pays (ML pour le Mali).
- **Devise :** pour la monnaie (XOF pour le FCFA).

Lors du paiement, vous pourrez choisir le mode d'affichage du texte, logo de Vitepay et d'Orange money à l'aide des éléments ci-dessous:
- **PayNow Text** permet de changer le texte qui va s'afficher lors du paiement
- **PayNow Logo** permet d'afficher ou non le logo Vitepay.
- **PayNow logo Align** permet d'aligner le logo Vitepay à gauche ou à droite une fois le logo affiché.
Sauvegarder les informations saisies en cliquant sur le bouton **Save**.

### III. Tester Vitepay

Pour vérifier si le plugin **Vitepay** a été bien installé et configuré dans Pestashop, commander un produit sur l'interface du site et lors du paiement choisir Vitepay.
![](./static/img/demo-popup.png)

Vous serez redirigé vers la page Vitepay pour compléter la procédure d'achat effectué à travers le service Orange money.
![](./static/img/demo-popup.png)

