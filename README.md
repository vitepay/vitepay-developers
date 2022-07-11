# Introduction

Vitepay est un service qui permet aux marchands d'augmenter leur chiffre d'affaire en 
offrant des moyens de paiements supplémentaires aux clients.

Ceci se traduit concrètement par l'activation d'un bouton "Payer avec Vitepay" qui donne
le possibilité au client de valider son panier et payer avec :

- [x] Orange Monney
- [x] Sama Monney
- [ ] Visa/Mastercard
- [ ] Paypal

Notre objectif est de contiuer à fournir aux marchands des moyens simples et pratiques pour augmenter
leurs ventes.

## Site démo 

Pour voir comment fonctionne l'intégration sur votre site, vous pouvez [consulter le site démo](https://js.vitepay.com/v2/demo).

![Site démo Vitepay - https://js.vitepay.com/v2/demo](./static/img/demo-site.png)




```javascript
 <script
    src="https://js.vitepay.com/v2/button.umd.js"
    data-key="pk_test_MCVVzJXVK1f65WkGT03dYabHzO0"
    data-name="Maliba SARL"
    data-country="ML"
    data-method="orange_money"
    data-currency="XOF"
    data-currency-display="FCFA"
    data-description="Votre panier de courses chez Maliba"
    data-image="/img/maliba-logo.svg"
    data-amount="500">
</script>
```