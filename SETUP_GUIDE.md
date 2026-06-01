# 🚀 Guide Rapide de Configuration

## Dure combien de temps ?
⏱️ **Environ 10-15 minutes** pour configurer les deux services.

---

## 🎬 C'est parti !

### Étape 1 : Formspree (5 minutes)
```
1. Va sur https://formspree.io
2. Clique sur "Sign up"
3. Remplis le formulaire (email + mot de passe)
4. Clique sur "Create a form" ou "New form"
5. Tu verras un ID unique (genre: xeqkzvra)
6. COPIE cet ID
7. Reviens ici et mets à jour index.html
```

**Où le mettre dans index.html ?**
```javascript
// Ligne ~228
const FORMSPREE_ID = "TON_ID_ICI";  // ← change VOTRE_ID_FORMSPREE par ton ID
```

---

### Étape 2 : Stripe (5 minutes)
```
1. Va sur https://dashboard.stripe.com
2. Clique sur "Sign up"
3. Remplis tes infos
4. Dans le menu, va à "Payment Links"
5. Clique sur "+ New"
6. Mets "Pack Growth Mensuel" comme nom
7. Mets 97 comme prix
8. Choisis "Monthly" comme période
9. Clique sur "Create link"
10. Tu verras un long lien (https://buy.stripe.com/...)
11. COPIE CE LIEN COMPLET
12. Reviens ici et mets à jour index.html
```

**Où le mettre dans index.html ?**
```javascript
// Ligne ~363
const stripePaymentLink = "TON_LIEN_COMPLET_ICI";  // ← colle ton lien Stripe
```

---

### Étape 3 : Nettoyer (1 minute)
```
1. Va sur GitHub
2. Trouve le fichier INDEXhtml_20260505_3b29e2.htmlbaseexpermaketing.html
3. Clique sur 🗑️ Delete
4. Confirme
```

---

## ✅ C'est fait !

Ton site est maintenant configuré et prêt à :
- ✅ Capturer les emails via le formulaire
- ✅ Recevoir des paiements via Stripe
- ✅ Fonctionner en production

---

## 🧪 Teste ton site

1. **Teste le formulaire**
   - Remplis le formulaire avec ton email
   - Tu devrais recevoir un email de confirmation
   - Message vert : ✅ "Guide envoyé!"

2. **Teste Stripe**
   - Clique sur "💳 S'abonner"
   - Tu dois être redirigé vers Stripe
   - Pas d'alerte d'erreur

---

## 🆘 Problèmes ?

**Le formulaire dit "Erreur de configuration"**
→ Tu as oublié de remplacer `VOTRE_ID_FORMSPREE`

**Stripe affiche une alerte**
→ Tu as oublié de remplacer `VOTRE_LIEN_STRIPE` ou le lien est incomplet

**Les emails ne sont pas reçus**
→ Vérifie tes spams
→ Confirme ton email sur Formspree

---

**Questions ?** Contacte contact@basemarketing.io
