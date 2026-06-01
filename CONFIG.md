# 🔧 Configuration - BaseExpertMarketing Digital

## ⚡ AVANT DE LANCER LE SITE

Ce site a besoin de 2 configurations essentielles pour fonctionner correctement.

---

## 1️⃣ **FORMSPREE** - Pour capturer les emails

### 🎯 Objectif
Quand quelqu'un remplit le formulaire "Recevez le guide", ses emails seront envoyés automatiquement.

### 📝 Étapes

**ÉTAPE 1** : Créer un compte Formspree
- Allez sur 👉 https://formspree.io
- Cliquez sur "Sign Up" (inscription)
- Créez un compte avec votre email

**ÉTAPE 2** : Créer un formulaire
- Une fois connecté, cliquez sur "New Form"
- Donnez un nom : `BaseExpertMarketing Lead Form`
- Confirmez

**ÉTAPE 3** : Obtenir votre ID Formspree
- Vous verrez un formulaire avec un ID unique (exemple: `abc123xyz`)
- **COPIEZ CET ID**

**ÉTAPE 4** : Ajouter l'ID dans le code
- Ouvrez `index.html` dans votre repo
- Trouvez la ligne ~228 :
```javascript
const FORMSPREE_ID = "VOTRE_ID_FORMSPREE";
```
- Remplacez `VOTRE_ID_FORMSPREE` par votre ID réel (exemple: `abc123xyz`)
- Commitez le changement

### ✅ Vérification
- Allez sur votre site
- Remplissez le formulaire
- Vous devriez recevoir un email avec la soumission

---

## 2️⃣ **STRIPE** - Pour les paiements

### 🎯 Objectif
Quand quelqu'un clique sur "S'abonner – 97€/mois", il sera redirigé vers Stripe pour payer.

### 📝 Étapes

**ÉTAPE 1** : Créer un compte Stripe
- Allez sur 👉 https://dashboard.stripe.com
- Cliquez sur "Sign Up" (inscription)
- Suivez le processus de création de compte

**ÉTAPE 2** : Créer un Payment Link
- Dans le dashboard, allez à **Payment Links**
- Cliquez sur **+ New**
- Remplissez :
  - **Product name** : `Pack Growth Mensuel`
  - **Price** : `97` (euros)
  - **Billing period** : `Monthly` (mensuel)
- Cliquez sur **Create link**

**ÉTAPE 3** : Copier votre lien Stripe
- Vous verrez un lien : `https://buy.stripe.com/7sI...` (très long)
- **COPIEZ CE LIEN COMPLET**

**ÉTAPE 4** : Ajouter le lien dans le code
- Ouvrez `index.html` dans votre repo
- Trouvez la ligne ~363 :
```javascript
const stripePaymentLink = "VOTRE_LIEN_STRIPE";
```
- Remplacez `VOTRE_LIEN_STRIPE` par votre lien Stripe réel
- Commitez le changement

### ✅ Vérification
- Allez sur votre site
- Cliquez sur le bouton "💳 S'abonner"
- Vous serez redirigé vers Stripe
- L'alerte d'erreur disparaîtra

---

## 🧹 **Supprimer le fichier doublon**

Sur GitHub :
1. Allez à votre repo
2. Trouvez `INDEXhtml_20260505_3b29e2.htmlbaseexpermaketing.html`
3. Cliquez sur le fichier
4. Cliquez sur 🗑️ **Delete**
5. Confirmez

---

## ✅ **Checklist Finale**

```
☐ Créer compte Formspree (https://formspree.io)
☐ Créer formulaire Formspree
☐ Copier ID Formspree (exemple: abc123xyz)
☐ Remplacer VOTRE_ID_FORMSPREE dans index.html (ligne ~228)
☐ Tester le formulaire
☐ Créer compte Stripe (https://dashboard.stripe.com)
☐ Créer Payment Link Stripe (97€/mois)
☐ Copier lien Stripe complet
☐ Remplacer VOTRE_LIEN_STRIPE dans index.html (ligne ~363)
☐ Tester le bouton Stripe
☐ Supprimer fichier doublon
☐ Site prêt pour la production! 🚀
```

---

## 🆘 **Troubleshooting**

### Le formulaire ne fonctionne pas
- Vérifiez que l'ID Formspree est correct (pas d'espaces supplémentaires)
- Ouvrez la console (F12 → Console) pour voir les erreurs
- Assurez-vous que votre email est confirmé sur Formspree

### Stripe affiche une alerte
- Vérifiez que le lien commence par `https://buy.stripe.com/`
- Assurez-vous que le lien est complet (très long, ~50+ caractères)
- Le lien ne doit pas contenir `test_` en production

### Les emails ne sont pas reçus
- Vérifiez vos spams/indésirables
- Confirmez votre adresse email sur Formspree
- Testez avec une adresse différente

---

## 📞 **Support**

Pour toute question :
- **Formspree Help** : https://formspree.io/help
- **Stripe Support** : https://support.stripe.com
- **Votre email** : contact@basemarketing.io

---

**Status** : Site configuré et prêt ✅
